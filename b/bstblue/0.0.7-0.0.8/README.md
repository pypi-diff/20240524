# Comparing `tmp/bstblue-0.0.7.tar.gz` & `tmp/bstblue-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstblue-0.0.7.tar", last modified: Fri May 24 08:39:01 2024, max compression
+gzip compressed data, was "bstblue-0.0.8.tar", last modified: Fri May 24 09:16:13 2024, max compression
```

## Comparing `bstblue-0.0.7.tar` & `bstblue-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 08:39:01.197522 bstblue-0.0.7/
--rw-rw-rw-   0        0        0        0 2024-05-23 13:29:33.000000 bstblue-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      654 2024-05-24 08:39:01.196527 bstblue-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      159 2024-05-24 07:58:37.000000 bstblue-0.0.7/README.md
--rw-rw-rw-   0        0        0      103 2024-05-23 13:32:24.000000 bstblue-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      632 2024-05-24 08:39:01.202544 bstblue-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-24 08:39:01.150650 bstblue-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-24 08:39:01.166605 bstblue-0.0.7/src/bstblue/
--rw-rw-rw-   0        0        0        0 2024-05-23 13:48:24.000000 bstblue-0.0.7/src/bstblue/__init__.py
--rw-rw-rw-   0        0        0      438 2024-05-24 08:38:39.000000 bstblue-0.0.7/src/bstblue/bstblue.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:39:01.192544 bstblue-0.0.7/src/bstblue.egg-info/
--rw-rw-rw-   0        0        0      654 2024-05-24 08:39:01.000000 bstblue-0.0.7/src/bstblue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-24 08:39:01.000000 bstblue-0.0.7/src/bstblue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 08:39:01.000000 bstblue-0.0.7/src/bstblue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-24 08:39:01.000000 bstblue-0.0.7/src/bstblue.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 09:16:13.940378 bstblue-0.0.8/
+-rw-rw-rw-   0        0        0        0 2024-05-23 13:29:33.000000 bstblue-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      654 2024-05-24 09:16:13.939378 bstblue-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2024-05-24 07:58:37.000000 bstblue-0.0.8/README.md
+-rw-rw-rw-   0        0        0      103 2024-05-23 13:32:24.000000 bstblue-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      632 2024-05-24 09:16:13.945368 bstblue-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 09:16:13.880538 bstblue-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 09:16:13.910458 bstblue-0.0.8/src/bstblue/
+-rw-rw-rw-   0        0        0        0 2024-05-23 13:48:24.000000 bstblue-0.0.8/src/bstblue/__init__.py
+-rw-rw-rw-   0        0        0      170 2024-05-24 09:15:58.000000 bstblue-0.0.8/src/bstblue/bstblue.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:16:13.937389 bstblue-0.0.8/src/bstblue.egg-info/
+-rw-rw-rw-   0        0        0      654 2024-05-24 09:16:13.000000 bstblue-0.0.8/src/bstblue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-24 09:16:13.000000 bstblue-0.0.8/src/bstblue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:16:13.000000 bstblue-0.0.8/src/bstblue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 09:16:13.000000 bstblue-0.0.8/src/bstblue.egg-info/top_level.txt
```

### Comparing `bstblue-0.0.7/PKG-INFO` & `bstblue-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstblue
-Version: 0.0.7
+Version: 0.0.8
 Summary: bstblue
 Home-page: https://github.com/Blueboy0999/bstblue/
 Author: Blueboy
 Author-email: contact-pypi@blueboy.dev
 Project-URL: Bug Tracker, https://github.com/Blueboy0999/bstblue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bstblue-0.0.7/setup.cfg` & `bstblue-0.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7374 626c 7565 0d0a 7665 7273   = bstblue..vers
-00000020: 696f 6e20 3d20 302e 302e 370d 0a61 7574  ion = 0.0.7..aut
+00000020: 696f 6e20 3d20 302e 302e 380d 0a61 7574  ion = 0.0.8..aut
 00000030: 686f 7220 3d20 426c 7565 626f 790d 0a61  hor = Blueboy..a
 00000040: 7574 686f 725f 656d 6169 6c20 3d20 636f  uthor_email = co
 00000050: 6e74 6163 742d 7079 7069 4062 6c75 6562  ntact-pypi@blueb
 00000060: 6f79 2e64 6576 0d0a 6465 7363 7269 7074  oy.dev..descript
 00000070: 696f 6e20 3d20 6273 7462 6c75 650d 0a6c  ion = bstblue..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
```

### Comparing `bstblue-0.0.7/src/bstblue.egg-info/PKG-INFO` & `bstblue-0.0.8/src/bstblue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstblue
-Version: 0.0.7
+Version: 0.0.8
 Summary: bstblue
 Home-page: https://github.com/Blueboy0999/bstblue/
 Author: Blueboy
 Author-email: contact-pypi@blueboy.dev
 Project-URL: Bug Tracker, https://github.com/Blueboy0999/bstblue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

