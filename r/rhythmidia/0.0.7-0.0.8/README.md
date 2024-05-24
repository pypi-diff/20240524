# Comparing `tmp/rhythmidia-0.0.7.tar.gz` & `tmp/rhythmidia-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhythmidia-0.0.7.tar", last modified: Fri May 24 16:59:28 2024, max compression
+gzip compressed data, was "rhythmidia-0.0.8.tar", last modified: Fri May 24 17:35:50 2024, max compression
```

## Comparing `rhythmidia-0.0.7.tar` & `rhythmidia-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.908012 rhythmidia-0.0.7/
--rw-r--r--   0 akeeley    (504) staff       (20)     3552 2023-11-17 22:38:38.000000 rhythmidia-0.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 akeeley    (504) staff       (20)     1068 2024-05-13 17:38:39.000000 rhythmidia-0.0.7/LICENSE
--rw-r--r--   0 akeeley    (504) staff       (20)       70 2023-11-17 22:38:38.000000 rhythmidia-0.0.7/MANIFEST.in
--rw-r--r--   0 akeeley    (504) staff       (20)     9216 2024-05-24 16:59:28.907887 rhythmidia-0.0.7/PKG-INFO
--rw-r--r--   0 akeeley    (504) staff       (20)     8484 2024-05-24 16:57:32.000000 rhythmidia-0.0.7/README.md
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.897378 rhythmidia-0.0.7/images/
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.904117 rhythmidia-0.0.7/images/icons/
--rw-r--r--   0 akeeley    (504) staff       (20)   297429 2024-05-10 20:19:43.000000 rhythmidia-0.0.7/images/icons/pelhamLogoSquare.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)   106534 2024-05-10 20:19:43.000000 rhythmidia-0.0.7/images/icons/rhythmidiaLogoBannerText.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)   885265 2024-05-10 20:19:43.000000 rhythmidia-0.0.7/images/icons/rhythmidiaLogoSquare.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)     3517 2024-05-17 20:41:21.000000 rhythmidia-0.0.7/pyproject.toml
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.900023 rhythmidia-0.0.7/rhythmidia/
--rw-r--r--   0 akeeley    (504) staff       (20)      372 2024-05-17 20:31:36.000000 rhythmidia-0.0.7/rhythmidia/__init__.py
--rw-r--r--   0 akeeley    (504) staff       (20)       22 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia/_version.py
--rw-r--r--   0 akeeley    (504) staff       (20)        0 2024-05-10 20:19:44.000000 rhythmidia-0.0.7/rhythmidia/parameters.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       61 2023-11-17 22:38:38.000000 rhythmidia-0.0.7/rhythmidia/py.typed
--rw-r--r--   0 akeeley    (504) staff       (20)      295 2024-05-17 20:18:49.000000 rhythmidia-0.0.7/rhythmidia/rhythmidia.py
--rw-r--r--   0 akeeley    (504) staff       (20)   147957 2024-05-17 20:35:38.000000 rhythmidia-0.0.7/rhythmidia/rhythmidia_gui.py
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.906761 rhythmidia-0.0.7/rhythmidia/tests/
--rw-r--r--   0 akeeley    (504) staff       (20)      113 2023-11-17 22:38:38.000000 rhythmidia-0.0.7/rhythmidia/tests/__init__.py
--rw-r--r--   0 akeeley    (504) staff       (20)     6373 2024-05-10 20:19:44.000000 rhythmidia-0.0.7/rhythmidia/tests/test_rhythmidia.py
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:59:28.907391 rhythmidia-0.0.7/rhythmidia.egg-info/
--rw-r--r--   0 akeeley    (504) staff       (20)     9216 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/PKG-INFO
--rw-r--r--   0 akeeley    (504) staff       (20)      679 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/SOURCES.txt
--rw-r--r--   0 akeeley    (504) staff       (20)        1 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/dependency_links.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       57 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/entry_points.txt
--rw-r--r--   0 akeeley    (504) staff       (20)        1 2023-11-17 23:02:20.000000 rhythmidia-0.0.7/rhythmidia.egg-info/not-zip-safe
--rw-r--r--   0 akeeley    (504) staff       (20)      157 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/requires.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       11 2024-05-24 16:59:28.000000 rhythmidia-0.0.7/rhythmidia.egg-info/top_level.txt
--rw-r--r--   0 akeeley    (504) staff       (20)      215 2024-05-24 16:59:28.908326 rhythmidia-0.0.7/setup.cfg
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 17:35:50.555890 rhythmidia-0.0.8/
+-rw-r--r--   0 akeeley    (504) staff       (20)     3552 2023-11-17 22:38:38.000000 rhythmidia-0.0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 akeeley    (504) staff       (20)     1068 2024-05-13 17:38:39.000000 rhythmidia-0.0.8/LICENSE
+-rw-r--r--   0 akeeley    (504) staff       (20)       70 2023-11-17 22:38:38.000000 rhythmidia-0.0.8/MANIFEST.in
+-rw-r--r--   0 akeeley    (504) staff       (20)    11697 2024-05-24 17:35:50.555791 rhythmidia-0.0.8/PKG-INFO
+-rw-r--r--   0 akeeley    (504) staff       (20)    10965 2024-05-24 17:32:46.000000 rhythmidia-0.0.8/README.md
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 17:35:50.545675 rhythmidia-0.0.8/images/
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 17:35:50.552501 rhythmidia-0.0.8/images/icons/
+-rw-r--r--   0 akeeley    (504) staff       (20)   297429 2024-05-10 20:19:43.000000 rhythmidia-0.0.8/images/icons/pelhamLogoSquare.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)   106534 2024-05-10 20:19:43.000000 rhythmidia-0.0.8/images/icons/rhythmidiaLogoBannerText.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)   885265 2024-05-10 20:19:43.000000 rhythmidia-0.0.8/images/icons/rhythmidiaLogoSquare.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)     3517 2024-05-17 20:41:21.000000 rhythmidia-0.0.8/pyproject.toml
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 17:35:50.548347 rhythmidia-0.0.8/rhythmidia/
+-rw-r--r--   0 akeeley    (504) staff       (20)      372 2024-05-17 20:31:36.000000 rhythmidia-0.0.8/rhythmidia/__init__.py
+-rw-r--r--   0 akeeley    (504) staff       (20)       22 2024-05-24 17:35:50.000000 rhythmidia-0.0.8/rhythmidia/_version.py
+-rw-r--r--   0 akeeley    (504) staff       (20)        0 2024-05-10 20:19:44.000000 rhythmidia-0.0.8/rhythmidia/parameters.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       61 2023-11-17 22:38:38.000000 rhythmidia-0.0.8/rhythmidia/py.typed
+-rw-r--r--   0 akeeley    (504) staff       (20)      295 2024-05-17 20:18:49.000000 rhythmidia-0.0.8/rhythmidia/rhythmidia.py
+-rw-r--r--   0 akeeley    (504) staff       (20)   147957 2024-05-17 20:35:38.000000 rhythmidia-0.0.8/rhythmidia/rhythmidia_gui.py
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 17:35:50.554972 rhythmidia-0.0.8/rhythmidia/tests/
+-rw-r--r--   0 akeeley    (504) staff       (20)      113 2023-11-17 22:38:38.000000 rhythmidia-0.0.8/rhythmidia/tests/__init__.py
+-rw-r--r--   0 akeeley    (504) staff       (20)     6373 2024-05-10 20:19:44.000000 rhythmidia-0.0.8/rhythmidia/tests/test_rhythmidia.py
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 17:35:50.555287 rhythmidia-0.0.8/rhythmidia.egg-info/
+-rw-r--r--   0 akeeley    (504) staff       (20)    11697 2024-05-24 17:35:50.000000 rhythmidia-0.0.8/rhythmidia.egg-info/PKG-INFO
+-rw-r--r--   0 akeeley    (504) staff       (20)      679 2024-05-24 17:35:50.000000 rhythmidia-0.0.8/rhythmidia.egg-info/SOURCES.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)        1 2024-05-24 17:35:50.000000 rhythmidia-0.0.8/rhythmidia.egg-info/dependency_links.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       57 2024-05-24 17:35:50.000000 rhythmidia-0.0.8/rhythmidia.egg-info/entry_points.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)        1 2023-11-17 23:02:20.000000 rhythmidia-0.0.8/rhythmidia.egg-info/not-zip-safe
+-rw-r--r--   0 akeeley    (504) staff       (20)      157 2024-05-24 17:35:50.000000 rhythmidia-0.0.8/rhythmidia.egg-info/requires.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       11 2024-05-24 17:35:50.000000 rhythmidia-0.0.8/rhythmidia.egg-info/top_level.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)      215 2024-05-24 17:35:50.556186 rhythmidia-0.0.8/setup.cfg
```

### Comparing `rhythmidia-0.0.7/CODE_OF_CONDUCT.md` & `rhythmidia-0.0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.7/LICENSE` & `rhythmidia-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.7/PKG-INFO` & `rhythmidia-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhythmidia
-Version: 0.0.7
+Version: 0.0.8
 Summary: Race tube image analysis and period elucidation in Python.
 Author-email: Alex Keeley <alex.k@wustl.edu>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -55,86 +55,108 @@
 1. Crop your scanned race tube image as desired, in the image viewer program of choice, leaving a small amount of background on either long edge
 2. No need to make your image greyscale, fix its rotation, or increase contrast- Rhythmidia will take care of all of this internally!
 3. Race tube images can be .png, .tif, .tiff, .jpg, .jpeg, or .svg
 
 ---
 ## Uploading and Analyzing an Image
 1. Upon opening the software, you will be greeted with the “Home” tab, which will look like this:
