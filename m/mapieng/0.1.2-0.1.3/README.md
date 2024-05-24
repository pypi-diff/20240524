# Comparing `tmp/mapieng-0.1.2.tar.gz` & `tmp/mapieng-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapieng-0.1.2.tar", last modified: Thu May 23 06:03:49 2024, max compression
+gzip compressed data, was "mapieng-0.1.3.tar", last modified: Fri May 24 05:35:37 2024, max compression
```

## Comparing `mapieng-0.1.2.tar` & `mapieng-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.416991 mapieng-0.1.2/
--rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 mapieng-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7146 2024-05-23 06:03:49.414990 mapieng-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 mapieng-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.389849 mapieng-0.1.2/base/
--rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/ReportUtil.py
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.2/base/__init__.py
--rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 mapieng-0.1.2/base/baseformidasapi.py
--rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 mapieng-0.1.2/base/calculator_asd.py
--rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 mapieng-0.1.2/base/dgncodeutil.py
--rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 mapieng-0.1.2/base/engineers.py
--rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 mapieng-0.1.2/base/geometry.py
--rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 mapieng-0.1.2/base/hello.html
--rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 mapieng-0.1.2/base/meshutil.py
--rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/midasapi.py
--rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/midasapi.pyi
--rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 mapieng-0.1.2/base/midasutil.py
--rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/midasutil_server.py
--rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 mapieng-0.1.2/base/midasutil_web.py
--rw-rw-rw-   0        0        0     1275 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/section_property.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.393847 mapieng-0.1.2/base/steel/
--rw-rw-rw-   0        0        0     1141 2024-04-05 06:25:39.000000 mapieng-0.1.2/base/steel/KS18.json
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.2/base/steel/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 mapieng-0.1.2/base/steel/steelutil.py
--rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 mapieng-0.1.2/base/symbol.py
--rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 mapieng-0.1.2/base/test.py
--rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 mapieng-0.1.2/base/testmesh.py
--rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 mapieng-0.1.2/base/unit_converter.py
--rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 mapieng-0.1.2/base/vector.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.413991 mapieng-0.1.2/mapieng.egg-info/
--rw-rw-rw-   0        0        0     7146 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.402992 mapieng-0.1.2/project/
--rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.2/project/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.407994 mapieng-0.1.2/project/baseplate_KDS41_30_2022/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 mapieng-0.1.2/project/baseplate_KDS41_30_2022/__init__.py
--rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 mapieng-0.1.2/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
--rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 mapieng-0.1.2/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.408992 mapieng-0.1.2/project/sectionproperty/
--rw-rw-rw-   0        0        0      485 2024-05-23 05:53:17.000000 mapieng-0.1.2/project/sectionproperty/report_sectionproperty.py
--rw-rw-rw-   0        0        0       42 2024-05-23 06:03:49.417992 mapieng-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      606 2024-05-23 06:03:03.000000 mapieng-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.411991 mapieng-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 mapieng-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2219 2024-05-23 05:53:17.000000 mapieng-0.1.2/tests/test_baseplate_kds.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:37.798646 mapieng-0.1.3/
+-rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 mapieng-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7146 2024-05-24 05:35:37.795405 mapieng-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 mapieng-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:37.737848 mapieng-0.1.3/base/
+-rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 mapieng-0.1.3/base/ReportUtil.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.3/base/__init__.py
+-rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 mapieng-0.1.3/base/baseformidasapi.py
+-rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 mapieng-0.1.3/base/calculator_asd.py
+-rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 mapieng-0.1.3/base/dgncodeutil.py
+-rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 mapieng-0.1.3/base/engineers.py
+-rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 mapieng-0.1.3/base/geometry.py
+-rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 mapieng-0.1.3/base/hello.html
+-rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 mapieng-0.1.3/base/meshutil.py
+-rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 mapieng-0.1.3/base/midasapi.py
+-rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 mapieng-0.1.3/base/midasapi.pyi
+-rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 mapieng-0.1.3/base/midasutil.py
+-rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 mapieng-0.1.3/base/midasutil_server.py
+-rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 mapieng-0.1.3/base/midasutil_web.py
+-rw-rw-rw-   0        0        0     1275 2024-05-23 05:53:17.000000 mapieng-0.1.3/base/section_property.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:37.747239 mapieng-0.1.3/base/steel/
+-rw-rw-rw-   0        0        0     1141 2024-04-05 06:25:39.000000 mapieng-0.1.3/base/steel/KS18.json
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.3/base/steel/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 mapieng-0.1.3/base/steel/steelutil.py
+-rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 mapieng-0.1.3/base/symbol.py
+-rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 mapieng-0.1.3/base/test.py
+-rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 mapieng-0.1.3/base/testmesh.py
+-rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 mapieng-0.1.3/base/unit_converter.py
+-rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 mapieng-0.1.3/base/vector.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:37.792798 mapieng-0.1.3/mapieng.egg-info/
+-rw-rw-rw-   0        0        0     7146 2024-05-24 05:35:37.000000 mapieng-0.1.3/mapieng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2024-05-24 05:35:37.000000 mapieng-0.1.3/mapieng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 05:35:37.000000 mapieng-0.1.3/mapieng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-24 05:35:37.000000 mapieng-0.1.3/mapieng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 05:35:37.000000 mapieng-0.1.3/mapieng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:37.769101 mapieng-0.1.3/project/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.3/project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:37.779909 mapieng-0.1.3/project/baseplate_KDS41_30_2022/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 mapieng-0.1.3/project/baseplate_KDS41_30_2022/__init__.py
+-rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 mapieng-0.1.3/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
+-rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 mapieng-0.1.3/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:37.783908 mapieng-0.1.3/project/sectionproperty/
+-rw-rw-rw-   0        0        0      485 2024-05-23 05:53:17.000000 mapieng-0.1.3/project/sectionproperty/report_sectionproperty.py
+-rw-rw-rw-   0        0        0       42 2024-05-24 05:35:37.798646 mapieng-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      846 2024-05-24 05:35:32.000000 mapieng-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:37.788919 mapieng-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 mapieng-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2219 2024-05-23 05:53:17.000000 mapieng-0.1.3/tests/test_baseplate_kds.py
```

### Comparing `mapieng-0.1.2/PKG-INFO` & `mapieng-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapieng
-Version: 0.1.2
+Version: 0.1.3
 Summary: mapi engineers
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `mapieng-0.1.2/README.md` & `mapieng-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/ReportUtil.py` & `mapieng-0.1.3/base/ReportUtil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/baseformidasapi.py` & `mapieng-0.1.3/base/baseformidasapi.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/calculator_asd.py` & `mapieng-0.1.3/base/calculator_asd.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/dgncodeutil.py` & `mapieng-0.1.3/base/dgncodeutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/geometry.py` & `mapieng-0.1.3/base/geometry.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/hello.html` & `mapieng-0.1.3/base/hello.html`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/meshutil.py` & `mapieng-0.1.3/base/meshutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/midasapi.py` & `mapieng-0.1.3/base/midasapi.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/midasapi.pyi` & `mapieng-0.1.3/base/midasapi.pyi`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/midasutil.py` & `mapieng-0.1.3/base/midasutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/midasutil_server.py` & `mapieng-0.1.3/base/midasutil_server.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/midasutil_web.py` & `mapieng-0.1.3/base/midasutil_web.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/section_property.py` & `mapieng-0.1.3/base/section_property.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/steel/KS18.json` & `mapieng-0.1.3/base/steel/KS18.json`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/steel/steelutil.py` & `mapieng-0.1.3/base/steel/steelutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/symbol.py` & `mapieng-0.1.3/base/symbol.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/unit_converter.py` & `mapieng-0.1.3/base/unit_converter.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/base/vector.py` & `mapieng-0.1.3/base/vector.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/mapieng.egg-info/PKG-INFO` & `mapieng-0.1.3/mapieng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapieng
-Version: 0.1.2
+Version: 0.1.3
 Summary: mapi engineers
 Home-page: https://github.com/MIDASIT-Co-Ltd/engineers-api-python
 Author: bschoi
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: mdutils
 Requires-Dist: numpy
