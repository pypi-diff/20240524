# Comparing `tmp/e2tapi-0.0.8.tar.gz` & `tmp/e2tapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2tapi-0.0.8.tar", last modified: Thu May 23 19:53:01 2024, max compression
+gzip compressed data, was "e2tapi-0.0.9.tar", last modified: Thu May 23 19:57:52 2024, max compression
```

## Comparing `e2tapi-0.0.8.tar` & `e2tapi-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.890423 e2tapi-0.0.8/
--rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-23 19:53:01.886423 e2tapi-0.0.8/PKG-INFO
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6188 2024-05-22 15:19:56.000000 e2tapi-0.0.8/README.md
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.878423 e2tapi-0.0.8/e2t/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       42 2024-05-22 20:13:00.000000 e2tapi-0.0.8/e2t/__init__.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.882423 e2tapi-0.0.8/e2t/mktdata/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    97648 2024-05-23 19:46:58.000000 e2tapi-0.0.8/e2t/mktdata/BYMA_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    42353 2024-05-23 19:50:12.000000 e2tapi-0.0.8/e2t/mktdata/IBKR_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       19 2024-05-22 20:08:02.000000 e2tapi-0.0.8/e2t/mktdata/__init__.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    12652 2024-05-23 19:51:38.000000 e2tapi-0.0.8/e2t/mktdata/byma.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6015 2024-05-23 19:51:38.000000 e2tapi-0.0.8/e2t/mktdata/ibkr.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.886423 e2tapi-0.0.8/e2t/oms/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    36422 2024-05-23 19:38:27.000000 e2tapi-0.0.8/e2t/oms/BYMA_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    23586 2024-05-23 19:45:17.000000 e2tapi-0.0.8/e2t/oms/IBKR_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       39 2024-05-23 19:01:40.000000 e2tapi-0.0.8/e2t/oms/__init__.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     5650 2024-05-23 19:40:58.000000 e2tapi-0.0.8/e2t/oms/byma.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     4491 2024-05-23 19:24:30.000000 e2tapi-0.0.8/e2t/oms/ibkr.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:53:01.886423 e2tapi-0.0.8/e2tapi.egg-info/
--rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/PKG-INFO
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      423 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/SOURCES.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        1 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/dependency_links.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       16 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/requires.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        4 2024-05-23 19:53:01.000000 e2tapi-0.0.8/e2tapi.egg-info/top_level.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       38 2024-05-23 19:53:01.890423 e2tapi-0.0.8/setup.cfg
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      697 2024-05-23 19:52:57.000000 e2tapi-0.0.8/setup.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:57:52.992113 e2tapi-0.0.9/
+-rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-23 19:57:52.992113 e2tapi-0.0.9/PKG-INFO
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6188 2024-05-22 15:19:56.000000 e2tapi-0.0.9/README.md
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:57:52.980113 e2tapi-0.0.9/e2t/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       42 2024-05-22 20:13:00.000000 e2tapi-0.0.9/e2t/__init__.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:57:52.984113 e2tapi-0.0.9/e2t/mktdata/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    97648 2024-05-23 19:46:58.000000 e2tapi-0.0.9/e2t/mktdata/BYMA_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    42353 2024-05-23 19:50:12.000000 e2tapi-0.0.9/e2t/mktdata/IBKR_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       39 2024-05-23 19:57:51.000000 e2tapi-0.0.9/e2t/mktdata/__init__.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    12652 2024-05-23 19:51:38.000000 e2tapi-0.0.9/e2t/mktdata/byma.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6015 2024-05-23 19:51:38.000000 e2tapi-0.0.9/e2t/mktdata/ibkr.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:57:52.988113 e2tapi-0.0.9/e2t/oms/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    36422 2024-05-23 19:38:27.000000 e2tapi-0.0.9/e2t/oms/BYMA_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    23586 2024-05-23 19:45:17.000000 e2tapi-0.0.9/e2t/oms/IBKR_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       39 2024-05-23 19:01:40.000000 e2tapi-0.0.9/e2t/oms/__init__.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     5650 2024-05-23 19:40:58.000000 e2tapi-0.0.9/e2t/oms/byma.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     4491 2024-05-23 19:24:30.000000 e2tapi-0.0.9/e2t/oms/ibkr.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-23 19:57:52.992113 e2tapi-0.0.9/e2tapi.egg-info/
+-rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-23 19:57:52.000000 e2tapi-0.0.9/e2tapi.egg-info/PKG-INFO
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      423 2024-05-23 19:57:52.000000 e2tapi-0.0.9/e2tapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        1 2024-05-23 19:57:52.000000 e2tapi-0.0.9/e2tapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       16 2024-05-23 19:57:52.000000 e2tapi-0.0.9/e2tapi.egg-info/requires.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        4 2024-05-23 19:57:52.000000 e2tapi-0.0.9/e2tapi.egg-info/top_level.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       38 2024-05-23 19:57:52.992113 e2tapi-0.0.9/setup.cfg
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      697 2024-05-23 19:57:51.000000 e2tapi-0.0.9/setup.py
```

### Comparing `e2tapi-0.0.8/PKG-INFO` & `e2tapi-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2tapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for e2t OMS
 Home-page: http://gitlab.event2trading.com/utilities/e2tapi.git
 Author: Event2trading
 Author-email: admin@event2trading.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `e2tapi-0.0.8/README.md` & `e2tapi-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2t/mktdata/BYMA_Messages_pb2.py` & `e2tapi-0.0.9/e2t/mktdata/BYMA_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2t/mktdata/IBKR_Messages_pb2.py` & `e2tapi-0.0.9/e2t/mktdata/IBKR_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2t/mktdata/byma.py` & `e2tapi-0.0.9/e2t/mktdata/byma.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2t/mktdata/ibkr.py` & `e2tapi-0.0.9/e2t/mktdata/ibkr.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2t/oms/BYMA_Messages_pb2.py` & `e2tapi-0.0.9/e2t/oms/BYMA_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2t/oms/IBKR_Messages_pb2.py` & `e2tapi-0.0.9/e2t/oms/IBKR_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2t/oms/byma.py` & `e2tapi-0.0.9/e2t/oms/byma.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2t/oms/ibkr.py` & `e2tapi-0.0.9/e2t/oms/ibkr.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.8/e2tapi.egg-info/PKG-INFO` & `e2tapi-0.0.9/e2tapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2tapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for e2t OMS
 Home-page: http://gitlab.event2trading.com/utilities/e2tapi.git
 Author: Event2trading
 Author-email: admin@event2trading.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `e2tapi-0.0.8/setup.py` & `e2tapi-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='e2tapi',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[
         'protobuf>=3.0.0',
     ],
     include_package_data=True,
     description='SDK for e2t OMS',
     long_description=open('README.md').read(),
```

