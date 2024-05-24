# Comparing `tmp/rhythmidia-0.0.4.tar.gz` & `tmp/rhythmidia-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhythmidia-0.0.4.tar", last modified: Fri May 17 20:52:49 2024, max compression
+gzip compressed data, was "rhythmidia-0.0.5.tar", last modified: Fri May 24 16:16:29 2024, max compression
```

## Comparing `rhythmidia-0.0.4.tar` & `rhythmidia-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-17 20:52:49.698484 rhythmidia-0.0.4/
--rw-r--r--   0 akeeley    (504) staff       (20)     3552 2023-11-17 22:38:38.000000 rhythmidia-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 akeeley    (504) staff       (20)     1068 2024-05-13 17:38:39.000000 rhythmidia-0.0.4/LICENSE
--rw-r--r--   0 akeeley    (504) staff       (20)       70 2023-11-17 22:38:38.000000 rhythmidia-0.0.4/MANIFEST.in
--rw-r--r--   0 akeeley    (504) staff       (20)     8950 2024-05-17 20:52:49.698397 rhythmidia-0.0.4/PKG-INFO
--rw-r--r--   0 akeeley    (504) staff       (20)     8218 2024-05-14 18:05:26.000000 rhythmidia-0.0.4/README.md
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-17 20:52:49.686076 rhythmidia-0.0.4/images/
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-17 20:52:49.693843 rhythmidia-0.0.4/images/icons/
--rw-r--r--   0 akeeley    (504) staff       (20)   297429 2024-05-10 20:19:43.000000 rhythmidia-0.0.4/images/icons/pelhamLogoSquare.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)   106534 2024-05-10 20:19:43.000000 rhythmidia-0.0.4/images/icons/rhythmidiaLogoBannerText.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)   885265 2024-05-10 20:19:43.000000 rhythmidia-0.0.4/images/icons/rhythmidiaLogoSquare.jpg
--rw-r--r--   0 akeeley    (504) staff       (20)     3517 2024-05-17 20:41:21.000000 rhythmidia-0.0.4/pyproject.toml
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-17 20:52:49.688832 rhythmidia-0.0.4/rhythmidia/
--rw-r--r--   0 akeeley    (504) staff       (20)      372 2024-05-17 20:31:36.000000 rhythmidia-0.0.4/rhythmidia/__init__.py
--rw-r--r--   0 akeeley    (504) staff       (20)       22 2024-05-17 20:52:49.000000 rhythmidia-0.0.4/rhythmidia/_version.py
--rw-r--r--   0 akeeley    (504) staff       (20)        0 2024-05-10 20:19:44.000000 rhythmidia-0.0.4/rhythmidia/parameters.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       61 2023-11-17 22:38:38.000000 rhythmidia-0.0.4/rhythmidia/py.typed
--rw-r--r--   0 akeeley    (504) staff       (20)      295 2024-05-17 20:18:49.000000 rhythmidia-0.0.4/rhythmidia/rhythmidia.py
--rw-r--r--   0 akeeley    (504) staff       (20)   147957 2024-05-17 20:35:38.000000 rhythmidia-0.0.4/rhythmidia/rhythmidia_gui.py
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-17 20:52:49.697492 rhythmidia-0.0.4/rhythmidia/tests/
--rw-r--r--   0 akeeley    (504) staff       (20)      113 2023-11-17 22:38:38.000000 rhythmidia-0.0.4/rhythmidia/tests/__init__.py
--rw-r--r--   0 akeeley    (504) staff       (20)     6373 2024-05-10 20:19:44.000000 rhythmidia-0.0.4/rhythmidia/tests/test_rhythmidia.py
-drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-17 20:52:49.697850 rhythmidia-0.0.4/rhythmidia.egg-info/
--rw-r--r--   0 akeeley    (504) staff       (20)     8950 2024-05-17 20:52:49.000000 rhythmidia-0.0.4/rhythmidia.egg-info/PKG-INFO
--rw-r--r--   0 akeeley    (504) staff       (20)      679 2024-05-17 20:52:49.000000 rhythmidia-0.0.4/rhythmidia.egg-info/SOURCES.txt
--rw-r--r--   0 akeeley    (504) staff       (20)        1 2024-05-17 20:52:49.000000 rhythmidia-0.0.4/rhythmidia.egg-info/dependency_links.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       57 2024-05-17 20:52:49.000000 rhythmidia-0.0.4/rhythmidia.egg-info/entry_points.txt
--rw-r--r--   0 akeeley    (504) staff       (20)        1 2023-11-17 23:02:20.000000 rhythmidia-0.0.4/rhythmidia.egg-info/not-zip-safe
--rw-r--r--   0 akeeley    (504) staff       (20)      157 2024-05-17 20:52:49.000000 rhythmidia-0.0.4/rhythmidia.egg-info/requires.txt
--rw-r--r--   0 akeeley    (504) staff       (20)       11 2024-05-17 20:52:49.000000 rhythmidia-0.0.4/rhythmidia.egg-info/top_level.txt
--rw-r--r--   0 akeeley    (504) staff       (20)      215 2024-05-17 20:52:49.698791 rhythmidia-0.0.4/setup.cfg
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.160488 rhythmidia-0.0.5/
+-rw-r--r--   0 akeeley    (504) staff       (20)     3552 2023-11-17 22:38:38.000000 rhythmidia-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 akeeley    (504) staff       (20)     1068 2024-05-13 17:38:39.000000 rhythmidia-0.0.5/LICENSE
+-rw-r--r--   0 akeeley    (504) staff       (20)       70 2023-11-17 22:38:38.000000 rhythmidia-0.0.5/MANIFEST.in
+-rw-r--r--   0 akeeley    (504) staff       (20)     9099 2024-05-24 16:16:29.160382 rhythmidia-0.0.5/PKG-INFO
+-rw-r--r--   0 akeeley    (504) staff       (20)     8367 2024-05-24 16:10:59.000000 rhythmidia-0.0.5/README.md
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.149870 rhythmidia-0.0.5/images/
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.157131 rhythmidia-0.0.5/images/icons/
+-rw-r--r--   0 akeeley    (504) staff       (20)   297429 2024-05-10 20:19:43.000000 rhythmidia-0.0.5/images/icons/pelhamLogoSquare.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)   106534 2024-05-10 20:19:43.000000 rhythmidia-0.0.5/images/icons/rhythmidiaLogoBannerText.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)   885265 2024-05-10 20:19:43.000000 rhythmidia-0.0.5/images/icons/rhythmidiaLogoSquare.jpg
+-rw-r--r--   0 akeeley    (504) staff       (20)     3517 2024-05-17 20:41:21.000000 rhythmidia-0.0.5/pyproject.toml
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.152655 rhythmidia-0.0.5/rhythmidia/
+-rw-r--r--   0 akeeley    (504) staff       (20)      372 2024-05-17 20:31:36.000000 rhythmidia-0.0.5/rhythmidia/__init__.py
+-rw-r--r--   0 akeeley    (504) staff       (20)       22 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia/_version.py
+-rw-r--r--   0 akeeley    (504) staff       (20)        0 2024-05-10 20:19:44.000000 rhythmidia-0.0.5/rhythmidia/parameters.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       61 2023-11-17 22:38:38.000000 rhythmidia-0.0.5/rhythmidia/py.typed
+-rw-r--r--   0 akeeley    (504) staff       (20)      295 2024-05-17 20:18:49.000000 rhythmidia-0.0.5/rhythmidia/rhythmidia.py
+-rw-r--r--   0 akeeley    (504) staff       (20)   147957 2024-05-17 20:35:38.000000 rhythmidia-0.0.5/rhythmidia/rhythmidia_gui.py
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.159528 rhythmidia-0.0.5/rhythmidia/tests/
+-rw-r--r--   0 akeeley    (504) staff       (20)      113 2023-11-17 22:38:38.000000 rhythmidia-0.0.5/rhythmidia/tests/__init__.py
+-rw-r--r--   0 akeeley    (504) staff       (20)     6373 2024-05-10 20:19:44.000000 rhythmidia-0.0.5/rhythmidia/tests/test_rhythmidia.py
+drwxr-xr-x   0 akeeley    (504) staff       (20)        0 2024-05-24 16:16:29.159885 rhythmidia-0.0.5/rhythmidia.egg-info/
+-rw-r--r--   0 akeeley    (504) staff       (20)     9099 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/PKG-INFO
+-rw-r--r--   0 akeeley    (504) staff       (20)      679 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/SOURCES.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)        1 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/dependency_links.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       57 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/entry_points.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)        1 2023-11-17 23:02:20.000000 rhythmidia-0.0.5/rhythmidia.egg-info/not-zip-safe
+-rw-r--r--   0 akeeley    (504) staff       (20)      157 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/requires.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)       11 2024-05-24 16:16:29.000000 rhythmidia-0.0.5/rhythmidia.egg-info/top_level.txt
+-rw-r--r--   0 akeeley    (504) staff       (20)      215 2024-05-24 16:16:29.160776 rhythmidia-0.0.5/setup.cfg
```

### Comparing `rhythmidia-0.0.4/CODE_OF_CONDUCT.md` & `rhythmidia-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.4/LICENSE` & `rhythmidia-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.4/PKG-INFO` & `rhythmidia-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhythmidia
-Version: 0.0.4
+Version: 0.0.5
 Summary: Race tube image analysis and period elucidation in Python.
 Author-email: Alex Keeley <alex.k@wustl.edu>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -18,15 +18,16 @@
 Requires-Dist: guizero
 Requires-Dist: pytest
 Requires-Dist: PyWavelets
 Provides-Extra: test
 Requires-Dist: pytest>=6.1.2; extra == "test"
 Requires-Dist: pytest-runner; extra == "test"
 
