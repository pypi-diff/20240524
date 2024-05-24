# Comparing `tmp/unprint-0.0.6.tar.gz` & `tmp/unprint-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unprint-0.0.6.tar", last modified: Fri May 24 15:31:48 2024, max compression
+gzip compressed data, was "unprint-0.0.7.tar", last modified: Fri May 24 15:43:10 2024, max compression
```

## Comparing `unprint-0.0.6.tar` & `unprint-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:31:48.234459 unprint-0.0.6/
--rw-r--r--   0 lzl        (501) staff       (20)     1073 2024-05-24 15:30:50.000000 unprint-0.0.6/LICENSE
--rw-r--r--   0 lzl        (501) staff       (20)      576 2024-05-24 15:31:48.234264 unprint-0.0.6/PKG-INFO
--rw-r--r--   0 lzl        (501) staff       (20)      170 2024-05-24 15:30:39.000000 unprint-0.0.6/README.md
--rw-r--r--   0 lzl        (501) staff       (20)      458 2024-05-24 15:30:28.000000 unprint-0.0.6/pyproject.toml
--rw-r--r--   0 lzl        (501) staff       (20)       38 2024-05-24 15:31:48.234503 unprint-0.0.6/setup.cfg
--rw-r--r--   0 lzl        (501) staff       (20)      675 2024-05-24 15:26:08.000000 unprint-0.0.6/setup.py
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:31:48.234088 unprint-0.0.6/unprint.egg-info/
--rw-r--r--   0 lzl        (501) staff       (20)      576 2024-05-24 15:31:48.000000 unprint-0.0.6/unprint.egg-info/PKG-INFO
--rw-r--r--   0 lzl        (501) staff       (20)      165 2024-05-24 15:31:48.000000 unprint-0.0.6/unprint.egg-info/SOURCES.txt
--rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:31:48.000000 unprint-0.0.6/unprint.egg-info/dependency_links.txt
--rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:31:48.000000 unprint-0.0.6/unprint.egg-info/top_level.txt
+drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:43:10.615559 unprint-0.0.7/
+-rw-r--r--   0 lzl        (501) staff       (20)     1073 2024-05-24 15:30:50.000000 unprint-0.0.7/LICENSE
+-rw-r--r--   0 lzl        (501) staff       (20)      576 2024-05-24 15:43:10.615364 unprint-0.0.7/PKG-INFO
+-rw-r--r--   0 lzl        (501) staff       (20)      170 2024-05-24 15:30:39.000000 unprint-0.0.7/README.md
+-rw-r--r--   0 lzl        (501) staff       (20)      458 2024-05-24 15:43:08.000000 unprint-0.0.7/pyproject.toml
+-rw-r--r--   0 lzl        (501) staff       (20)       38 2024-05-24 15:43:10.615600 unprint-0.0.7/setup.cfg
+-rw-r--r--   0 lzl        (501) staff       (20)      675 2024-05-24 15:26:08.000000 unprint-0.0.7/setup.py
+drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:43:10.615160 unprint-0.0.7/unprint.egg-info/
+-rw-r--r--   0 lzl        (501) staff       (20)      576 2024-05-24 15:43:10.000000 unprint-0.0.7/unprint.egg-info/PKG-INFO
+-rw-r--r--   0 lzl        (501) staff       (20)      165 2024-05-24 15:43:10.000000 unprint-0.0.7/unprint.egg-info/SOURCES.txt
+-rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:43:10.000000 unprint-0.0.7/unprint.egg-info/dependency_links.txt
+-rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:43:10.000000 unprint-0.0.7/unprint.egg-info/top_level.txt
```

### Comparing `unprint-0.0.6/LICENSE` & `unprint-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unprint-0.0.6/PKG-INFO` & `unprint-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unprint
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple package to unprint stuff in terminal
 Author: Liu Zuo Lin
 Author-email: Liu Zuo Lin <zlliu246@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `unprint-0.0.6/setup.py` & `unprint-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `unprint-0.0.6/unprint.egg-info/PKG-INFO` & `unprint-0.0.7/unprint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unprint
-Version: 0.0.6
+Version: 0.0.7
 Summary: A simple package to unprint stuff in terminal
 Author: Liu Zuo Lin
 Author-email: Liu Zuo Lin <zlliu246@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

