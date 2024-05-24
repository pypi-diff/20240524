# Comparing `tmp/pythub-0.1.0.tar.gz` & `tmp/pythub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythub-0.1.0.tar", last modified: Thu May 23 21:21:00 2024, max compression
+gzip compressed data, was "pythub-0.1.1.tar", last modified: Fri May 24 08:45:09 2024, max compression
```

## Comparing `pythub-0.1.0.tar` & `pythub-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 moustafa   (501) staff       (20)        0 2024-05-23 21:21:00.620666 pythub-0.1.0/
--rw-r--r--   0 moustafa   (501) staff       (20)     1056 2024-05-23 20:45:23.000000 pythub-0.1.0/LICENSE
--rw-r--r--   0 moustafa   (501) staff       (20)     3361 2024-05-23 21:21:00.620177 pythub-0.1.0/PKG-INFO
--rw-rw-r--   0 moustafa   (501) staff       (20)     2724 2024-05-23 21:20:56.000000 pythub-0.1.0/README.md
-drwxr-xr-x   0 moustafa   (501) staff       (20)        0 2024-05-23 21:21:00.619542 pythub-0.1.0/pythub.egg-info/
--rw-r--r--   0 moustafa   (501) staff       (20)     3361 2024-05-23 21:21:00.000000 pythub-0.1.0/pythub.egg-info/PKG-INFO
--rw-r--r--   0 moustafa   (501) staff       (20)      175 2024-05-23 21:21:00.000000 pythub-0.1.0/pythub.egg-info/SOURCES.txt
--rw-r--r--   0 moustafa   (501) staff       (20)        1 2024-05-23 21:21:00.000000 pythub-0.1.0/pythub.egg-info/dependency_links.txt
--rw-r--r--   0 moustafa   (501) staff       (20)       31 2024-05-23 21:21:00.000000 pythub-0.1.0/pythub.egg-info/requires.txt
--rw-r--r--   0 moustafa   (501) staff       (20)        1 2024-05-23 21:21:00.000000 pythub-0.1.0/pythub.egg-info/top_level.txt
--rw-r--r--   0 moustafa   (501) staff       (20)       38 2024-05-23 21:21:00.620803 pythub-0.1.0/setup.cfg
--rw-r--r--   0 moustafa   (501) staff       (20)      809 2024-05-23 21:20:57.000000 pythub-0.1.0/setup.py
+drwxr-xr-x   0 moustafa   (501) staff       (20)        0 2024-05-24 08:45:09.462133 pythub-0.1.1/
+-rw-r--r--   0 moustafa   (501) staff       (20)     1056 2024-05-23 20:45:23.000000 pythub-0.1.1/LICENSE
+-rw-r--r--   0 moustafa   (501) staff       (20)     3361 2024-05-24 08:45:09.461655 pythub-0.1.1/PKG-INFO
+-rw-rw-r--   0 moustafa   (501) staff       (20)     2724 2024-05-23 21:20:56.000000 pythub-0.1.1/README.md
+drwxr-xr-x   0 moustafa   (501) staff       (20)        0 2024-05-24 08:45:09.461031 pythub-0.1.1/pythub.egg-info/
+-rw-r--r--   0 moustafa   (501) staff       (20)     3361 2024-05-24 08:45:09.000000 pythub-0.1.1/pythub.egg-info/PKG-INFO
+-rw-r--r--   0 moustafa   (501) staff       (20)      175 2024-05-24 08:45:09.000000 pythub-0.1.1/pythub.egg-info/SOURCES.txt
+-rw-r--r--   0 moustafa   (501) staff       (20)        1 2024-05-24 08:45:09.000000 pythub-0.1.1/pythub.egg-info/dependency_links.txt
+-rw-r--r--   0 moustafa   (501) staff       (20)       31 2024-05-24 08:45:09.000000 pythub-0.1.1/pythub.egg-info/requires.txt
+-rw-r--r--   0 moustafa   (501) staff       (20)        1 2024-05-24 08:45:09.000000 pythub-0.1.1/pythub.egg-info/top_level.txt
+-rw-r--r--   0 moustafa   (501) staff       (20)       38 2024-05-24 08:45:09.462230 pythub-0.1.1/setup.cfg
+-rw-r--r--   0 moustafa   (501) staff       (20)      809 2024-05-24 08:44:23.000000 pythub-0.1.1/setup.py
```

### Comparing `pythub-0.1.0/LICENSE` & `pythub-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythub-0.1.0/PKG-INFO` & `pythub-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythub
-Version: 0.1.0
+Version: 0.1.1
 Summary: A comprehensive Python library for data preprocessing tasks
 Home-page: https://github.com/mehmetrecep/pythub
 Author: MOHAMED RAGAB ABDELFATTAH ABDELFADEEL-MHD Alhabeb Alshalah-AHMED EMAD ELSAYED MOHAMED ABDELFATTAH
 Author-email: mehmetrecep650@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pythub-0.1.0/README.md` & `pythub-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pythub-0.1.0/pythub.egg-info/PKG-INFO` & `pythub-0.1.1/pythub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythub
-Version: 0.1.0
+Version: 0.1.1
 Summary: A comprehensive Python library for data preprocessing tasks
 Home-page: https://github.com/mehmetrecep/pythub
 Author: MOHAMED RAGAB ABDELFATTAH ABDELFADEEL-MHD Alhabeb Alshalah-AHMED EMAD ELSAYED MOHAMED ABDELFATTAH
 Author-email: mehmetrecep650@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pythub-0.1.0/setup.py` & `pythub-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pythub',
-    version='0.1.0',
+    version='0.1.1',
     author='MOHAMED RAGAB ABDELFATTAH ABDELFADEEL-MHD Alhabeb Alshalah-AHMED EMAD ELSAYED MOHAMED ABDELFATTAH',
     author_email='mehmetrecep650@gmail.com',
     description='A comprehensive Python library for data preprocessing tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/mehmetrecep/pythub',
     packages=find_packages(),
```

