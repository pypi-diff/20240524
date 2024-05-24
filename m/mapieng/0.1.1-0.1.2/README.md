# Comparing `tmp/mapieng-0.1.1.tar.gz` & `tmp/mapieng-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapieng-0.1.1.tar", last modified: Tue May 14 08:45:05 2024, max compression
+gzip compressed data, was "mapieng-0.1.2.tar", last modified: Thu May 23 06:03:49 2024, max compression
```

## Comparing `mapieng-0.1.1.tar` & `mapieng-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.238845 mapieng-0.1.1/
--rw-rw-rw-   0        0        0       79 2024-05-14 08:44:17.000000 mapieng-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      326 2024-05-14 08:45:05.237845 mapieng-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-05-14 08:44:17.000000 mapieng-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.213331 mapieng-0.1.1/base/
--rw-rw-rw-   0        0        0     2988 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/ReportUtil.py
--rw-rw-rw-   0        0        0        0 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/__init__.py
--rw-rw-rw-   0        0        0     7980 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/baseformidasapi.py
--rw-rw-rw-   0        0        0    18374 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/calculator_asd.py
--rw-rw-rw-   0        0        0       38 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/engineers.py
--rw-rw-rw-   0        0        0     7065 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/engineers_server.py
--rw-rw-rw-   0        0        0     9894 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/engineers_web.py
--rw-rw-rw-   0        0        0     8194 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/geometry.py
--rw-rw-rw-   0        0        0    13475 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/hello.html
--rw-rw-rw-   0        0        0     7301 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/midasapi.py
--rw-rw-rw-   0        0        0     3412 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/midasutil.py
--rw-rw-rw-   0        0        0      449 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/section_property.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.217337 mapieng-0.1.1/base/steel/
--rw-rw-rw-   0        0        0     1141 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/steel/KS18.json
--rw-rw-rw-   0        0        0        0 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/steel/__init__.py
--rw-rw-rw-   0        0        0     2527 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/steel/steelutil.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/symbol.py
--rw-rw-rw-   0        0        0      126 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/test.py
--rw-rw-rw-   0        0        0    35253 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/unit_converter.py
--rw-rw-rw-   0        0        0    19024 2024-05-14 08:44:17.000000 mapieng-0.1.1/base/vector.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.235845 mapieng-0.1.1/mapieng.egg-info/
--rw-rw-rw-   0        0        0      326 2024-05-14 08:45:04.000000 mapieng-0.1.1/mapieng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2024-05-14 08:45:05.000000 mapieng-0.1.1/mapieng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 08:45:04.000000 mapieng-0.1.1/mapieng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-14 08:45:04.000000 mapieng-0.1.1/mapieng.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-14 08:45:04.000000 mapieng-0.1.1/mapieng.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.226336 mapieng-0.1.1/project/
--rw-rw-rw-   0        0        0        0 2024-05-14 08:44:18.000000 mapieng-0.1.1/project/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.230845 mapieng-0.1.1/project/baseplate_KDS41_30_2022/
--rw-rw-rw-   0        0        0        0 2024-05-14 08:44:18.000000 mapieng-0.1.1/project/baseplate_KDS41_30_2022/__init__.py
--rw-rw-rw-   0        0        0     5747 2024-05-14 08:44:18.000000 mapieng-0.1.1/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
--rw-rw-rw-   0        0        0     7275 2024-05-14 08:44:18.000000 mapieng-0.1.1/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
--rw-rw-rw-   0        0        0       42 2024-05-14 08:45:05.239846 mapieng-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      547 2024-05-14 08:44:53.000000 mapieng-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 08:45:05.233845 mapieng-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-05-14 08:44:18.000000 mapieng-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0      808 2024-05-14 08:44:18.000000 mapieng-0.1.1/tests/test_baseplate_kds.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.416991 mapieng-0.1.2/
+-rw-rw-rw-   0        0        0       49 2024-05-23 05:53:17.000000 mapieng-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7146 2024-05-23 06:03:49.414990 mapieng-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7292 2024-05-17 06:44:23.000000 mapieng-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.389849 mapieng-0.1.2/base/
+-rw-rw-rw-   0        0        0     2993 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/ReportUtil.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.2/base/__init__.py
+-rw-rw-rw-   0        0        0     8187 2024-05-17 07:41:47.000000 mapieng-0.1.2/base/baseformidasapi.py
+-rw-rw-rw-   0        0        0    18374 2024-04-23 03:19:00.000000 mapieng-0.1.2/base/calculator_asd.py
+-rw-rw-rw-   0        0        0     1510 2024-05-20 02:33:29.000000 mapieng-0.1.2/base/dgncodeutil.py
+-rw-rw-rw-   0        0        0       47 2024-05-17 06:44:23.000000 mapieng-0.1.2/base/engineers.py
+-rw-rw-rw-   0        0        0     8194 2024-04-23 03:16:42.000000 mapieng-0.1.2/base/geometry.py
+-rw-rw-rw-   0        0        0    13475 2024-04-04 07:56:20.000000 mapieng-0.1.2/base/hello.html
+-rw-rw-rw-   0        0        0      961 2024-04-15 02:58:29.000000 mapieng-0.1.2/base/meshutil.py
+-rw-rw-rw-   0        0        0    14602 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/midasapi.py
+-rw-rw-rw-   0        0        0     9039 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/midasapi.pyi
+-rw-rw-rw-   0        0        0     3153 2024-05-17 06:44:23.000000 mapieng-0.1.2/base/midasutil.py
+-rw-rw-rw-   0        0        0     1967 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/midasutil_server.py
+-rw-rw-rw-   0        0        0     3607 2024-05-17 06:44:23.000000 mapieng-0.1.2/base/midasutil_web.py
+-rw-rw-rw-   0        0        0     1275 2024-05-23 05:53:17.000000 mapieng-0.1.2/base/section_property.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.393847 mapieng-0.1.2/base/steel/
+-rw-rw-rw-   0        0        0     1141 2024-04-05 06:25:39.000000 mapieng-0.1.2/base/steel/KS18.json
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.2/base/steel/__init__.py
+-rw-rw-rw-   0        0        0     2527 2024-04-23 03:19:00.000000 mapieng-0.1.2/base/steel/steelutil.py
+-rw-rw-rw-   0        0        0     1100 2024-04-05 06:25:39.000000 mapieng-0.1.2/base/symbol.py
+-rw-rw-rw-   0        0        0       94 2024-05-17 06:44:23.000000 mapieng-0.1.2/base/test.py
+-rw-rw-rw-   0        0        0      502 2024-04-15 01:54:35.000000 mapieng-0.1.2/base/testmesh.py
+-rw-rw-rw-   0        0        0    35253 2024-04-15 07:11:36.000000 mapieng-0.1.2/base/unit_converter.py
+-rw-rw-rw-   0        0        0    19024 2024-04-04 07:56:20.000000 mapieng-0.1.2/base/vector.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.413991 mapieng-0.1.2/mapieng.egg-info/
+-rw-rw-rw-   0        0        0     7146 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 06:03:49.000000 mapieng-0.1.2/mapieng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.402992 mapieng-0.1.2/project/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:56:24.000000 mapieng-0.1.2/project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.407994 mapieng-0.1.2/project/baseplate_KDS41_30_2022/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:07:01.000000 mapieng-0.1.2/project/baseplate_KDS41_30_2022/__init__.py
+-rw-rw-rw-   0        0        0     5747 2024-04-22 08:16:48.000000 mapieng-0.1.2/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py
+-rw-rw-rw-   0        0        0     7275 2024-04-19 01:44:54.000000 mapieng-0.1.2/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.408992 mapieng-0.1.2/project/sectionproperty/
+-rw-rw-rw-   0        0        0      485 2024-05-23 05:53:17.000000 mapieng-0.1.2/project/sectionproperty/report_sectionproperty.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:03:49.417992 mapieng-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      606 2024-05-23 06:03:03.000000 mapieng-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:03:49.411991 mapieng-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:02:44.000000 mapieng-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2219 2024-05-23 05:53:17.000000 mapieng-0.1.2/tests/test_baseplate_kds.py
```

### Comparing `mapieng-0.1.1/base/ReportUtil.py` & `mapieng-0.1.2/base/ReportUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def add_image(self, path, image_text=""):
         self.new_line(self.new_inline_image(text=image_text, path=path))
 
     def add_line_svu(self, str, value, unit):
         self.new_line(f"{str} {value} {self.get_str_unit(unit)}")
 
     def add_line_fvu(self, formula, value, unit):