-<img src="images/icons/rhythmidiaLogoBanner.jpg" width=50% margin-left=25%></img>
+<!--<img src="images/icons/rhythmidiaLogoBanner.jpg" width=50% margin-left=25%></img>-->
+<img src="https://github.com/Pelham-Lab/rhythmidia/blob/main/images/icons/rhythmidiaLogoBanner.jpg?raw=true" width=50% margin-left=25%></img>
 
 Rhythmidia
 ---
 ### Race tube image analysis for circadian period elucidation in Python.
 ---
 ## Installation and Program Launch
 1. Rhythmidia must be installed in a Python environment running Python 3.11 or higher using pip. Rhythmidia runs on Unix-like operating systems including macOS and Linux. In order to install Rhythmidia, simply run the command:
```

### Comparing `rhythmidia-0.0.4/README.md` & `rhythmidia-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-<img src="images/icons/rhythmidiaLogoBanner.jpg" width=50% margin-left=25%></img>
+<!--<img src="images/icons/rhythmidiaLogoBanner.jpg" width=50% margin-left=25%></img>-->
+<img src="https://github.com/Pelham-Lab/rhythmidia/blob/main/images/icons/rhythmidiaLogoBanner.jpg?raw=true" width=50% margin-left=25%></img>
 
 Rhythmidia
 ---
 ### Race tube image analysis for circadian period elucidation in Python.
 ---
 ## Installation and Program Launch
 1. Rhythmidia must be installed in a Python environment running Python 3.11 or higher using pip. Rhythmidia runs on Unix-like operating systems including macOS and Linux. In order to install Rhythmidia, simply run the command:
