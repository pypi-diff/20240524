# Comparing `tmp/e2tapi-0.0.14.tar.gz` & `tmp/e2tapi-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2tapi-0.0.14.tar", last modified: Fri May 24 17:33:38 2024, max compression
+gzip compressed data, was "e2tapi-0.0.15.tar", last modified: Fri May 24 18:14:15 2024, max compression
```

## Comparing `e2tapi-0.0.14.tar` & `e2tapi-0.0.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 17:33:38.234827 e2tapi-0.0.14/
--rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6643 2024-05-24 17:33:38.234827 e2tapi-0.0.14/PKG-INFO
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6188 2024-05-22 15:19:56.000000 e2tapi-0.0.14/README.md
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 17:33:38.226827 e2tapi-0.0.14/e2t/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       42 2024-05-22 20:13:00.000000 e2tapi-0.0.14/e2t/__init__.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 17:33:38.230827 e2tapi-0.0.14/e2t/mktdata/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)   105039 2024-05-24 16:37:00.000000 e2tapi-0.0.14/e2t/mktdata/BYMA_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    12660 2024-05-24 17:28:30.000000 e2tapi-0.0.14/e2t/mktdata/E2T_MDG_BYMA.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6023 2024-05-24 17:28:30.000000 e2tapi-0.0.14/e2t/mktdata/E2T_MDG_IBKR.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    45661 2024-05-24 16:37:00.000000 e2tapi-0.0.14/e2t/mktdata/IBKR_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       56 2024-05-24 17:30:24.000000 e2tapi-0.0.14/e2t/mktdata/__init__.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 17:33:38.234827 e2tapi-0.0.14/e2t/oms/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    38777 2024-05-24 16:37:00.000000 e2tapi-0.0.14/e2t/oms/BYMA_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     5655 2024-05-24 17:28:30.000000 e2tapi-0.0.14/e2t/oms/E2T_OMS_BYMA.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     4495 2024-05-24 17:28:30.000000 e2tapi-0.0.14/e2t/oms/E2T_OMS_IBKR.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    25143 2024-05-24 16:37:00.000000 e2tapi-0.0.14/e2t/oms/IBKR_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       56 2024-05-24 17:30:24.000000 e2tapi-0.0.14/e2t/oms/__init__.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 17:33:38.234827 e2tapi-0.0.14/e2tapi.egg-info/
--rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6643 2024-05-24 17:33:38.000000 e2tapi-0.0.14/e2tapi.egg-info/PKG-INFO
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      455 2024-05-24 17:33:38.000000 e2tapi-0.0.14/e2tapi.egg-info/SOURCES.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        1 2024-05-24 17:33:38.000000 e2tapi-0.0.14/e2tapi.egg-info/dependency_links.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       17 2024-05-24 17:33:38.000000 e2tapi-0.0.14/e2tapi.egg-info/requires.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        4 2024-05-24 17:33:38.000000 e2tapi-0.0.14/e2tapi.egg-info/top_level.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       38 2024-05-24 17:33:38.234827 e2tapi-0.0.14/setup.cfg
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      699 2024-05-24 17:33:16.000000 e2tapi-0.0.14/setup.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 18:14:15.622764 e2tapi-0.0.15/
+-rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    11473 2024-05-24 18:14:15.622764 e2tapi-0.0.15/PKG-INFO
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    11018 2024-05-24 18:05:27.000000 e2tapi-0.0.15/README.md
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 18:14:15.614764 e2tapi-0.0.15/e2t/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       42 2024-05-22 20:13:00.000000 e2tapi-0.0.15/e2t/__init__.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 18:14:15.618764 e2tapi-0.0.15/e2t/mktdata/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)   105039 2024-05-24 16:37:00.000000 e2tapi-0.0.15/e2t/mktdata/BYMA_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    12660 2024-05-24 17:28:30.000000 e2tapi-0.0.15/e2t/mktdata/E2T_MDG_BYMA.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6023 2024-05-24 17:28:30.000000 e2tapi-0.0.15/e2t/mktdata/E2T_MDG_IBKR.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    45661 2024-05-24 16:37:00.000000 e2tapi-0.0.15/e2t/mktdata/IBKR_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       56 2024-05-24 17:30:24.000000 e2tapi-0.0.15/e2t/mktdata/__init__.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 18:14:15.618764 e2tapi-0.0.15/e2t/oms/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    38777 2024-05-24 16:37:00.000000 e2tapi-0.0.15/e2t/oms/BYMA_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     5655 2024-05-24 17:28:30.000000 e2tapi-0.0.15/e2t/oms/E2T_OMS_BYMA.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     4495 2024-05-24 17:28:30.000000 e2tapi-0.0.15/e2t/oms/E2T_OMS_IBKR.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    25143 2024-05-24 16:37:00.000000 e2tapi-0.0.15/e2t/oms/IBKR_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       56 2024-05-24 17:30:24.000000 e2tapi-0.0.15/e2t/oms/__init__.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-24 18:14:15.622764 e2tapi-0.0.15/e2tapi.egg-info/
+-rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    11473 2024-05-24 18:14:15.000000 e2tapi-0.0.15/e2tapi.egg-info/PKG-INFO
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      455 2024-05-24 18:14:15.000000 e2tapi-0.0.15/e2tapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        1 2024-05-24 18:14:15.000000 e2tapi-0.0.15/e2tapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       17 2024-05-24 18:14:15.000000 e2tapi-0.0.15/e2tapi.egg-info/requires.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        4 2024-05-24 18:14:15.000000 e2tapi-0.0.15/e2tapi.egg-info/top_level.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       38 2024-05-24 18:14:15.622764 e2tapi-0.0.15/setup.cfg
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      699 2024-05-24 18:14:11.000000 e2tapi-0.0.15/setup.py
```

### Comparing `e2tapi-0.0.14/e2t/mktdata/BYMA_Messages_pb2.py` & `e2tapi-0.0.15/e2t/mktdata/BYMA_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.14/e2t/mktdata/E2T_MDG_BYMA.py` & `e2tapi-0.0.15/e2t/mktdata/E2T_MDG_BYMA.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.14/e2t/mktdata/E2T_MDG_IBKR.py` & `e2tapi-0.0.15/e2t/mktdata/E2T_MDG_IBKR.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.14/e2t/mktdata/IBKR_Messages_pb2.py` & `e2tapi-0.0.15/e2t/mktdata/IBKR_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.14/e2t/oms/BYMA_Messages_pb2.py` & `e2tapi-0.0.15/e2t/oms/BYMA_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.14/e2t/oms/E2T_OMS_BYMA.py` & `e2tapi-0.0.15/e2t/oms/E2T_OMS_BYMA.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.14/e2t/oms/E2T_OMS_IBKR.py` & `e2tapi-0.0.15/e2t/oms/E2T_OMS_IBKR.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.14/e2t/oms/IBKR_Messages_pb2.py` & `e2tapi-0.0.15/e2t/oms/IBKR_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.14/setup.py` & `e2tapi-0.0.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='e2tapi',
-    version='0.0.14',
+    version='0.0.15',
     packages=find_packages(),
     install_requires=[
-        'protobuf>=3.20.0',
+        'protobuf==3.20.3',
     ],
     include_package_data=True,
     description='SDK for e2t OMS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='http://gitlab.event2trading.com/utilities/e2tapi.git',
     author='Event2trading',
```

