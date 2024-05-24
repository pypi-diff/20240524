# Comparing `tmp/picopy-1.0.7.tar.gz` & `tmp/picopy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopy-1.0.7.tar", last modified: Fri May 24 02:07:33 2024, max compression
+gzip compressed data, was "picopy-1.0.8.tar", last modified: Fri May 24 02:34:53 2024, max compression
```

## Comparing `picopy-1.0.7.tar` & `picopy-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:33.824887 picopy-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:07:30.000000 picopy-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-24 02:07:33.824887 picopy-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-24 02:07:30.000000 picopy-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:33.824887 picopy-1.0.7/picopy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:30.000000 picopy-1.0.7/picopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-24 02:07:30.000000 picopy-1.0.7/picopy/picopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:33.824887 picopy-1.0.7/picopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 02:07:30.000000 picopy-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 02:07:33.824887 picopy-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-24 02:07:30.000000 picopy-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:33.824887 picopy-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 02:07:30.000000 picopy-1.0.7/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:53.532739 picopy-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:34:49.000000 picopy-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-24 02:34:53.528738 picopy-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 02:34:49.000000 picopy-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:53.528738 picopy-1.0.8/picopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:49.000000 picopy-1.0.8/picopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-24 02:34:49.000000 picopy-1.0.8/picopy/picopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:53.528738 picopy-1.0.8/picopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 02:34:49.000000 picopy-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 02:34:53.532739 picopy-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 02:34:49.000000 picopy-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:53.528738 picopy-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 02:34:49.000000 picopy-1.0.8/tests/test_package.py
```

### Comparing `picopy-1.0.7/PKG-INFO` & `picopy-1.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: picopy
-Version: 1.0.7
+Version: 1.0.8
 Summary: convert an image to a watercolor image 🎨
+Home-page: https://github.com/Kiana-Jahanshid/picopy
 Author: kiki js
 Author-email: k.jhnshid@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: numpy
 
 # Convert an Image To a Watercolor Image 
 
 + Input :
 <p align="center">
-    <img src="picopy/na.jpg" width="290" height="200" >
+    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/na.jpg" width="290" height="200" >
 </p> 
 
 <br>
 
 + Output :
 <p align= "center">
-    <img src="picopy/watercolor.jpg" width="410" height="300" >
+    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/watercolor.jpg" width="410" height="300" >
 </p>
 
 <br/>
 
 # Installation 
 
 ```bash
```

### Comparing `picopy-1.0.7/picopy/picopy.py` & `picopy-1.0.8/picopy/picopy.py`

 * *Files identical despite different names*

### Comparing `picopy-1.0.7/picopy.egg-info/PKG-INFO` & `picopy-1.0.8/picopy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: picopy
-Version: 1.0.7
+Version: 1.0.8
 Summary: convert an image to a watercolor image 🎨
+Home-page: https://github.com/Kiana-Jahanshid/picopy
 Author: kiki js
 Author-email: k.jhnshid@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: numpy
 
 # Convert an Image To a Watercolor Image 
 
 + Input :
 <p align="center">
-    <img src="picopy/na.jpg" width="290" height="200" >
+    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/na.jpg" width="290" height="200" >
 </p> 
 
 <br>
 
 + Output :
 <p align= "center">
-    <img src="picopy/watercolor.jpg" width="410" height="300" >
+    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/watercolor.jpg" width="410" height="300" >
 </p>
 
 <br/>
 
 # Installation 
 
 ```bash
```

### Comparing `picopy-1.0.7/setup.py` & `picopy-1.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,21 @@
     return long_description
 
 with open('./requirements.txt') as f:
     install_requires = f.read().splitlines()
 
 
 setup(name="picopy" ,
-    version="1.0.7", 
+    version="1.0.8", 
     author="kiki js" , 
     description="convert an image to a watercolor image 🎨", 
     long_description=pre_install() ,
     requires= [] ,
     author_email="k.jhnshid@gmail.com",
     packages=["picopy"] ,
     long_description_content_type='text/markdown' ,
-    install_requires= install_requires
+    install_requires= install_requires ,
+    url="https://github.com/Kiana-Jahanshid/picopy" ,
+    entry_points={"console_scripts": ["picopy=picopy.picopy:convert_image_to_watercolor"]}
     )
```