```

### Comparing `mapieng-0.1.2/mapieng.egg-info/SOURCES.txt` & `mapieng-0.1.3/mapieng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py` & `mapieng-0.1.3/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py` & `mapieng-0.1.3/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.2/setup.py` & `mapieng-0.1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+import platform
 from setuptools import setup, find_packages
 
 def readme():
     with open('README_en.md', encoding='utf-8') as f:
         return f.read()
 
 
+# platform에 따른 install_requires
+install_requires = []
+if platform.system() == 'Emscripten':
+    install_requires = ['mdutils', "numpy", "matplotlib", "requests"]
+else:
+    install_requires = ['mdutils', "numpy", "matplotlib", "sectionproperties", "concreteproperties", "requests"]
+
+
 setup(
     name='mapieng',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     include_package_data=True,
     description='mapi engineers',
     long_description=readme(),
     long_description_content_type='text/markdown',
     license='MIT',
     author='bschoi',
     url='https://github.com/MIDASIT-Co-Ltd/engineers-api-python',
-    install_requires=['mdutils', "numpy", "matplotlib", "sectionproperties", "concreteproperties", "requests"],
+    install_requires=install_requires
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mapieng-0.1.2/tests/test_baseplate_kds.py` & `mapieng-0.1.3/tests/test_baseplate_kds.py`

 * *Files identical despite different names*

