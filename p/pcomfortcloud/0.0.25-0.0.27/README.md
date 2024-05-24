# Comparing `tmp/pcomfortcloud-0.0.25.tar.gz` & `tmp/pcomfortcloud-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-panasonic-comfort-cloud/python-panasonic-comfort-cloud/dist/.tmp-fr4nehhi/pcomfortcloud-0.0.25.tar", last modified: Thu Dec 14 17:51:38 2023, max compression
+gzip compressed data, was "/home/runner/work/python-panasonic-comfort-cloud/python-panasonic-comfort-cloud/dist/.tmp-azf9dgel/pcomfortcloud-0.0.27.tar", last modified: Fri May 24 12:07:44 2024, max compression
```

## Comparing `pcomfortcloud-0.0.25.tar` & `pcomfortcloud-0.0.27.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/pcomfortcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9569 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/pcomfortcloud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/pcomfortcloud/certificatechain.pem
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/pcomfortcloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14888 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/pcomfortcloud/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/pcomfortcloud/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/pcomfortcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 17:51:38.000000 pcomfortcloud-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-12-14 17:51:30.000000 pcomfortcloud-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/pcomfortcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/pcomfortcloud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/pcomfortcloud/certificatechain.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/pcomfortcloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14888 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/pcomfortcloud/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/pcomfortcloud/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/pcomfortcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:07:44.000000 pcomfortcloud-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 12:07:39.000000 pcomfortcloud-0.0.27/setup.py
```

### Comparing `pcomfortcloud-0.0.25/LICENSE` & `pcomfortcloud-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `pcomfortcloud-0.0.25/PKG-INFO` & `pcomfortcloud-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcomfortcloud
-Version: 0.0.25
+Version: 0.0.27
 Summary: Read and change status of Panasonic Comfort Cloud devices
 Home-page: http://github.com/lostfields/python-panasonic-comfort-cloud
 Author: Lostfields
 License: MIT
 Keywords: home automation panasonic climate
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pcomfortcloud-0.0.25/README.md` & `pcomfortcloud-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `pcomfortcloud-0.0.25/pcomfortcloud/__main__.py` & `pcomfortcloud-0.0.27/pcomfortcloud/__main__.py`

 * *Files identical despite different names*

### Comparing `pcomfortcloud-0.0.25/pcomfortcloud/certificatechain.pem` & `pcomfortcloud-0.0.27/pcomfortcloud/certificatechain.pem`

 * *Files identical despite different names*

### Comparing `pcomfortcloud-0.0.25/pcomfortcloud/constants.py` & `pcomfortcloud-0.0.27/pcomfortcloud/constants.py`

 * *Files identical despite different names*

### Comparing `pcomfortcloud-0.0.25/pcomfortcloud/session.py` & `pcomfortcloud-0.0.27/pcomfortcloud/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
     def logout(self):
         """ Logout """
 
     def _headers(self):
         return {
             "X-APP-TYPE": "1",
-            "X-APP-VERSION": "1.19.0",
+            "X-APP-VERSION": "1.20.1",
             "X-User-Authorization": self._vid,
             "X-APP-TIMESTAMP": "1",
             "X-APP-NAME": "Comfort Cloud",
             "X-CFC-API-KEY": "Comfort Cloud",
             "User-Agent": "G-RAC",
             "Accept": "application/json; charset=utf-8",
             "Content-Type": "application/json; charset=utf-8"
```

### Comparing `pcomfortcloud-0.0.25/pcomfortcloud/urls.py` & `pcomfortcloud-0.0.27/pcomfortcloud/urls.py`

 * *Files identical despite different names*

### Comparing `pcomfortcloud-0.0.25/pcomfortcloud.egg-info/PKG-INFO` & `pcomfortcloud-0.0.27/pcomfortcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcomfortcloud
-Version: 0.0.25
+Version: 0.0.27
 Summary: Read and change status of Panasonic Comfort Cloud devices
 Home-page: http://github.com/lostfields/python-panasonic-comfort-cloud
 Author: Lostfields
 License: MIT
 Keywords: home automation panasonic climate
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pcomfortcloud-0.0.25/setup.py` & `pcomfortcloud-0.0.27/setup.py`

 * *Files identical despite different names*

