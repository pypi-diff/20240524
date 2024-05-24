# Comparing `tmp/holiday_predictor-0.11.1.tar.gz` & `tmp/holiday_predictor-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holiday_predictor-0.11.1.tar", last modified: Sun May 12 13:14:35 2024, max compression
+gzip compressed data, was "holiday_predictor-0.12.0.tar", last modified: Fri May 24 15:54:20 2024, max compression
```

## Comparing `holiday_predictor-0.11.1.tar` & `holiday_predictor-0.12.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 13:14:35.178931 holiday_predictor-0.11.1/
--rw-rw-rw-   0        0        0    35823 2024-05-10 06:09:49.000000 holiday_predictor-0.11.1/LICENSE
--rw-rw-rw-   0        0        0     3237 2024-05-12 13:14:35.176935 holiday_predictor-0.11.1/PKG-INFO
--rw-rw-rw-   0        0        0     2658 2024-05-12 13:11:17.000000 holiday_predictor-0.11.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 13:14:35.158224 holiday_predictor-0.11.1/holiday_predictor/
--rw-rw-rw-   0        0        0    12232 2024-05-12 13:11:17.000000 holiday_predictor-0.11.1/holiday_predictor/__init__.py
--rw-rw-rw-   0        0        0     2389 2024-05-12 13:11:17.000000 holiday_predictor-0.11.1/holiday_predictor/data.py
-drwxrwxrwx   0        0        0        0 2024-05-12 13:14:35.175937 holiday_predictor-0.11.1/holiday_predictor.egg-info/
--rw-rw-rw-   0        0        0     3237 2024-05-12 13:14:35.000000 holiday_predictor-0.11.1/holiday_predictor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-05-12 13:14:35.000000 holiday_predictor-0.11.1/holiday_predictor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 13:14:35.000000 holiday_predictor-0.11.1/holiday_predictor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-12 13:14:35.000000 holiday_predictor-0.11.1/holiday_predictor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-12 13:14:35.000000 holiday_predictor-0.11.1/holiday_predictor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 13:14:35.178931 holiday_predictor-0.11.1/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-12 13:12:00.000000 holiday_predictor-0.11.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:20.793403 holiday_predictor-0.12.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-10 06:09:49.000000 holiday_predictor-0.12.0/LICENSE
+-rw-rw-rw-   0        0        0     3237 2024-05-24 15:54:20.791408 holiday_predictor-0.12.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2658 2024-05-12 13:11:17.000000 holiday_predictor-0.12.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:20.776448 holiday_predictor-0.12.0/holiday_predictor/
+-rw-rw-rw-   0        0        0    12232 2024-05-24 14:58:46.000000 holiday_predictor-0.12.0/holiday_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2389 2024-05-12 13:11:17.000000 holiday_predictor-0.12.0/holiday_predictor/data.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:54:20.790413 holiday_predictor-0.12.0/holiday_predictor.egg-info/
+-rw-rw-rw-   0        0        0     3237 2024-05-24 15:54:20.000000 holiday_predictor-0.12.0/holiday_predictor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-24 15:54:20.000000 holiday_predictor-0.12.0/holiday_predictor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:54:20.000000 holiday_predictor-0.12.0/holiday_predictor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 15:54:20.000000 holiday_predictor-0.12.0/holiday_predictor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-24 15:54:20.000000 holiday_predictor-0.12.0/holiday_predictor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 15:54:20.793403 holiday_predictor-0.12.0/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-24 15:49:57.000000 holiday_predictor-0.12.0/setup.py
```

### Comparing `holiday_predictor-0.11.1/LICENSE` & `holiday_predictor-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `holiday_predictor-0.11.1/PKG-INFO` & `holiday_predictor-0.12.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holiday_predictor
-Version: 0.11.1
+Version: 0.12.0
 Summary: 一个预测中国的假期安排的小工具
 Home-page: https://github.com/azaz-az/holiday-predictor
 Author: azaz-az
 Author-email: a233d@outlook.com
 Keywords: holiday,predictor,holiday_predictor,chinese_holiday
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `holiday_predictor-0.11.1/README.md` & `holiday_predictor-0.12.0/README.md`

 * *Files identical despite different names*

### Comparing `holiday_predictor-0.11.1/holiday_predictor/__init__.py` & `holiday_predictor-0.12.0/holiday_predictor/__init__.py`

 * *Files identical despite different names*

### Comparing `holiday_predictor-0.11.1/holiday_predictor/data.py` & `holiday_predictor-0.12.0/holiday_predictor/data.py`

 * *Files identical despite different names*

### Comparing `holiday_predictor-0.11.1/holiday_predictor.egg-info/PKG-INFO` & `holiday_predictor-0.12.0/holiday_predictor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holiday_predictor
-Version: 0.11.1
+Version: 0.12.0
 Summary: 一个预测中国的假期安排的小工具
 Home-page: https://github.com/azaz-az/holiday-predictor
 Author: azaz-az
 Author-email: a233d@outlook.com
 Keywords: holiday,predictor,holiday_predictor,chinese_holiday
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `holiday_predictor-0.11.1/setup.py` & `holiday_predictor-0.12.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="holiday_predictor",
-    version="0.11.1",
+    version="0.12.0",
     author="azaz-az",
     author_email="a233d@outlook.com",
     description="一个预测中国的假期安排的小工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/azaz-az/holiday-predictor",
     packages=setuptools.find_packages(),
```

