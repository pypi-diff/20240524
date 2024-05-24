# Comparing `tmp/picopy-1.0.8.tar.gz` & `tmp/picopy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopy-1.0.8.tar", last modified: Fri May 24 02:34:53 2024, max compression
+gzip compressed data, was "picopy-1.0.9.tar", last modified: Fri May 24 02:55:32 2024, max compression
```

## Comparing `picopy-1.0.8.tar` & `picopy-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:53.532739 picopy-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:34:49.000000 picopy-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-24 02:34:53.528738 picopy-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 02:34:49.000000 picopy-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:53.528738 picopy-1.0.8/picopy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:49.000000 picopy-1.0.8/picopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-24 02:34:49.000000 picopy-1.0.8/picopy/picopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:53.528738 picopy-1.0.8/picopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 02:34:53.000000 picopy-1.0.8/picopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 02:34:49.000000 picopy-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 02:34:53.532739 picopy-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 02:34:49.000000 picopy-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:34:53.528738 picopy-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 02:34:49.000000 picopy-1.0.8/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:55:32.306871 picopy-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:55:27.000000 picopy-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-24 02:55:32.306871 picopy-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-24 02:55:27.000000 picopy-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:55:32.302871 picopy-1.0.9/picopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:55:27.000000 picopy-1.0.9/picopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-24 02:55:27.000000 picopy-1.0.9/picopy/picopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:55:32.306871 picopy-1.0.9/picopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-24 02:55:32.000000 picopy-1.0.9/picopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 02:55:32.000000 picopy-1.0.9/picopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:55:32.000000 picopy-1.0.9/picopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 02:55:32.000000 picopy-1.0.9/picopy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:55:32.000000 picopy-1.0.9/picopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 02:55:32.000000 picopy-1.0.9/picopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 02:55:27.000000 picopy-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 02:55:32.306871 picopy-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-24 02:55:27.000000 picopy-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:55:32.306871 picopy-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 02:55:27.000000 picopy-1.0.9/tests/test_package.py
```

### Comparing `picopy-1.0.8/PKG-INFO` & `picopy-1.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: picopy
-Version: 1.0.8
+Version: 1.0.9
 Summary: convert an image to a watercolor image 🎨
 Home-page: https://github.com/Kiana-Jahanshid/picopy
 Author: kiki js
 Author-email: k.jhnshid@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: numpy
 
 # Convert an Image To a Watercolor Image 
 
 + Input :
-<p align="center">
-    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/na.jpg" width="290" height="200" >
-</p> 
+<p align="center"><img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/na.jpg" width="290" height="200" ></p> 
 
 <br>
 
 + Output :
-<p align= "center">
-    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/watercolor.jpg" width="410" height="300" >
-</p>
+<p align="center"><img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/watercolor.jpg" width="410" height="300" ></p>
 
 <br/>
 
 # Installation 
 
 ```bash
 pip install picopy
```

### Comparing `picopy-1.0.8/README.md` & `picopy-1.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # Convert an Image To a Watercolor Image 
 
 + Input :
-<p align="center">
-    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/na.jpg" width="290" height="200" >
-</p> 
+<p align="center"><img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/na.jpg" width="290" height="200" ></p> 
 
 <br>
 
 + Output :
-<p align= "center">
-    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/watercolor.jpg" width="410" height="300" >
-</p>
+<p align="center"><img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/watercolor.jpg" width="410" height="300" ></p>
 
 <br/>
 
 # Installation 
 
 ```bash
 pip install picopy
```

### Comparing `picopy-1.0.8/picopy/picopy.py` & `picopy-1.0.9/picopy/picopy.py`

 * *Files identical despite different names*

### Comparing `picopy-1.0.8/picopy.egg-info/PKG-INFO` & `picopy-1.0.9/picopy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: picopy
-Version: 1.0.8
+Version: 1.0.9
 Summary: convert an image to a watercolor image 🎨
 Home-page: https://github.com/Kiana-Jahanshid/picopy
 Author: kiki js
 Author-email: k.jhnshid@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: numpy
 
 # Convert an Image To a Watercolor Image 
 
 + Input :
-<p align="center">
-    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/na.jpg" width="290" height="200" >
-</p> 
+<p align="center"><img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/na.jpg" width="290" height="200" ></p> 
 
 <br>
 
 + Output :
-<p align= "center">
-    <img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/picopy/watercolor.jpg" width="410" height="300" >
-</p>
+<p align="center"><img src="https://github.com/Kiana-Jahanshid/picopy/blob/main/watercolor.jpg" width="410" height="300" ></p>
 
 <br/>
 
 # Installation 
 
 ```bash
 pip install picopy
```

### Comparing `picopy-1.0.8/setup.py` & `picopy-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,22 @@
     return long_description
 
 with open('./requirements.txt') as f:
     install_requires = f.read().splitlines()
 
 
 setup(name="picopy" ,
-    version="1.0.8", 
+    version="1.0.9", 
     author="kiki js" , 
     description="convert an image to a watercolor image 🎨", 
     long_description=pre_install() ,
     requires= [] ,
     author_email="k.jhnshid@gmail.com",
     packages=["picopy"] ,
     long_description_content_type='text/markdown' ,
     install_requires= install_requires ,
     url="https://github.com/Kiana-Jahanshid/picopy" ,
-    entry_points={"console_scripts": ["picopy=picopy.picopy:convert_image_to_watercolor"]}
+    entry_points={"console_scripts": ["picopy=picopy.picopy:convert_image_to_watercolor"]},
+    include_package_data=True
     )
```

