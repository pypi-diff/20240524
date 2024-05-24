# Comparing `tmp/picopy-1.0.5.tar.gz` & `tmp/picopy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopy-1.0.5.tar", last modified: Thu May 23 21:45:55 2024, max compression
+gzip compressed data, was "picopy-1.0.6.tar", last modified: Thu May 23 23:21:17 2024, max compression
```

## Comparing `picopy-1.0.5.tar` & `picopy-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:55.769512 picopy-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 21:45:47.000000 picopy-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-23 21:45:55.769512 picopy-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 21:45:47.000000 picopy-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:55.769512 picopy-1.0.5/picopy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:47.000000 picopy-1.0.5/picopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 21:45:47.000000 picopy-1.0.5/picopy/picopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:55.769512 picopy-1.0.5/picopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-23 21:45:55.000000 picopy-1.0.5/picopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 21:45:55.000000 picopy-1.0.5/picopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:45:55.000000 picopy-1.0.5/picopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 21:45:55.000000 picopy-1.0.5/picopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:47.000000 picopy-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:45:55.769512 picopy-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-23 21:45:47.000000 picopy-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:55.769512 picopy-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 21:45:47.000000 picopy-1.0.5/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:17.785627 picopy-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 23:21:13.000000 picopy-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-23 23:21:17.785627 picopy-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 23:21:13.000000 picopy-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:17.785627 picopy-1.0.6/picopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:13.000000 picopy-1.0.6/picopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 23:21:13.000000 picopy-1.0.6/picopy/picopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:17.785627 picopy-1.0.6/picopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 23:21:13.000000 picopy-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 23:21:17.785627 picopy-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 23:21:13.000000 picopy-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:17.785627 picopy-1.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 23:21:13.000000 picopy-1.0.6/tests/test_package.py
```

### Comparing `picopy-1.0.5/picopy/picopy.py` & `picopy-1.0.6/picopy/picopy.py`

 * *Files identical despite different names*

