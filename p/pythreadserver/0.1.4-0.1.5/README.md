# Comparing `tmp/pythreadserver-0.1.4.tar.gz` & `tmp/pythreadserver-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythreadserver-0.1.4.tar", last modified: Sat May 18 16:34:59 2024, max compression
+gzip compressed data, was "pythreadserver-0.1.5.tar", last modified: Thu May 23 19:26:30 2024, max compression
```

## Comparing `pythreadserver-0.1.4.tar` & `pythreadserver-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 16:34:59.644030 pythreadserver-0.1.4/
--rw-rw-rw-   0        0        0      512 2024-05-18 16:34:59.644030 pythreadserver-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-11 10:23:05.000000 pythreadserver-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 16:34:59.634147 pythreadserver-0.1.4/pythreadserver/
--rw-rw-rw-   0        0        0       60 2024-05-11 10:43:35.000000 pythreadserver-0.1.4/pythreadserver/__init__.py
--rw-rw-rw-   0        0        0     3312 2024-05-17 17:27:10.000000 pythreadserver-0.1.4/pythreadserver/client.py
--rw-rw-rw-   0        0        0      115 2024-05-17 17:38:09.000000 pythreadserver-0.1.4/pythreadserver/constants.py
--rw-rw-rw-   0        0        0     4994 2024-05-17 20:19:39.000000 pythreadserver-0.1.4/pythreadserver/server.py
--rw-rw-rw-   0        0        0      561 2024-05-11 10:43:35.000000 pythreadserver-0.1.4/pythreadserver/textlog.py
-drwxrwxrwx   0        0        0        0 2024-05-18 16:34:59.643030 pythreadserver-0.1.4/pythreadserver.egg-info/
--rw-rw-rw-   0        0        0      512 2024-05-18 16:34:59.000000 pythreadserver-0.1.4/pythreadserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-05-18 16:34:59.000000 pythreadserver-0.1.4/pythreadserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 16:34:59.000000 pythreadserver-0.1.4/pythreadserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-18 16:34:59.000000 pythreadserver-0.1.4/pythreadserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 16:34:59.644030 pythreadserver-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      781 2024-05-18 16:32:02.000000 pythreadserver-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:26:30.754998 pythreadserver-0.1.5/
+-rw-rw-rw-   0        0        0      512 2024-05-23 19:26:30.751770 pythreadserver-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-11 10:23:05.000000 pythreadserver-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 19:26:30.739788 pythreadserver-0.1.5/pythreadserver/
+-rw-rw-rw-   0        0        0       60 2024-05-11 10:43:35.000000 pythreadserver-0.1.5/pythreadserver/__init__.py
+-rw-rw-rw-   0        0        0     3312 2024-05-17 17:27:10.000000 pythreadserver-0.1.5/pythreadserver/client.py
+-rw-rw-rw-   0        0        0      115 2024-05-17 17:38:09.000000 pythreadserver-0.1.5/pythreadserver/constants.py
+-rw-rw-rw-   0        0        0     4994 2024-05-17 20:19:39.000000 pythreadserver-0.1.5/pythreadserver/server.py
+-rw-rw-rw-   0        0        0      561 2024-05-11 10:43:35.000000 pythreadserver-0.1.5/pythreadserver/textlog.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:26:30.750770 pythreadserver-0.1.5/pythreadserver.egg-info/
+-rw-rw-rw-   0        0        0      512 2024-05-23 19:26:30.000000 pythreadserver-0.1.5/pythreadserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-05-23 19:26:30.000000 pythreadserver-0.1.5/pythreadserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:26:30.000000 pythreadserver-0.1.5/pythreadserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 19:26:30.000000 pythreadserver-0.1.5/pythreadserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:26:30.754998 pythreadserver-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-05-23 19:26:12.000000 pythreadserver-0.1.5/setup.py
```

### Comparing `pythreadserver-0.1.4/PKG-INFO` & `pythreadserver-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythreadserver
-Version: 0.1.4
+Version: 0.1.5
 Summary: Socket-based server package
 Author: rain1107
 Author-email: ryanbays@icloud.com
 Keywords: python,socket,threading
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythreadserver-0.1.4/pythreadserver/client.py` & `pythreadserver-0.1.5/pythreadserver/client.py`

 * *Files identical despite different names*

### Comparing `pythreadserver-0.1.4/pythreadserver/server.py` & `pythreadserver-0.1.5/pythreadserver/server.py`

 * *Files identical despite different names*

### Comparing `pythreadserver-0.1.4/pythreadserver/textlog.py` & `pythreadserver-0.1.5/pythreadserver/textlog.py`

 * *Files identical despite different names*

### Comparing `pythreadserver-0.1.4/pythreadserver.egg-info/PKG-INFO` & `pythreadserver-0.1.5/pythreadserver.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythreadserver
-Version: 0.1.4
+Version: 0.1.5
 Summary: Socket-based server package
 Author: rain1107
 Author-email: ryanbays@icloud.com
 Keywords: python,socket,threading
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythreadserver-0.1.4/setup.py` & `pythreadserver-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Socket-based server package'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="pythreadserver",
     version=VERSION,
```

