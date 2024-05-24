# Comparing `tmp/picopy-1.0.6.tar.gz` & `tmp/picopy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopy-1.0.6.tar", last modified: Thu May 23 23:21:17 2024, max compression
+gzip compressed data, was "picopy-1.0.7.tar", last modified: Fri May 24 02:07:33 2024, max compression
```

## Comparing `picopy-1.0.6.tar` & `picopy-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:17.785627 picopy-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 23:21:13.000000 picopy-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-23 23:21:17.785627 picopy-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 23:21:13.000000 picopy-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:17.785627 picopy-1.0.6/picopy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:13.000000 picopy-1.0.6/picopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-23 23:21:13.000000 picopy-1.0.6/picopy/picopy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:17.785627 picopy-1.0.6/picopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 23:21:17.000000 picopy-1.0.6/picopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 23:21:13.000000 picopy-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 23:21:17.785627 picopy-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 23:21:13.000000 picopy-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:21:17.785627 picopy-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 23:21:13.000000 picopy-1.0.6/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:33.824887 picopy-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:07:30.000000 picopy-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-24 02:07:33.824887 picopy-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-24 02:07:30.000000 picopy-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:33.824887 picopy-1.0.7/picopy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:30.000000 picopy-1.0.7/picopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-24 02:07:30.000000 picopy-1.0.7/picopy/picopy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:33.824887 picopy-1.0.7/picopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 02:07:33.000000 picopy-1.0.7/picopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 02:07:30.000000 picopy-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 02:07:33.824887 picopy-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-24 02:07:30.000000 picopy-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:07:33.824887 picopy-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 02:07:30.000000 picopy-1.0.7/tests/test_package.py
```

### Comparing `picopy-1.0.6/picopy/picopy.py` & `picopy-1.0.7/picopy/picopy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import cv2
 import numpy as np
+import argparse 
 
 def convert_image_to_watercolor(input_image):
     image = cv2.imread(input_image)
     image_resized = cv2.resize(image, None, fx=1.5, fy=1.5)
 
     #removing impurities from image
     image_cleared = cv2.medianBlur(image_resized, 3)
-    #image_cleared = cv2.medianBlur(image_cleared, 3)
     image_cleared = cv2.medianBlur(image_cleared, 3)
+    #image_cleared = cv2.medianBlur(image_cleared, 3)
     image_cleared = cv2.edgePreservingFilter(image_cleared, sigma_s=5)
 
     #Bilateral Image filtering 
     image_filtered = cv2.bilateralFilter(image_cleared, 5, 10, 5)
     for i in range(2):
         image_filtered = cv2.bilateralFilter(image_filtered, 9, 20, 10)
     for i in range(3):
@@ -28,20 +29,28 @@
     image_sharp = cv2.addWeighted(image_sharp, 1.4, gaussian_mask, -0.2, 10)
     cv2.imwrite("watercolor.jpg" , img=image_sharp)
     #cv2.imshow('Final Image', image_sharp)
     #cv2.waitKey(0)
 
 
 if __name__ == "__main__":
-    input_image = "c1.jpg"
-    watercolor_image = convert_image_to_watercolor(input_image=input_image)
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--imagepath" , type=str , help="write your image's path")
+    arg = parser.parse_args()
+    watercolor_image = convert_image_to_watercolor(input_image=arg.imagepath)
     
 
 
 
-'''
-! pip install picopy
-# from package_name import filename
-from picopy import picopy
-picopy.convert_to_watercolor("image.jpg")
+''' 
+how to run :
+
+!pip install picopy
+from picopy import picopy   # from package_name import filename
+picopy.convert_image_to_watercolor("image.jpg")
+
+or 
+
+pip install picopy
+picopy --imagepath "image.jpg"
 
 '''
```

### Comparing `picopy-1.0.6/setup.py` & `picopy-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     return long_description
 
 with open('./requirements.txt') as f:
     install_requires = f.read().splitlines()
 
 
 setup(name="picopy" ,
-    version="1.0.6", 
+    version="1.0.7", 
     author="kiki js" , 
     description="convert an image to a watercolor image 🎨", 
     long_description=pre_install() ,
     requires= [] ,
     author_email="k.jhnshid@gmail.com",
     packages=["picopy"] ,
     long_description_content_type='text/markdown' ,
```