-        self.new_line(f"{self.add_formula(formula)} = {value} {self.get_str_unit(unit)}")
+        self.new_line(f"{self.add_formula(formula)} = {value :.2f} {self.get_str_unit(unit)}")
 
     def add_line(self, text):
         self.new_line(text)
 
     def add_formula(self, text):
         return f"${text}$"
```

### Comparing `mapieng-0.1.1/base/baseformidasapi.py` & `mapieng-0.1.2/base/baseformidasapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,23 @@
         return midas_util.put(url, headers=g_headers, json={'Assign': items})
 
     def db_update_item(item_name, item_id, item):
         url = f'{g_base_url}/db/{item_name}/{item_id}'
         return midas_util.put(url, headers=g_headers, json={'Assign': item})
 
     def db_delete(item_name, item_id):
+        """_summary_
+        
+        Args:
+            item_name : _description_
+            item_id : _description_
+        
+        Returns:
+            _type_: _description_
+        """        
         url = f'{g_base_url}/db/{item_name}/{item_id}'
         return midas_util.delete(url, headers=g_headers)
 
     def db_get_next_id(item_name):
         res_all = midas_util.db_read(item_name)
         if not res_all:
             return 1
```

### Comparing `mapieng-0.1.1/base/calculator_asd.py` & `mapieng-0.1.2/base/calculator_asd.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/base/geometry.py` & `mapieng-0.1.2/base/geometry.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/base/hello.html` & `mapieng-0.1.2/base/hello.html`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/base/midasutil.py` & `mapieng-0.1.2/base/midasutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,16 +86,7 @@
 		except requests.exceptions.RequestException as e:
 			return midas_util.ERROR_DICT(postfix=url)
 
 
 class Product(Enum):
     CIVIL = 1,
     GEN = 2,
-
-# from base.engineers import midas_util, Product
-
-global g_base_url, g_headers
-g_base_url = midas_util.get_base_url(Product.CIVIL, "KR")   
-g_headers = {
-	'MAPI-Key': midas_util.get_MAPI_Key(Product.CIVIL, "KR"),
-	'Content-Type': 'application/json'
-}
```

