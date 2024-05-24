# Comparing `tmp/mapieng-0.1.6.tar.gz` & `tmp/mapieng-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapieng-0.1.6.tar", last modified: Fri May 24 07:27:48 2024, max compression
+gzip compressed data, was "mapieng-0.1.7.tar", last modified: Fri May 24 07:55:35 2024, max compression
```

## Comparing `mapieng-0.1.6.tar` & `mapieng-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 07:27:48.234786 mapieng-0.1.6/
--rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 mapieng-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     7121 2024-05-24 07:27:48.232786 mapieng-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 mapieng-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 07:27:48.200792 mapieng-0.1.6/base/
--rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 mapieng-0.1.6/base/ReportUtil.py
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.6/base/__init__.py
--rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 mapieng-0.1.6/base/baseformidasapi.py
--rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 mapieng-0.1.6/base/calculator_asd.py
--rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 mapieng-0.1.6/base/dgncodeutil.py
--rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 mapieng-0.1.6/base/engineers.py
--rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 mapieng-0.1.6/base/geometry.py
--rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 mapieng-0.1.6/base/hello.html
--rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 mapieng-0.1.6/base/meshutil.py
--rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 mapieng-0.1.6/base/midasapi.py
--rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 mapieng-0.1.6/base/midasapi.pyi
--rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 mapieng-0.1.6/base/midasutil.py
--rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 mapieng-0.1.6/base/midasutil_server.py
--rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 mapieng-0.1.6/base/midasutil_web.py
--rw-rw-rw-   0        0        0     1275 2024-05-23 05:53:17.000000 mapieng-0.1.6/base/section_property.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:27:48.205786 mapieng-0.1.6/base/steel/
--rw-rw-rw-   0        0        0     1141 2024-04-05 06:25:39.000000 mapieng-0.1.6/base/steel/KS18.json
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.6/base/steel/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 mapieng-0.1.6/base/steel/steelutil.py
--rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 mapieng-0.1.6/base/symbol.py
--rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 mapieng-0.1.6/base/test.py
--rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 mapieng-0.1.6/base/testmesh.py
--rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 mapieng-0.1.6/base/unit_converter.py
--rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 mapieng-0.1.6/base/vector.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:27:48.230786 mapieng-0.1.6/mapieng.egg-info/
--rw-rw-rw-   0        0        0     7121 2024-05-24 07:27:48.000000 mapieng-0.1.6/mapieng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2024-05-24 07:27:48.000000 mapieng-0.1.6/mapieng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 07:27:48.000000 mapieng-0.1.6/mapieng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-24 07:27:48.000000 mapieng-0.1.6/mapieng.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 07:27:48.000000 mapieng-0.1.6/mapieng.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-24 07:27:48.216789 mapieng-0.1.6/project/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.6/project/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:27:48.222786 mapieng-0.1.6/project/baseplate_KDS41_30_2022/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 mapieng-0.1.6/project/baseplate_KDS41_30_2022/__init__.py
--rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 mapieng-0.1.6/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
--rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 mapieng-0.1.6/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:27:48.224786 mapieng-0.1.6/project/sectionproperty/
--rw-rw-rw-   0        0        0      485 2024-05-23 05:53:17.000000 mapieng-0.1.6/project/sectionproperty/report_sectionproperty.py
--rw-rw-rw-   0        0        0       42 2024-05-24 07:27:48.234786 mapieng-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      722 2024-05-24 07:27:24.000000 mapieng-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:27:48.227789 mapieng-0.1.6/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 mapieng-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0     2219 2024-05-23 05:53:17.000000 mapieng-0.1.6/tests/test_baseplate_kds.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:55:35.527074 mapieng-0.1.7/
+-rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 mapieng-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     7121 2024-05-24 07:55:35.523964 mapieng-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 mapieng-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 07:55:35.463110 mapieng-0.1.7/base/
+-rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 mapieng-0.1.7/base/ReportUtil.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.7/base/__init__.py
+-rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 mapieng-0.1.7/base/baseformidasapi.py
+-rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 mapieng-0.1.7/base/calculator_asd.py
+-rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 mapieng-0.1.7/base/dgncodeutil.py
+-rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 mapieng-0.1.7/base/engineers.py
+-rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 mapieng-0.1.7/base/geometry.py
+-rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 mapieng-0.1.7/base/hello.html
+-rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 mapieng-0.1.7/base/meshutil.py
+-rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 mapieng-0.1.7/base/midasapi.py
+-rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 mapieng-0.1.7/base/midasapi.pyi
+-rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 mapieng-0.1.7/base/midasutil.py
+-rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 mapieng-0.1.7/base/midasutil_server.py
+-rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 mapieng-0.1.7/base/midasutil_web.py
+-rw-rw-rw-   0        0        0     1275 2024-05-23 05:53:17.000000 mapieng-0.1.7/base/section_property.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:55:35.473385 mapieng-0.1.7/base/steel/
+-rw-rw-rw-   0        0        0     1141 2024-04-05 06:25:39.000000 mapieng-0.1.7/base/steel/KS18.json
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.7/base/steel/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 mapieng-0.1.7/base/steel/steelutil.py
+-rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 mapieng-0.1.7/base/symbol.py
+-rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 mapieng-0.1.7/base/test.py
+-rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 mapieng-0.1.7/base/testmesh.py
+-rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 mapieng-0.1.7/base/unit_converter.py
+-rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 mapieng-0.1.7/base/vector.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:55:35.520450 mapieng-0.1.7/mapieng.egg-info/
+-rw-rw-rw-   0        0        0     7121 2024-05-24 07:55:35.000000 mapieng-0.1.7/mapieng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2024-05-24 07:55:35.000000 mapieng-0.1.7/mapieng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:55:35.000000 mapieng-0.1.7/mapieng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-24 07:55:35.000000 mapieng-0.1.7/mapieng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 07:55:35.000000 mapieng-0.1.7/mapieng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 07:55:35.497280 mapieng-0.1.7/project/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.7/project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:55:35.507687 mapieng-0.1.7/project/baseplate_KDS41_30_2022/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 mapieng-0.1.7/project/baseplate_KDS41_30_2022/__init__.py
+-rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 mapieng-0.1.7/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
+-rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 mapieng-0.1.7/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:55:35.510687 mapieng-0.1.7/project/sectionproperty/
+-rw-rw-rw-   0        0        0      485 2024-05-23 05:53:17.000000 mapieng-0.1.7/project/sectionproperty/report_sectionproperty.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:55:35.528078 mapieng-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-05-24 07:55:31.000000 mapieng-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:55:35.517278 mapieng-0.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 mapieng-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     2219 2024-05-23 05:53:17.000000 mapieng-0.1.7/tests/test_baseplate_kds.py
```

### Comparing `mapieng-0.1.6/PKG-INFO` & `mapieng-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapieng
-Version: 0.1.6
+Version: 0.1.7
 Summary: mapi engineers
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `mapieng-0.1.6/README.md` & `mapieng-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/ReportUtil.py` & `mapieng-0.1.7/base/ReportUtil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/baseformidasapi.py` & `mapieng-0.1.7/base/baseformidasapi.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/calculator_asd.py` & `mapieng-0.1.7/base/calculator_asd.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/dgncodeutil.py` & `mapieng-0.1.7/base/dgncodeutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/geometry.py` & `mapieng-0.1.7/base/geometry.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/hello.html` & `mapieng-0.1.7/base/hello.html`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/meshutil.py` & `mapieng-0.1.7/base/meshutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/midasapi.py` & `mapieng-0.1.7/base/midasapi.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/midasapi.pyi` & `mapieng-0.1.7/base/midasapi.pyi`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/midasutil.py` & `mapieng-0.1.7/base/midasutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/midasutil_server.py` & `mapieng-0.1.7/base/midasutil_server.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/midasutil_web.py` & `mapieng-0.1.7/base/midasutil_web.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/section_property.py` & `mapieng-0.1.7/base/section_property.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/steel/KS18.json` & `mapieng-0.1.7/base/steel/KS18.json`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/steel/steelutil.py` & `mapieng-0.1.7/base/steel/steelutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/symbol.py` & `mapieng-0.1.7/base/symbol.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/unit_converter.py` & `mapieng-0.1.7/base/unit_converter.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/base/vector.py` & `mapieng-0.1.7/base/vector.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/mapieng.egg-info/PKG-INFO` & `mapieng-0.1.7/mapieng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapieng
-Version: 0.1.6
+Version: 0.1.7
 Summary: mapi engineers
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `mapieng-0.1.6/mapieng.egg-info/SOURCES.txt` & `mapieng-0.1.7/mapieng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py` & `mapieng-0.1.7/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py` & `mapieng-0.1.7/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.6/setup.py` & `mapieng-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import sys
+import os
 from setuptools import setup, find_packages
 
 def readme():
     with open('README_en.md', encoding='utf-8') as f:
         return f.read()
 
 
-if "pyodide" in sys.modules:
+if "PYODIDE" in os.environ:
     requires = ['mdutils', "numpy", "matplotlib",]
 else:
     requires = ['mdutils', "numpy", "matplotlib", "concreteproperties", "sectionproperties"]
 
 setup(
     name='mapieng',
-    version='0.1.6',
+    version='0.1.7',
     packages=find_packages(),
     include_package_data=True,
     description='mapi engineers',
     long_description=readme(),
     long_description_content_type='text/markdown',
     license='MIT',
     author='bschoi',
```

### Comparing `mapieng-0.1.6/tests/test_baseplate_kds.py` & `mapieng-0.1.7/tests/test_baseplate_kds.py`

 * *Files identical despite different names*

