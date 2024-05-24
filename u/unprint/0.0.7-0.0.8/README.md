# Comparing `tmp/unprint-0.0.7.tar.gz` & `tmp/unprint-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unprint-0.0.7.tar", last modified: Fri May 24 15:43:10 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `unprint-0.0.7.tar` & `unprint-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,7 @@
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:43:10.615559 unprint-0.0.7/
--rw-r--r--   0 lzl        (501) staff       (20)     1073 2024-05-24 15:30:50.000000 unprint-0.0.7/LICENSE
--rw-r--r--   0 lzl        (501) staff       (20)      576 2024-05-24 15:43:10.615364 unprint-0.0.7/PKG-INFO
--rw-r--r--   0 lzl        (501) staff       (20)      170 2024-05-24 15:30:39.000000 unprint-0.0.7/README.md
--rw-r--r--   0 lzl        (501) staff       (20)      458 2024-05-24 15:43:08.000000 unprint-0.0.7/pyproject.toml
--rw-r--r--   0 lzl        (501) staff       (20)       38 2024-05-24 15:43:10.615600 unprint-0.0.7/setup.cfg
--rw-r--r--   0 lzl        (501) staff       (20)      675 2024-05-24 15:26:08.000000 unprint-0.0.7/setup.py
-drwxr-xr-x   0 lzl        (501) staff       (20)        0 2024-05-24 15:43:10.615160 unprint-0.0.7/unprint.egg-info/
--rw-r--r--   0 lzl        (501) staff       (20)      576 2024-05-24 15:43:10.000000 unprint-0.0.7/unprint.egg-info/PKG-INFO
--rw-r--r--   0 lzl        (501) staff       (20)      165 2024-05-24 15:43:10.000000 unprint-0.0.7/unprint.egg-info/SOURCES.txt
--rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:43:10.000000 unprint-0.0.7/unprint.egg-info/dependency_links.txt
--rw-r--r--   0 lzl        (501) staff       (20)        1 2024-05-24 15:43:10.000000 unprint-0.0.7/unprint.egg-info/top_level.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 unprint-0.0.8/src/unprint/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 unprint-0.0.8/src/unprint/unprinter.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 unprint-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 unprint-0.0.8/LICENSE
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 unprint-0.0.8/README.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 unprint-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 unprint-0.0.8/PKG-INFO
```

### Comparing `unprint-0.0.7/LICENSE` & `unprint-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unprint-0.0.7/PKG-INFO` & `unprint-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: unprint
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple package to unprint stuff in terminal
-Author: Liu Zuo Lin
 Author-email: Liu Zuo Lin <zlliu246@gmail.com>
-Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Example Package
 
 This is a simple example package. You can use
 [GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+to write your content.
```

