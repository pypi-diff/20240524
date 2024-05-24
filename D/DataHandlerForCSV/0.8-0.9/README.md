# Comparing `tmp/DataHandlerForCSV-0.8.tar.gz` & `tmp/datahandlerforcsv-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataHandlerForCSV-0.8.tar", last modified: Thu May 23 15:42:14 2024, max compression
+gzip compressed data, was "datahandlerforcsv-0.9.tar", last modified: Thu May 23 17:22:01 2024, max compression
```

## Comparing `DataHandlerForCSV-0.8.tar` & `datahandlerforcsv-0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 15:42:14.257873 DataHandlerForCSV-0.8/
--rw-rw-rw-   0        0        0      486 2024-05-23 15:42:14.256868 DataHandlerForCSV-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 15:42:14.239930 DataHandlerForCSV-0.8/pypi/
-drwxrwxrwx   0        0        0        0 2024-05-23 15:42:14.256868 DataHandlerForCSV-0.8/pypi/DataHandlerForCSV.egg-info/
--rw-rw-rw-   0        0        0      486 2024-05-23 15:42:14.000000 DataHandlerForCSV-0.8/pypi/DataHandlerForCSV.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-23 15:42:14.000000 DataHandlerForCSV-0.8/pypi/DataHandlerForCSV.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 15:42:14.000000 DataHandlerForCSV-0.8/pypi/DataHandlerForCSV.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 15:42:14.000000 DataHandlerForCSV-0.8/pypi/DataHandlerForCSV.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 15:42:14.257873 DataHandlerForCSV-0.8/setup.cfg
--rw-rw-rw-   0        0        0      743 2024-05-23 15:41:54.000000 DataHandlerForCSV-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:22:01.543049 datahandlerforcsv-0.9/
+-rw-rw-rw-   0        0        0     1193 2024-05-23 17:22:01.541571 datahandlerforcsv-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 17:22:01.532571 datahandlerforcsv-0.9/pypi/
+drwxrwxrwx   0        0        0        0 2024-05-23 17:22:01.540572 datahandlerforcsv-0.9/pypi/DataHandlerForCSV.egg-info/
+-rw-rw-rw-   0        0        0     1193 2024-05-23 17:22:01.000000 datahandlerforcsv-0.9/pypi/DataHandlerForCSV.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-23 17:22:01.000000 datahandlerforcsv-0.9/pypi/DataHandlerForCSV.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:22:01.000000 datahandlerforcsv-0.9/pypi/DataHandlerForCSV.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:22:01.000000 datahandlerforcsv-0.9/pypi/DataHandlerForCSV.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:22:01.543049 datahandlerforcsv-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      743 2024-05-23 17:20:42.000000 datahandlerforcsv-0.9/setup.py
```

### Comparing `DataHandlerForCSV-0.8/setup.py` & `datahandlerforcsv-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("pypi/README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="DataHandlerForCSV",
-    version="0.8",
+    version="0.9",
     description="data cleaner",
     package_dir={"": "pypi"},
     packages=find_packages(where="pypi"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CorbeauDistingue/dataHandlerCSV/tree/main",
     author="Burak Nafi Girgin",
```

