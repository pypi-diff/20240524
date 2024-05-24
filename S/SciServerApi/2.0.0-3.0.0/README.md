# Comparing `tmp/SciServerApi-2.0.0.tar.gz` & `tmp/SciServerApi-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SciServerApi-2.0.0.tar", last modified: Tue May 21 05:48:23 2024, max compression
+gzip compressed data, was "SciServerApi-3.0.0.tar", last modified: Fri May 24 01:35:34 2024, max compression
```

## Comparing `SciServerApi-2.0.0.tar` & `SciServerApi-3.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/
--rw-r--r--   0 lxj       (1000) lxj       (1000)     1068 2024-05-20 02:42:11.000000 SciServerApi-2.0.0/LICENSE.txt
--rw-r--r--   0 lxj       (1000) lxj       (1000)     1036 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/PKG-INFO
--rw-r--r--   0 lxj       (1000) lxj       (1000)      517 2024-05-20 02:40:38.000000 SciServerApi-2.0.0/README.md
-drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi/
--rw-r--r--   0 lxj       (1000) lxj       (1000)      798 2024-05-20 23:54:12.000000 SciServerApi-2.0.0/SciServerApi/Authentication.py
--rw-r--r--   0 lxj       (1000) lxj       (1000)     9879 2024-05-21 00:47:20.000000 SciServerApi-2.0.0/SciServerApi/Files.py
--rw-r--r--   0 lxj       (1000) lxj       (1000)    15248 2024-05-21 00:34:44.000000 SciServerApi-2.0.0/SciServerApi/Jobs.py
--rw-r--r--   0 lxj       (1000) lxj       (1000)     7655 2024-05-21 05:27:42.000000 SciServerApi-2.0.0/SciServerApi/Opt.py
--rw-r--r--   0 lxj       (1000) lxj       (1000)       27 2024-05-19 13:01:51.000000 SciServerApi-2.0.0/SciServerApi/__init__.py
-drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/
--rw-r--r--   0 lxj       (1000) lxj       (1000)     1036 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/PKG-INFO
--rw-r--r--   0 lxj       (1000) lxj       (1000)      293 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/SOURCES.txt
--rw-r--r--   0 lxj       (1000) lxj       (1000)        1 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/dependency_links.txt
--rw-r--r--   0 lxj       (1000) lxj       (1000)       13 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/SciServerApi.egg-info/top_level.txt
--rw-r--r--   0 lxj       (1000) lxj       (1000)       38 2024-05-21 05:48:23.000000 SciServerApi-2.0.0/setup.cfg
--rw-r--r--   0 lxj       (1000) lxj       (1000)      683 2024-05-21 05:48:08.000000 SciServerApi-2.0.0/setup.py
+drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-24 01:35:34.206514 SciServerApi-3.0.0/
+-rw-r--r--   0 lxj       (1000) lxj       (1000)     1068 2024-05-20 02:42:11.000000 SciServerApi-3.0.0/LICENSE.txt
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      920 2024-05-24 01:35:34.206514 SciServerApi-3.0.0/PKG-INFO
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      517 2024-05-20 02:40:38.000000 SciServerApi-3.0.0/README.md
+drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-24 01:35:34.206514 SciServerApi-3.0.0/SciServerApi/
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      798 2024-05-20 23:54:12.000000 SciServerApi-3.0.0/SciServerApi/Authentication.py
+-rw-r--r--   0 lxj       (1000) lxj       (1000)     9879 2024-05-21 00:47:20.000000 SciServerApi-3.0.0/SciServerApi/Files.py
+-rw-r--r--   0 lxj       (1000) lxj       (1000)    15248 2024-05-21 00:34:44.000000 SciServerApi-3.0.0/SciServerApi/Jobs.py
+-rw-r--r--   0 lxj       (1000) lxj       (1000)     7655 2024-05-24 01:34:12.000000 SciServerApi-3.0.0/SciServerApi/Opt.py
+-rw-r--r--   0 lxj       (1000) lxj       (1000)       27 2024-05-19 13:01:51.000000 SciServerApi-3.0.0/SciServerApi/__init__.py
+drwxr-xr-x   0 lxj       (1000) lxj       (1000)        0 2024-05-24 01:35:34.206514 SciServerApi-3.0.0/SciServerApi.egg-info/
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      920 2024-05-24 01:35:34.000000 SciServerApi-3.0.0/SciServerApi.egg-info/PKG-INFO
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      293 2024-05-24 01:35:34.000000 SciServerApi-3.0.0/SciServerApi.egg-info/SOURCES.txt
+-rw-r--r--   0 lxj       (1000) lxj       (1000)        1 2024-05-24 01:35:34.000000 SciServerApi-3.0.0/SciServerApi.egg-info/dependency_links.txt
+-rw-r--r--   0 lxj       (1000) lxj       (1000)       13 2024-05-24 01:35:34.000000 SciServerApi-3.0.0/SciServerApi.egg-info/top_level.txt
+-rw-r--r--   0 lxj       (1000) lxj       (1000)       38 2024-05-24 01:35:34.206514 SciServerApi-3.0.0/setup.cfg
+-rw-r--r--   0 lxj       (1000) lxj       (1000)      683 2024-05-24 01:35:27.000000 SciServerApi-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `SciServerApi-2.0.0/LICENSE.txt` & `SciServerApi-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SciServerApi-2.0.0/PKG-INFO` & `SciServerApi-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: SciServerApi
-Version: 2.0.0
+Version: 3.0.0
 Summary: quick access to sciserver
-Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: MIT License
-Description: 
-        This python package provides functions for quick access to [SciServer](http://www.sciserver.org) APIs (web services) and tools.
-        
-         * [Login](http://portal.sciserver.org): Single sign-on portal to all SciServer applications.
-        
-         * [Jobs](http://apps.sciserver.org/compute/jobs) and [SciQuery Jobs](http://apps.sciserver.org/sciquery-ui/): Synch and asynch submission of Jupyter notebooks, shell commands and SQL queries.
-         
-         * [Files](http://apps.sciserver.org/dashboard/files): Interact with the SciServer file system.
-        
-        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE.txt
+
+
+This python package provides functions for quick access to [SciServer](http://www.sciserver.org) APIs (web services) and tools.
+
+ * [Login](http://portal.sciserver.org): Single sign-on portal to all SciServer applications.
+
+ * [Jobs](http://apps.sciserver.org/compute/jobs) and [SciQuery Jobs](http://apps.sciserver.org/sciquery-ui/): Synch and asynch submission of Jupyter notebooks, shell commands and SQL queries.
+ 
+ * [Files](http://apps.sciserver.org/dashboard/files): Interact with the SciServer file system.
+
```

