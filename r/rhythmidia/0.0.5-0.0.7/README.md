# Comparing `tmp/rhythmidia-0.0.5.tar.gz` & `tmp/rhythmidia-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhythmidia-0.0.5.tar", last modified: Fri May 24 16:16:29 2024, max compression
+gzip compressed data, was "rhythmidia-0.0.7.tar", last modified: Fri May 24 16:59:28 2024, max compression
```

## Comparing `rhythmidia-0.0.5.tar` & `rhythmidia-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.160488 rhythmidia-0.0.5/
--rw-r--r--   0 akeeley    (504) staff       (20)     3552 2023-11-17 22:38:38.000000 rhythmidia-0.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 akeeley    (504) staff       (20)     1068 2024-05-13 17:38:39.000000 rhythmidia-0.0.5/LICENSE
--rw-r--r--   0 akeeley    (504) staff       (20)       70 2023-11-17 22:38:38.000000 rhythmidia-0.0.5/MANIFEST.in
--rw-r--r--   0 akeeley    (504) staff       (20)     9099 2024-05-24 16:16:29.160382 rhythmidia-0.0.5/PKG-INFO
--rw-r--r--   0 akeeley    (504) staff       (20)     8367 2024-05-24 16:10:59.000000 rhythmidia-0.0.5/README.md
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.149870 rhythmidia-0.0.5/images/
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.157131 rhythmidia-0.0.5/images/icons/
--rw-r--r--   0 akeeley    (504) staff       (20)   297429 2024-05-10 20:19:43.000000 rhythmidia-0.0.5/images/icons/pelhamLogoSquare.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)   106534 2024-05-10 20:19:43.000000 rhythmidia-0.0.5/images/icons/rhythmidiaLogoBannerText.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)   885265 2024-05-10 20:19:43.000000 rhythmidia-0.0.5/images/icons/rhythmidiaLogoSquare.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)     3517 2024-05-17 20:41:21.000000 rhythmidia-0.0.5/pyproject.toml
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.152655 rhythmidia-0.0.5/rhythmidia/
--rw-r--r--   0 akeeley    (504) staff       (20)      372 2024-05-17 20:31:36.000000 rhythmidia-0.0.5/rhythmidia/__init__.py
--rw-r--r--   0 akeeley    (504) staff       (20)       22 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia/_version.py
--rw-r--r--   0 akeeley    (504) staff       (20)        0 2024-05-10 20:19:44.000000 rhythmidia-0.0.5/rhythmidia/parameters.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       61 2023-11-17 22:38:38.000000 rhythmidia-0.0.5/rhythmidia/py.typed
--rw-r--r--   0 akeeley    (504) staff       (20)      295 2024-05-17 20:18:49.000000 rhythmidia-0.0.5/rhythmidia/rhythmidia.py
--rw-r--r--   0 akeeley    (504) staff       (20)   147957 2024-05-17 20:35:38.000000 rhythmidia-0.0.5/rhythmidia/rhythmidia_gui.py
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.159528 rhythmidia-0.0.5/rhythmidia/tests/
--rw-r--r--   0 akeeley    (504) staff       (20)      113 2023-11-17 22:38:38.000000 rhythmidia-0.0.5/rhythmidia/tests/__init__.py
--rw-r--r--   0 akeeley    (504) staff       (20)     6373 2024-05-10 20:19:44.000000 rhythmidia-0.0.5/rhythmidia/tests/test_rhythmidia.py
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.159885 rhythmidia-0.0.5/rhythmidia.egg-info/
--rw-r--r--   0 akeeley    (504) staff       (20)     9099 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/PKG-INFO
--rw-r--r--   0 akeeley    (504) staff       (20)      679 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/SOURCES.txt
--rw-r--r--   0 akeeley    (504) staff       (20)        1 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/dependency_links.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       57 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/entry_points.txt
--rw-r--r--   0 akeeley    (504) staff       (20)        1 2023-11-17 23:02:20.000000 rhythmidia-0.0.5/rhythmidia.egg-info/not-zip-safe
--rw-r--r--   0 akeeley    (504) staff       (20)      157 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/requires.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       11 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/top_level.txt
--rw-r--r--   0 akeeley    (504) staff       (20)      215 2024-05-24 16:16:29.160776 rhythmidia-0.0.5/setup.cfg
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.908012 rhythmidia-0.0.7/
+-rw-r--r--   0 akeeley    (504) staff       (20)     3552 2023-11-17 22:38:38.000000 rhythmidia-0.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 akeeley    (504) staff       (20)     1068 2024-05-13 17:38:39.000000 rhythmidia-0.0.7/LICENSE
+-rw-r--r--   0 akeeley    (504) staff       (20)       70 2023-11-17 22:38:38.000000 rhythmidia-0.0.7/MANIFEST.in
+-rw-r--r--   0 akeeley    (504) staff       (20)     9216 2024-05-24 16:59:28.907887 rhythmidia-0.0.7/PKG-INFO
+-rw-r--r--   0 akeeley    (504) staff       (20)     8484 2024-05-24 16:57:32.000000 rhythmidia-0.0.7/README.md
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.897378 rhythmidia-0.0.7/images/
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.904117 rhythmidia-0.0.7/images/icons/
+-rw-r--r--   0 akeeley    (504) staff       (20)   297429 2024-05-10 20:19:43.000000 rhythmidia-0.0.7/images/icons/pelhamLogoSquare.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)   106534 2024-05-10 20:19:43.000000 rhythmidia-0.0.7/images/icons/rhythmidiaLogoBannerText.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)   885265 2024-05-10 20:19:43.000000 rhythmidia-0.0.7/images/icons/rhythmidiaLogoSquare.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)     3517 2024-05-17 20:41:21.000000 rhythmidia-0.0.7/pyproject.toml
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.900023 rhythmidia-0.0.7/rhythmidia/
+-rw-r--r--   0 akeeley    (504) staff       (20)      372 2024-05-17 20:31:36.000000 rhythmidia-0.0.7/rhythmidia/__init__.py
+-rw-r--r--   0 akeeley    (504) staff       (20)       22 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia/_version.py
+-rw-r--r--   0 akeeley    (504) staff       (20)        0 2024-05-10 20:19:44.000000 rhythmidia-0.0.7/rhythmidia/parameters.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       61 2023-11-17 22:38:38.000000 rhythmidia-0.0.7/rhythmidia/py.typed
+-rw-r--r--   0 akeeley    (504) staff       (20)      295 2024-05-17 20:18:49.000000 rhythmidia-0.0.7/rhythmidia/rhythmidia.py
+-rw-r--r--   0 akeeley    (504) staff       (20)   147957 2024-05-17 20:35:38.000000 rhythmidia-0.0.7/rhythmidia/rhythmidia_gui.py
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.906761 rhythmidia-0.0.7/rhythmidia/tests/
+-rw-r--r--   0 akeeley    (504) staff       (20)      113 2023-11-17 22:38:38.000000 rhythmidia-0.0.7/rhythmidia/tests/__init__.py
+-rw-r--r--   0 akeeley    (504) staff       (20)     6373 2024-05-10 20:19:44.000000 rhythmidia-0.0.7/rhythmidia/tests/test_rhythmidia.py
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.907391 rhythmidia-0.0.7/rhythmidia.egg-info/
+-rw-r--r--   0 akeeley    (504) staff       (20)     9216 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/PKG-INFO
+-rw-r--r--   0 akeeley    (504) staff       (20)      679 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/SOURCES.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)        1 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/dependency_links.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       57 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/entry_points.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)        1 2023-11-17 23:02:20.000000 rhythmidia-0.0.7/rhythmidia.egg-info/not-zip-safe
+-rw-r--r--   0 akeeley    (504) staff       (20)      157 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/requires.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       11 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/top_level.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)      215 2024-05-24 16:59:28.908326 rhythmidia-0.0.7/setup.cfg
```

### Comparing `rhythmidia-0.0.5/CODE_OF_CONDUCT.md` & `rhythmidia-0.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.5/LICENSE` & `rhythmidia-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.5/PKG-INFO` & `rhythmidia-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhythmidia
-Version: 0.0.5
+Version: 0.0.7
 Summary: Race tube image analysis and period elucidation in Python.
 Author-email: Alex Keeley <alex.k@wustl.edu>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -56,14 +56,15 @@
 2. No need to make your image greyscale, fix its rotation, or increase contrast- Rhythmidia will take care of all of this internally!
 3. Race tube images can be .png, .tif, .tiff, .jpg, .jpeg, or .svg
 
 ---
 ## Uploading and Analyzing an Image
 1. Upon opening the software, you will be greeted with the “Home” tab, which will look like this:
 ![Home Tab (blank)](images/screenshots/HomeTabBlank.png)