```

### Comparing `rhythmidia-0.0.4/images/icons/pelhamLogoSquare.jpg` & `rhythmidia-0.0.5/images/icons/pelhamLogoSquare.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.4/images/icons/rhythmidiaLogoBannerText.jpg` & `rhythmidia-0.0.5/images/icons/rhythmidiaLogoBannerText.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.4/images/icons/rhythmidiaLogoSquare.jpg` & `rhythmidia-0.0.5/images/icons/rhythmidiaLogoSquare.jpg`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.4/pyproject.toml` & `rhythmidia-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.4/rhythmidia/rhythmidia_gui.py` & `rhythmidia-0.0.5/rhythmidia/rhythmidia_gui.py`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.4/rhythmidia/tests/test_rhythmidia.py` & `rhythmidia-0.0.5/rhythmidia/tests/test_rhythmidia.py`

 * *Files identical despite different names*

### Comparing `rhythmidia-0.0.4/rhythmidia.egg-info/PKG-INFO` & `rhythmidia-0.0.5/rhythmidia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhythmidia
-Version: 0.0.4
+Version: 0.0.5
 Summary: Race tube image analysis and period elucidation in Python.
 Author-email: Alex Keeley <alex.k@wustl.edu>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -18,15 +18,16 @@
 Requires-Dist: guizero
 Requires-Dist: pytest
 Requires-Dist: PyWavelets
 Provides-Extra: test
 Requires-Dist: pytest>=6.1.2; extra == "test"
 Requires-Dist: pytest-runner; extra == "test"
 
-<img src="images/icons/rhythmidiaLogoBanner.jpg" width=50% margin-left=25%></img>
+<!--<img src="images/icons/rhythmidiaLogoBanner.jpg" width=50% margin-left=25%></img>-->
+<img src="https://github.com/Pelham-Lab/rhythmidia/blob/main/images/icons/rhythmidiaLogoBanner.jpg?raw=true" width=50% margin-left=25%></img>
 
 Rhythmidia
 ---
 ### Race tube image analysis for circadian period elucidation in Python.
 ---
 ## Installation and Program Launch
 1. Rhythmidia must be installed in a Python environment running Python 3.11 or higher using pip. Rhythmidia runs on Unix-like operating systems including macOS and Linux. In order to install Rhythmidia, simply run the command:
```

### Comparing `rhythmidia-0.0.4/rhythmidia.egg-info/SOURCES.txt` & `rhythmidia-0.0.5/rhythmidia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