-![Home Tab (blank)](images/screenshots/HomeTabBlank.png)
+<!--![Home Tab (blank)](images/screenshots/HomeTabBlank.png)-->
 ![Home Tab (blank)](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/HomeTabBlank.png?raw=true)
     NOTE:If you want to add tubes to an existing experiment file, go to File -> Open experiment File (or press ⌘O), although this is not necessary
 2. To upload a new race tube image, click the button labeled “Upload Race Tube Image”<br />
-![Upload Image Button](images/screenshots/UploadImageButton.png)
+<!--![Upload Image Button](images/screenshots/UploadImageButton.png)-->
+![Upload Image Button](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/UploadImageButton.png?raw=true)
     a. Your image will appear in the center of the screen<br />
-    ![Image Analysis](images/screenshots/ImageAnal1.png)
+    <!--![Image Analysis](images/screenshots/ImageAnal1.png)-->
+    ![Image Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal1.png?raw=true)
     b. Uploading an image enables the options to rotate and to lock & analyze your image<br />
-    ![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)
+    <!--![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)-->
+    ![Image Adjustment Buttons](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageChangeButtons.png?raw=true)
 3. Rotate your image so that the growth direction of the tubes is from left to right across your screen<br />
     a. To rotate your image 90 degrees clockwise, click the button labeled “Rotate”<br />
 4. When you are satisfied with your image’s orientation, click the button labeled “Lock & Analyze Image”
 5. Rhythmidia will try to identify horizontal lines corresponding to the horizontal boundaries of the tubes in your image, including the lower and upper bounds below and above the final and first tubes
     a. One line between each two tubes
