# Comparing `tmp/mdod-0.1.7.tar.gz` & `tmp/mdod-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdod-0.1.7.tar", last modified: Sun Apr 21 05:06:04 2024, max compression
+gzip compressed data, was "mdod-0.1.8.tar", last modified: Fri May 24 13:48:35 2024, max compression
```

## Comparing `mdod-0.1.7.tar` & `mdod-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 05:06:04.199370 mdod-0.1.7/
--rw-rw-rw-   0        0        0     1492 2024-04-15 08:05:38.000000 mdod-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0      609 2024-04-21 05:06:04.179650 mdod-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1084 2024-04-21 04:47:37.000000 mdod-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 05:06:04.099636 mdod-0.1.7/mdod/
--rw-rw-rw-   0        0        0       71 2024-04-15 15:08:34.000000 mdod-0.1.7/mdod/__init__.py
--rw-rw-rw-   0        0        0     2400 2024-04-02 04:07:58.000000 mdod-0.1.7/mdod/mdod.py
-drwxrwxrwx   0        0        0        0 2024-04-21 05:06:04.169396 mdod-0.1.7/mdod.egg-info/
--rw-rw-rw-   0        0        0      609 2024-04-21 05:06:03.000000 mdod-0.1.7/mdod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-21 05:06:03.000000 mdod-0.1.7/mdod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 05:06:03.000000 mdod-0.1.7/mdod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-21 05:06:03.000000 mdod-0.1.7/mdod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 05:06:04.199370 mdod-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      809 2024-04-21 04:53:24.000000 mdod-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:48:35.589478 mdod-0.1.8/
+-rw-rw-rw-   0        0        0     1492 2024-04-15 08:05:38.000000 mdod-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      630 2024-05-24 13:48:35.587456 mdod-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2024-05-24 12:46:30.000000 mdod-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 13:48:35.583456 mdod-0.1.8/mdod/
+-rw-rw-rw-   0        0        0       71 2024-04-15 15:08:34.000000 mdod-0.1.8/mdod/__init__.py
+-rw-rw-rw-   0        0        0     2400 2024-04-02 04:07:58.000000 mdod-0.1.8/mdod/mdod.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:48:35.586457 mdod-0.1.8/mdod.egg-info/
+-rw-rw-rw-   0        0        0      630 2024-05-24 13:48:35.000000 mdod-0.1.8/mdod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-05-24 13:48:35.000000 mdod-0.1.8/mdod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 13:48:35.000000 mdod-0.1.8/mdod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-24 13:48:35.000000 mdod-0.1.8/mdod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 13:48:35.590460 mdod-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      809 2024-05-24 12:46:09.000000 mdod-0.1.8/setup.py
```

### Comparing `mdod-0.1.7/LICENSE.txt` & `mdod-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mdod-0.1.7/PKG-INFO` & `mdod-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: mdod
-Version: 0.1.7
+Version: 0.1.8
 Summary: MDOD, Multi-Dimensional data Outlier Detection
 Home-page: https://github.com/mddod/mdod
 Author: Z Shen
 Author-email: 626456708@qq.com
 License: BSD 3-Clause License
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm. For details please read README.md ,  or visit https://github.com/mddod/mdod
+
```

### Comparing `mdod-0.1.7/README.md` & `mdod-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 [data1 data2 data3 data4 data5 data6] 
 
 [data1 data2 data3 data4 data5 data6] 
 
 ...]
 
-# rusult format:
+# result format:
 [value1, '[data1 data2 data3 data4 data5 data6]', '0']
 
 [value2, '[data1 data2 data3 data4 data5 data6]', '1']
 
 [value3, '[data1 data2 data3 data4 data5 data6]', '2']
 
 ...
```

### Comparing `mdod-0.1.7/mdod/mdod.py` & `mdod-0.1.8/mdod/mdod.py`

 * *Files identical despite different names*

### Comparing `mdod-0.1.7/mdod.egg-info/PKG-INFO` & `mdod-0.1.8/mdod.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: mdod
-Version: 0.1.7
+Version: 0.1.8
 Summary: MDOD, Multi-Dimensional data Outlier Detection
 Home-page: https://github.com/mddod/mdod
 Author: Z Shen
 Author-email: 626456708@qq.com
 License: BSD 3-Clause License
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 Python library for Multi-Dimensional data Outlier/Anomaly Detection algorithm. For details please read README.md ,  or visit https://github.com/mddod/mdod
+
```

### Comparing `mdod-0.1.7/setup.py` & `mdod-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mdod",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     package_data={"": ["*"]},  
     install_requires=[
         '',
     ],
     author="Z Shen",
     author_email="626456708@qq.com",
```