### Comparing `SciServerApi-2.0.0/README.md` & `SciServerApi-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `SciServerApi-2.0.0/SciServerApi/Authentication.py` & `SciServerApi-3.0.0/SciServerApi/Authentication.py`

 * *Files identical despite different names*

### Comparing `SciServerApi-2.0.0/SciServerApi/Files.py` & `SciServerApi-3.0.0/SciServerApi/Files.py`

 * *Files identical despite different names*

### Comparing `SciServerApi-2.0.0/SciServerApi/Jobs.py` & `SciServerApi-3.0.0/SciServerApi/Jobs.py`

 * *Files identical despite different names*

### Comparing `SciServerApi-2.0.0/SciServerApi/Opt.py` & `SciServerApi-3.0.0/SciServerApi/Opt.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,9 +155,9 @@
         proxy = ""
 
     url = fileService.get("apiEndpoint") + "api/file/" + remotePath.strip("/") + "?TaskName=SciScript-Python.Files.DownloadFile"
     headers = f"X-Auth-Token: {keyToken}"
 
     cmd = proxy + f"sleep {pollTime} && wget \"{url}\" --header \"{headers}\" --output-document \"{localFilePath}\" {wgetArgs}"
     
-    return subprocess.Ppoen(cmd,shell=True)
+    return subprocess.Popen(cmd,shell=True)
```

### Comparing `SciServerApi-2.0.0/SciServerApi.egg-info/PKG-INFO` & `SciServerApi-3.0.0/SciServerApi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: SciServerApi
-Version: 2.0.0
+Version: 3.0.0
 Summary: quick access to sciserver
-Home-page: UNKNOWN
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: MIT License
-Description: 
-        This python package provides functions for quick access to [SciServer](http://www.sciserver.org) APIs (web services) and tools.
-        
-         * [Login](http://portal.sciserver.org): Single sign-on portal to all SciServer applications.
-        
-         * [Jobs](http://apps.sciserver.org/compute/jobs) and [SciQuery Jobs](http://apps.sciserver.org/sciquery-ui/): Synch and asynch submission of Jupyter notebooks, shell commands and SQL queries.
-         
-         * [Files](http://apps.sciserver.org/dashboard/files): Interact with the SciServer file system.
-        
-        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE.txt
+
+
+This python package provides functions for quick access to [SciServer](http://www.sciserver.org) APIs (web services) and tools.
+
+ * [Login](http://portal.sciserver.org): Single sign-on portal to all SciServer applications.
+
+ * [Jobs](http://apps.sciserver.org/compute/jobs) and [SciQuery Jobs](http://apps.sciserver.org/sciquery-ui/): Synch and asynch submission of Jupyter notebooks, shell commands and SQL queries.
+ 
+ * [Files](http://apps.sciserver.org/dashboard/files): Interact with the SciServer file system.
+
```

### Comparing `SciServerApi-2.0.0/setup.py` & `SciServerApi-3.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='SciServerApi',  # 包名
-      version='2.0.0',  # 版本号
+      version='3.0.0',  # 版本号
       description='quick access to sciserver',
       long_description=open("README.md", "r").read(),
       install_requires=[],
       license='MIT License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
```

