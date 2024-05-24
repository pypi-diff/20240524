# Comparing `tmp/SIST02_converter-0.1.0.tar.gz` & `tmp/SIST02_converter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIST02_converter-0.1.0.tar", last modified: Fri May 24 09:05:08 2024, max compression
+gzip compressed data, was "SIST02_converter-0.1.1.tar", last modified: Fri May 24 09:12:42 2024, max compression
```

## Comparing `SIST02_converter-0.1.0.tar` & `SIST02_converter-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:05:08.466858 SIST02_converter-0.1.0/
--rw-r--r--   0 yasufumi   (501) staff       (20)     1367 2024-05-24 09:05:08.466734 SIST02_converter-0.1.0/PKG-INFO
--rw-r--r--   0 yasufumi   (501) staff       (20)     1158 2024-05-24 08:52:14.000000 SIST02_converter-0.1.0/README.md
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:05:08.465801 SIST02_converter-0.1.0/SIST02_converter/
--rw-r--r--   0 yasufumi   (501) staff       (20)       36 2024-05-24 08:35:45.000000 SIST02_converter-0.1.0/SIST02_converter/__init__.py
--rw-r--r--   0 yasufumi   (501) staff       (20)     2130 2024-05-24 08:52:33.000000 SIST02_converter-0.1.0/SIST02_converter/module.py
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:05:08.466459 SIST02_converter-0.1.0/SIST02_converter.egg-info/
--rw-r--r--   0 yasufumi   (501) staff       (20)     1367 2024-05-24 09:05:08.000000 SIST02_converter-0.1.0/SIST02_converter.egg-info/PKG-INFO
--rw-r--r--   0 yasufumi   (501) staff       (20)      234 2024-05-24 09:05:08.000000 SIST02_converter-0.1.0/SIST02_converter.egg-info/SOURCES.txt
--rw-r--r--   0 yasufumi   (501) staff       (20)        1 2024-05-24 09:05:08.000000 SIST02_converter-0.1.0/SIST02_converter.egg-info/dependency_links.txt
--rw-r--r--   0 yasufumi   (501) staff       (20)       17 2024-05-24 09:05:08.000000 SIST02_converter-0.1.0/SIST02_converter.egg-info/top_level.txt
--rw-r--r--   0 yasufumi   (501) staff       (20)       38 2024-05-24 09:05:08.467006 SIST02_converter-0.1.0/setup.cfg
--rw-r--r--   0 yasufumi   (501) staff       (20)      541 2024-05-24 09:00:56.000000 SIST02_converter-0.1.0/setup.py
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:12:42.231125 SIST02_converter-0.1.1/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1367 2024-05-24 09:12:42.230996 SIST02_converter-0.1.1/PKG-INFO
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1158 2024-05-24 08:52:14.000000 SIST02_converter-0.1.1/README.md
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:12:42.230228 SIST02_converter-0.1.1/SIST02_converter/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     2122 2024-05-24 09:11:07.000000 SIST02_converter-0.1.1/SIST02_converter/SIST02_convert_URL.py
+-rw-r--r--   0 yasufumi   (501) staff       (20)       43 2024-05-24 09:11:56.000000 SIST02_converter-0.1.1/SIST02_converter/__init__.py
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 09:12:42.230736 SIST02_converter-0.1.1/SIST02_converter.egg-info/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1367 2024-05-24 09:12:42.000000 SIST02_converter-0.1.1/SIST02_converter.egg-info/PKG-INFO
+-rw-r--r--   0 yasufumi   (501) staff       (20)      246 2024-05-24 09:12:42.000000 SIST02_converter-0.1.1/SIST02_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 yasufumi   (501) staff       (20)        1 2024-05-24 09:12:42.000000 SIST02_converter-0.1.1/SIST02_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 yasufumi   (501) staff       (20)       17 2024-05-24 09:12:42.000000 SIST02_converter-0.1.1/SIST02_converter.egg-info/top_level.txt
+-rw-r--r--   0 yasufumi   (501) staff       (20)       38 2024-05-24 09:12:42.231172 SIST02_converter-0.1.1/setup.cfg
+-rw-r--r--   0 yasufumi   (501) staff       (20)      541 2024-05-24 09:12:37.000000 SIST02_converter-0.1.1/setup.py
```

### Comparing `SIST02_converter-0.1.0/PKG-INFO` & `SIST02_converter-0.1.1/SIST02_converter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SIST02_converter
-Version: 0.1.0
+Name: SIST02-converter
+Version: 0.1.1
 Summary: Conversion of input URLs to SIST02 format.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### パッケージについて
```

### Comparing `SIST02_converter-0.1.0/README.md` & `SIST02_converter-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `SIST02_converter-0.1.0/SIST02_converter/module.py` & `SIST02_converter-0.1.1/SIST02_converter/SIST02_convert_URL.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from bs4 import BeautifulSoup
 from datetime import datetime
 
-def SIST02_convert_text(url):
+def Convert_URL(url):
     # HTTPリクエストを送信してページの内容を取得
     response = requests.get(url)
     response.raise_for_status()  # リクエストが成功したかどうかをチェック
 
     # BeautifulSoupを使用してページを解析
     soup = BeautifulSoup(response.content, 'html.parser')
```

### Comparing `SIST02_converter-0.1.0/SIST02_converter.egg-info/PKG-INFO` & `SIST02_converter-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SIST02-converter
-Version: 0.1.0
+Name: SIST02_converter
+Version: 0.1.1
 Summary: Conversion of input URLs to SIST02 format.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### パッケージについて
```

### Comparing `SIST02_converter-0.1.0/setup.py` & `SIST02_converter-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 setup(
     name="SIST02_converter",
-    version="0.1.0",
+    version="0.1.1",
     LICENSE = 'MIT',
     description="Conversion of input URLs to SIST02 format.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
```

