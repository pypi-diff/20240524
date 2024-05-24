# Comparing `tmp/color_change_filter-1.0.8.tar.gz` & `tmp/color_change_filter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "color_change_filter-1.0.8.tar", last modified: Fri May 24 17:36:53 2024, max compression
+gzip compressed data, was "color_change_filter-1.0.9.tar", last modified: Fri May 24 17:46:09 2024, max compression
```

## Comparing `color_change_filter-1.0.8.tar` & `color_change_filter-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:36:53.896599 color_change_filter-1.0.8/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       16 2024-05-24 16:02:48.000000 color_change_filter-1.0.8/.gitignore
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 17:36:53.896370 color_change_filter-1.0.8/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      457 2024-05-24 16:47:02.000000 color_change_filter-1.0.8/README.md
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-24 17:36:53.896638 color_change_filter-1.0.8/setup.cfg
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      973 2024-05-24 17:36:26.000000 color_change_filter-1.0.8/setup.py
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:36:53.894869 color_change_filter-1.0.8/src/
-drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:36:53.896080 color_change_filter-1.0.8/src/color_change_filter.egg-info/
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 17:36:53.000000 color_change_filter-1.0.8/src/color_change_filter.egg-info/PKG-INFO
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      340 2024-05-24 17:36:53.000000 color_change_filter-1.0.8/src/color_change_filter.egg-info/SOURCES.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-24 17:36:53.000000 color_change_filter-1.0.8/src/color_change_filter.egg-info/dependency_links.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       54 2024-05-24 17:36:53.000000 color_change_filter-1.0.8/src/color_change_filter.egg-info/entry_points.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-24 17:36:53.000000 color_change_filter-1.0.8/src/color_change_filter.egg-info/requires.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        9 2024-05-24 17:36:53.000000 color_change_filter-1.0.8/src/color_change_filter.egg-info/top_level.txt
--rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4805 2024-05-24 17:01:29.000000 color_change_filter-1.0.8/src/color_change_filter.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:46:09.176286 color_change_filter-1.0.9/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       16 2024-05-24 16:02:48.000000 color_change_filter-1.0.9/.gitignore
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 17:46:09.176070 color_change_filter-1.0.9/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      457 2024-05-24 16:47:02.000000 color_change_filter-1.0.9/README.md
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       38 2024-05-24 17:46:09.176322 color_change_filter-1.0.9/setup.cfg
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      984 2024-05-24 17:45:58.000000 color_change_filter-1.0.9/setup.py
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:46:09.174689 color_change_filter-1.0.9/src/
+drwxr-xr-x   0 senbonmatsuchihiro   (501) staff       (20)        0 2024-05-24 17:46:09.175832 color_change_filter-1.0.9/src/color_change_filter.egg-info/
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      987 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/PKG-INFO
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)      340 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        1 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       65 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/entry_points.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)       20 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/requires.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)        9 2024-05-24 17:46:09.000000 color_change_filter-1.0.9/src/color_change_filter.egg-info/top_level.txt
+-rw-r--r--   0 senbonmatsuchihiro   (501) staff       (20)     4805 2024-05-24 17:01:29.000000 color_change_filter-1.0.9/src/color_change_filter.py
```

### Comparing `color_change_filter-1.0.8/PKG-INFO` & `color_change_filter-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.0.8
+Version: 1.0.9
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `color_change_filter-1.0.8/setup.py` & `color_change_filter-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r",encoding="UTF-8") as fh:
     long_description = fh.read()
 setuptools.setup(
   name="color_change_filter",
-  version="1.0.8",
+  version="1.0.9",
   author="Chihiro senbonmatsu",
   author_email="s2222020@stu.musahino-u.ac.jp",
   description="Change color of image",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/senbonmatsu/color_changer",
   project_urls={
@@ -25,11 +25,11 @@
     ],
   package_dir={"": "src"},
   py_modules=["program6"],
   packages=setuptools.find_packages(where="src"),
   Python_requires=">=3.6",
   entry_points={
     "console_scripts": [
-      "color_change_filter = program6:main",
+      "color_change_filter = color_change_filter:main",
     ],
   },
 )
```

### Comparing `color_change_filter-1.0.8/src/color_change_filter.egg-info/PKG-INFO` & `color_change_filter-1.0.9/src/color_change_filter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: color_change_filter
-Version: 1.0.8
+Version: 1.0.9
 Summary: Change color of image
 Home-page: https://github.com/senbonmatsu/color_changer
 Author: Chihiro senbonmatsu
 Author-email: s2222020@stu.musahino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/senbonmatsu/color_changer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `color_change_filter-1.0.8/src/color_change_filter.py` & `color_change_filter-1.0.9/src/color_change_filter.py`

 * *Files identical despite different names*

