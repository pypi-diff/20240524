# Comparing `tmp/unprint-0.0.2.tar.gz` & `tmp/unprint-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unprint-0.0.2.tar", last modified: Fri May 24 11:46:16 2024, max compression
+gzip compressed data, was "unprint-0.0.4.tar", last modified: Fri May 24 12:04:38 2024, max compression
```

## Comparing `unprint-0.0.2.tar` & `unprint-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 11:46:16.039829 unprint-0.0.2/
--rw-r--r--   0 lzl        (501) staff       (20)        0 2024-05-24 11:43:40.000000 unprint-0.0.2/LICENSE
--rw-r--r--   0 lzl        (501) staff       (20)      560 2024-05-24 11:46:16.039570 unprint-0.0.2/PKG-INFO
--rw-r--r--   0 lzl        (501) staff       (20)       45 2024-05-24 11:23:44.000000 unprint-0.0.2/README.md
--rw-r--r--   0 lzl        (501) staff       (20)       84 2024-05-24 11:24:20.000000 unprint-0.0.2/pyproject.toml
--rw-r--r--   0 lzl        (501) staff       (20)       38 2024-05-24 11:46:16.039881 unprint-0.0.2/setup.cfg
--rw-r--r--   0 lzl        (501) staff       (20)      836 2024-05-24 11:45:01.000000 unprint-0.0.2/setup.py
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 11:46:16.038272 unprint-0.0.2/src/
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 11:46:16.039358 unprint-0.0.2/src/unprint.egg-info/
--rw-r--r--   0 lzl        (501) staff       (20)      560 2024-05-24 11:46:16.000000 unprint-0.0.2/src/unprint.egg-info/PKG-INFO
--rw-r--r--   0 lzl        (501) staff       (20)      181 2024-05-24 11:46:16.000000 unprint-0.0.2/src/unprint.egg-info/SOURCES.txt
--rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 11:46:16.000000 unprint-0.0.2/src/unprint.egg-info/dependency_links.txt
--rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 11:46:16.000000 unprint-0.0.2/src/unprint.egg-info/top_level.txt
+drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 12:04:38.301885 unprint-0.0.4/
+-rw-r--r--   0 lzl        (501) staff       (20)        0 2024-05-24 11:43:40.000000 unprint-0.0.4/LICENSE
+-rw-r--r--   0 lzl        (501) staff       (20)      560 2024-05-24 12:04:38.301653 unprint-0.0.4/PKG-INFO
+-rw-r--r--   0 lzl        (501) staff       (20)       45 2024-05-24 11:23:44.000000 unprint-0.0.4/README.md
+-rw-r--r--   0 lzl        (501) staff       (20)       84 2024-05-24 11:24:20.000000 unprint-0.0.4/pyproject.toml
+-rw-r--r--   0 lzl        (501) staff       (20)       38 2024-05-24 12:04:38.301930 unprint-0.0.4/setup.cfg
+-rw-r--r--   0 lzl        (501) staff       (20)      836 2024-05-24 12:04:27.000000 unprint-0.0.4/setup.py
+drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 12:04:38.300444 unprint-0.0.4/src/
+drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 12:04:38.301460 unprint-0.0.4/src/unprint.egg-info/
+-rw-r--r--   0 lzl        (501) staff       (20)      560 2024-05-24 12:04:38.000000 unprint-0.0.4/src/unprint.egg-info/PKG-INFO
+-rw-r--r--   0 lzl        (501) staff       (20)      181 2024-05-24 12:04:38.000000 unprint-0.0.4/src/unprint.egg-info/SOURCES.txt
+-rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 12:04:38.000000 unprint-0.0.4/src/unprint.egg-info/dependency_links.txt
+-rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 12:04:38.000000 unprint-0.0.4/src/unprint.egg-info/top_level.txt
```

### Comparing `unprint-0.0.2/PKG-INFO` & `unprint-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unprint
-Version: 0.0.2
+Version: 0.0.4
 Summary: A simple package to unprint lines in the terminal
 Home-page: https://github.com/pypa/sampleproject
 Author: Liu Zuo Lin
 Author-email: zlliu246@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `unprint-0.0.2/setup.py` & `unprint-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="unprint",
-    version="0.0.2",
+    version="0.0.4",
     author="Liu Zuo Lin",
     author_email="zlliu246@gmail.com",
     description="A simple package to unprint lines in the terminal",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     project_urls={
```

### Comparing `unprint-0.0.2/src/unprint.egg-info/PKG-INFO` & `unprint-0.0.4/src/unprint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unprint
-Version: 0.0.2
+Version: 0.0.4
 Summary: A simple package to unprint lines in the terminal
 Home-page: https://github.com/pypa/sampleproject
 Author: Liu Zuo Lin
 Author-email: zlliu246@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

