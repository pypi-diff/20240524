# Comparing `tmp/color_change_filter-1.0.9.tar.gz` & `tmp/color_change_filter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color_change_filter-1.0.9.tar", last modified: Fri May 24 17:46:09 2024, max compression
+gzip compressed data, was "color_change_filter-1.1.0.tar", last modified: Fri May 24 18:26:44 2024, max compression
```

## Comparing `color_change_filter-1.0.9.tar` & `color_change_filter-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:46:09.176286 color_change_filter-1.0.9/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       16 2024-05-24 16:02:48.000000 color_change_filter-1.0.9/.gitignore
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 17:46:09.176070 color_change_filter-1.0.9/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      457 2024-05-24 16:47:02.000000 color_change_filter-1.0.9/README.md
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-24 17:46:09.176322 color_change_filter-1.0.9/setup.cfg
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      984 2024-05-24 17:45:58.000000 color_change_filter-1.0.9/setup.py
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:46:09.174689 color_change_filter-1.0.9/src/
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:46:09.175832 color_change_filter-1.0.9/src/color_change_filter.egg-info/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      340 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/SOURCES.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/dependency_links.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/entry_points.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/requires.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        9 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/top_level.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4805 2024-05-24 17:01:29.000000 color_change_filter-1.0.9/src/color_change_filter.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 18:26:44.686449 color_change_filter-1.1.0/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       24 2024-05-24 18:09:24.000000 color_change_filter-1.1.0/.gitignore
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 18:26:44.686245 color_change_filter-1.1.0/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      457 2024-05-24 16:47:02.000000 color_change_filter-1.1.0/README.md
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-24 18:26:44.686483 color_change_filter-1.1.0/setup.cfg
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      984 2024-05-24 18:26:28.000000 color_change_filter-1.1.0/setup.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 18:26:44.685295 color_change_filter-1.1.0/src/
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 18:26:44.685997 color_change_filter-1.1.0/src/color_change_filter.egg-info/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 18:26:44.000000 color_change_filter-1.1.0/src/color_change_filter.egg-info/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      340 2024-05-24 18:26:44.000000 color_change_filter-1.1.0/src/color_change_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-24 18:26:44.000000 color_change_filter-1.1.0/src/color_change_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-24 18:26:44.000000 color_change_filter-1.1.0/src/color_change_filter.egg-info/entry_points.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-24 18:26:44.000000 color_change_filter-1.1.0/src/color_change_filter.egg-info/requires.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        9 2024-05-24 18:26:44.000000 color_change_filter-1.1.0/src/color_change_filter.egg-info/top_level.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4805 2024-05-24 17:01:29.000000 color_change_filter-1.1.0/src/color_change_filter.py
```

### Comparing `color_change_filter-1.0.9/PKG-INFO` & `color_change_filter-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.0.9
+Version: 1.1.0
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `color_change_filter-1.0.9/setup.py` & `color_change_filter-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r",encoding="UTF-8") as fh:
     long_description = fh.read()
 setuptools.setup(
   name="color_change_filter",
-  version="1.0.9",
+  version="1.1.0",
   author="Chihiro senbonmatsu",
   author_email="s2222020@stu.musahino-u.ac.jp",
   description="Change color of image",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/senbonmatsu/color_changer",
   project_urls={
```

### Comparing `color_change_filter-1.0.9/src/color_change_filter.egg-info/PKG-INFO` & `color_change_filter-1.1.0/src/color_change_filter.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: color_change_filter
-Version: 1.0.9
+Name: color-change-filter
+Version: 1.1.0
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `color_change_filter-1.0.9/src/color_change_filter.py` & `color_change_filter-1.1.0/src/color_change_filter.py`

 * *Files identical despite different names*

