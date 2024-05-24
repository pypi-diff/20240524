# Comparing `tmp/mapieng-0.1.4.tar.gz` & `tmp/mapieng-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapieng-0.1.4.tar", last modified: Fri May 24 07:16:13 2024, max compression
+gzip compressed data, was "mapieng-0.1.5.tar", last modified: Fri May 24 07:24:05 2024, max compression
```

## Comparing `mapieng-0.1.4.tar` & `mapieng-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 07:16:13.029806 mapieng-0.1.4/
--rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 mapieng-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7052 2024-05-24 07:16:13.027348 mapieng-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 mapieng-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 07:16:12.983181 mapieng-0.1.4/base/
--rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 mapieng-0.1.4/base/ReportUtil.py
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.4/base/__init__.py
--rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 mapieng-0.1.4/base/baseformidasapi.py
--rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 mapieng-0.1.4/base/calculator_asd.py
--rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 mapieng-0.1.4/base/dgncodeutil.py
--rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 mapieng-0.1.4/base/engineers.py
--rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 mapieng-0.1.4/base/geometry.py
--rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 mapieng-0.1.4/base/hello.html
--rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 mapieng-0.1.4/base/meshutil.py
--rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 mapieng-0.1.4/base/midasapi.py
--rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 mapieng-0.1.4/base/midasapi.pyi
--rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 mapieng-0.1.4/base/midasutil.py
--rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 mapieng-0.1.4/base/midasutil_server.py
--rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 mapieng-0.1.4/base/midasutil_web.py
--rw-rw-rw-   0        0        0     1275 2024-05-23 05:53:17.000000 mapieng-0.1.4/base/section_property.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:16:12.989328 mapieng-0.1.4/base/steel/
--rw-rw-rw-   0        0        0     1141 2024-04-05 06:25:39.000000 mapieng-0.1.4/base/steel/KS18.json
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.4/base/steel/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 mapieng-0.1.4/base/steel/steelutil.py
--rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 mapieng-0.1.4/base/symbol.py
--rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 mapieng-0.1.4/base/test.py
--rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 mapieng-0.1.4/base/testmesh.py
--rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 mapieng-0.1.4/base/unit_converter.py
--rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 mapieng-0.1.4/base/vector.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:16:13.024342 mapieng-0.1.4/mapieng.egg-info/
--rw-rw-rw-   0        0        0     7052 2024-05-24 07:16:12.000000 mapieng-0.1.4/mapieng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2024-05-24 07:16:12.000000 mapieng-0.1.4/mapieng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 07:16:12.000000 mapieng-0.1.4/mapieng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-24 07:16:12.000000 mapieng-0.1.4/mapieng.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 07:16:12.000000 mapieng-0.1.4/mapieng.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-24 07:16:13.005336 mapieng-0.1.4/project/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.4/project/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:16:13.012333 mapieng-0.1.4/project/baseplate_KDS41_30_2022/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 mapieng-0.1.4/project/baseplate_KDS41_30_2022/__init__.py
--rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 mapieng-0.1.4/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
--rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 mapieng-0.1.4/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:16:13.016341 mapieng-0.1.4/project/sectionproperty/
--rw-rw-rw-   0        0        0      485 2024-05-23 05:53:17.000000 mapieng-0.1.4/project/sectionproperty/report_sectionproperty.py
--rw-rw-rw-   0        0        0       42 2024-05-24 07:16:13.030814 mapieng-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-05-24 07:16:02.000000 mapieng-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 07:16:13.021340 mapieng-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 mapieng-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0     2219 2024-05-23 05:53:17.000000 mapieng-0.1.4/tests/test_baseplate_kds.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:24:05.519483 mapieng-0.1.5/
+-rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 mapieng-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7052 2024-05-24 07:24:05.516485 mapieng-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 mapieng-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 07:24:05.475735 mapieng-0.1.5/base/
+-rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 mapieng-0.1.5/base/ReportUtil.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.5/base/__init__.py
+-rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 mapieng-0.1.5/base/baseformidasapi.py
+-rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 mapieng-0.1.5/base/calculator_asd.py
+-rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 mapieng-0.1.5/base/dgncodeutil.py
+-rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 mapieng-0.1.5/base/engineers.py
+-rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 mapieng-0.1.5/base/geometry.py
+-rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 mapieng-0.1.5/base/hello.html
+-rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 mapieng-0.1.5/base/meshutil.py
+-rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 mapieng-0.1.5/base/midasapi.py
+-rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 mapieng-0.1.5/base/midasapi.pyi
+-rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 mapieng-0.1.5/base/midasutil.py
+-rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 mapieng-0.1.5/base/midasutil_server.py
+-rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 mapieng-0.1.5/base/midasutil_web.py
+-rw-rw-rw-   0        0        0     1275 2024-05-23 05:53:17.000000 mapieng-0.1.5/base/section_property.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:24:05.481999 mapieng-0.1.5/base/steel/
+-rw-rw-rw-   0        0        0     1141 2024-04-05 06:25:39.000000 mapieng-0.1.5/base/steel/KS18.json
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.5/base/steel/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 mapieng-0.1.5/base/steel/steelutil.py
+-rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 mapieng-0.1.5/base/symbol.py
+-rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 mapieng-0.1.5/base/test.py
+-rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 mapieng-0.1.5/base/testmesh.py
+-rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 mapieng-0.1.5/base/unit_converter.py
+-rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 mapieng-0.1.5/base/vector.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:24:05.514485 mapieng-0.1.5/mapieng.egg-info/
+-rw-rw-rw-   0        0        0     7052 2024-05-24 07:24:05.000000 mapieng-0.1.5/mapieng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2024-05-24 07:24:05.000000 mapieng-0.1.5/mapieng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:24:05.000000 mapieng-0.1.5/mapieng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-24 07:24:05.000000 mapieng-0.1.5/mapieng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 07:24:05.000000 mapieng-0.1.5/mapieng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 07:24:05.496004 mapieng-0.1.5/project/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.5/project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:24:05.502999 mapieng-0.1.5/project/baseplate_KDS41_30_2022/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 mapieng-0.1.5/project/baseplate_KDS41_30_2022/__init__.py
+-rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 mapieng-0.1.5/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
+-rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 mapieng-0.1.5/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:24:05.506485 mapieng-0.1.5/project/sectionproperty/
+-rw-rw-rw-   0        0        0      485 2024-05-23 05:53:17.000000 mapieng-0.1.5/project/sectionproperty/report_sectionproperty.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:24:05.519483 mapieng-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      552 2024-05-24 07:23:59.000000 mapieng-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:24:05.511482 mapieng-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 mapieng-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     2219 2024-05-23 05:53:17.000000 mapieng-0.1.5/tests/test_baseplate_kds.py
```

### Comparing `mapieng-0.1.4/PKG-INFO` & `mapieng-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapieng
-Version: 0.1.4
+Version: 0.1.5
 Summary: mapi engineers
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `mapieng-0.1.4/README.md` & `mapieng-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/ReportUtil.py` & `mapieng-0.1.5/base/ReportUtil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/baseformidasapi.py` & `mapieng-0.1.5/base/baseformidasapi.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/calculator_asd.py` & `mapieng-0.1.5/base/calculator_asd.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/dgncodeutil.py` & `mapieng-0.1.5/base/dgncodeutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/geometry.py` & `mapieng-0.1.5/base/geometry.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/hello.html` & `mapieng-0.1.5/base/hello.html`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/meshutil.py` & `mapieng-0.1.5/base/meshutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/midasapi.py` & `mapieng-0.1.5/base/midasapi.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/midasapi.pyi` & `mapieng-0.1.5/base/midasapi.pyi`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/midasutil.py` & `mapieng-0.1.5/base/midasutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/midasutil_server.py` & `mapieng-0.1.5/base/midasutil_server.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/midasutil_web.py` & `mapieng-0.1.5/base/midasutil_web.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/section_property.py` & `mapieng-0.1.5/base/section_property.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/steel/KS18.json` & `mapieng-0.1.5/base/steel/KS18.json`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/steel/steelutil.py` & `mapieng-0.1.5/base/steel/steelutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/symbol.py` & `mapieng-0.1.5/base/symbol.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/unit_converter.py` & `mapieng-0.1.5/base/unit_converter.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/base/vector.py` & `mapieng-0.1.5/base/vector.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/mapieng.egg-info/PKG-INFO` & `mapieng-0.1.5/mapieng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapieng
-Version: 0.1.4
+Version: 0.1.5
 Summary: mapi engineers
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `mapieng-0.1.4/mapieng.egg-info/SOURCES.txt` & `mapieng-0.1.5/mapieng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py` & `mapieng-0.1.5/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py` & `mapieng-0.1.5/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.4/tests/test_baseplate_kds.py` & `mapieng-0.1.5/tests/test_baseplate_kds.py`

 * *Files identical despite different names*

