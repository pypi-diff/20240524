# Comparing `tmp/sakura_fm-0.0.4.tar.gz` & `tmp/sakura_fm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakura_fm-0.0.4.tar", last modified: Fri May 24 09:53:10 2024, max compression
+gzip compressed data, was "sakura_fm-0.0.5.tar", last modified: Fri May 24 10:08:29 2024, max compression
```

## Comparing `sakura_fm-0.0.4.tar` & `sakura_fm-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 09:53:10.563824 sakura_fm-0.0.4/
--rw-rw-rw-   0        0        0     1083 2024-05-24 09:50:28.000000 sakura_fm-0.0.4/LICENCE
--rw-rw-rw-   0        0        0      379 2024-05-24 09:53:10.560840 sakura_fm-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1756 2024-05-24 09:46:07.000000 sakura_fm-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 09:53:10.420368 sakura_fm-0.0.4/sakura/
--rw-rw-rw-   0        0        0       26 2024-05-24 08:11:31.000000 sakura_fm-0.0.4/sakura/__init__.py
--rw-rw-rw-   0        0        0     1891 2024-05-24 09:44:39.000000 sakura_fm-0.0.4/sakura/client.py
--rw-rw-rw-   0        0        0      980 2024-05-24 09:28:13.000000 sakura_fm-0.0.4/sakura/db.py
--rw-rw-rw-   0        0        0     4506 2024-05-24 08:34:13.000000 sakura_fm-0.0.4/sakura/sakura.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:53:10.558824 sakura_fm-0.0.4/sakura_fm.egg-info/
--rw-rw-rw-   0        0        0      379 2024-05-24 09:53:10.000000 sakura_fm-0.0.4/sakura_fm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-05-24 09:53:10.000000 sakura_fm-0.0.4/sakura_fm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 09:53:10.000000 sakura_fm-0.0.4/sakura_fm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-24 09:53:10.000000 sakura_fm-0.0.4/sakura_fm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2024-05-24 09:53:10.000000 sakura_fm-0.0.4/sakura_fm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-24 09:53:10.000000 sakura_fm-0.0.4/sakura_fm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 09:53:10.565086 sakura_fm-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      647 2024-05-24 09:51:04.000000 sakura_fm-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:08:29.938464 sakura_fm-0.0.5/
+-rw-rw-rw-   0        0        0     1083 2024-05-24 09:50:28.000000 sakura_fm-0.0.5/LICENCE
+-rw-rw-rw-   0        0        0     2139 2024-05-24 10:08:29.935467 sakura_fm-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1756 2024-05-24 09:46:07.000000 sakura_fm-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 10:08:29.896520 sakura_fm-0.0.5/sakura/
+-rw-rw-rw-   0        0        0       26 2024-05-24 08:11:31.000000 sakura_fm-0.0.5/sakura/__init__.py
+-rw-rw-rw-   0        0        0     1891 2024-05-24 09:44:39.000000 sakura_fm-0.0.5/sakura/client.py
+-rw-rw-rw-   0        0        0      980 2024-05-24 09:28:13.000000 sakura_fm-0.0.5/sakura/db.py
+-rw-rw-rw-   0        0        0     4506 2024-05-24 08:34:13.000000 sakura_fm-0.0.5/sakura/sakura.py
+drwxrwxrwx   0        0        0        0 2024-05-24 10:08:29.932461 sakura_fm-0.0.5/sakura_fm.egg-info/
+-rw-rw-rw-   0        0        0     2139 2024-05-24 10:08:29.000000 sakura_fm-0.0.5/sakura_fm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-05-24 10:08:29.000000 sakura_fm-0.0.5/sakura_fm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 10:08:29.000000 sakura_fm-0.0.5/sakura_fm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-24 10:08:29.000000 sakura_fm-0.0.5/sakura_fm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2024-05-24 10:08:29.000000 sakura_fm-0.0.5/sakura_fm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 10:08:29.000000 sakura_fm-0.0.5/sakura_fm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 10:08:29.938464 sakura_fm-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      846 2024-05-24 10:07:17.000000 sakura_fm-0.0.5/setup.py
```

### Comparing `sakura_fm-0.0.4/LICENCE` & `sakura_fm-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.4/README.md` & `sakura_fm-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.4/sakura/client.py` & `sakura_fm-0.0.5/sakura/client.py`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.4/sakura/db.py` & `sakura_fm-0.0.5/sakura/db.py`

 * *Files identical despite different names*

### Comparing `sakura_fm-0.0.4/sakura/sakura.py` & `sakura_fm-0.0.5/sakura/sakura.py`

 * *Files identical despite different names*

