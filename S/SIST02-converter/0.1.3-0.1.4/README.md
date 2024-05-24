# Comparing `tmp/SIST02-Converter-0.1.3.tar.gz` & `tmp/SIST02-converter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIST02-Converter-0.1.3.tar", last modified: Fri May 24 11:15:29 2024, max compression
+gzip compressed data, was "SIST02-converter-0.1.4.tar", last modified: Fri May 24 11:23:59 2024, max compression
```

## Comparing `SIST02-Converter-0.1.3.tar` & `SIST02-converter-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:15:29.426913 SIST02-Converter-0.1.3/
--rw-r--r--   0 yasufumi   (501) staff       (20)     1371 2024-05-24 11:15:29.426755 SIST02-Converter-0.1.3/PKG-INFO
--rw-r--r--   0 yasufumi   (501) staff       (20)     1164 2024-05-24 11:15:00.000000 SIST02-Converter-0.1.3/README.md
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:15:29.425867 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/
--rw-r--r--   0 yasufumi   (501) staff       (20)     1371 2024-05-24 11:15:29.000000 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/PKG-INFO
--rw-r--r--   0 yasufumi   (501) staff       (20)      246 2024-05-24 11:15:29.000000 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/SOURCES.txt
--rw-r--r--   0 yasufumi   (501) staff       (20)        1 2024-05-24 11:15:29.000000 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/dependency_links.txt
--rw-r--r--   0 yasufumi   (501) staff       (20)       17 2024-05-24 11:15:29.000000 SIST02-Converter-0.1.3/SIST02_Converter.egg-info/top_level.txt
-drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:15:29.426399 SIST02-Converter-0.1.3/SIST02_converter/
--rw-r--r--   0 yasufumi   (501) staff       (20)     2122 2024-05-24 09:11:07.000000 SIST02-Converter-0.1.3/SIST02_converter/SIST02_convert_URL.py
--rw-r--r--   0 yasufumi   (501) staff       (20)       43 2024-05-24 09:11:56.000000 SIST02-Converter-0.1.3/SIST02_converter/__init__.py
--rw-r--r--   0 yasufumi   (501) staff       (20)       38 2024-05-24 11:15:29.426972 SIST02-Converter-0.1.3/setup.cfg
--rw-r--r--   0 yasufumi   (501) staff       (20)      539 2024-05-24 11:15:14.000000 SIST02-Converter-0.1.3/setup.py
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:23:59.342943 SIST02-converter-0.1.4/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1371 2024-05-24 11:23:59.342811 SIST02-converter-0.1.4/PKG-INFO
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1164 2024-05-24 11:15:00.000000 SIST02-converter-0.1.4/README.md
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:23:59.342131 SIST02-converter-0.1.4/SIST02_converter/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     2122 2024-05-24 09:11:07.000000 SIST02-converter-0.1.4/SIST02_converter/SIST02_convert_URL.py
+-rw-r--r--   0 yasufumi   (501) staff       (20)       43 2024-05-24 09:11:56.000000 SIST02-converter-0.1.4/SIST02_converter/__init__.py
+drwxr-xr-x   0 yasufumi   (501) staff       (20)        0 2024-05-24 11:23:59.342652 SIST02-converter-0.1.4/SIST02_converter.egg-info/
+-rw-r--r--   0 yasufumi   (501) staff       (20)     1371 2024-05-24 11:23:59.000000 SIST02-converter-0.1.4/SIST02_converter.egg-info/PKG-INFO
+-rw-r--r--   0 yasufumi   (501) staff       (20)      246 2024-05-24 11:23:59.000000 SIST02-converter-0.1.4/SIST02_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 yasufumi   (501) staff       (20)        1 2024-05-24 11:23:59.000000 SIST02-converter-0.1.4/SIST02_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 yasufumi   (501) staff       (20)       17 2024-05-24 11:23:59.000000 SIST02-converter-0.1.4/SIST02_converter.egg-info/top_level.txt
+-rw-r--r--   0 yasufumi   (501) staff       (20)       38 2024-05-24 11:23:59.342986 SIST02-converter-0.1.4/setup.cfg
+-rw-r--r--   0 yasufumi   (501) staff       (20)      539 2024-05-24 11:23:54.000000 SIST02-converter-0.1.4/setup.py
```

### Comparing `SIST02-Converter-0.1.3/PKG-INFO` & `SIST02-converter-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SIST02-Converter
-Version: 0.1.3
+Name: SIST02-converter
+Version: 0.1.4
 Summary: Conversion of input URL to SIST02 style.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### パッケージについて
```

### Comparing `SIST02-Converter-0.1.3/README.md` & `SIST02-converter-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `SIST02-Converter-0.1.3/SIST02_Converter.egg-info/PKG-INFO` & `SIST02-converter-0.1.4/SIST02_converter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SIST02-Converter
-Version: 0.1.3
+Name: SIST02-converter
+Version: 0.1.4
 Summary: Conversion of input URL to SIST02 style.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ### パッケージについて
```

### Comparing `SIST02-Converter-0.1.3/SIST02_converter/SIST02_convert_URL.py` & `SIST02-converter-0.1.4/SIST02_converter/SIST02_convert_URL.py`

 * *Files identical despite different names*

### Comparing `SIST02-Converter-0.1.3/setup.py` & `SIST02-converter-0.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 setup(
-    name="SIST02-Converter",
-    version="0.1.3",
+    name="SIST02-converter",
+    version="0.1.4",
     LICENSE = 'MIT',
     description="Conversion of input URL to SIST02 style.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
```

