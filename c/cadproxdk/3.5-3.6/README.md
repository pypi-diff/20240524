# Comparing `tmp/cadproxdk-3.5.tar.gz` & `tmp/cadproxdk-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-3.5.tar", last modified: Fri May 24 09:02:42 2024, max compression
+gzip compressed data, was "cadproxdk-3.6.tar", last modified: Fri May 24 09:09:22 2024, max compression
```

## Comparing `cadproxdk-3.5.tar` & `cadproxdk-3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:02:42.005694 cadproxdk-3.5/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-3.5/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:02:42.005694 cadproxdk-3.5/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-3.5/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:02:42.001695 cadproxdk-3.5/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-3.5/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-3.5/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-3.5/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:02:42.005694 cadproxdk-3.5/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 09:02:42.005694 cadproxdk-3.5/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2645 2024-05-24 09:02:34.000000 cadproxdk-3.5/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:09:22.644856 cadproxdk-3.6/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-3.6/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:09:22.644856 cadproxdk-3.6/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-3.6/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:09:22.636856 cadproxdk-3.6/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-3.6/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-3.6/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-3.6/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:09:22.640856 cadproxdk-3.6/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:09:22.000000 cadproxdk-3.6/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 09:09:22.000000 cadproxdk-3.6/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 09:09:22.000000 cadproxdk-3.6/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 09:09:22.000000 cadproxdk-3.6/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 09:09:22.000000 cadproxdk-3.6/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 09:09:22.000000 cadproxdk-3.6/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 09:09:22.644856 cadproxdk-3.6/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1369 2024-05-24 09:09:14.000000 cadproxdk-3.6/setup.py
```

### Comparing `cadproxdk-3.5/PKG-INFO` & `cadproxdk-3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 3.5
+Version: 3.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-3.5/README.md` & `cadproxdk-3.6/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.5/app/main.py` & `cadproxdk-3.6/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.5/app/utils.py` & `cadproxdk-3.6/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.5/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-3.6/cadproxdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 3.5
+Version: 3.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

