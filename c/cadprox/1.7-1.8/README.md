# Comparing `tmp/cadprox-1.7.tar.gz` & `tmp/cadprox-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-1.7.tar", last modified: Fri May 24 04:28:00 2024, max compression
+gzip compressed data, was "cadprox-1.8.tar", last modified: Fri May 24 04:45:38 2024, max compression
```

## Comparing `cadprox-1.7.tar` & `cadprox-1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:28:00.977989 cadprox-1.7/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.7/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:28:00.977989 cadprox-1.7/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-24 03:13:51.000000 cadprox-1.7/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:28:00.969988 cadprox-1.7/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.7/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.7/app/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3094 2024-05-24 04:27:05.000000 cadprox-1.7/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8164 2024-05-24 04:27:16.000000 cadprox-1.7/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:28:00.977989 cadprox-1.7/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:28:00.977989 cadprox-1.7/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)      933 2024-05-24 04:27:55.000000 cadprox-1.7/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:45:38.963753 cadprox-1.8/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.8/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4679 2024-05-24 04:45:38.963753 cadprox-1.8/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4095 2024-05-24 04:38:51.000000 cadprox-1.8/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:45:38.955753 cadprox-1.8/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.8/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.8/app/config.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3094 2024-05-24 04:27:05.000000 cadprox-1.8/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8164 2024-05-24 04:27:16.000000 cadprox-1.8/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:45:38.963753 cadprox-1.8/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4679 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:45:38.963753 cadprox-1.8/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1756 2024-05-24 04:45:18.000000 cadprox-1.8/setup.py
```

### Comparing `cadprox-1.7/app/main.py` & `cadprox-1.8/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-1.7/app/utils.py` & `cadprox-1.8/app/utils.py`

 * *Files identical despite different names*