+![Home Tab (blank)](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/HomeTabBlank.png?raw=true)
     NOTE:If you want to add tubes to an existing experiment file, go to File -> Open experiment File (or press ⌘O), although this is not necessary
 2. To upload a new race tube image, click the button labeled “Upload Race Tube Image”<br />
 ![Upload Image Button](images/screenshots/UploadImageButton.png)
     a. Your image will appear in the center of the screen<br />
     ![Image Analysis](images/screenshots/ImageAnal1.png)
     b. Uploading an image enables the options to rotate and to lock & analyze your image<br />
     ![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)
```

### Comparing `rhythmidia-0.0.5/README.md` & `rhythmidia-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 2. No need to make your image greyscale, fix its rotation, or increase contrast- Rhythmidia will take care of all of this internally!
 3. Race tube images can be .png, .tif, .tiff, .jpg, .jpeg, or .svg
 
 ---
 ## Uploading and Analyzing an Image
 1. Upon opening the software, you will be greeted with the “Home” tab, which will look like this:
 ![Home Tab (blank)](images/screenshots/HomeTabBlank.png)
+![Home Tab (blank)](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/HomeTabBlank.png?raw=true)
     NOTE:If you want to add tubes to an existing experiment file, go to File -> Open experiment File (or press ⌘O), although this is not necessary
 2. To upload a new race tube image, click the button labeled “Upload Race Tube Image”<br />
 ![Upload Image Button](images/screenshots/UploadImageButton.png)
     a. Your image will appear in the center of the screen<br />
     ![Image Analysis](images/screenshots/ImageAnal1.png)
     b. Uploading an image enables the options to rotate and to lock & analyze your image<br />
     ![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)