### Comparing `mapieng-0.1.1/base/steel/KS18.json` & `mapieng-0.1.2/base/steel/KS18.json`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/base/steel/steelutil.py` & `mapieng-0.1.2/base/steel/steelutil.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/base/symbol.py` & `mapieng-0.1.2/base/symbol.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/base/unit_converter.py` & `mapieng-0.1.2/base/unit_converter.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/base/vector.py` & `mapieng-0.1.2/base/vector.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py` & `mapieng-0.1.2/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_calc.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py` & `mapieng-0.1.2/project/baseplate_KDS41_30_2022/baseplate_KDS41_30_2022_report.py`

 * *Files identical despite different names*

### Comparing `mapieng-0.1.1/setup.py` & `mapieng-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 def readme():
-    with open('README.md') as f:
+    with open('README_en.md', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='mapieng',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     include_package_data=True,
     description='mapi engineers',
-    long_description=open('README.md').read(),
+    long_description=readme(),
     long_description_content_type='text/markdown',
     license='MIT',
     author='bschoi',
     url='https://github.com/MIDASIT-Co-Ltd/engineers-api-python',
-    install_requires=['mdutils', "numpy", "matplotlib",],
+    install_requires=['mdutils', "numpy", "matplotlib", "sectionproperties", "concreteproperties", "requests"],
     )
```

