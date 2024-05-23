# Comparing `tmp/picopy-1.0.3.tar.gz` & `tmp/picopy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopy-1.0.3.tar", last modified: Thu May 23 21:19:23 2024, max compression
+gzip compressed data, was "picopy-1.0.5.tar", last modified: Thu May 23 21:45:55 2024, max compression
```

## Comparing `picopy-1.0.3.tar` & `picopy-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:23.664076 picopy-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 21:19:19.000000 picopy-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-23 21:19:23.664076 picopy-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-23 21:19:19.000000 picopy-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:23.664076 picopy-1.0.3/picopy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:19.000000 picopy-1.0.3/picopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 21:19:19.000000 picopy-1.0.3/picopy/picopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:23.664076 picopy-1.0.3/picopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-23 21:19:23.000000 picopy-1.0.3/picopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 21:19:23.000000 picopy-1.0.3/picopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:19:23.000000 picopy-1.0.3/picopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 21:19:23.000000 picopy-1.0.3/picopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:19.000000 picopy-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:19:23.664076 picopy-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-23 21:19:19.000000 picopy-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:19:23.664076 picopy-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 21:19:19.000000 picopy-1.0.3/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:55.769512 picopy-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 21:45:47.000000 picopy-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-23 21:45:55.769512 picopy-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 21:45:47.000000 picopy-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:55.769512 picopy-1.0.5/picopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:47.000000 picopy-1.0.5/picopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 21:45:47.000000 picopy-1.0.5/picopy/picopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:55.769512 picopy-1.0.5/picopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-23 21:45:55.000000 picopy-1.0.5/picopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-23 21:45:55.000000 picopy-1.0.5/picopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:45:55.000000 picopy-1.0.5/picopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 21:45:55.000000 picopy-1.0.5/picopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:47.000000 picopy-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:45:55.769512 picopy-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-23 21:45:47.000000 picopy-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:45:55.769512 picopy-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 21:45:47.000000 picopy-1.0.5/tests/test_package.py
```

### Comparing `picopy-1.0.3/picopy/picopy.py` & `picopy-1.0.5/picopy/picopy.py`

 * *Files identical despite different names*

### Comparing `picopy-1.0.3/setup.py` & `picopy-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def pre_install():
     f = open("README.md" , "r")
     text = f.read()
     return text
 
 setup(name="picopy" ,
-      version="1.0.3", 
+      version="1.0.5", 
       author="kiki js" , 
       description="convert an image to a watercolor image 🎨", 
       long_description=pre_install() , # its like readme
       requires= [] ,
       author_email="k.jhnshid@gmail.com",
       packages=["picopy"]
       )
```