-![Horizontal Line Identification](images/screenshots/ImageAnal2.png)
+<!--![Horizontal Line Identification](images/screenshots/ImageAnal2.png)-->
+![Horizontal Line Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal2.png?raw=true)
 6. You will be directed to verify these lines:<br />
     a. To remove an incorrect line, simply click on the line<br />
     b. To add a missing line, simply click in an unoccupied position on the image<br />
 7. When you are satisfied with the positions of all tube demarcation lines, click the button labeled “Proceed”
 8. Repeat steps 6-8 for time marks (red) and for bands (orange)<br />
-![Time Mark Identification](images/screenshots/ImageAnal3.png)
-![Banding Identification](images/screenshots/ImageAnal4.png)
-![Time Marks and Banding Identification](images/screenshots/ImageAnal5.png)
+<!--![Time Mark Identification](images/screenshots/ImageAnal3.png)-->
+<!--![Banding Identification](images/screenshots/ImageAnal4.png)-->
+<!--![Time Marks and Banding Identification](images/screenshots/ImageAnal5.png)-->
+![Time Mark Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal3.png?raw=true)
+![Banding Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal4.png?raw=true)
+![Time Marks and Banding Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal5.png?raw=true)
     NOTE: At any time before saving tubes to the file, you may click the button labeled “Cancel image analysis”, which will reset the image analysis process and remove your uploaded image, while leaving open any open experiment file<br />
     NOTE: Be certain to record any differences in marking times in the mark sheet (left) before proceeding further. If tubes were marked at the same time every day, leave as the default setting (0 for all)<br />
     NOTE: The time marks will temporarily disappear while marking conidial peaks.
 9. After you are satisfied with the positions of the bands and click “Proceed”, you will be able to see a preliminary calculation of the period of each tube below<br />
     NOTE: if there is an issue at this stage (i.e. a missed or duplicated identifier) cancel image analysis and reload the image
-![Preliminary Data](images/screenshots/ImageAnal6.png)
+<!--![Preliminary Data](images/screenshots/ImageAnal6.png)-->
+![Preliminary Data](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal6.png?raw=true)
 10. You will now have the option to click the button labeled “Save Tubes to File”<br />
     a.  This will bring up a popup asking for a name for the pack of tubes in the current image before it saves them to file<br />
-    ![Pack Name Prompt](images/screenshots/PackName.png)
+    <!--![Pack Name Prompt](images/screenshots/PackName.png)-->
+    ![Pack Name Prompt](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/PackName.png?raw=true)
     <br />b. If you are working within an existing experiment file, this will simply add this pack to the file and update it<br />
     c. Otherwise, you will be prompted to Save As a new experiment file for these tubes<br />
 
 ## The Experiment Tab
 1. Whether opening an existing experiment file or working from a new pack image, granular experiment data, plots, and statistical analysis data are located on the Experiment tab
