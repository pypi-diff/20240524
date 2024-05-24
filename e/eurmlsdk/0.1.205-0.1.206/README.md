# Comparing `tmp/eurmlsdk-0.1.205.tar.gz` & `tmp/eurmlsdk-0.1.206.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.1.205.tar", last modified: Thu May 23 08:43:17 2024, max compression
+gzip compressed data, was "eurmlsdk-0.1.206.tar", last modified: Thu May 23 09:40:46 2024, max compression
```

## Comparing `eurmlsdk-0.1.205.tar` & `eurmlsdk-0.1.206.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.205/LICENSE.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.205/MANIFEST.in
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      665 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:05.000000 eurmlsdk-0.1.205/README.md
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/eurmlsdk/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.205/eurmlsdk/__init__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6424 2024-05-21 10:12:39.000000 eurmlsdk-0.1.205/eurmlsdk/__main__.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9564 2024-05-23 08:15:17.000000 eurmlsdk-0.1.205/eurmlsdk/eur_sdk.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1441 2024-05-23 07:55:38.000000 eurmlsdk-0.1.205/eurmlsdk/hello.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      312 2024-05-23 07:57:34.000000 eurmlsdk-0.1.205/eurmlsdk/pt.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.205/eurmlsdk/pytorch.py
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1508 2024-05-23 08:18:45.000000 eurmlsdk-0.1.205/eurmlsdk/yolo.py
-drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/eurmlsdk.egg-info/
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      665 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      368 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       52 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      136 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-23 08:43:17.000000 eurmlsdk-0.1.205/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-23 08:43:17.687239 eurmlsdk-0.1.205/setup.cfg
--rw-r--r--   0 sanjay    (1000) sanjay    (1000)      914 2024-05-23 08:41:21.000000 eurmlsdk-0.1.205/setup.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 09:40:46.726891 eurmlsdk-0.1.206/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       16 2024-05-07 10:55:35.000000 eurmlsdk-0.1.206/LICENSE.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-07 10:55:35.000000 eurmlsdk-0.1.206/MANIFEST.in
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      681 2024-05-23 09:40:46.726891 eurmlsdk-0.1.206/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 08:43:05.000000 eurmlsdk-0.1.206/README.md
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 09:40:46.726891 eurmlsdk-0.1.206/eurmlsdk/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       33 2024-05-15 11:40:23.000000 eurmlsdk-0.1.206/eurmlsdk/__init__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     6424 2024-05-21 10:12:39.000000 eurmlsdk-0.1.206/eurmlsdk/__main__.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     9564 2024-05-23 08:15:17.000000 eurmlsdk-0.1.206/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1441 2024-05-23 07:55:38.000000 eurmlsdk-0.1.206/eurmlsdk/hello.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      312 2024-05-23 07:57:34.000000 eurmlsdk-0.1.206/eurmlsdk/pt.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     4036 2024-05-16 09:13:37.000000 eurmlsdk-0.1.206/eurmlsdk/pytorch.py
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)     1508 2024-05-23 08:18:45.000000 eurmlsdk-0.1.206/eurmlsdk/yolo.py
+drwxr-xr-x   0 sanjay    (1000) sanjay    (1000)        0 2024-05-23 09:40:46.726891 eurmlsdk-0.1.206/eurmlsdk.egg-info/
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      681 2024-05-23 09:40:46.000000 eurmlsdk-0.1.206/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      368 2024-05-23 09:40:46.000000 eurmlsdk-0.1.206/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        1 2024-05-23 09:40:46.000000 eurmlsdk-0.1.206/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       52 2024-05-23 09:40:46.000000 eurmlsdk-0.1.206/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      137 2024-05-23 09:40:46.000000 eurmlsdk-0.1.206/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)        9 2024-05-23 09:40:46.000000 eurmlsdk-0.1.206/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)       38 2024-05-23 09:40:46.726891 eurmlsdk-0.1.206/setup.cfg
+-rw-r--r--   0 sanjay    (1000) sanjay    (1000)      915 2024-05-23 09:40:32.000000 eurmlsdk-0.1.206/setup.py
```

### Comparing `eurmlsdk-0.1.205/PKG-INFO` & `eurmlsdk-0.1.206/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurmlsdk
-Version: 0.1.205
+Version: 0.1.206
 Summary: eUR ML SDK
 Author: eUR
 Author-email: aiml@embedur.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,8 +17,9 @@
 Requires-Dist: tensorflow==2.13.1
 Requires-Dist: tqdm
 Requires-Dist: ultralytics
 Requires-Dist: torch
 Requires-Dist: timm
 Requires-Dist: torchvision
 Requires-Dist: menpo
-Requires-Dist: opencv-contrib-pythonnetron
+Requires-Dist: opencv-contrib-python
+Requires-Dist: netron
```

### Comparing `eurmlsdk-0.1.205/eurmlsdk/__main__.py` & `eurmlsdk-0.1.206/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.205/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.1.206/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.205/eurmlsdk/hello.py` & `eurmlsdk-0.1.206/eurmlsdk/hello.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.205/eurmlsdk/pytorch.py` & `eurmlsdk-0.1.206/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.205/eurmlsdk/yolo.py` & `eurmlsdk-0.1.206/eurmlsdk/yolo.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.1.205/eurmlsdk.egg-info/PKG-INFO` & `eurmlsdk-0.1.206/eurmlsdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurmlsdk
-Version: 0.1.205
+Version: 0.1.206
 Summary: eUR ML SDK
 Author: eUR
 Author-email: aiml@embedur.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,8 +17,9 @@
 Requires-Dist: tensorflow==2.13.1
 Requires-Dist: tqdm
 Requires-Dist: ultralytics
 Requires-Dist: torch
 Requires-Dist: timm
 Requires-Dist: torchvision
 Requires-Dist: menpo
-Requires-Dist: opencv-contrib-pythonnetron
+Requires-Dist: opencv-contrib-python
+Requires-Dist: netron
```

### Comparing `eurmlsdk-0.1.205/setup.py` & `eurmlsdk-0.1.206/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.1.205',
+    version='0.1.206',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
@@ -14,15 +14,15 @@
         'tensorflow==2.13.1',
         'tqdm',
         'ultralytics',
         'torch',
         'timm',
         'torchvision',
         'menpo',
-        'opencv-contrib-python'    
+        'opencv-contrib-python' ,   
         'netron'
 ],
     author='eUR',
     author_email='aiml@embedur.com',
     license='MIT',
     entry_points={
         "console_scripts": [
```