```

### Comparing `rhythmidia-0.0.5/images/icons/pelhamLogoSquare.jpg` & `rhythmidia-0.0.7/images/icons/pelhamLogoSquare.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.5/images/icons/rhythmidiaLogoBannerText.jpg` & `rhythmidia-0.0.7/images/icons/rhythmidiaLogoBannerText.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.5/images/icons/rhythmidiaLogoSquare.jpg` & `rhythmidia-0.0.7/images/icons/rhythmidiaLogoSquare.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.5/pyproject.toml` & `rhythmidia-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.5/rhythmidia/rhythmidia_gui.py` & `rhythmidia-0.0.7/rhythmidia/rhythmidia_gui.py`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.5/rhythmidia/tests/test_rhythmidia.py` & `rhythmidia-0.0.7/rhythmidia/tests/test_rhythmidia.py`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.5/rhythmidia.egg-info/PKG-INFO` & `rhythmidia-0.0.7/rhythmidia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhythmidia
-Version: 0.0.5
+Version: 0.0.7
 Summary: Race tube image analysis and period elucidation in Python.
 Author-email: Alex Keeley <alex.k@wustl.edu>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -56,14 +56,15 @@
 2. No need to make your image greyscale, fix its rotation, or increase contrast- Rhythmidia will take care of all of this internally!
 3. Race tube images can be .png, .tif, .tiff, .jpg, .jpeg, or .svg
 
 ---
 ## Uploading and Analyzing an Image
 1. Upon opening the software, you will be greeted with the “Home” tab, which will look like this:
 ![Home Tab (blank)](images/screenshots/HomeTabBlank.png)
+![Home Tab (blank)](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/HomeTabBlank.png?raw=true)
     NOTE:If you want to add tubes to an existing experiment file, go to File -> Open experiment File (or press ⌘O), although this is not necessary
 2. To upload a new race tube image, click the button labeled “Upload Race Tube Image”<br />
 ![Upload Image Button](images/screenshots/UploadImageButton.png)
     a. Your image will appear in the center of the screen<br />
     ![Image Analysis](images/screenshots/ImageAnal1.png)
     b. Uploading an image enables the options to rotate and to lock & analyze your image<br />
     ![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)
```

### Comparing `rhythmidia-0.0.5/rhythmidia.egg-info/SOURCES.txt` & `rhythmidia-0.0.7/rhythmidia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

