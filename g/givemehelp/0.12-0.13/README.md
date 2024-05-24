# Comparing `tmp/givemehelp-0.12.tar.gz` & `tmp/givemehelp-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\givemehelp-0.12.tar", last modified: Fri May 24 12:24:03 2024, max compression
+gzip compressed data, was "dist\givemehelp-0.13.tar", last modified: Fri May 24 12:27:19 2024, max compression
```

## Comparing `givemehelp-0.12.tar` & `givemehelp-0.13.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 12:24:03.283430 givemehelp-0.12/
--rw-rw-rw-   0        0        0      193 2024-05-24 12:24:03.283430 givemehelp-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 12:24:03.274038 givemehelp-0.12/givemehelp/
--rw-rw-rw-   0        0        0       35 2024-05-24 12:09:58.000000 givemehelp-0.12/givemehelp/__init__.py
--rw-rw-rw-   0        0        0     1582 2024-05-24 12:10:02.000000 givemehelp-0.12/givemehelp/main.py
-drwxrwxrwx   0        0        0        0 2024-05-24 12:24:03.281428 givemehelp-0.12/givemehelp.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-24 12:24:03.000000 givemehelp-0.12/givemehelp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-24 12:24:03.000000 givemehelp-0.12/givemehelp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 12:24:03.000000 givemehelp-0.12/givemehelp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-24 12:24:03.000000 givemehelp-0.12/givemehelp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 12:24:03.000000 givemehelp-0.12/givemehelp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-24 12:24:03.000000 givemehelp-0.12/givemehelp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 12:24:03.284572 givemehelp-0.12/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-05-24 12:23:58.000000 givemehelp-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:27:19.492846 givemehelp-0.13/
+-rw-rw-rw-   0        0        0      193 2024-05-24 12:27:19.492846 givemehelp-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 12:27:19.482741 givemehelp-0.13/givemehelp/
+-rw-rw-rw-   0        0        0       35 2024-05-24 12:09:58.000000 givemehelp-0.13/givemehelp/__init__.py
+-rw-rw-rw-   0        0        0     1582 2024-05-24 12:10:02.000000 givemehelp-0.13/givemehelp/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:27:19.491342 givemehelp-0.13/givemehelp.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-24 12:27:19.000000 givemehelp-0.13/givemehelp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-24 12:27:19.000000 givemehelp-0.13/givemehelp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 12:27:19.000000 givemehelp-0.13/givemehelp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-24 12:27:19.000000 givemehelp-0.13/givemehelp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 12:27:19.000000 givemehelp-0.13/givemehelp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 12:27:19.000000 givemehelp-0.13/givemehelp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 12:27:19.493851 givemehelp-0.13/setup.cfg
+-rw-rw-rw-   0        0        0      336 2024-05-24 12:27:13.000000 givemehelp-0.13/setup.py
```

### Comparing `givemehelp-0.12/givemehelp/main.py` & `givemehelp-0.13/givemehelp/main.py`

 * *Files identical despite different names*

