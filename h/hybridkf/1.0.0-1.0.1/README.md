# Comparing `tmp/hybridkf-1.0.0.tar.gz` & `tmp/hybridkf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybridkf-1.0.0.tar", last modified: Fri May 24 17:25:58 2024, max compression
+gzip compressed data, was "hybridkf-1.0.1.tar", last modified: Fri May 24 18:22:48 2024, max compression
```

## Comparing `hybridkf-1.0.0.tar` & `hybridkf-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 17:25:58.233305 hybridkf-1.0.0/
--rw-r--r--   0 aleckain   (501) staff       (20)      319 2024-05-24 17:25:58.233143 hybridkf-1.0.0/PKG-INFO
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 17:25:58.232943 hybridkf-1.0.0/hybridkf.egg-info/
--rw-r--r--   0 aleckain   (501) staff       (20)      319 2024-05-24 17:25:58.000000 hybridkf-1.0.0/hybridkf.egg-info/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)      167 2024-05-24 17:25:58.000000 hybridkf-1.0.0/hybridkf.egg-info/SOURCES.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 17:25:58.000000 hybridkf-1.0.0/hybridkf.egg-info/dependency_links.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       35 2024-05-24 17:25:58.000000 hybridkf-1.0.0/hybridkf.egg-info/requires.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 17:25:58.000000 hybridkf-1.0.0/hybridkf.egg-info/top_level.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 17:25:58.233349 hybridkf-1.0.0/setup.cfg
--rw-r--r--   0 aleckain   (501) staff       (20)      536 2024-05-24 17:25:36.000000 hybridkf-1.0.0/setup.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 18:22:48.475611 hybridkf-1.0.1/
+-rw-r--r--   0 aleckain   (501) staff       (20)     5707 2024-05-24 18:22:48.475326 hybridkf-1.0.1/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)     5192 2024-05-24 17:56:29.000000 hybridkf-1.0.1/README.md
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 18:22:48.475116 hybridkf-1.0.1/hybridkf.egg-info/
+-rw-r--r--   0 aleckain   (501) staff       (20)     5707 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)      177 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/SOURCES.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/dependency_links.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/requires.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/top_level.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 18:22:48.475673 hybridkf-1.0.1/setup.cfg
+-rw-r--r--   0 aleckain   (501) staff       (20)      783 2024-05-24 18:22:31.000000 hybridkf-1.0.1/setup.py
```

### Comparing `hybridkf-1.0.0/setup.py` & `hybridkf-1.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hybridkf',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     description='''An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.'''
     ,
     author='akain0',
-    url='https://github.com/yourusername/your-package-name',
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
-        'random',
-        'math'
     ],
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    url='https://github.com/akain0/hybridkf',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+    python_requires='>=3.6',
 )
```

