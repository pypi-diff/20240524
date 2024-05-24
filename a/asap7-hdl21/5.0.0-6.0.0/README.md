# Comparing `tmp/asap7-hdl21-5.0.0.tar.gz` & `tmp/asap7_hdl21-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asap7-hdl21-5.0.0.tar", last modified: Tue Nov 14 18:40:25 2023, max compression
+gzip compressed data, was "asap7_hdl21-6.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `asap7-hdl21-5.0.0.tar` & `asap7_hdl21-6.0.0.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:25.785971 asap7-hdl21-5.0.0/
--rw-r--r--   0 dan        (501) staff       (20)      247 2023-11-14 18:40:25.785814 asap7-hdl21-5.0.0/PKG-INFO
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:25.784828 asap7-hdl21-5.0.0/asap7_hdl21/
--rw-r--r--   0 dan        (501) staff       (20)      315 2023-07-11 14:50:48.000000 asap7-hdl21-5.0.0/asap7_hdl21/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3985 2023-07-11 14:50:48.000000 asap7-hdl21-5.0.0/asap7_hdl21/pdk.py
--rw-r--r--   0 dan        (501) staff       (20)      180 2023-07-11 14:50:48.000000 asap7-hdl21-5.0.0/asap7_hdl21/test_pdk.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:25.785619 asap7-hdl21-5.0.0/asap7_hdl21.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      247 2023-11-14 18:40:25.000000 asap7-hdl21-5.0.0/asap7_hdl21.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      259 2023-11-14 18:40:25.000000 asap7-hdl21-5.0.0/asap7_hdl21.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-11-14 18:40:25.000000 asap7-hdl21-5.0.0/asap7_hdl21.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       58 2023-11-14 18:40:25.000000 asap7-hdl21-5.0.0/asap7_hdl21.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       12 2023-11-14 18:40:25.000000 asap7-hdl21-5.0.0/asap7_hdl21.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-05-03 17:59:57.000000 asap7-hdl21-5.0.0/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-11-14 18:40:25.786023 asap7-hdl21-5.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      888 2023-11-14 18:31:59.000000 asap7-hdl21-5.0.0/setup.py
+-rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035628 asap7_hdl21-6.0.0/LICENSE
+-rw-r--r--   0        0        0      315 2023-07-11 14:50:48.444752 asap7_hdl21-6.0.0/asap7_hdl21/__init__.py
+-rw-r--r--   0        0        0     3985 2023-07-11 14:50:48.444618 asap7_hdl21-6.0.0/asap7_hdl21/pdk.py
+-rw-r--r--   0        0        0      180 2023-07-11 14:50:48.444416 asap7_hdl21-6.0.0/asap7_hdl21/test_pdk.py
+-rw-r--r--   0        0        0     1298 2024-05-24 17:12:01.379907 asap7_hdl21-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-05-24 17:18:05.507739 asap7_hdl21-6.0.0/readme.md
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 asap7_hdl21-6.0.0/PKG-INFO
```

### Comparing `asap7-hdl21-5.0.0/asap7_hdl21/pdk.py` & `asap7_hdl21-6.0.0/asap7_hdl21/pdk.py`

 * *Files identical despite different names*

