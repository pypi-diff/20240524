# Comparing `tmp/bstblue-0.0.2.tar.gz` & `tmp/bstblue-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstblue-0.0.2.tar", last modified: Thu May 23 14:32:09 2024, max compression
+gzip compressed data, was "bstblue-0.0.3.tar", last modified: Thu May 23 14:56:24 2024, max compression
```

## Comparing `bstblue-0.0.2.tar` & `bstblue-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:32:09.286245 bstblue-0.0.2/
--rw-rw-rw-   0        0        0        0 2024-05-23 13:29:33.000000 bstblue-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      491 2024-05-23 14:32:09.285254 bstblue-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      103 2024-05-23 13:32:24.000000 bstblue-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      632 2024-05-23 14:32:09.290234 bstblue-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 14:32:09.225414 bstblue-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 14:32:09.252344 bstblue-0.0.2/src/bstblue/
--rw-rw-rw-   0        0        0        0 2024-05-23 13:48:24.000000 bstblue-0.0.2/src/bstblue/__init__.py
--rw-rw-rw-   0        0        0      378 2024-05-23 14:31:43.000000 bstblue-0.0.2/src/bstblue/main.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:32:09.283260 bstblue-0.0.2/src/bstblue.egg-info/
--rw-rw-rw-   0        0        0      491 2024-05-23 14:32:09.000000 bstblue-0.0.2/src/bstblue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-05-23 14:32:09.000000 bstblue-0.0.2/src/bstblue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:32:09.000000 bstblue-0.0.2/src/bstblue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-23 14:32:09.000000 bstblue-0.0.2/src/bstblue.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 14:56:24.850671 bstblue-0.0.3/
+-rw-rw-rw-   0        0        0        0 2024-05-23 13:29:33.000000 bstblue-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      491 2024-05-23 14:56:24.850671 bstblue-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2024-05-23 13:32:24.000000 bstblue-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      632 2024-05-23 14:56:24.858118 bstblue-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 14:56:24.803533 bstblue-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 14:56:24.815360 bstblue-0.0.3/src/bstblue/
+-rw-rw-rw-   0        0        0        0 2024-05-23 13:48:24.000000 bstblue-0.0.3/src/bstblue/__init__.py
+-rw-rw-rw-   0        0        0      561 2024-05-23 14:56:04.000000 bstblue-0.0.3/src/bstblue/bstblue.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:56:24.849046 bstblue-0.0.3/src/bstblue.egg-info/
+-rw-rw-rw-   0        0        0      491 2024-05-23 14:56:24.000000 bstblue-0.0.3/src/bstblue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2024-05-23 14:56:24.000000 bstblue-0.0.3/src/bstblue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:56:24.000000 bstblue-0.0.3/src/bstblue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 14:56:24.000000 bstblue-0.0.3/src/bstblue.egg-info/top_level.txt
```

### Comparing `bstblue-0.0.2/setup.cfg` & `bstblue-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7374 626c 7565 0d0a 7665 7273   = bstblue..vers
-00000020: 696f 6e20 3d20 302e 302e 320d 0a61 7574  ion = 0.0.2..aut
+00000020: 696f 6e20 3d20 302e 302e 330d 0a61 7574  ion = 0.0.3..aut
 00000030: 686f 7220 3d20 426c 7565 626f 790d 0a61  hor = Blueboy..a
 00000040: 7574 686f 725f 656d 6169 6c20 3d20 636f  uthor_email = co
 00000050: 6e74 6163 742d 7079 7069 4062 6c75 6562  ntact-pypi@blueb
 00000060: 6f79 2e64 6576 0d0a 6465 7363 7269 7074  oy.dev..descript
 00000070: 696f 6e20 3d20 6273 7462 6c75 650d 0a6c  ion = bstblue..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
```

