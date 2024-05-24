# Comparing `tmp/color_change_filter-1.0.4.tar.gz` & `tmp/color_change_filter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color_change_filter-1.0.4.tar", last modified: Fri May 24 17:09:14 2024, max compression
+gzip compressed data, was "color_change_filter-1.0.5.tar", last modified: Fri May 24 17:21:11 2024, max compression
```

## Comparing `color_change_filter-1.0.4.tar` & `color_change_filter-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:09:14.022586 color_change_filter-1.0.4/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      937 2024-05-24 17:09:14.022359 color_change_filter-1.0.4/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      457 2024-05-24 16:47:02.000000 color_change_filter-1.0.4/README.md
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:02:26.000000 color_change_filter-1.0.4/__init__.py
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-24 17:09:14.022623 color_change_filter-1.0.4/setup.cfg
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      903 2024-05-24 17:08:32.000000 color_change_filter-1.0.4/setup.py
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:09:14.021314 color_change_filter-1.0.4/src/
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:09:14.022128 color_change_filter-1.0.4/src/color_change_filter.egg-info/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      937 2024-05-24 17:09:13.000000 color_change_filter-1.0.4/src/color_change_filter.egg-info/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      284 2024-05-24 17:09:14.000000 color_change_filter-1.0.4/src/color_change_filter.egg-info/SOURCES.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-24 17:09:13.000000 color_change_filter-1.0.4/src/color_change_filter.egg-info/dependency_links.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       54 2024-05-24 17:09:13.000000 color_change_filter-1.0.4/src/color_change_filter.egg-info/entry_points.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        9 2024-05-24 17:09:13.000000 color_change_filter-1.0.4/src/color_change_filter.egg-info/top_level.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4805 2024-05-24 17:01:29.000000 color_change_filter-1.0.4/src/program6.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:21:11.237092 color_change_filter-1.0.5/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       16 2024-05-24 16:02:48.000000 color_change_filter-1.0.5/.gitignore
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      937 2024-05-24 17:21:11.236833 color_change_filter-1.0.5/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      457 2024-05-24 16:47:02.000000 color_change_filter-1.0.5/README.md
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:02:26.000000 color_change_filter-1.0.5/__init__.py
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-24 17:21:11.237133 color_change_filter-1.0.5/setup.cfg
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      903 2024-05-24 17:21:04.000000 color_change_filter-1.0.5/setup.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:21:11.235548 color_change_filter-1.0.5/src/
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:21:11.236582 color_change_filter-1.0.5/src/color_change_filter.egg-info/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      937 2024-05-24 17:21:11.000000 color_change_filter-1.0.5/src/color_change_filter.egg-info/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      306 2024-05-24 17:21:11.000000 color_change_filter-1.0.5/src/color_change_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-24 17:21:11.000000 color_change_filter-1.0.5/src/color_change_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       54 2024-05-24 17:21:11.000000 color_change_filter-1.0.5/src/color_change_filter.egg-info/entry_points.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        9 2024-05-24 17:21:11.000000 color_change_filter-1.0.5/src/color_change_filter.egg-info/top_level.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4805 2024-05-24 17:01:29.000000 color_change_filter-1.0.5/src/color_change_filter.py
```

### Comparing `color_change_filter-1.0.4/PKG-INFO` & `color_change_filter-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.0.4
+Version: 1.0.5
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `color_change_filter-1.0.4/setup.py` & `color_change_filter-1.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r",encoding="UTF-8") as fh:
     long_description = fh.read()
 setuptools.setup(
   name="color_change_filter",
-  version="1.0.4",
+  version="1.0.5",
   author="Chihiro senbonmatsu",
   author_email="s2222020@stu.musahino-u.ac.jp",
   description="Change color of image",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/senbonmatsu/color_changer",
   project_urls={
```

### Comparing `color_change_filter-1.0.4/src/color_change_filter.egg-info/PKG-INFO` & `color_change_filter-1.0.5/src/color_change_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.0.4
+Version: 1.0.5
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `color_change_filter-1.0.4/src/program6.py` & `color_change_filter-1.0.5/src/color_change_filter.py`

 * *Files identical despite different names*