-![Experiment Tab](images/screenshots/ExperimentTabBlank.png)
+<!--![Experiment Tab](images/screenshots/ExperimentTabBlank.png)-->
+![Experiment Tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTabBlank.png?raw=true)
 2. Experiment data (Entry, Pack, Tube # in pack, Period calculated 3 ways, and Growth rate) is located in the table in the top left
-![Experiment tab](images/screenshots/ExperimentTab.png)
-![Experiment tab](images/screenshots/ExperimentTab2.png)
+<!--![Experiment tab](images/screenshots/ExperimentTab.png)-->
+<!--![Experiment tab](images/screenshots/ExperimentTab2.png)-->
+![Experiment tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTab.png?raw=true)
+![Experiment tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTab2.png?raw=true)
 3. In the top right is the frame for statistical analysis of any number of tubes:<br />
-![Manual Statistical Analysis](images/screenshots/ManualStatAnal.png)
-![CWT Statistical Analysis](images/screenshots/WaveletStatAnal.png)
+<!--![Manual Statistical Analysis](images/screenshots/ManualStatAnal.png)-->
+<!--[CWT Statistical Analysis](images/screenshots/WaveletStatAnal.png)-->
+![Manual Statistical Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ManualStatAnal.png?raw=true)
+![CWT Statistical Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/WaveletStatAnal.png?raw=true)
     a. Select packs, tubes, and a method of period analysis in the 3 lists<br />
     b. To select multiple packs or tubes, use control-click<br />
     c. Click the button labeled “Analyze” to generate mean period, standard deviation, and standard error<br />
     d. Click the button labeled “Export Data” to export a .csv of the data for each tube selected<br />
     e. Click the button labeled “Export Analysis” to export a .csv of the analysis of the selected tubes<br />
 4. In the bottom half is the plot frame for plotting densitometry and a periodogram of a single tube:<br />
-![Sokolove-Bushell Periodogram](images/screenshots/SokoloveBushellPlot.png)
-![Lomb-Scargle Periodogram](images/screenshots/LombScarglePlot.png)
-![CWT Heatmap](images/screenshots/WaveletPlot.png)
+<!--![Sokolove-Bushell Periodogram](images/screenshots/SokoloveBushellPlot.png)-->
+<!--![Lomb-Scargle Periodogram](images/screenshots/LombScarglePlot.png)-->
+<!--![CWT Heatmap](images/screenshots/WaveletPlot.png)-->
+![Sokolove-Bushell Periodogram](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/SokoloveBushellPlot.png?raw=true)
+![Lomb-Scargle Periodogram](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/LombScarglePlot.png?raw=true)
+![CWT Heatmap](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/WaveletPlot.png?raw=true)
     a. Select pack, tube, and type of periodogram in the 3 lists<br />
     b. Click the button labeled “Plot” to generate a densitometry plot and periodogram of the selected data<br />
     c. Click the button labeled “Save Plot” to save an image of the dual plot in file format of choice<br />
     d. Click the button labeled “Save Densitometry” to save a .csv of the densitometry data<br />
     e. Click the button labeled “Save Periodogrammetry” to save a .csv of the periodogrammetry data<br />
 5. At the bottom left is a button labeled "Display Pack Image"
     a. This button will display a popup window containing the greyscale version of the image corresponding to whichever pack is selected in the bottom left list that was the exact image used for analysis<br />
-![Image Popup](images/screenshots/PackImagePopup.png)
+<!--![Image Popup](images/screenshots/PackImagePopup.png)-->
+![Image Popup](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/PackImagePopup.png?raw=true)
 
 ## Functions Overview
 Open Experiment File      (⌘O)<br />
 Close Experiment File     (⌘C)<br />
 Save File                 (⌘S)<br />
 Save as…                 (↑⌘S)<br />
 Set working directory     (⌘D)<br />
 Open graphics preferences (⌘P)<br />
 
 ---
 ## Changelog
+v0.0.8: Documentation update to display images in PyPI documentation.
+
+V0.0.4: Documentation update to create readthedocs files.
+
 V0.0.1: First public, stable release concurrent with upload to PyPI.
 
 
 ---
 
 ### Copyright
```

### Comparing `rhythmidia-0.0.7/README.md` & `rhythmidia-0.0.8/rhythmidia.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: rhythmidia
+Version: 0.0.8
+Summary: Race tube image analysis and period elucidation in Python.
+Author-email: Alex Keeley <alex.k@wustl.edu>
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: importlib-resources; python_version >= "3.11"
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: scipy
+Requires-Dist: pyautogui
+Requires-Dist: scikit-image
+Requires-Dist: guizero
+Requires-Dist: pytest
+Requires-Dist: PyWavelets
+Provides-Extra: test
+Requires-Dist: pytest>=6.1.2; extra == "test"
+Requires-Dist: pytest-runner; extra == "test"
+
 <!--<img src="images/icons/rhythmidiaLogoBanner.jpg" width=50% margin-left=25%></img>-->
 <img src="https://github.com/Pelham-Lab/rhythmidia/blob/main/images/icons/rhythmidiaLogoBanner.jpg?raw=true" width=50% margin-left=25%></img>
 
 Rhythmidia
 ---
 ### Race tube image analysis for circadian period elucidation in Python.
 ---
@@ -31,86 +55,108 @@
 1. Crop your scanned race tube image as desired, in the image viewer program of choice, leaving a small amount of background on either long edge
 2. No need to make your image greyscale, fix its rotation, or increase contrast- Rhythmidia will take care of all of this internally!
 3. Race tube images can be .png, .tif, .tiff, .jpg, .jpeg, or .svg
 
 ---
 ## Uploading and Analyzing an Image
 1. Upon opening the software, you will be greeted with the “Home” tab, which will look like this:
-![Home Tab (blank)](images/screenshots/HomeTabBlank.png)
+<!--![Home Tab (blank)](images/screenshots/HomeTabBlank.png)-->
 ![Home Tab (blank)](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/HomeTabBlank.png?raw=true)
     NOTE:If you want to add tubes to an existing experiment file, go to File -> Open experiment File (or press ⌘O), although this is not necessary
 2. To upload a new race tube image, click the button labeled “Upload Race Tube Image”<br />
-![Upload Image Button](images/screenshots/UploadImageButton.png)
+<!--![Upload Image Button](images/screenshots/UploadImageButton.png)-->
+![Upload Image Button](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/UploadImageButton.png?raw=true)
     a. Your image will appear in the center of the screen<br />
-    ![Image Analysis](images/screenshots/ImageAnal1.png)
+    <!--![Image Analysis](images/screenshots/ImageAnal1.png)-->
+    ![Image Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal1.png?raw=true)
     b. Uploading an image enables the options to rotate and to lock & analyze your image<br />
-    ![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)
+    <!--![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)-->
+    ![Image Adjustment Buttons](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageChangeButtons.png?raw=true)
 3. Rotate your image so that the growth direction of the tubes is from left to right across your screen<br />
     a. To rotate your image 90 degrees clockwise, click the button labeled “Rotate”<br />
 4. When you are satisfied with your image’s orientation, click the button labeled “Lock & Analyze Image”
 5. Rhythmidia will try to identify horizontal lines corresponding to the horizontal boundaries of the tubes in your image, including the lower and upper bounds below and above the final and first tubes
     a. One line between each two tubes
-![Horizontal Line Identification](images/screenshots/ImageAnal2.png)
+<!--![Horizontal Line Identification](images/screenshots/ImageAnal2.png)-->
+![Horizontal Line Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal2.png?raw=true)
 6. You will be directed to verify these lines:<br />
     a. To remove an incorrect line, simply click on the line<br />
     b. To add a missing line, simply click in an unoccupied position on the image<br />
 7. When you are satisfied with the positions of all tube demarcation lines, click the button labeled “Proceed”
 8. Repeat steps 6-8 for time marks (red) and for bands (orange)<br />
-![Time Mark Identification](images/screenshots/ImageAnal3.png)
-![Banding Identification](images/screenshots/ImageAnal4.png)
-![Time Marks and Banding Identification](images/screenshots/ImageAnal5.png)
+<!--![Time Mark Identification](images/screenshots/ImageAnal3.png)-->
+<!--![Banding Identification](images/screenshots/ImageAnal4.png)-->
+<!--![Time Marks and Banding Identification](images/screenshots/ImageAnal5.png)-->
+![Time Mark Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal3.png?raw=true)
+![Banding Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal4.png?raw=true)
+![Time Marks and Banding Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal5.png?raw=true)
     NOTE: At any time before saving tubes to the file, you may click the button labeled “Cancel image analysis”, which will reset the image analysis process and remove your uploaded image, while leaving open any open experiment file<br />
     NOTE: Be certain to record any differences in marking times in the mark sheet (left) before proceeding further. If tubes were marked at the same time every day, leave as the default setting (0 for all)<br />
     NOTE: The time marks will temporarily disappear while marking conidial peaks.
 9. After you are satisfied with the positions of the bands and click “Proceed”, you will be able to see a preliminary calculation of the period of each tube below<br />
     NOTE: if there is an issue at this stage (i.e. a missed or duplicated identifier) cancel image analysis and reload the image
-![Preliminary Data](images/screenshots/ImageAnal6.png)
+<!--![Preliminary Data](images/screenshots/ImageAnal6.png)-->
+![Preliminary Data](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal6.png?raw=true)
 10. You will now have the option to click the button labeled “Save Tubes to File”<br />
     a.  This will bring up a popup asking for a name for the pack of tubes in the current image before it saves them to file<br />
-    ![Pack Name Prompt](images/screenshots/PackName.png)
+    <!--![Pack Name Prompt](images/screenshots/PackName.png)-->
+    ![Pack Name Prompt](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/PackName.png?raw=true)
     <br />b. If you are working within an existing experiment file, this will simply add this pack to the file and update it<br />
     c. Otherwise, you will be prompted to Save As a new experiment file for these tubes<br />
 
 ## The Experiment Tab
 1. Whether opening an existing experiment file or working from a new pack image, granular experiment data, plots, and statistical analysis data are located on the Experiment tab
-![Experiment Tab](images/screenshots/ExperimentTabBlank.png)
+<!--![Experiment Tab](images/screenshots/ExperimentTabBlank.png)-->
+![Experiment Tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTabBlank.png?raw=true)
 2. Experiment data (Entry, Pack, Tube # in pack, Period calculated 3 ways, and Growth rate) is located in the table in the top left
-![Experiment tab](images/screenshots/ExperimentTab.png)
-![Experiment tab](images/screenshots/ExperimentTab2.png)
+<!--![Experiment tab](images/screenshots/ExperimentTab.png)-->
+<!--![Experiment tab](images/screenshots/ExperimentTab2.png)-->
+![Experiment tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTab.png?raw=true)
+![Experiment tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTab2.png?raw=true)
 3. In the top right is the frame for statistical analysis of any number of tubes:<br />
-![Manual Statistical Analysis](images/screenshots/ManualStatAnal.png)
-![CWT Statistical Analysis](images/screenshots/WaveletStatAnal.png)
+<!--![Manual Statistical Analysis](images/screenshots/ManualStatAnal.png)-->
+<!--[CWT Statistical Analysis](images/screenshots/WaveletStatAnal.png)-->
+![Manual Statistical Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ManualStatAnal.png?raw=true)
+![CWT Statistical Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/WaveletStatAnal.png?raw=true)
     a. Select packs, tubes, and a method of period analysis in the 3 lists<br />
     b. To select multiple packs or tubes, use control-click<br />
     c. Click the button labeled “Analyze” to generate mean period, standard deviation, and standard error<br />
     d. Click the button labeled “Export Data” to export a .csv of the data for each tube selected<br />
     e. Click the button labeled “Export Analysis” to export a .csv of the analysis of the selected tubes<br />
 4. In the bottom half is the plot frame for plotting densitometry and a periodogram of a single tube:<br />
-![Sokolove-Bushell Periodogram](images/screenshots/SokoloveBushellPlot.png)
-![Lomb-Scargle Periodogram](images/screenshots/LombScarglePlot.png)
-![CWT Heatmap](images/screenshots/WaveletPlot.png)
+<!--![Sokolove-Bushell Periodogram](images/screenshots/SokoloveBushellPlot.png)-->
+<!--![Lomb-Scargle Periodogram](images/screenshots/LombScarglePlot.png)-->
+<!--![CWT Heatmap](images/screenshots/WaveletPlot.png)-->
+![Sokolove-Bushell Periodogram](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/SokoloveBushellPlot.png?raw=true)
+![Lomb-Scargle Periodogram](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/LombScarglePlot.png?raw=true)
+![CWT Heatmap](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/WaveletPlot.png?raw=true)
     a. Select pack, tube, and type of periodogram in the 3 lists<br />
     b. Click the button labeled “Plot” to generate a densitometry plot and periodogram of the selected data<br />
     c. Click the button labeled “Save Plot” to save an image of the dual plot in file format of choice<br />
     d. Click the button labeled “Save Densitometry” to save a .csv of the densitometry data<br />
     e. Click the button labeled “Save Periodogrammetry” to save a .csv of the periodogrammetry data<br />
 5. At the bottom left is a button labeled "Display Pack Image"
     a. This button will display a popup window containing the greyscale version of the image corresponding to whichever pack is selected in the bottom left list that was the exact image used for analysis<br />
-![Image Popup](images/screenshots/PackImagePopup.png)
+<!--![Image Popup](images/screenshots/PackImagePopup.png)-->
+![Image Popup](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/PackImagePopup.png?raw=true)
 
 ## Functions Overview
 Open Experiment File      (⌘O)<br />
 Close Experiment File     (⌘C)<br />
 Save File                 (⌘S)<br />
 Save as…                 (↑⌘S)<br />
 Set working directory     (⌘D)<br />
 Open graphics preferences (⌘P)<br />
 
 ---
 ## Changelog
+v0.0.8: Documentation update to display images in PyPI documentation.
+
+V0.0.4: Documentation update to create readthedocs files.
+
 V0.0.1: First public, stable release concurrent with upload to PyPI.
 
 
 ---
 
 ### Copyright
```

### Comparing `rhythmidia-0.0.7/images/icons/pelhamLogoSquare.jpg` & `rhythmidia-0.0.8/images/icons/pelhamLogoSquare.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.7/images/icons/rhythmidiaLogoBannerText.jpg` & `rhythmidia-0.0.8/images/icons/rhythmidiaLogoBannerText.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.7/images/icons/rhythmidiaLogoSquare.jpg` & `rhythmidia-0.0.8/images/icons/rhythmidiaLogoSquare.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.7/pyproject.toml` & `rhythmidia-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.7/rhythmidia/rhythmidia_gui.py` & `rhythmidia-0.0.8/rhythmidia/rhythmidia_gui.py`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.7/rhythmidia/tests/test_rhythmidia.py` & `rhythmidia-0.0.8/rhythmidia/tests/test_rhythmidia.py`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.7/rhythmidia.egg-info/PKG-INFO` & `rhythmidia-0.0.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: rhythmidia
-Version: 0.0.7
-Summary: Race tube image analysis and period elucidation in Python.
-Author-email: Alex Keeley <alex.k@wustl.edu>
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: importlib-resources; python_version >= "3.11"
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-Requires-Dist: pyautogui
-Requires-Dist: scikit-image
-Requires-Dist: guizero
-Requires-Dist: pytest
-Requires-Dist: PyWavelets
-Provides-Extra: test
-Requires-Dist: pytest>=6.1.2; extra == "test"
-Requires-Dist: pytest-runner; extra == "test"
-
 <!--<img src="images/icons/rhythmidiaLogoBanner.jpg" width=50% margin-left=25%></img>-->
 <img src="https://github.com/Pelham-Lab/rhythmidia/blob/main/images/icons/rhythmidiaLogoBanner.jpg?raw=true" width=50% margin-left=25%></img>
 
 Rhythmidia
 ---
 ### Race tube image analysis for circadian period elucidation in Python.
 ---
@@ -55,86 +31,108 @@
 1. Crop your scanned race tube image as desired, in the image viewer program of choice, leaving a small amount of background on either long edge
 2. No need to make your image greyscale, fix its rotation, or increase contrast- Rhythmidia will take care of all of this internally!
 3. Race tube images can be .png, .tif, .tiff, .jpg, .jpeg, or .svg
 
 ---
 ## Uploading and Analyzing an Image
 1. Upon opening the software, you will be greeted with the “Home” tab, which will look like this:
-![Home Tab (blank)](images/screenshots/HomeTabBlank.png)
+<!--![Home Tab (blank)](images/screenshots/HomeTabBlank.png)-->
 ![Home Tab (blank)](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/HomeTabBlank.png?raw=true)
     NOTE:If you want to add tubes to an existing experiment file, go to File -> Open experiment File (or press ⌘O), although this is not necessary
 2. To upload a new race tube image, click the button labeled “Upload Race Tube Image”<br />
-![Upload Image Button](images/screenshots/UploadImageButton.png)
+<!--![Upload Image Button](images/screenshots/UploadImageButton.png)-->
+![Upload Image Button](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/UploadImageButton.png?raw=true)
     a. Your image will appear in the center of the screen<br />
-    ![Image Analysis](images/screenshots/ImageAnal1.png)
+    <!--![Image Analysis](images/screenshots/ImageAnal1.png)-->
+    ![Image Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal1.png?raw=true)
     b. Uploading an image enables the options to rotate and to lock & analyze your image<br />
-    ![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)
+    <!--![Image Adjustment Buttons](images/screenshots/ImageChangeButtons.png)-->
+    ![Image Adjustment Buttons](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageChangeButtons.png?raw=true)
 3. Rotate your image so that the growth direction of the tubes is from left to right across your screen<br />
     a. To rotate your image 90 degrees clockwise, click the button labeled “Rotate”<br />
 4. When you are satisfied with your image’s orientation, click the button labeled “Lock & Analyze Image”
 5. Rhythmidia will try to identify horizontal lines corresponding to the horizontal boundaries of the tubes in your image, including the lower and upper bounds below and above the final and first tubes
     a. One line between each two tubes
-![Horizontal Line Identification](images/screenshots/ImageAnal2.png)
+<!--![Horizontal Line Identification](images/screenshots/ImageAnal2.png)-->
+![Horizontal Line Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal2.png?raw=true)
 6. You will be directed to verify these lines:<br />
     a. To remove an incorrect line, simply click on the line<br />
     b. To add a missing line, simply click in an unoccupied position on the image<br />
 7. When you are satisfied with the positions of all tube demarcation lines, click the button labeled “Proceed”
 8. Repeat steps 6-8 for time marks (red) and for bands (orange)<br />
-![Time Mark Identification](images/screenshots/ImageAnal3.png)
-![Banding Identification](images/screenshots/ImageAnal4.png)
-![Time Marks and Banding Identification](images/screenshots/ImageAnal5.png)
+<!--![Time Mark Identification](images/screenshots/ImageAnal3.png)-->
+<!--![Banding Identification](images/screenshots/ImageAnal4.png)-->
+<!--![Time Marks and Banding Identification](images/screenshots/ImageAnal5.png)-->
+![Time Mark Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal3.png?raw=true)
+![Banding Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal4.png?raw=true)
+![Time Marks and Banding Identification](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal5.png?raw=true)
     NOTE: At any time before saving tubes to the file, you may click the button labeled “Cancel image analysis”, which will reset the image analysis process and remove your uploaded image, while leaving open any open experiment file<br />
     NOTE: Be certain to record any differences in marking times in the mark sheet (left) before proceeding further. If tubes were marked at the same time every day, leave as the default setting (0 for all)<br />
     NOTE: The time marks will temporarily disappear while marking conidial peaks.
 9. After you are satisfied with the positions of the bands and click “Proceed”, you will be able to see a preliminary calculation of the period of each tube below<br />
     NOTE: if there is an issue at this stage (i.e. a missed or duplicated identifier) cancel image analysis and reload the image
-![Preliminary Data](images/screenshots/ImageAnal6.png)
+<!--![Preliminary Data](images/screenshots/ImageAnal6.png)-->
+![Preliminary Data](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ImageAnal6.png?raw=true)
 10. You will now have the option to click the button labeled “Save Tubes to File”<br />
     a.  This will bring up a popup asking for a name for the pack of tubes in the current image before it saves them to file<br />
-    ![Pack Name Prompt](images/screenshots/PackName.png)
+    <!--![Pack Name Prompt](images/screenshots/PackName.png)-->
+    ![Pack Name Prompt](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/PackName.png?raw=true)
     <br />b. If you are working within an existing experiment file, this will simply add this pack to the file and update it<br />
     c. Otherwise, you will be prompted to Save As a new experiment file for these tubes<br />
 
 ## The Experiment Tab
 1. Whether opening an existing experiment file or working from a new pack image, granular experiment data, plots, and statistical analysis data are located on the Experiment tab
-![Experiment Tab](images/screenshots/ExperimentTabBlank.png)
+<!--![Experiment Tab](images/screenshots/ExperimentTabBlank.png)-->
+![Experiment Tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTabBlank.png?raw=true)
 2. Experiment data (Entry, Pack, Tube # in pack, Period calculated 3 ways, and Growth rate) is located in the table in the top left
-![Experiment tab](images/screenshots/ExperimentTab.png)
-![Experiment tab](images/screenshots/ExperimentTab2.png)
+<!--![Experiment tab](images/screenshots/ExperimentTab.png)-->
+<!--![Experiment tab](images/screenshots/ExperimentTab2.png)-->
+![Experiment tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTab.png?raw=true)
+![Experiment tab](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ExperimentTab2.png?raw=true)
 3. In the top right is the frame for statistical analysis of any number of tubes:<br />
-![Manual Statistical Analysis](images/screenshots/ManualStatAnal.png)
-![CWT Statistical Analysis](images/screenshots/WaveletStatAnal.png)
+<!--![Manual Statistical Analysis](images/screenshots/ManualStatAnal.png)-->
+<!--[CWT Statistical Analysis](images/screenshots/WaveletStatAnal.png)-->
+![Manual Statistical Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/ManualStatAnal.png?raw=true)
+![CWT Statistical Analysis](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/WaveletStatAnal.png?raw=true)
     a. Select packs, tubes, and a method of period analysis in the 3 lists<br />
     b. To select multiple packs or tubes, use control-click<br />
     c. Click the button labeled “Analyze” to generate mean period, standard deviation, and standard error<br />
     d. Click the button labeled “Export Data” to export a .csv of the data for each tube selected<br />
     e. Click the button labeled “Export Analysis” to export a .csv of the analysis of the selected tubes<br />
 4. In the bottom half is the plot frame for plotting densitometry and a periodogram of a single tube:<br />
-![Sokolove-Bushell Periodogram](images/screenshots/SokoloveBushellPlot.png)
-![Lomb-Scargle Periodogram](images/screenshots/LombScarglePlot.png)
-![CWT Heatmap](images/screenshots/WaveletPlot.png)
+<!--![Sokolove-Bushell Periodogram](images/screenshots/SokoloveBushellPlot.png)-->
+<!--![Lomb-Scargle Periodogram](images/screenshots/LombScarglePlot.png)-->
+<!--![CWT Heatmap](images/screenshots/WaveletPlot.png)-->
+![Sokolove-Bushell Periodogram](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/SokoloveBushellPlot.png?raw=true)
+![Lomb-Scargle Periodogram](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/LombScarglePlot.png?raw=true)
+![CWT Heatmap](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/WaveletPlot.png?raw=true)
     a. Select pack, tube, and type of periodogram in the 3 lists<br />
     b. Click the button labeled “Plot” to generate a densitometry plot and periodogram of the selected data<br />
     c. Click the button labeled “Save Plot” to save an image of the dual plot in file format of choice<br />
     d. Click the button labeled “Save Densitometry” to save a .csv of the densitometry data<br />
     e. Click the button labeled “Save Periodogrammetry” to save a .csv of the periodogrammetry data<br />
 5. At the bottom left is a button labeled "Display Pack Image"
     a. This button will display a popup window containing the greyscale version of the image corresponding to whichever pack is selected in the bottom left list that was the exact image used for analysis<br />
-![Image Popup](images/screenshots/PackImagePopup.png)
+<!--![Image Popup](images/screenshots/PackImagePopup.png)-->
+![Image Popup](https://github.com/Pelham-Lab/rhythmidia/blob/main/images/screenshots/PackImagePopup.png?raw=true)
 
 ## Functions Overview
 Open Experiment File      (⌘O)<br />
 Close Experiment File     (⌘C)<br />
 Save File                 (⌘S)<br />
 Save as…                 (↑⌘S)<br />
 Set working directory     (⌘D)<br />
 Open graphics preferences (⌘P)<br />
 
 ---
 ## Changelog
+v0.0.8: Documentation update to display images in PyPI documentation.
+
+V0.0.4: Documentation update to create readthedocs files.
+
 V0.0.1: First public, stable release concurrent with upload to PyPI.
 
 
 ---
 
 ### Copyright
```

### Comparing `rhythmidia-0.0.7/rhythmidia.egg-info/SOURCES.txt` & `rhythmidia-0.0.8/rhythmidia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

