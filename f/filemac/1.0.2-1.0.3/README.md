# Comparing `tmp/filemac-1.0.2.tar.gz` & `tmp/filemac-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filemac-1.0.2.tar", last modified: Wed Apr 24 09:28:44 2024, max compression
+gzip compressed data, was "filemac-1.0.3.tar", last modified: Fri May 24 08:57:00 2024, max compression
```

## Comparing `filemac-1.0.2.tar` & `filemac-1.0.3.tar`

### file list

```diff
@@ -1,47 +1,58 @@
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.210000 filemac-1.0.2/
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.200000 filemac-1.0.2/.github/
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.200000 filemac-1.0.2/.github/workflows/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1070 2024-04-24 09:25:49.000000 filemac-1.0.2/.github/workflows/python-publish.yml
--rwxr-xr-x   0 skye      (1000) skye      (1000)    35149 2024-03-24 06:23:20.000000 filemac-1.0.2/LICENSE
--rwxr-xr-x   0 skye      (1000) skye      (1000)       80 2024-03-24 07:29:02.000000 filemac-1.0.2/MANIFEST.ini
--rwxr-xr-x   0 skye      (1000) skye      (1000)     4748 2024-04-24 09:28:44.210000 filemac-1.0.2/PKG-INFO
--rwxr-xr-x   0 skye      (1000) skye      (1000)     3861 2024-04-24 09:25:49.000000 filemac-1.0.2/README.md
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.200000 filemac-1.0.2/__pycache__/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2386 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/Analyzer.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     3992 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/AudioExtractor.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     6728 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/OCRTextExtractor.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2521 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/Simple_v_Analyzer.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)    57828 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/converter.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      723 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/formarts.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      725 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/formats.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      957 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/show_progress.cpython-311.pyc
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.210000 filemac-1.0.2/filemac/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1957 2024-04-09 17:35:21.000000 filemac-1.0.2/filemac/AudioExtractor.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     3978 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/OCRTextExtractor.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1723 2024-04-09 17:40:51.000000 filemac-1.0.2/filemac/Simple_v_Analyzer.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)       23 2024-03-24 07:50:06.000000 filemac-1.0.2/filemac/__init__.py
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.210000 filemac-1.0.2/filemac/__pycache__/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     4000 2024-03-24 06:16:58.000000 filemac-1.0.2/filemac/__pycache__/AudioExtractor.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     6471 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/__pycache__/OCRTextExtractor.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2526 2024-03-24 06:16:56.000000 filemac-1.0.2/filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1118 2024-04-18 10:35:04.000000 filemac-1.0.2/filemac/__pycache__/colors.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)    57833 2024-03-24 06:16:56.000000 filemac-1.0.2/filemac/__pycache__/converter.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      730 2024-03-24 06:16:58.000000 filemac-1.0.2/filemac/__pycache__/formats.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      939 2024-04-18 10:35:04.000000 filemac-1.0.2/filemac/colors.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)    42300 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/converter.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)      307 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/dd.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     8163 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/fmac.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     5580 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/formats.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)      254 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/handle_warnings.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2589 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/image_op.py
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.210000 filemac-1.0.2/filemac.egg-info/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     4748 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/PKG-INFO
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1159 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/SOURCES.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)        1 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/dependency_links.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)       41 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/entry_points.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)        1 2024-04-13 09:48:20.000000 filemac-1.0.2/filemac.egg-info/not-zip-safe
--rwxr-xr-x   0 skye      (1000) skye      (1000)      174 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/requires.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)       14 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/top_level.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)       38 2024-04-24 09:28:44.210000 filemac-1.0.2/setup.cfg
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2459 2024-04-24 09:25:49.000000 filemac-1.0.2/setup.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)        6 2024-04-24 09:28:39.000000 filemac-1.0.2/version.txt
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:57:00.565402 filemac-1.0.3/
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:56:59.913416 filemac-1.0.3/.github/
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:56:59.917416 filemac-1.0.3/.github/workflows/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1070 2024-04-25 17:10:07.000000 filemac-1.0.3/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 skye      (1000) skye      (1000)    35149 2024-03-24 06:23:20.000000 filemac-1.0.3/LICENSE
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       80 2024-03-24 07:29:02.000000 filemac-1.0.3/MANIFEST.ini
+-rw-r--r--   0 skye      (1000) skye      (1000)     4825 2024-05-24 08:57:00.565402 filemac-1.0.3/PKG-INFO
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     3938 2024-05-24 08:51:48.000000 filemac-1.0.3/README.md
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     3930 2024-05-24 08:51:48.000000 filemac-1.0.3/README.md~
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:57:00.557402 filemac-1.0.3/__pycache__/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2386 2024-04-09 15:25:19.000000 filemac-1.0.3/__pycache__/Analyzer.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     3992 2024-04-09 15:25:19.000000 filemac-1.0.3/__pycache__/AudioExtractor.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     6728 2024-04-09 15:25:19.000000 filemac-1.0.3/__pycache__/OCRTextExtractor.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2521 2024-04-09 15:25:19.000000 filemac-1.0.3/__pycache__/Simple_v_Analyzer.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)    57828 2024-04-09 15:25:19.000000 filemac-1.0.3/__pycache__/converter.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      723 2024-04-09 15:25:19.000000 filemac-1.0.3/__pycache__/formarts.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      725 2024-04-09 15:25:19.000000 filemac-1.0.3/__pycache__/formats.cpython-311.pyc
+-rw-r--r--   0 skye      (1000) skye      (1000)     3177 2024-05-24 08:56:50.000000 filemac-1.0.3/__pycache__/setup.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      957 2024-04-09 15:25:19.000000 filemac-1.0.3/__pycache__/show_progress.cpython-311.pyc
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:57:00.561402 filemac-1.0.3/filemac/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2017 2024-05-22 10:50:34.000000 filemac-1.0.3/filemac/AudioExtractor.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     4081 2024-05-22 11:10:24.000000 filemac-1.0.3/filemac/OCRTextExtractor.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1773 2024-04-26 06:11:48.000000 filemac-1.0.3/filemac/Simple_v_Analyzer.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       23 2024-03-24 07:50:06.000000 filemac-1.0.3/filemac/__init__.py
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:57:00.565402 filemac-1.0.3/filemac/__pycache__/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     4000 2024-03-24 06:16:58.000000 filemac-1.0.3/filemac/__pycache__/AudioExtractor.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     6471 2024-04-25 17:29:35.000000 filemac-1.0.3/filemac/__pycache__/OCRTextExtractor.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2526 2024-03-24 06:16:56.000000 filemac-1.0.3/filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1279 2024-04-26 14:17:54.000000 filemac-1.0.3/filemac/__pycache__/colors.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)    66273 2024-04-25 14:56:38.000000 filemac-1.0.3/filemac/__pycache__/converter.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      730 2024-03-24 06:16:58.000000 filemac-1.0.3/filemac/__pycache__/formats.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1416 2024-05-22 15:44:52.000000 filemac-1.0.3/filemac/colors.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)    48277 2024-05-23 09:57:56.000000 filemac-1.0.3/filemac/converter.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      185 2024-05-23 09:55:54.000000 filemac-1.0.3/filemac/dd.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     8906 2024-05-22 10:53:05.000000 filemac-1.0.3/filemac/fmac.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     5580 2024-04-24 09:25:49.000000 filemac-1.0.3/filemac/formats.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      254 2024-04-24 09:25:49.000000 filemac-1.0.3/filemac/handle_warnings.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2738 2024-05-11 16:35:34.000000 filemac-1.0.3/filemac/image_op.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2253 2024-05-22 11:06:09.000000 filemac-1.0.3/filemac/longImg.py
+-rw-r--r--   0 skye      (1000) skye      (1000)     1077 2024-05-24 07:16:44.000000 filemac-1.0.3/filemac/pdfaudio.py
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:57:00.561402 filemac-1.0.3/filemac.egg-info/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     4825 2024-05-24 08:56:59.000000 filemac-1.0.3/filemac.egg-info/PKG-INFO
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1326 2024-05-24 08:56:59.000000 filemac-1.0.3/filemac.egg-info/SOURCES.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)        1 2024-05-24 08:56:59.000000 filemac-1.0.3/filemac.egg-info/dependency_links.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       87 2024-05-24 08:56:59.000000 filemac-1.0.3/filemac.egg-info/entry_points.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)        1 2024-04-13 09:48:20.000000 filemac-1.0.3/filemac.egg-info/not-zip-safe
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      174 2024-05-24 08:56:59.000000 filemac-1.0.3/filemac.egg-info/requires.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       19 2024-05-24 08:56:59.000000 filemac-1.0.3/filemac.egg-info/top_level.txt
+-rw-r--r--   0 skye      (1000) skye      (1000)       38 2024-05-24 08:57:00.565402 filemac-1.0.3/setup.cfg
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2536 2024-05-24 08:50:55.000000 filemac-1.0.3/setup.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2535 2024-05-24 08:50:54.000000 filemac-1.0.3/setup.py~
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:57:00.565402 filemac-1.0.3/tets/
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-05-24 08:57:00.565402 filemac-1.0.3/tets/__pycache__/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1111 2024-04-18 10:35:04.000000 filemac-1.0.3/tets/__pycache__/dd.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      891 2024-04-18 10:35:04.000000 filemac-1.0.3/tets/dd.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      715 2024-04-18 10:35:04.000000 filemac-1.0.3/tets/test.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)        6 2024-05-24 08:46:24.000000 filemac-1.0.3/version.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)        6 2024-05-24 08:46:24.000000 filemac-1.0.3/version.txt~
```

### Comparing `filemac-1.0.2/.github/workflows/python-publish.yml` & `filemac-1.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/LICENSE` & `filemac-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/PKG-INFO` & `filemac-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filemac
-Version: 1.0.2
+Version: 1.0.3
 Summary: Open source Python CLI toolkit for conversion, manipulation, Analysis
 Author: wambua
 Author-email: wambuamwiky2001@gmail.com
 License: GPL v3
 Keywords: file-conversion,file-analysis,file-manipulation,ocr,image-conversion
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
@@ -22,14 +22,20 @@
 License-File: LICENSE
 
 # fconverter
 A python file `conversion`, `manipulation`, `Analysis` toolkit
 `This is a Linux command-line interface (CLI) utility that coverts documents from one format to another,
 analyzes files, manipulates files.
 Your can also convert text file to mp3 formart using google Text to speech library (gTTS).
+## Name variations
+```shell
+   filemac -h
+   Filemac -h
+   FILEMAC -h
+   ```
 
 ## Installation
 1. using pip
 
    ```shell
 	pip install filemac
    ```
```

### Comparing `filemac-1.0.2/README.md` & `filemac-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # fconverter
 A python file `conversion`, `manipulation`, `Analysis` toolkit
 `This is a Linux command-line interface (CLI) utility that coverts documents from one format to another,
 analyzes files, manipulates files.
 Your can also convert text file to mp3 formart using google Text to speech library (gTTS).
+## Name variations
+```shell
+   filemac -h
+   Filemac -h
+   FILEMAC -h
+   ```
 
 ## Installation
 1. using pip
 
    ```shell
 	pip install filemac
    ```
```

### Comparing `filemac-1.0.2/__pycache__/Analyzer.cpython-311.pyc` & `filemac-1.0.3/__pycache__/Analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/__pycache__/AudioExtractor.cpython-311.pyc` & `filemac-1.0.3/__pycache__/AudioExtractor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/__pycache__/OCRTextExtractor.cpython-311.pyc` & `filemac-1.0.3/__pycache__/OCRTextExtractor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/__pycache__/Simple_v_Analyzer.cpython-311.pyc` & `filemac-1.0.3/__pycache__/Simple_v_Analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/__pycache__/converter.cpython-311.pyc` & `filemac-1.0.3/__pycache__/converter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/__pycache__/formarts.cpython-311.pyc` & `filemac-1.0.3/__pycache__/formarts.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/__pycache__/formats.cpython-311.pyc` & `filemac-1.0.3/__pycache__/formats.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/__pycache__/show_progress.cpython-311.pyc` & `filemac-1.0.3/__pycache__/show_progress.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/filemac/AudioExtractor.py` & `filemac-1.0.3/filemac/AudioExtractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import logging
+import logging.handlers
 import os
 import sys
+
 from moviepy.editor import VideoFileClip
-import logging
-import logging.handlers
+
+from .colors import DCYAN, DYELLOW, RED, RESET
+
 ###############################################################################
 logging.basicConfig(level=logging.INFO, format='%(levelname)-8s %(message)s')
 logger = logging.getLogger(__name__)
 
 
 class ExtractAudio:
     def __init__(self, input_file):
@@ -16,15 +20,15 @@
         try:
             files_to_process = []
 
             if os.path.isfile(self.input_file):
                 files_to_process.append(self.input_file)
             elif os.path.isdir(self.input_file):
                 if os.listdir(self.input_file) is None:
-                    print("Cannot work with empty folder")
+                    print(f"{RED}Cannot work with empty folder{RESET}")
                     sys.exit(1)
                 for file in os.listdir(self.input_file):
                     file_path = os.path.join(self.input_file, file)
                     ls = ["mp4", "mkv"]
                     if os.path.isfile(file_path) and any(file_path.lower().endswith(ext) for ext in ls):
                         files_to_process.append(file_path)
 
@@ -32,15 +36,15 @@
         except Exception as e:
             print(e)
 
     def moviepyextract(self):
         try:
             video_list = self.preprocess()
             for input_video in video_list:
-                print("\033[1;33mExtracting..\033[1;36m")
+                print(F"{DYELLOW}Extracting..{DCYAN}")
                 video = VideoFileClip(input_video)
                 audio = video.audio
                 basename, _ = os.path.splitext(input_video)
                 outfile = basename + ".wav"
                 audio.write_audiofile(outfile)
                 # print(f"\033[1;32mFile saved as \033[36m{outfile}\033[0m")
         except KeyboardInterrupt:
```

### Comparing `filemac-1.0.2/filemac/OCRTextExtractor.py` & `filemac-1.0.3/filemac/OCRTextExtractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import sys
 import cv2
 import pytesseract
 from PIL import Image
 import logging
 import logging.handlers
+from .colors import (RESET, RED, DGREEN, BBWHITE, DYELLOW, CYAN,
+                     FMAGENTA)
 ###############################################################################
 logging.basicConfig(level=logging.INFO, format='%(levelname)-8s %(message)s')
 logger = logging.getLogger(__name__)
 ###############################################################################
 '''Do OCR text extraction from a given image file and display the extracted
     text
     to the screen finally save it to a text file assuming the name of the input
@@ -24,15 +26,15 @@
     def preprocess(self):
         files_to_process = []
 
         if os.path.isfile(self.input_file):
             files_to_process.append(self.input_file)
         elif os.path.isdir(self.input_file):
             if os.listdir(self.input_file) is None:
-                print("Cannot work with empty folder")
+                print(f"{RED}Cannot work with empty folder{RESET}")
                 sys.exit(1)
             for file in os.listdir(self.input_file):
                 file_path = os.path.join(self.input_file, file)
                 if os.path.isfile(file_path):
                     files_to_process.append(file_path)
 
         return files_to_process
@@ -44,58 +46,58 @@
             item for item in image_list if any(item.lower().endswith(ext)
                                                for ext in ls)]
 
         def ocr_text_extraction(image_path):
             '''Load image using OpenCV'''
             img = cv2.imread(image_path)
 
-            logger.info(f"\033[2;95mprocessing {image_path}...\033[0m")
+            logger.info(f"{FMAGENTA}processing {image_path}...{RESET}")
 
             try:
                 '''Preprocess image for better OCR results'''
                 gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
                 thresh = cv2.threshold(
                     gray, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1]
                 img_pil = Image.fromarray(thresh)
 
                 '''Perform OCR using pytesseract'''
                 config = ("-l eng --oem 3 --psm 6")
                 text = pytesseract.image_to_string((img_pil), config=config)
 
                 '''Remove extra whitespaces and newlines
                 text = ' '.join(text.split()).strip()'''
-                logger.info("\033[36mFound:\n\033[0m")
+                logger.info(F"{CYAN}Found:\n{RESET}")
                 print(text)
                 current_path = os.getcwd()
                 file_path = os.path.join(current_path, OCR_file)
                 ''' Save the extracted text to specified file '''
-                logger.info("\033[1;92mGenerating text file for the extracted \
-text..\033[0m")
+                logger.info(f"{DGREEN}Generating text file for the extracted \
+text..{RESET}")
 
                 with open(file_path, 'w') as file:
                     file.write(text)
                 logger.info(
-                    f"File saved as \033[1;93m{OCR_file}\033[0m:")
+                    f"File saved as {DYELLOW}{OCR_file}{RESET}:")
                 '''If there are multiple candidate images for text extraction,
                 wait for key press before proceeding to the next
                 image otherwise don't wait
                 size = [i for i in enumerate(image_list)]'''
                 if len(image_list) >= 2:
-                    input("\033[5;97mPress Enter to continue\033[0m")
+                    input(F"{BBWHITE}Press Enter to continue{RESET}")
             except KeyboardInterrupt:
                 print("\nExiting")
                 sys.exit(0)
             except FileNotFoundError as e:
                 logger.error(f"Error: {str(e)}")
             except IOError as e:
                 logger.error(
                     f"Could not write to output file '{OCR_file}'. \
-Reason: {str(e)}\033[0m")
+Reason: {str(e)}{RESET}")
             except Exception as e:
                 logger.error(f"Error: {type(e).__name__}: {str(e)}")
             except Exception as e:
-                logger.error(f"Error:>>\033[31m{e}\033[0m")
+                logger.error(f"Error:>>{RED}{e}{RESET}")
             return text
 
         for image_path in image_list:
             OCR_file = image_path[:-4] + ".txt"
             ocr_text_extraction(image_path)
```

### Comparing `filemac-1.0.2/filemac/Simple_v_Analyzer.py` & `filemac-1.0.3/filemac/Simple_v_Analyzer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import sys
 import cv2
 import numpy as np
+from .colors import DYELLOW, RESET, DCYAN, DGREEN
 
 
 class SA:
 
     def __init__(self, video):
         self.video = video
 
     def SimpleAnalyzer(self):
         try:
             # Read the video file
             cap = cv2.VideoCapture(self.video)
-            print("\033[1;33mInitializing..\033[0m")
+            print(f"{DYELLOW}Initializing..{RESET}")
             # Initialize variables
             frame_count = 0
             total_area = 0
             duration = 0
 
-            print("\033[1;36mWorking on it")
+            print(f"{DCYAN}mWorking on it{RESET}")
             while True:
                 ret, frame = cap.read()
 
                 if not ret:
                     break
                 # Increase frame count and accumulate area
                 frame_count += 1
@@ -40,17 +41,17 @@
                     break
 
             # Release the video capture object and close all windows
             cap.release()
             cv2.destroyAllWindows()
 
             # Print results
-            print(f"Total Frames: \033[1;32m{frame_count}\033[0m")
-            print(f"Average Frame Area: \033[1;32m{total_area / frame_count}\033[0m")
-            print(f"Duration: \033[1;32m{duration}\033[0m seconds")
+            print(f"Total Frames: {DGREEN}{frame_count}{RESET}")
+            print(f"Average Frame Area: {DGREEN}{total_area / frame_count}{RESET}")
+            print(f"Duration: {DGREEN}{duration}{RESET} seconds")
         except KeyboardInterrupt:
             print("\nExiting")
             sys.exit(1)
         except Exception as e:
             print(e)
             sys.exit(1)
```

### Comparing `filemac-1.0.2/filemac/__pycache__/AudioExtractor.cpython-311.pyc` & `filemac-1.0.3/filemac/__pycache__/AudioExtractor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/filemac/__pycache__/OCRTextExtractor.cpython-311.pyc` & `filemac-1.0.3/filemac/__pycache__/OCRTextExtractor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc` & `filemac-1.0.3/filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/filemac/__pycache__/colors.cpython-311.pyc` & `filemac-1.0.3/filemac/__pycache__/colors.cpython-311.pyc`

 * *Files 18% similar despite different names*

#### Python bytecode

```diff
@@ -1,28 +1,30 @@
 magic:    0xa70d0d0a
-moddate:  0x720c2066 (Wed Apr 17 17:52:50 2024 UTC)
-files sz: 891
+moddate:  0x0d462b66 (Fri Apr 26 06:13:33 2024 UTC)
+files sz: 1058
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a0401
       00020065046403ac04a6010000ab010000000000000000010065006a0500
-      0000000000000064056b0200000000721c64065a0664075a0764085a0864
+      0000000000000064056b0200000000722264065a0664075a0764085a0864
       095a09640a5a0a640b5a0b640c5a0c640d5a0d640e5a0e640f5a0f64105a
-      1064115a1164125a126401530065006a05000000000000000064136b0200
-      000000725d65036a1300000000000000005a0665026a1400000000000000
-      005a0765026a0700000000000000005a0865026a1500000000000000005a
-      0965026a0900000000000000005a0a65026a1600000000000000005a0b65
-      026a0b00000000000000005a0c65026a1700000000000000005a0d65026a
-      0d00000000000000005a0e65026a1800000000000000005a0f65026a0f00
-      000000000000005a1065026a1900000000000000005a1165026a11000000
-      00000000005a126401530064015300
+      1064115a1164125a1264135a1364145a1464155a156401530065006a0500
+      0000000000000064166b0200000000727265036a1600000000000000005a
+      0665026a1700000000000000005a0765026a0700000000000000005a0865
+      026a1800000000000000005a0965026a0900000000000000005a0a65026a
+      1900000000000000005a0b65026a0b00000000000000005a0c65026a1a00
+      000000000000005a0d65026a0d00000000000000005a0e65026a1b000000
+      00000000005a0f65026a0f00000000000000005a1065026a1b0000000000
+      0000005a1165026a1c00000000000000005a1265026a1200000000000000
+      005a1365026a1d00000000000000005a1465026a1d00000000000000005a
+      1e6401530064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
@@ -45,15 +47,15 @@
                 42 CALL                     1
                 52 POP_TOP
    
      7          54 LOAD_NAME                0 (os)
                 56 LOAD_ATTR                5 (name)
                 66 LOAD_CONST               5 ('posix')
                 68 COMPARE_OP               2 (==)
-                74 POP_JUMP_FORWARD_IF_FALSE    28 (to 132)
+                74 POP_JUMP_FORWARD_IF_FALSE    34 (to 144)
    
      8          76 LOAD_CONST               6 ('\x1b[0m')
                 78 STORE_NAME               6 (RESET)
    
      9          80 LOAD_CONST               7 ('\x1b[91m')
                 82 STORE_NAME               7 (RED)
    
@@ -80,84 +82,105 @@
    
     17         112 LOAD_CONST              15 ('\x1b[95m')
                114 STORE_NAME              15 (MAGENTA)
    
     18         116 LOAD_CONST              16 ('\x1b[1;95m')
                118 STORE_NAME              16 (DMAGENTA)
    
-    19         120 LOAD_CONST              17 ('\x1b[96m')
-               122 STORE_NAME              17 (CYAN)
+    19         120 LOAD_CONST              17 ('\x1b[3;95m')
+               122 STORE_NAME              17 (FMAGENTA)
    
-    20         124 LOAD_CONST              18 ('\x1b[1;96m')
-               126 STORE_NAME              18 (DCYAN)
-               128 LOAD_CONST               1 (None)
-               130 RETURN_VALUE
-   
-    22     >>  132 LOAD_NAME                0 (os)
-               134 LOAD_ATTR                5 (name)
-               144 LOAD_CONST              19 ('nt')
-               146 COMPARE_OP               2 (==)
-               152 POP_JUMP_FORWARD_IF_FALSE    93 (to 340)
-   
-    23         154 LOAD_NAME                3 (Style)
-               156 LOAD_ATTR               19 (RESET_ALL)
-               166 STORE_NAME               6 (RESET)
-   
-    24         168 LOAD_NAME                2 (Fore)
-               170 LOAD_ATTR               20 (LIGHTRED_EX)
-               180 STORE_NAME               7 (RED)
-   
-    25         182 LOAD_NAME                2 (Fore)
-               184 LOAD_ATTR                7 (RED)
-               194 STORE_NAME               8 (DRED)
-   
-    26         196 LOAD_NAME                2 (Fore)
-               198 LOAD_ATTR               21 (LIGHTGREEN_EX)
-               208 STORE_NAME               9 (GREEN)
-   
-    27         210 LOAD_NAME                2 (Fore)
-               212 LOAD_ATTR                9 (GREEN)
-               222 STORE_NAME              10 (DGREEN)
-   
-    28         224 LOAD_NAME                2 (Fore)
-               226 LOAD_ATTR               22 (LIGHTYELLOW_EX)
-               236 STORE_NAME              11 (YELLOW)
-   
-    29         238 LOAD_NAME                2 (Fore)
-               240 LOAD_ATTR               11 (YELLOW)
-               250 STORE_NAME              12 (DYELLOW)
-   
-    30         252 LOAD_NAME                2 (Fore)
-               254 LOAD_ATTR               23 (LIGHTBLUE_EX)
-               264 STORE_NAME              13 (BLUE)
-   
-    31         266 LOAD_NAME                2 (Fore)
-               268 LOAD_ATTR               13 (BLUE)
-               278 STORE_NAME              14 (DBLUE)
-   
-    32         280 LOAD_NAME                2 (Fore)
-               282 LOAD_ATTR               24 (LIGHTMAGENTA_EX)
-               292 STORE_NAME              15 (MAGENTA)
-   
-    33         294 LOAD_NAME                2 (Fore)
-               296 LOAD_ATTR               15 (MAGENTA)
-               306 STORE_NAME              16 (DMAGENTA)
-   
-    34         308 LOAD_NAME                2 (Fore)
-               310 LOAD_ATTR               25 (LIGHTCYAN_EX)
-               320 STORE_NAME              17 (CYAN)
-   
-    35         322 LOAD_NAME                2 (Fore)
-               324 LOAD_ATTR               17 (CYAN)
-               334 STORE_NAME              18 (DCYAN)
-               336 LOAD_CONST               1 (None)
-               338 RETURN_VALUE
+    20         124 LOAD_CONST              18 ('\x1b[96m')
+               126 STORE_NAME              18 (CYAN)
    
-    22     >>  340 LOAD_CONST               1 (None)
-               342 RETURN_VALUE
+    21         128 LOAD_CONST              19 ('\x1b[1;96m')
+               130 STORE_NAME              19 (DCYAN)
+   
+    22         132 LOAD_CONST              20 ('\x1b[3;96m')
+               134 STORE_NAME              20 (ICYAN)
+   
+    23         136 LOAD_CONST              21 ('\x1b[5;97;1m')
+               138 STORE_NAME              21 (BBWHITE)
+               140 LOAD_CONST               1 (None)
+               142 RETURN_VALUE
+   
+    25     >>  144 LOAD_NAME                0 (os)
+               146 LOAD_ATTR                5 (name)
+               156 LOAD_CONST              22 ('nt')
+               158 COMPARE_OP               2 (==)
+               164 POP_JUMP_FORWARD_IF_FALSE   114 (to 394)
+   
+    26         166 LOAD_NAME                3 (Style)
+               168 LOAD_ATTR               22 (RESET_ALL)
+               178 STORE_NAME               6 (RESET)
+   
+    27         180 LOAD_NAME                2 (Fore)
+               182 LOAD_ATTR               23 (LIGHTRED_EX)
+               192 STORE_NAME               7 (RED)
+   
+    28         194 LOAD_NAME                2 (Fore)
+               196 LOAD_ATTR                7 (RED)
+               206 STORE_NAME               8 (DRED)
+   
+    29         208 LOAD_NAME                2 (Fore)
+               210 LOAD_ATTR               24 (LIGHTGREEN_EX)
+               220 STORE_NAME               9 (GREEN)
+   
+    30         222 LOAD_NAME                2 (Fore)
+               224 LOAD_ATTR                9 (GREEN)
+               234 STORE_NAME              10 (DGREEN)
+   
+    31         236 LOAD_NAME                2 (Fore)
+               238 LOAD_ATTR               25 (LIGHTYELLOW_EX)
+               248 STORE_NAME              11 (YELLOW)
+   
+    32         250 LOAD_NAME                2 (Fore)
+               252 LOAD_ATTR               11 (YELLOW)
+               262 STORE_NAME              12 (DYELLOW)
+   
+    33         264 LOAD_NAME                2 (Fore)
+               266 LOAD_ATTR               26 (LIGHTBLUE_EX)
+               276 STORE_NAME              13 (BLUE)
+   
+    34         278 LOAD_NAME                2 (Fore)
+               280 LOAD_ATTR               13 (BLUE)
+               290 STORE_NAME              14 (DBLUE)
+   
+    35         292 LOAD_NAME                2 (Fore)
+               294 LOAD_ATTR               27 (LIGHTMAGENTA_EX)
+               304 STORE_NAME              15 (MAGENTA)
+   
+    36         306 LOAD_NAME                2 (Fore)
+               308 LOAD_ATTR               15 (MAGENTA)
+               318 STORE_NAME              16 (DMAGENTA)
+   
+    37         320 LOAD_NAME                2 (Fore)
+               322 LOAD_ATTR               27 (LIGHTMAGENTA_EX)
+               332 STORE_NAME              17 (FMAGENTA)
+   
+    38         334 LOAD_NAME                2 (Fore)
+               336 LOAD_ATTR               28 (LIGHTCYAN_EX)
+               346 STORE_NAME              18 (CYAN)
+   
+    39         348 LOAD_NAME                2 (Fore)
+               350 LOAD_ATTR               18 (CYAN)
+               360 STORE_NAME              19 (DCYAN)
+   
+    40         362 LOAD_NAME                2 (Fore)
+               364 LOAD_ATTR               29 (WHITE)
+               374 STORE_NAME              20 (ICYAN)
+   
+    41         376 LOAD_NAME                2 (Fore)
+               378 LOAD_ATTR               29 (WHITE)
+               388 STORE_NAME              30 (BWHITE)
+               390 LOAD_CONST               1 (None)
+               392 RETURN_VALUE
+   
+    25     >>  394 LOAD_CONST               1 (None)
+               396 RETURN_VALUE
    consts
       0
       None
       ('Fore', 'Style', 'init')
       True
       ('autoreset',)
       'posix'
@@ -168,21 +191,24 @@
       '\x1b[1;92m'
       '\x1b[93m'
       '\x1b[1;93m'
       '\x1b[94m'
       '\x1b[1;94m'
       '\x1b[95m'
       '\x1b[1;95m'
+      '\x1b[3;95m'
       '\x1b[96m'
       '\x1b[1;96m'
+      '\x1b[3;96m'
+      '\x1b[5;97;1m'
       'nt'
-   names      ('os', 'colorama', 'Fore', 'Style', 'init', 'name', 'RESET', 'RED', 'DRED', 'GREEN', 'DGREEN', 'YELLOW', 'DYELLOW', 'BLUE', 'DBLUE', 'MAGENTA', 'DMAGENTA', 'CYAN', 'DCYAN', 'RESET_ALL', 'LIGHTRED_EX', 'LIGHTGREEN_EX', 'LIGHTYELLOW_EX', 'LIGHTBLUE_EX', 'LIGHTMAGENTA_EX', 'LIGHTCYAN_EX')
+   names      ('os', 'colorama', 'Fore', 'Style', 'init', 'name', 'RESET', 'RED', 'DRED', 'GREEN', 'DGREEN', 'YELLOW', 'DYELLOW', 'BLUE', 'DBLUE', 'MAGENTA', 'DMAGENTA', 'FMAGENTA', 'CYAN', 'DCYAN', 'ICYAN', 'BBWHITE', 'RESET_ALL', 'LIGHTRED_EX', 'LIGHTGREEN_EX', 'LIGHTYELLOW_EX', 'LIGHTBLUE_EX', 'LIGHTMAGENTA_EX', 'LIGHTCYAN_EX', 'WHITE', 'BWHITE')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/media/skye/Skye/FileMAC/filemac/colors.py'
+   filename   '/media/skye/skye/FileMAC/filemac/colors.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108021402180216010401040104010401040104010401040104
-      01040104010401080216010e010e010e010e010e010e010e010e010e010e
-      010e010e0112f3
+      01040104010401040104010401080216010e010e010e010e010e010e010e
+      010e010e010e010e010e010e010e010e0112f0
```

### Comparing `filemac-1.0.2/filemac/__pycache__/converter.cpython-311.pyc` & `filemac-1.0.3/filemac/__pycache__/converter.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,402 +1,429 @@
 magic:    0xa70d0d0a
-moddate:  0xd7e9ff65 (Sun Mar 24 08:52:39 2024 UTC)
-files sz: 37955
+moddate:  0x58642a66 (Thu Apr 25 14:10:32 2024 UTC)
+files sz: 42649
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a00640064016c025a02640064
       016c035a03640064016c045a04640064016c055a05640064016c065a0664
-      0064016c075a07640064026c086d095a090100640064016c0a5a0a640064
-      036c0b6d0c5a0c0100640064016c0d5a0d640064016c0e5a0f640064016c
-      105a10640064016c115a11640064016c125a12640064016c135a13640064
-      016c145a14640064046c156d165a160100640064056c176d185a18010064
-      0064066c196d1a5a1a0100640064076c1b6d1c5a1c0100640064086c106d
-      1d5a1d0100640064096c1e6d1f5a1f01006400640a6c206d215a21010064
-      00640b6c226d235a2301006400640c6c246d255a256d265a260100640064
-      0d6c206d275a2701006400640e6c206d285a280100640f5a29020065006a
-      2a000000000000000065006a2b00000000000000006410ac11a6020000ab
-      0200000000000000000100020065006a2c0000000000000000652da60100
-      00ab0100000000000000005a2e02004700641284006413a6020000ab0200
-      000000000000005a2f02004700641484006415a6020000ab020000000000
-      0000005a3002004700641684006417a6020000ab0200000000000000005a
-      3102004700641884006419a6020000ab0200000000000000005a32020047
-      00641a8400641ba6020000ab0200000000000000005a3364015300
+      0064016c075a07640064016c085a08640064026c096d0a5a0a0100640064
+      016c0b5a0b640064016c0c5a0d640064016c0e5a0e640064016c0f5a0f64
+      0064016c105a10640064016c115a11640064036c126d135a130100640064
+      046c146d155a150100640064056c166d175a170100640064066c186d195a
+      190100640064076c1a6d1b5a1b0100640064086c1c6d1d5a1d0100640064
+      096c0e6d1e5a1e0100640a640b6c1f6d205a206d215a216d225a226d235a
+      236d245a246d255a256d265a266d275a276d285a286d295a296d2a5a2a01
+      006400640c6c2b6d2c5a2c01006400640d6c2d6d2e5a2e6d2f5a2f010064
+      0a640e6c306d315a316d325a326d335a330100640a5a34020065006a3500
+      0000000000000065006a360000000000000000640fac10a6020000ab0200
+      000000000000000100020065006a3700000000000000006538a6010000ab
+      0100000000000000005a3902004700641184006412a6020000ab02000000
+      00000000005a3a02004700641384006414a6020000ab0200000000000000
+      005a3b02004700641584006416a6020000ab0200000000000000005a3c02
+      004700641784006418a6020000ab0200000000000000005a3d0200470064
+      198400641aa6020000ab0200000000000000005a3e02004700641b840064
+      1ca6020000ab0200000000000000005a3f64015300
      0           0 RESUME                   0
    
      2           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
      3          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
                 14 IMPORT_NAME              1 (logging.handlers)
                 16 STORE_NAME               0 (logging)
    
-     4          18 LOAD_CONST               0 (0)
+     5          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               1 (None)
-                22 IMPORT_NAME              2 (math)
-                24 STORE_NAME               2 (math)
+                22 IMPORT_NAME              2 (os)
+                24 STORE_NAME               2 (os)
    
-     5          26 LOAD_CONST               0 (0)
+     6          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               1 (None)
-                30 IMPORT_NAME              3 (os)
-                32 STORE_NAME               3 (os)
+                30 IMPORT_NAME              3 (re)
+                32 STORE_NAME               3 (re)
    
-     6          34 LOAD_CONST               0 (0)
+     7          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               1 (None)
-                38 IMPORT_NAME              4 (re)
-                40 STORE_NAME               4 (re)
+                38 IMPORT_NAME              4 (sqlite3)
+                40 STORE_NAME               4 (sqlite3)
    
-     7          42 LOAD_CONST               0 (0)
+     8          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               1 (None)
-                46 IMPORT_NAME              5 (sqlite3)
-                48 STORE_NAME               5 (sqlite3)
+                46 IMPORT_NAME              5 (subprocess)
+                48 STORE_NAME               5 (subprocess)
    
-     8          50 LOAD_CONST               0 (0)
+     9          50 LOAD_CONST               0 (0)
                 52 LOAD_CONST               1 (None)
                 54 IMPORT_NAME              6 (sys)
                 56 STORE_NAME               6 (sys)
    
-     9          58 LOAD_CONST               0 (0)
+    10          58 LOAD_CONST               0 (0)
                 60 LOAD_CONST               1 (None)
                 62 IMPORT_NAME              7 (time)
                 64 STORE_NAME               7 (time)
    
-    10          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               2 (('parse',))
-                70 IMPORT_NAME              8 (pdf2docx)
-                72 IMPORT_FROM              9 (parse)
-                74 STORE_NAME               9 (parse)
-                76 POP_TOP
+    11          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               1 (None)
+                70 IMPORT_NAME              8 (traceback)
+                72 STORE_NAME               8 (traceback)
    
-    11          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               1 (None)
-                82 IMPORT_NAME             10 (traceback)
-                84 STORE_NAME              10 (traceback)
+    14          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               2 (('convert_from_path',))
+                78 IMPORT_NAME              9 (pdf2image)
+                80 IMPORT_FROM             10 (convert_from_path)
+                82 STORE_NAME              10 (convert_from_path)
+                84 POP_TOP
    
-    13          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               3 (('Iterable',))
-                90 IMPORT_NAME             11 (typing)
-                92 IMPORT_FROM             12 (Iterable)
-                94 STORE_NAME              12 (Iterable)
-                96 POP_TOP
+    15          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               1 (None)
+                90 IMPORT_NAME             11 (cv2)
+                92 STORE_NAME              11 (cv2)
    
-    14          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               1 (None)
-               102 IMPORT_NAME             13 (cv2)
-               104 STORE_NAME              13 (cv2)
+    16          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               1 (None)
+                98 IMPORT_NAME             12 (pandas)
+               100 STORE_NAME              13 (pd)
    
-    15         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               1 (None)
-               110 IMPORT_NAME             14 (pandas)
-               112 STORE_NAME              15 (pd)
+    17         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               1 (None)
+               106 IMPORT_NAME             14 (pydub)
+               108 STORE_NAME              14 (pydub)
    
-    16         114 LOAD_CONST               0 (0)
-               116 LOAD_CONST               1 (None)
-               118 IMPORT_NAME             16 (pydub)
-               120 STORE_NAME              16 (pydub)
+    18         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               1 (None)
+               114 IMPORT_NAME             15 (PyPDF2)
+               116 STORE_NAME              15 (PyPDF2)
    
-    17         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST               1 (None)
-               126 IMPORT_NAME             17 (PyPDF2)
-               128 STORE_NAME              17 (PyPDF2)
+    20         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               1 (None)
+               122 IMPORT_NAME             16 (requests)
+               124 STORE_NAME              16 (requests)
    
-    18         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST               1 (None)
-               134 IMPORT_NAME             18 (subprocess)
-               136 STORE_NAME              18 (subprocess)
+    21         126 LOAD_CONST               0 (0)
+               128 LOAD_CONST               1 (None)
+               130 IMPORT_NAME             17 (speedtest)
+               132 STORE_NAME              17 (speedtest)
    
-    20         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST               1 (None)
-               142 IMPORT_NAME             19 (requests)
-               144 STORE_NAME              19 (requests)
+    22         134 LOAD_CONST               0 (0)
+               136 LOAD_CONST               3 (('Document',))
+               138 IMPORT_NAME             18 (docx)
+               140 IMPORT_FROM             19 (Document)
+               142 STORE_NAME              19 (Document)
+               144 POP_TOP
    
-    21         146 LOAD_CONST               0 (0)
-               148 LOAD_CONST               1 (None)
-               150 IMPORT_NAME             20 (speedtest)
-               152 STORE_NAME              20 (speedtest)
+    24         146 LOAD_CONST               0 (0)
+               148 LOAD_CONST               4 (('gTTS',))
+               150 IMPORT_NAME             20 (gtts)
+               152 IMPORT_FROM             21 (gTTS)
+               154 STORE_NAME              21 (gTTS)
+               156 POP_TOP
    
-    22         154 LOAD_CONST               0 (0)
-               156 LOAD_CONST               4 (('Image',))
-               158 IMPORT_NAME             21 (PIL)
-               160 IMPORT_FROM             22 (Image)
-               162 STORE_NAME              22 (Image)
-               164 POP_TOP
+    26         158 LOAD_CONST               0 (0)
+               160 LOAD_CONST               5 (('VideoFileClip',))
+               162 IMPORT_NAME             22 (moviepy.editor)
+               164 IMPORT_FROM             23 (VideoFileClip)
+               166 STORE_NAME              23 (VideoFileClip)
+               168 POP_TOP
    
-    23         166 LOAD_CONST               0 (0)
-               168 LOAD_CONST               5 (('Document',))
-               170 IMPORT_NAME             23 (docx)
-               172 IMPORT_FROM             24 (Document)
-               174 STORE_NAME              24 (Document)
-               176 POP_TOP
+    27         170 LOAD_CONST               0 (0)
+               172 LOAD_CONST               6 (('parse',))
+               174 IMPORT_NAME             24 (pdf2docx)
+               176 IMPORT_FROM             25 (parse)
+               178 STORE_NAME              25 (parse)
+               180 POP_TOP
    
-    25         178 LOAD_CONST               0 (0)
-               180 LOAD_CONST               6 (('gTTS',))
-               182 IMPORT_NAME             25 (gtts)
-               184 IMPORT_FROM             26 (gTTS)
-               186 STORE_NAME              26 (gTTS)
-               188 POP_TOP
+    28         182 LOAD_CONST               0 (0)
+               184 LOAD_CONST               7 (('Image',))
+               186 IMPORT_NAME             26 (PIL)
+               188 IMPORT_FROM             27 (Image)
+               190 STORE_NAME              27 (Image)
+               192 POP_TOP
    
-    28         190 LOAD_CONST               0 (0)
-               192 LOAD_CONST               7 (('Presentation',))
-               194 IMPORT_NAME             27 (pptx)
-               196 IMPORT_FROM             28 (Presentation)
-               198 STORE_NAME              28 (Presentation)
-               200 POP_TOP
+    29         194 LOAD_CONST               0 (0)
+               196 LOAD_CONST               8 (('Presentation',))
+               198 IMPORT_NAME             28 (pptx)
+               200 IMPORT_FROM             29 (Presentation)
+               202 STORE_NAME              29 (Presentation)
+               204 POP_TOP
    
-    29         202 LOAD_CONST               0 (0)
-               204 LOAD_CONST               8 (('AudioSegment',))
-               206 IMPORT_NAME             16 (pydub)
-               208 IMPORT_FROM             29 (AudioSegment)
-               210 STORE_NAME              29 (AudioSegment)
-               212 POP_TOP
+    30         206 LOAD_CONST               0 (0)
+               208 LOAD_CONST               9 (('AudioSegment',))
+               210 IMPORT_NAME             14 (pydub)
+               212 IMPORT_FROM             30 (AudioSegment)
+               214 STORE_NAME              30 (AudioSegment)
+               216 POP_TOP
    
-    31         214 LOAD_CONST               0 (0)
-               216 LOAD_CONST               9 (('VideoFileClip',))
-               218 IMPORT_NAME             30 (moviepy.editor)
-               220 IMPORT_FROM             31 (VideoFileClip)
-               222 STORE_NAME              31 (VideoFileClip)
-               224 POP_TOP
+    31         218 LOAD_CONST              10 (1)
+               220 LOAD_CONST              11 (('RESET', 'GREEN', 'DGREEN', 'YELLOW', 'DYELLOW', 'CYAN', 'BLUE', 'DBLUE', 'DMAGENTA', 'DRED', 'ICYAN'))
+               222 IMPORT_NAME             31 (colors)
+               224 IMPORT_FROM             32 (RESET)
+               226 STORE_NAME              32 (RESET)
+               228 IMPORT_FROM             33 (GREEN)
+               230 STORE_NAME              33 (GREEN)
+               232 IMPORT_FROM             34 (DGREEN)
+               234 STORE_NAME              34 (DGREEN)
+               236 IMPORT_FROM             35 (YELLOW)
+               238 STORE_NAME              35 (YELLOW)
+               240 IMPORT_FROM             36 (DYELLOW)
+               242 STORE_NAME              36 (DYELLOW)
+               244 IMPORT_FROM             37 (CYAN)
+               246 STORE_NAME              37 (CYAN)
+               248 IMPORT_FROM             38 (BLUE)
+               250 STORE_NAME              38 (BLUE)
+               252 IMPORT_FROM             39 (DBLUE)
+               254 STORE_NAME              39 (DBLUE)
+               256 IMPORT_FROM             40 (DMAGENTA)
+               258 STORE_NAME              40 (DMAGENTA)
+               260 IMPORT_FROM             41 (DRED)
+               262 STORE_NAME              41 (DRED)
+               264 IMPORT_FROM             42 (ICYAN)
+               266 STORE_NAME              42 (ICYAN)
+               268 POP_TOP
    
-    32         226 LOAD_CONST               0 (0)
-               228 LOAD_CONST              10 (('SUPPORTED_VIDEO_FORMATS',))
-               230 IMPORT_NAME             32 (formats)
-               232 IMPORT_FROM             33 (SUPPORTED_VIDEO_FORMATS)
-               234 STORE_NAME              33 (SUPPORTED_VIDEO_FORMATS)
-               236 POP_TOP
+    33         270 LOAD_CONST               0 (0)
+               272 LOAD_CONST              12 (('letter',))
+               274 IMPORT_NAME             43 (reportlab.lib.pagesizes)
+               276 IMPORT_FROM             44 (letter)
+               278 STORE_NAME              44 (letter)
+               280 POP_TOP
    
-    33         238 LOAD_CONST               0 (0)
-               240 LOAD_CONST              11 (('letter',))
-               242 IMPORT_NAME             34 (reportlab.lib.pagesizes)
-               244 IMPORT_FROM             35 (letter)
-               246 STORE_NAME              35 (letter)
-               248 POP_TOP
+    34         282 LOAD_CONST               0 (0)
+               284 LOAD_CONST              13 (('Paragraph', 'SimpleDocTemplate'))
+               286 IMPORT_NAME             45 (reportlab.platypus)
+               288 IMPORT_FROM             46 (Paragraph)
+               290 STORE_NAME              46 (Paragraph)
+               292 IMPORT_FROM             47 (SimpleDocTemplate)
+               294 STORE_NAME              47 (SimpleDocTemplate)
+               296 POP_TOP
    
-    34         250 LOAD_CONST               0 (0)
-               252 LOAD_CONST              12 (('Paragraph', 'SimpleDocTemplate'))
-               254 IMPORT_NAME             36 (reportlab.platypus)
-               256 IMPORT_FROM             37 (Paragraph)
-               258 STORE_NAME              37 (Paragraph)
-               260 IMPORT_FROM             38 (SimpleDocTemplate)
-               262 STORE_NAME              38 (SimpleDocTemplate)
-               264 POP_TOP
+    36         298 LOAD_CONST              10 (1)
+               300 LOAD_CONST              14 (('SUPPORTED_AUDIO_FORMATS', 'SUPPORTED_IMAGE_FORMATS', 'SUPPORTED_VIDEO_FORMATS'))
+               302 IMPORT_NAME             48 (formats)
+               304 IMPORT_FROM             49 (SUPPORTED_AUDIO_FORMATS)
+               306 STORE_NAME              49 (SUPPORTED_AUDIO_FORMATS)
+               308 IMPORT_FROM             50 (SUPPORTED_IMAGE_FORMATS)
+               310 STORE_NAME              50 (SUPPORTED_IMAGE_FORMATS)
+               312 IMPORT_FROM             51 (SUPPORTED_VIDEO_FORMATS)
+               314 STORE_NAME              51 (SUPPORTED_VIDEO_FORMATS)
+               316 POP_TOP
    
-    35         266 LOAD_CONST               0 (0)
-               268 LOAD_CONST              13 (('SUPPORTED_AUDIO_FORMATS',))
-               270 IMPORT_NAME             32 (formats)
-               272 IMPORT_FROM             39 (SUPPORTED_AUDIO_FORMATS)
-               274 STORE_NAME              39 (SUPPORTED_AUDIO_FORMATS)
-               276 POP_TOP
+    46         318 LOAD_CONST              10 (1)
+               320 STORE_NAME              52 (PYGAME_DETECT_AVX2)
    
-    36         278 LOAD_CONST               0 (0)
-               280 LOAD_CONST              14 (('SUPPORTED_IMAGE_FORMATS',))
-               282 IMPORT_NAME             32 (formats)
-               284 IMPORT_FROM             40 (SUPPORTED_IMAGE_FORMATS)
-               286 STORE_NAME              40 (SUPPORTED_IMAGE_FORMATS)
-               288 POP_TOP
+    47         322 PUSH_NULL
+               324 LOAD_NAME                0 (logging)
+               326 LOAD_ATTR               53 (basicConfig)
+               336 LOAD_NAME                0 (logging)
+               338 LOAD_ATTR               54 (INFO)
+               348 LOAD_CONST              15 ('%(levelname)-8s %(message)s')
+               350 KW_NAMES                16
+               352 PRECALL                  2
+               356 CALL                     2
+               366 POP_TOP
    
-    44         290 LOAD_CONST              15 (1)
-               292 STORE_NAME              41 (PYGAME_DETECT_AVX2)
+    48         368 PUSH_NULL
+               370 LOAD_NAME                0 (logging)
+               372 LOAD_ATTR               55 (getLogger)
+               382 LOAD_NAME               56 (__name__)
+               384 PRECALL                  1
+               388 CALL                     1
+               398 STORE_NAME              57 (logger)
    
-    45         294 PUSH_NULL
-               296 LOAD_NAME                0 (logging)
-               298 LOAD_ATTR               42 (basicConfig)
-               308 LOAD_NAME                0 (logging)
-               310 LOAD_ATTR               43 (INFO)
-               320 LOAD_CONST              16 ('%(levelname)-8s %(message)s')
-               322 KW_NAMES                17
-               324 PRECALL                  2
-               328 CALL                     2
-               338 POP_TOP
+    51         400 PUSH_NULL
+               402 LOAD_BUILD_CLASS
+               404 LOAD_CONST              17 (<code object MakeConversion, file "/media/skye/skye/FileMAC/filemac/converter.py", line 51>)
+               406 MAKE_FUNCTION            0
+               408 LOAD_CONST              18 ('MakeConversion')
+               410 PRECALL                  2
+               414 CALL                     2
+               424 STORE_NAME              58 (MakeConversion)
    
-    46         340 PUSH_NULL
-               342 LOAD_NAME                0 (logging)
-               344 LOAD_ATTR               44 (getLogger)
-               354 LOAD_NAME               45 (__name__)
-               356 PRECALL                  1
-               360 CALL                     1
-               370 STORE_NAME              46 (logger)
+   588         426 PUSH_NULL
+               428 LOAD_BUILD_CLASS
+               430 LOAD_CONST              19 (<code object Scanner, file "/media/skye/skye/FileMAC/filemac/converter.py", line 588>)
+               432 MAKE_FUNCTION            0
+               434 LOAD_CONST              20 ('Scanner')
+               436 PRECALL                  2
+               440 CALL                     2
+               450 STORE_NAME              59 (Scanner)
    
-    49         372 PUSH_NULL
-               374 LOAD_BUILD_CLASS
-               376 LOAD_CONST              18 (<code object MakeConversion, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 49>)
-               378 MAKE_FUNCTION            0
-               380 LOAD_CONST              19 ('MakeConversion')
-               382 PRECALL                  2
-               386 CALL                     2
-               396 STORE_NAME              47 (MakeConversion)
+   661         452 PUSH_NULL
+               454 LOAD_BUILD_CLASS
+               456 LOAD_CONST              21 (<code object FileSynthesis, file "/media/skye/skye/FileMAC/filemac/converter.py", line 661>)
+               458 MAKE_FUNCTION            0
+               460 LOAD_CONST              22 ('FileSynthesis')
+               462 PRECALL                  2
+               466 CALL                     2
+               476 STORE_NAME              60 (FileSynthesis)
    
-   541         398 PUSH_NULL
-               400 LOAD_BUILD_CLASS
-               402 LOAD_CONST              20 (<code object FileSynthesis, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 541>)
-               404 MAKE_FUNCTION            0
-               406 LOAD_CONST              21 ('FileSynthesis')
-               408 PRECALL                  2
-               412 CALL                     2
-               422 STORE_NAME              48 (FileSynthesis)
+   855         478 PUSH_NULL
+               480 LOAD_BUILD_CLASS
+               482 LOAD_CONST              23 (<code object VideoConverter, file "/media/skye/skye/FileMAC/filemac/converter.py", line 855>)
+               484 MAKE_FUNCTION            0
+               486 LOAD_CONST              24 ('VideoConverter')
+               488 PRECALL                  2
+               492 CALL                     2
+               502 STORE_NAME              61 (VideoConverter)
    
-   723         424 PUSH_NULL
-               426 LOAD_BUILD_CLASS
-               428 LOAD_CONST              22 (<code object VideoConverter, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 723>)
-               430 MAKE_FUNCTION            0
-               432 LOAD_CONST              23 ('VideoConverter')
-               434 PRECALL                  2
-               438 CALL                     2
-               448 STORE_NAME              49 (VideoConverter)
+   925         504 PUSH_NULL
+               506 LOAD_BUILD_CLASS
+               508 LOAD_CONST              25 (<code object AudioConverter, file "/media/skye/skye/FileMAC/filemac/converter.py", line 925>)
+               510 MAKE_FUNCTION            0
+               512 LOAD_CONST              26 ('AudioConverter')
+               514 PRECALL                  2
+               518 CALL                     2
+               528 STORE_NAME              62 (AudioConverter)
    
-   793         450 PUSH_NULL
-               452 LOAD_BUILD_CLASS
-               454 LOAD_CONST              24 (<code object AudioConverter, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 793>)
-               456 MAKE_FUNCTION            0
-               458 LOAD_CONST              25 ('AudioConverter')
-               460 PRECALL                  2
-               464 CALL                     2
-               474 STORE_NAME              50 (AudioConverter)
-   
-   842         476 PUSH_NULL
-               478 LOAD_BUILD_CLASS
-               480 LOAD_CONST              26 (<code object ImageConverter, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 842>)
-               482 MAKE_FUNCTION            0
-               484 LOAD_CONST              27 ('ImageConverter')
-               486 PRECALL                  2
-               490 CALL                     2
-               500 STORE_NAME              51 (ImageConverter)
-               502 LOAD_CONST               1 (None)
-               504 RETURN_VALUE
+   976         530 PUSH_NULL
+               532 LOAD_BUILD_CLASS
+               534 LOAD_CONST              27 (<code object ImageConverter, file "/media/skye/skye/FileMAC/filemac/converter.py", line 976>)
+               536 MAKE_FUNCTION            0
+               538 LOAD_CONST              28 ('ImageConverter')
+               540 PRECALL                  2
+               544 CALL                     2
+               554 STORE_NAME              63 (ImageConverter)
+               556 LOAD_CONST               1 (None)
+               558 RETURN_VALUE
    consts
       0
       None
-      ('parse',)
-      ('Iterable',)
-      ('Image',)
+      ('convert_from_path',)
       ('Document',)
       ('gTTS',)
+      ('VideoFileClip',)
+      ('parse',)
+      ('Image',)
       ('Presentation',)
       ('AudioSegment',)
-      ('VideoFileClip',)
-      ('SUPPORTED_VIDEO_FORMATS',)
+      1
+      ('RESET', 'GREEN', 'DGREEN', 'YELLOW', 'DYELLOW', 'CYAN', 'BLUE', 'DBLUE', 'DMAGENTA', 'DRED', 'ICYAN')
       ('letter',)
       ('Paragraph', 'SimpleDocTemplate')
-      ('SUPPORTED_AUDIO_FORMATS',)
-      ('SUPPORTED_IMAGE_FORMATS',)
-      1
+      ('SUPPORTED_AUDIO_FORMATS', 'SUPPORTED_IMAGE_FORMATS', 'SUPPORTED_VIDEO_FORMATS')
       '%(levelname)-8s %(message)s'
       ('level', 'format')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 1
+         stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0264015a03640284005a040900640384005a0564
             0484005a06640584005a07640684005a08640784005a09640884005a0a64
             0984005a0b640a84005a0c640b84005a0d640c84005a0e0900640d84005a
-            0f0900640e84005a10640f84005a1164105300
-          49           0 RESUME                   0
+            0f0900640e84005a10640f84005a116413641184015a1264125300
+          51           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('MakeConversion')
                        8 STORE_NAME               2 (__qualname__)
          
-          51          10 LOAD_CONST               1 ('Initialize the class')
+          53          10 LOAD_CONST               1 ('Initialize the class')
                       12 STORE_NAME               3 (__doc__)
          
-          53          14 LOAD_CONST               2 (<code object __init__, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 53>)
+          55          14 LOAD_CONST               2 (<code object __init__, file "/media/skye/skye/FileMAC/filemac/converter.py", line 55>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (__init__)
          
-          56          20 NOP
+          58          20 NOP
          
-          65          22 LOAD_CONST               3 (<code object preprocess, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 65>)
+          67          22 LOAD_CONST               3 (<code object preprocess, file "/media/skye/skye/FileMAC/filemac/converter.py", line 67>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (preprocess)
          
-          87          28 LOAD_CONST               4 (<code object word_to_pdf, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 87>)
+          89          28 LOAD_CONST               4 (<code object word_to_pdf, file "/media/skye/skye/FileMAC/filemac/converter.py", line 89>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (word_to_pdf)
          
-         122          34 LOAD_CONST               5 (<code object pdf_to_word, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 122>)
+         132          34 LOAD_CONST               5 (<code object pdf_to_word, file "/media/skye/skye/FileMAC/filemac/converter.py", line 132>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               7 (pdf_to_word)
          
-         147          40 LOAD_CONST               6 (<code object txt_to_pdf, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 147>)
+         157          40 LOAD_CONST               6 (<code object txt_to_pdf, file "/media/skye/skye/FileMAC/filemac/converter.py", line 157>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               8 (txt_to_pdf)
          
-         170          46 LOAD_CONST               7 (<code object word_to_pptx, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 170>)
+         180          46 LOAD_CONST               7 (<code object word_to_pptx, file "/media/skye/skye/FileMAC/filemac/converter.py", line 180>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               9 (word_to_pptx)
          
-         224          52 LOAD_CONST               8 (<code object word_to_txt, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 224>)
+         234          52 LOAD_CONST               8 (<code object word_to_txt, file "/media/skye/skye/FileMAC/filemac/converter.py", line 234>)
                       54 MAKE_FUNCTION            0
                       56 STORE_NAME              10 (word_to_txt)
          
-         253          58 LOAD_CONST               9 (<code object pdf_to_txt, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 253>)
+         269          58 LOAD_CONST               9 (<code object pdf_to_txt, file "/media/skye/skye/FileMAC/filemac/converter.py", line 269>)
                       60 MAKE_FUNCTION            0
                       62 STORE_NAME              11 (pdf_to_txt)
          
-         280          64 LOAD_CONST              10 (<code object ppt_to_word, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 280>)
+         296          64 LOAD_CONST              10 (<code object ppt_to_word, file "/media/skye/skye/FileMAC/filemac/converter.py", line 296>)
                       66 MAKE_FUNCTION            0
                       68 STORE_NAME              12 (ppt_to_word)
          
-         335          70 LOAD_CONST              11 (<code object text_to_word, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 335>)
+         351          70 LOAD_CONST              11 (<code object text_to_word, file "/media/skye/skye/FileMAC/filemac/converter.py", line 351>)
                       72 MAKE_FUNCTION            0
                       74 STORE_NAME              13 (text_to_word)
          
-         373          76 LOAD_CONST              12 (<code object convert_xls_to_word, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 373>)
+         389          76 LOAD_CONST              12 (<code object convert_xls_to_word, file "/media/skye/skye/FileMAC/filemac/converter.py", line 389>)
                       78 MAKE_FUNCTION            0
                       80 STORE_NAME              14 (convert_xls_to_word)
          
-         416          82 NOP
+         432          82 NOP
          
-         419          84 LOAD_CONST              13 (<code object convert_xls_to_text, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 419>)
+         435          84 LOAD_CONST              13 (<code object convert_xls_to_text, file "/media/skye/skye/FileMAC/filemac/converter.py", line 435>)
                       86 MAKE_FUNCTION            0
                       88 STORE_NAME              15 (convert_xls_to_text)
          
-         458          90 NOP
+         474          90 NOP
          
-         461          92 LOAD_CONST              14 (<code object convert_xlsx_to_csv, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 461>)
+         477          92 LOAD_CONST              14 (<code object convert_xlsx_to_csv, file "/media/skye/skye/FileMAC/filemac/converter.py", line 477>)
                       94 MAKE_FUNCTION            0
                       96 STORE_NAME              16 (convert_xlsx_to_csv)
          
-         494          98 LOAD_CONST              15 (<code object convert_xlsx_to_database, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 494>)
+         510          98 LOAD_CONST              15 (<code object convert_xlsx_to_database, file "/media/skye/skye/FileMAC/filemac/converter.py", line 510>)
                      100 MAKE_FUNCTION            0
                      102 STORE_NAME              17 (convert_xlsx_to_database)
-                     104 LOAD_CONST              16 (None)
-                     106 RETURN_VALUE
+         
+         559         104 LOAD_CONST              19 (('png',))
+                     106 LOAD_CONST              17 (<code object doc2image, file "/media/skye/skye/FileMAC/filemac/converter.py", line 559>)
+                     108 MAKE_FUNCTION            1 (defaults)
+                     110 STORE_NAME              18 (doc2image)
+                     112 LOAD_CONST              18 (None)
+                     114 RETURN_VALUE
          consts
             'MakeConversion'
             'Initialize the class'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x97007c017c005f00000000000000000064005300
-                53           0 RESUME                   0
+                55           0 RESUME                   0
                
-                54           2 LOAD_FAST                1 (input_file)
+                56           2 LOAD_FAST                1 (input_file)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (input_file)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                names      ('input_file',)
                varnames   ('self', 'input_file')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       '__init__'
-               firstlineno 53
+               firstlineno 55
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
@@ -418,115 +445,115 @@
                   0000007d037400000000000000000000006a010000000000000000a00200
                   000000000000000000000000000000000000007c03a6010000ab01000000
                   000000000072157c01a00400000000000000000000000000000000000000
                   007c03a6010000ab01000000000000000001008c5c7c0153002300741600
                   0000000000000000002400721a7d04740f000000000000000000007c04a6
                   010000ab0100000000000000000100590064007d047e046400530064007d
                   047e0477017700780359007701
-                65           0 RESUME                   0
+                67           0 RESUME                   0
                
-                66           2 NOP
+                68           2 NOP
                
-                67           4 BUILD_LIST               0
+                69           4 BUILD_LIST               0
                              6 STORE_FAST               1 (files_to_process)
                
-                69           8 LOAD_GLOBAL              0 (os)
+                71           8 LOAD_GLOBAL              0 (os)
                             20 LOAD_ATTR                1 (path)
                             30 LOAD_METHOD              2 (isfile)
                             52 LOAD_FAST                0 (self)
                             54 LOAD_ATTR                3 (input_file)
                             64 PRECALL                  1
                             68 CALL                     1
                             78 POP_JUMP_FORWARD_IF_FALSE    27 (to 134)
                
-                70          80 LOAD_FAST                1 (files_to_process)
+                72          80 LOAD_FAST                1 (files_to_process)
                             82 LOAD_METHOD              4 (append)
                            104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                3 (input_file)
                            116 PRECALL                  1
                            120 CALL                     1
                            130 POP_TOP
                            132 JUMP_FORWARD           213 (to 560)
                
-                71     >>  134 LOAD_GLOBAL              0 (os)
+                73     >>  134 LOAD_GLOBAL              0 (os)
                            146 LOAD_ATTR                1 (path)
                            156 LOAD_METHOD              5 (isdir)
                            178 LOAD_FAST                0 (self)
                            180 LOAD_ATTR                3 (input_file)
                            190 PRECALL                  1
                            194 CALL                     1
                            204 POP_JUMP_FORWARD_IF_FALSE   177 (to 560)
                
-                72         206 LOAD_GLOBAL              1 (NULL + os)
+                74         206 LOAD_GLOBAL              1 (NULL + os)
                            218 LOAD_ATTR                6 (listdir)
                            228 LOAD_FAST                0 (self)
                            230 LOAD_ATTR                3 (input_file)
                            240 PRECALL                  1
                            244 CALL                     1
                            254 POP_JUMP_FORWARD_IF_NOT_NONE    35 (to 326)
                
-                73         256 LOAD_GLOBAL             15 (NULL + print)
+                75         256 LOAD_GLOBAL             15 (NULL + print)
                            268 LOAD_CONST               1 ('Cannot work with empty folder')
                            270 PRECALL                  1
                            274 CALL                     1
                            284 POP_TOP
                
-                74         286 LOAD_GLOBAL             17 (NULL + sys)
+                76         286 LOAD_GLOBAL             17 (NULL + sys)
                            298 LOAD_ATTR                9 (exit)
                            308 LOAD_CONST               2 (1)
                            310 PRECALL                  1
                            314 CALL                     1
                            324 POP_TOP
                
-                75     >>  326 LOAD_GLOBAL              1 (NULL + os)
+                77     >>  326 LOAD_GLOBAL              1 (NULL + os)
                            338 LOAD_ATTR                6 (listdir)
                            348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR                3 (input_file)
                            360 PRECALL                  1
                            364 CALL                     1
                            374 GET_ITER
                        >>  376 FOR_ITER                91 (to 560)
                            378 STORE_FAST               2 (file)
                
-                76         380 LOAD_GLOBAL              0 (os)
+                78         380 LOAD_GLOBAL              0 (os)
                            392 LOAD_ATTR                1 (path)
                            402 LOAD_METHOD             10 (join)
                            424 LOAD_FAST                0 (self)
                            426 LOAD_ATTR                3 (input_file)
                            436 LOAD_FAST                2 (file)
                            438 PRECALL                  2
                            442 CALL                     2
                            452 STORE_FAST               3 (file_path)
                
-                77         454 LOAD_GLOBAL              0 (os)
+                79         454 LOAD_GLOBAL              0 (os)
                            466 LOAD_ATTR                1 (path)
                            476 LOAD_METHOD              2 (isfile)
                            498 LOAD_FAST                3 (file_path)
                            500 PRECALL                  1
                            504 CALL                     1
                            514 POP_JUMP_FORWARD_IF_FALSE    21 (to 558)
                
-                78         516 LOAD_FAST                1 (files_to_process)
+                80         516 LOAD_FAST                1 (files_to_process)
                            518 LOAD_METHOD              4 (append)
                            540 LOAD_FAST                3 (file_path)
                            542 PRECALL                  1
                            546 CALL                     1
                            556 POP_TOP
                        >>  558 JUMP_BACKWARD           92 (to 376)
                
-                80     >>  560 LOAD_FAST                1 (files_to_process)
+                82     >>  560 LOAD_FAST                1 (files_to_process)
                            562 RETURN_VALUE
                        >>  564 PUSH_EXC_INFO
                
-                81         566 LOAD_GLOBAL             22 (Exception)
+                83         566 LOAD_GLOBAL             22 (Exception)
                            578 CHECK_EXC_MATCH
                            580 POP_JUMP_FORWARD_IF_FALSE    26 (to 634)
                            582 STORE_FAST               4 (e)
                
-                82         584 LOAD_GLOBAL             15 (NULL + print)
+                84         584 LOAD_GLOBAL             15 (NULL + print)
                            596 LOAD_FAST                4 (e)
                            598 PRECALL                  1
                            602 CALL                     1
                            612 POP_TOP
                            614 POP_EXCEPT
                            616 LOAD_CONST               0 (None)
                            618 STORE_FAST               4 (e)
@@ -534,15 +561,15 @@
                            622 LOAD_CONST               0 (None)
                            624 RETURN_VALUE
                        >>  626 LOAD_CONST               0 (None)
                            628 STORE_FAST               4 (e)
                            630 DELETE_FAST              4 (e)
                            632 RERAISE                  1
                
-                81     >>  634 RERAISE                  0
+                83     >>  634 RERAISE                  0
                        >>  636 COPY                     3
                            638 POP_EXCEPT
                            640 RERAISE                  1
                ExceptionTable:
                  4 to 560 -> 564 [0]
                  564 to 582 -> 636 [1] lasti
                  584 to 612 -> 626 [1] lasti
@@ -551,269 +578,344 @@
                   None
                   'Cannot work with empty folder'
                   1
                names      ('os', 'path', 'isfile', 'input_file', 'append', 'isdir', 'listdir', 'print', 'sys', 'exit', 'join', 'Exception')
                varnames   ('self', 'files_to_process', 'file', 'file_path', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'preprocess'
-               firstlineno 65
+               firstlineno 67
                lnotab
                   0x02010201040248013601480132011e01280136014a013e012c02060112
                   0132ff
             code
                argcount  : 1
-               nlocals   : 6
-               stacksize : 9
+               nlocals   : 7
+               stacksize : 12
                flags     : 3
                code
-                  0x870697007c00a0000000000000000000000000000000000000000000a6
-                  000000ab0000000000000000007d016401640267028a0688066601640384
-                  087c014400a6000000ab0000000000000000007d017c01440090015d617d
+                  0x870797007c00a0000000000000000000000000000000000000000000a6
+                  000000ab0000000000000000007d016401640267028a0788076601640384
+                  087c014400a6000000ab0000000000000000007d017c01440090015dcb7d
                   027c02a0010000000000000000000000000000000000000000a6000000ab
                   000000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab010000000000000000720e7c02640064048502190000
                   0000000000000064057a0000007d036e347c02a001000000000000000000
                   0000000000000000000000a6000000ab000000000000000000a002000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   000000720d7c026400640685021900000000000000000064057a0000007d
-                  0309007407000000000000000000007c02a6010000ab0100000000000000
-                  007d047c04a00400000000000000000000000000000000000000007c03a6
-                  010000ab0100000000000000000100740b00000000000000000000640764
-                  08ac09a6020000ab0200000000000000000100740c000000000000000000
-                  00a0070000000000000000000000000000000000000000640a7c029b0064
-                  0b7c039b00640c9d05a6010000ab01000000000000000001008cc4230074
-                  1000000000000000000000240072260100740b0000000000000000000064
-                  0da6010000ab01000000000000000001007413000000000000000000006a
-                  0a0000000000000000640ea6010000ab010000000000000000010059008c
-                  f37416000000000000000000002400726401000900741800000000000000
-                  0000006a0d0000000000000000640f6b02000000007219741d0000000000
-                  00000000006a0f00000000000000006410641164057c027c036705a60100
-                  00ab01000000000000000001006e35230074160000000000000000000024
-                  0072287d05740c00000000000000000000a0070000000000000000000000
-                  00000000000000000064127c059b00640c9d03a6010000ab010000000000
-                  0000000100590064007d057e056e0864007d057e05770177007803590077
-                  01590090018c5f770078035900770164005300
-                             0 MAKE_CELL                6 (ls)
+                  0309007407000000000000000000007408000000000000000000009b0064
+                  07740a000000000000000000009b007c029b006408740800000000000000
+                  0000009b006409740a000000000000000000009b007c039b009d09a60100
+                  00ab0100000000000000000100740c000000000000000000006a07000000
+                  0000000000640a6b0200000000726e7411000000000000000000006a0900
+                  000000000000006700640ba2017410000000000000000000006a0a000000
+                  0000000000640cac0da6030000ab0300000000000000007d047c046a0b00
+                  00000000000000640e6b0300000000722374070000000000000000000064
+                  0fa6010000ab01000000000000000001007419000000000000000000006a
+                  0d00000000000000006410a6010000ab0100000000000000000100741100
+                  0000000000000000006a0900000000000000006411641264057c027c0367
+                  05a6010000ab01000000000000000001007c03630201005300740c000000
+                  000000000000006a07000000000000000064136b0200000000726e090064
+                  0e64146c0e6d0f7d0501006e332300742000000000000000000000240072
+                  2601007407000000000000000000006415a6010000ab0100000000000000
+                  0001007419000000000000000000006a0d00000000000000006410a60100
+                  00ab010000000000000000010059006e04770078035900770102007c057c
+                  027c03a6020000ab02000000000000000001007407000000000000000000
+                  007422000000000000000000009b0064167c029b0064177c039b00740a00
+                  0000000000000000009b009d06a6010000ab01000000000000000001007c
+                  0363020100530090018c9d2300742400000000000000000000240072237d
+                  0674070000000000000000000064187c029b0064177c039b0064197c069b
+                  009d06a6010000ab0100000000000000000100590064007d067e0690018c
+                  c564007d067e067701770078035900770164005300
+                             0 MAKE_CELL                7 (ls)
                
-                87           2 RESUME                   0
+                89           2 RESUME                   0
                
-                88           4 LOAD_FAST                0 (self)
+                90           4 LOAD_FAST                0 (self)
                              6 LOAD_METHOD              0 (preprocess)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 STORE_FAST               1 (word_list)
                
-                89          44 LOAD_CONST               1 ('doc')
+                91          44 LOAD_CONST               1 ('doc')
                             46 LOAD_CONST               2 ('docx')
                             48 BUILD_LIST               2
-                            50 STORE_DEREF              6 (ls)
+                            50 STORE_DEREF              7 (ls)
                
-                90          52 LOAD_CLOSURE             6 (ls)
+                92          52 LOAD_CLOSURE             7 (ls)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 90>)
+                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 92>)
                             58 MAKE_FUNCTION            8 (closure)
                
-                91          60 LOAD_FAST                1 (word_list)
+                93          60 LOAD_FAST                1 (word_list)
                
-                90          62 GET_ITER
+                92          62 GET_ITER
                             64 PRECALL                  0
                             68 CALL                     0
                             78 STORE_FAST               1 (word_list)
                
-                92          80 LOAD_FAST                1 (word_list)
+                94          80 LOAD_FAST                1 (word_list)
                             82 GET_ITER
                        >>   84 EXTENDED_ARG             1
-                            86 FOR_ITER               353 (to 794)
+                            86 FOR_ITER               459 (to 1006)
                             88 STORE_FAST               2 (word_file)
                
-                93          90 LOAD_FAST                2 (word_file)
+                95          90 LOAD_FAST                2 (word_file)
                             92 LOAD_METHOD              1 (lower)
                            114 PRECALL                  0
                            118 CALL                     0
                            128 LOAD_METHOD              2 (endswith)
                            150 LOAD_CONST               1 ('doc')
                            152 PRECALL                  1
                            156 CALL                     1
                            166 POP_JUMP_FORWARD_IF_FALSE    14 (to 196)
                
-                94         168 LOAD_FAST                2 (word_file)
+                96         168 LOAD_FAST                2 (word_file)
                            170 LOAD_CONST               0 (None)
                            172 LOAD_CONST               4 (-3)
                            174 BUILD_SLICE              2
                            176 BINARY_SUBSCR
                            186 LOAD_CONST               5 ('pdf')
                            188 BINARY_OP                0 (+)
                            192 STORE_FAST               3 (pdf_file)
                            194 JUMP_FORWARD            52 (to 300)
                
-                95     >>  196 LOAD_FAST                2 (word_file)
+                97     >>  196 LOAD_FAST                2 (word_file)
                            198 LOAD_METHOD              1 (lower)
                            220 PRECALL                  0
                            224 CALL                     0
                            234 LOAD_METHOD              2 (endswith)
                            256 LOAD_CONST               2 ('docx')
                            258 PRECALL                  1
                            262 CALL                     1
                            272 POP_JUMP_FORWARD_IF_FALSE    13 (to 300)
                
-                96         274 LOAD_FAST                2 (word_file)
+                98         274 LOAD_FAST                2 (word_file)
                            276 LOAD_CONST               0 (None)
                            278 LOAD_CONST               6 (-4)
                            280 BUILD_SLICE              2
                            282 BINARY_SUBSCR
                            292 LOAD_CONST               5 ('pdf')
                            294 BINARY_OP                0 (+)
                            298 STORE_FAST               3 (pdf_file)
                
-                98     >>  300 NOP
+               100     >>  300 NOP
                
-               100         302 LOAD_GLOBAL              7 (NULL + Document)
-                           314 LOAD_FAST                2 (word_file)
-                           316 PRECALL                  1
-                           320 CALL                     1
-                           330 STORE_FAST               4 (doc)
-               
-               101         332 LOAD_FAST                4 (doc)
-                           334 LOAD_METHOD              4 (save)
-                           356 LOAD_FAST                3 (pdf_file)
-                           358 PRECALL                  1
-                           362 CALL                     1
-                           372 POP_TOP
+               101         302 LOAD_GLOBAL              7 (NULL + print)
                
-               103         374 LOAD_GLOBAL             11 (NULL + print)
-                           386 LOAD_CONST               7 ('\x1b[32mConverting to pdf..\x1b[0m')
-                           388 LOAD_CONST               8 ('\r')
-                           390 KW_NAMES                 9
-                           392 PRECALL                  2
-                           396 CALL                     2
-                           406 POP_TOP
-               
-               105         408 LOAD_GLOBAL             12 (logger)
-                           420 LOAD_METHOD              7 (info)
-                           442 LOAD_CONST              10 ('\x1b[1;95m Successfully converted')
-                           444 LOAD_FAST                2 (word_file)
-                           446 FORMAT_VALUE             0
-                           448 LOAD_CONST              11 (' to ')
+               102         314 LOAD_GLOBAL              8 (BLUE)
+                           326 FORMAT_VALUE             0
+                           328 LOAD_CONST               7 ('Converting: ')
+                           330 LOAD_GLOBAL             10 (RESET)
+                           342 FORMAT_VALUE             0
+                           344 LOAD_FAST                2 (word_file)
+                           346 FORMAT_VALUE             0
+                           348 LOAD_CONST               8 (' ')
+                           350 LOAD_GLOBAL              8 (BLUE)
+                           362 FORMAT_VALUE             0
+                           364 LOAD_CONST               9 ('to ')
+                           366 LOAD_GLOBAL             10 (RESET)
+                           378 FORMAT_VALUE             0
+                           380 LOAD_FAST                3 (pdf_file)
+                           382 FORMAT_VALUE             0
+                           384 BUILD_STRING             9
+               
+               101         386 PRECALL                  1
+                           390 CALL                     1
+                           400 POP_TOP
+               
+               103         402 LOAD_GLOBAL             12 (os)
+                           414 LOAD_ATTR                7 (name)
+                           424 LOAD_CONST              10 ('posix')
+                           426 COMPARE_OP               2 (==)
+                           432 POP_JUMP_FORWARD_IF_FALSE   110 (to 654)
+               
+               105         434 LOAD_GLOBAL             17 (NULL + subprocess)
+                           446 LOAD_ATTR                9 (run)
+               
+               106         456 BUILD_LIST               0
+                           458 LOAD_CONST              11 (('dpkg', '-l', 'libreoffice'))
+                           460 LIST_EXTEND              1
+                           462 LOAD_GLOBAL             16 (subprocess)
+                           474 LOAD_ATTR               10 (PIPE)
+                           484 LOAD_CONST              12 (True)
+               
+               105         486 KW_NAMES                13
+                           488 PRECALL                  3
+                           492 CALL                     3
+                           502 STORE_FAST               4 (result)
+               
+               107         504 LOAD_FAST                4 (result)
+                           506 LOAD_ATTR               11 (returncode)
+                           516 LOAD_CONST              14 (0)
+                           518 COMPARE_OP               3 (!=)
+                           524 POP_JUMP_FORWARD_IF_FALSE    35 (to 596)
                
-               106         450 LOAD_FAST                3 (pdf_file)
+               108         526 LOAD_GLOBAL              7 (NULL + print)
                
-               105         452 FORMAT_VALUE             0
-                           454 LOAD_CONST              12 ('\x1b[0m')
-                           456 BUILD_STRING             5
-                           458 PRECALL                  1
-                           462 CALL                     1
-                           472 POP_TOP
-                           474 JUMP_BACKWARD          196 (to 84)
-                       >>  476 PUSH_EXC_INFO
-               
-               107         478 LOAD_GLOBAL             16 (KeyboardInterrupt)
-                           490 CHECK_EXC_MATCH
-                           492 POP_JUMP_FORWARD_IF_FALSE    38 (to 570)
-                           494 POP_TOP
+               109         538 LOAD_CONST              15 ('Please install libreoffice to use this functionality !')
                
-               108         496 LOAD_GLOBAL             11 (NULL + print)
-                           508 LOAD_CONST              13 ('\nExiting..')
-                           510 PRECALL                  1
-                           514 CALL                     1
-                           524 POP_TOP
-               
-               109         526 LOAD_GLOBAL             19 (NULL + sys)
-                           538 LOAD_ATTR               10 (exit)
-                           548 LOAD_CONST              14 (1)
-                           550 PRECALL                  1
-                           554 CALL                     1
-                           564 POP_TOP
-                           566 POP_EXCEPT
-                           568 JUMP_BACKWARD          243 (to 84)
-               
-               110     >>  570 LOAD_GLOBAL             22 (Exception)
-                           582 CHECK_EXC_MATCH
-                           584 POP_JUMP_FORWARD_IF_FALSE   100 (to 786)
-                           586 POP_TOP
-               
-               111         588 NOP
-               
-               112         590 LOAD_GLOBAL             24 (os)
-                           602 LOAD_ATTR               13 (name)
-                           612 LOAD_CONST              15 ('posix')
-                           614 COMPARE_OP               2 (==)
-                           620 POP_JUMP_FORWARD_IF_FALSE    25 (to 672)
-               
-               113         622 LOAD_GLOBAL             29 (NULL + subprocess)
-                           634 LOAD_ATTR               15 (run)
-                           644 LOAD_CONST              16 ('soffice')
-                           646 LOAD_CONST              17 ('--convert-to')
-               
-               114         648 LOAD_CONST               5 ('pdf')
-                           650 LOAD_FAST                2 (word_file)
-                           652 LOAD_FAST                3 (pdf_file)
+               108         540 PRECALL                  1
+                           544 CALL                     1
+                           554 POP_TOP
                
-               113         654 BUILD_LIST               5
-                           656 PRECALL                  1
-                           660 CALL                     1
-                           670 POP_TOP
-                       >>  672 JUMP_FORWARD            53 (to 780)
-                       >>  674 PUSH_EXC_INFO
+               110         556 LOAD_GLOBAL             25 (NULL + sys)
+                           568 LOAD_ATTR               13 (exit)
+                           578 LOAD_CONST              16 (1)
+                           580 PRECALL                  1
+                           584 CALL                     1
+                           594 POP_TOP
+               
+               111     >>  596 LOAD_GLOBAL             17 (NULL + subprocess)
+                           608 LOAD_ATTR                9 (run)
+                           618 LOAD_CONST              17 ('soffice')
+                           620 LOAD_CONST              18 ('--convert-to')
+               
+               112         622 LOAD_CONST               5 ('pdf')
+                           624 LOAD_FAST                2 (word_file)
+                           626 LOAD_FAST                3 (pdf_file)
+               
+               111         628 BUILD_LIST               5
+                           630 PRECALL                  1
+                           634 CALL                     1
+                           644 POP_TOP
+               
+               113         646 LOAD_FAST                3 (pdf_file)
+                           648 SWAP                     2
+                           650 POP_TOP
+                           652 RETURN_VALUE
                
-               115         676 LOAD_GLOBAL             22 (Exception)
-                           688 CHECK_EXC_MATCH
-                           690 POP_JUMP_FORWARD_IF_FALSE    40 (to 772)
-                           692 STORE_FAST               5 (e)
-               
-               116         694 LOAD_GLOBAL             12 (logger)
-                           706 LOAD_METHOD              7 (info)
-                           728 LOAD_CONST              18 ('\x1b[31mAll conversion attempts have failed: ')
-               
-               117         730 LOAD_FAST                5 (e)
-               
-               116         732 FORMAT_VALUE             0
-                           734 LOAD_CONST              12 ('\x1b[0m')
-                           736 BUILD_STRING             3
-                           738 PRECALL                  1
-                           742 CALL                     1
-                           752 POP_TOP
-                           754 POP_EXCEPT
-                           756 LOAD_CONST               0 (None)
-                           758 STORE_FAST               5 (e)
-                           760 DELETE_FAST              5 (e)
-                           762 JUMP_FORWARD             8 (to 780)
-                       >>  764 LOAD_CONST               0 (None)
-                           766 STORE_FAST               5 (e)
-                           768 DELETE_FAST              5 (e)
-                           770 RERAISE                  1
-               
-               115     >>  772 RERAISE                  0
-                       >>  774 COPY                     3
-                           776 POP_EXCEPT
-                           778 RERAISE                  1
-                       >>  780 POP_EXCEPT
-                           782 EXTENDED_ARG             1
-                           784 JUMP_BACKWARD          351 (to 84)
-               
-               110     >>  786 RERAISE                  0
-                       >>  788 COPY                     3
-                           790 POP_EXCEPT
-                           792 RERAISE                  1
+               115     >>  654 LOAD_GLOBAL             12 (os)
+                           666 LOAD_ATTR                7 (name)
+                           676 LOAD_CONST              19 ('nt')
+                           678 COMPARE_OP               2 (==)
+                           684 POP_JUMP_FORWARD_IF_FALSE   110 (to 906)
+               
+               116         686 NOP
+               
+               117         688 LOAD_CONST              14 (0)
+                           690 LOAD_CONST              20 (('convert',))
+                           692 IMPORT_NAME             14 (docx2pdf)
+                           694 IMPORT_FROM             15 (convert)
+                           696 STORE_FAST               5 (convert)
+                           698 POP_TOP
+                           700 JUMP_FORWARD            51 (to 804)
+                       >>  702 PUSH_EXC_INFO
+               
+               118         704 LOAD_GLOBAL             32 (ImportError)
+                           716 CHECK_EXC_MATCH
+                           718 POP_JUMP_FORWARD_IF_FALSE    38 (to 796)
+                           720 POP_TOP
+               
+               119         722 LOAD_GLOBAL              7 (NULL + print)
+                           734 LOAD_CONST              21 ('Run pip install docx2pdf for this function to work')
+                           736 PRECALL                  1
+                           740 CALL                     1
+                           750 POP_TOP
+               
+               120         752 LOAD_GLOBAL             25 (NULL + sys)
+                           764 LOAD_ATTR               13 (exit)
+                           774 LOAD_CONST              16 (1)
+                           776 PRECALL                  1
+                           780 CALL                     1
+                           790 POP_TOP
+                           792 POP_EXCEPT
+                           794 JUMP_FORWARD             4 (to 804)
+               
+               118     >>  796 RERAISE                  0
+                       >>  798 COPY                     3
+                           800 POP_EXCEPT
+                           802 RERAISE                  1
+               
+               121     >>  804 PUSH_NULL
+                           806 LOAD_FAST                5 (convert)
+                           808 LOAD_FAST                2 (word_file)
+                           810 LOAD_FAST                3 (pdf_file)
+                           812 PRECALL                  2
+                           816 CALL                     2
+                           826 POP_TOP
+               
+               122         828 LOAD_GLOBAL              7 (NULL + print)
+               
+               123         840 LOAD_GLOBAL             34 (DMAGENTA)
+                           852 FORMAT_VALUE             0
+                           854 LOAD_CONST              22 (' Successfully converted ')
+                           856 LOAD_FAST                2 (word_file)
+                           858 FORMAT_VALUE             0
+                           860 LOAD_CONST              23 (' to ')
+                           862 LOAD_FAST                3 (pdf_file)
+                           864 FORMAT_VALUE             0
+                           866 LOAD_GLOBAL             10 (RESET)
+                           878 FORMAT_VALUE             0
+                           880 BUILD_STRING             6
+               
+               122         882 PRECALL                  1
+                           886 CALL                     1
+                           896 POP_TOP
+               
+               124         898 LOAD_FAST                3 (pdf_file)
+                           900 SWAP                     2
+                           902 POP_TOP
+                           904 RETURN_VALUE
+               
+               115     >>  906 EXTENDED_ARG             1
+                           908 JUMP_BACKWARD          413 (to 84)
+                       >>  910 PUSH_EXC_INFO
+               
+               126         912 LOAD_GLOBAL             36 (Exception)
+                           924 CHECK_EXC_MATCH
+                           926 POP_JUMP_FORWARD_IF_FALSE    35 (to 998)
+                           928 STORE_FAST               6 (e)
+               
+               127         930 LOAD_GLOBAL              7 (NULL + print)
+                           942 LOAD_CONST              24 ('Error converting ')
+                           944 LOAD_FAST                2 (word_file)
+                           946 FORMAT_VALUE             0
+                           948 LOAD_CONST              23 (' to ')
+                           950 LOAD_FAST                3 (pdf_file)
+                           952 FORMAT_VALUE             0
+                           954 LOAD_CONST              25 (': ')
+                           956 LOAD_FAST                6 (e)
+                           958 FORMAT_VALUE             0
+                           960 BUILD_STRING             6
+                           962 PRECALL                  1
+                           966 CALL                     1
+                           976 POP_TOP
+                           978 POP_EXCEPT
+                           980 LOAD_CONST               0 (None)
+                           982 STORE_FAST               6 (e)
+                           984 DELETE_FAST              6 (e)
+                           986 EXTENDED_ARG             1
+                           988 JUMP_BACKWARD          453 (to 84)
+                       >>  990 LOAD_CONST               0 (None)
+                           992 STORE_FAST               6 (e)
+                           994 DELETE_FAST              6 (e)
+                           996 RERAISE                  1
+               
+               126     >>  998 RERAISE                  0
+                       >> 1000 COPY                     3
+                          1002 POP_EXCEPT
+                          1004 RERAISE                  1
                
-                92     >>  794 LOAD_CONST               0 (None)
-                           796 RETURN_VALUE
+                94     >> 1006 LOAD_CONST               0 (None)
+                          1008 RETURN_VALUE
                ExceptionTable:
-                 302 to 472 -> 476 [1]
-                 476 to 564 -> 788 [2] lasti
-                 570 to 586 -> 788 [2] lasti
-                 590 to 670 -> 674 [2]
-                 672 to 672 -> 788 [2] lasti
-                 674 to 692 -> 774 [3] lasti
-                 694 to 752 -> 764 [3] lasti
-                 754 to 762 -> 788 [2] lasti
-                 764 to 772 -> 774 [3] lasti
-                 774 to 778 -> 788 [2] lasti
-                 786 to 786 -> 788 [2] lasti
+                 302 to 646 -> 910 [1]
+                 654 to 684 -> 910 [1]
+                 688 to 698 -> 702 [1]
+                 700 to 700 -> 910 [1]
+                 702 to 790 -> 798 [2] lasti
+                 792 to 794 -> 910 [1]
+                 796 to 796 -> 798 [2] lasti
+                 798 to 898 -> 910 [1]
+                 910 to 928 -> 1000 [2] lasti
+                 930 to 976 -> 990 [2] lasti
+                 990 to 998 -> 1000 [2] lasti
                consts
                   None
                   'doc'
                   'docx'
                   code
                      argcount  : 1
                      nlocals   : 1
@@ -822,37 +924,37 @@
                      code
                         0x95018701970067007c005d1f8a01740100000000000000000000880166
                         016400840889024400a6000000ab000000000000000000a6010000ab0100
                         00000000000000af1d890191028c205300
                                    0 COPY_FREE_VARS           1
                                    2 MAKE_CELL                1 (item)
                      
-                      90           4 RESUME                   0
+                      92           4 RESUME                   0
                                    6 BUILD_LIST               0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                31 (to 74)
                      
-                      91          12 STORE_DEREF              1 (item)
+                      93          12 STORE_DEREF              1 (item)
                                   14 LOAD_GLOBAL              1 (NULL + any)
                                   26 LOAD_CLOSURE             1 (item)
                                   28 BUILD_TUPLE              1
-                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 91>)
+                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 93>)
                                   32 MAKE_FUNCTION            8 (closure)
                                   34 LOAD_DEREF               2 (ls)
                                   36 GET_ITER
                                   38 PRECALL                  0
                                   42 CALL                     0
                                   52 PRECALL                  1
                                   56 CALL                     1
                      
-                      90          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
+                      92          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
                      
-                      91          68 LOAD_DEREF               1 (item)
+                      93          68 LOAD_DEREF               1 (item)
                      
-                      90          70 LIST_APPEND              2
+                      92          70 LIST_APPEND              2
                                   72 JUMP_BACKWARD           32 (to 10)
                              >>   74 RETURN_VALUE
                      consts
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
@@ -860,15 +962,15 @@
                            code
                               0x95014b00010097007c005d2b7d018902a0000000000000000000000000
                               000000000000000000a6000000ab000000000000000000a0010000000000
                               0000000000000000000000000000007c01a6010000ab0100000000000000
                               005600970101008c2c64005300
                                          0 COPY_FREE_VARS           1
                            
-                            91           2 RETURN_GENERATOR
+                            93           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                43 (to 98)
                                         12 STORE_FAST               1 (ext)
                                         14 LOAD_DEREF               2 (item)
                                         16 LOAD_METHOD              0 (lower)
@@ -886,227 +988,254 @@
                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('lower', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                            name       '<genexpr>'
-                           firstlineno 91
+                           firstlineno 93
                            lnotab 0x
                      names      ('any',)
                      varnames   ('.0',)
                      freevars   ('ls',)
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 90
+                     firstlineno 92
                      lnotab 0x0c0136ff020102ff
                   -3
                   'pdf'
                   -4
-                  '\x1b[32mConverting to pdf..\x1b[0m'
-                  '\r'
-                  ('end',)
-                  '\x1b[1;95m Successfully converted'
-                  ' to '
-                  '\x1b[0m'
-                  '\nExiting..'
-                  1
+                  'Converting: '
+                  ' '
+                  'to '
                   'posix'
+                  ('dpkg', '-l', 'libreoffice')
+                  True
+                  ('stdout', 'text')
+                  0
+                  'Please install libreoffice to use this functionality !'
+                  1
                   'soffice'
                   '--convert-to'
-                  '\x1b[31mAll conversion attempts have failed: '
-               names      ('preprocess', 'lower', 'endswith', 'Document', 'save', 'print', 'logger', 'info', 'KeyboardInterrupt', 'sys', 'exit', 'Exception', 'os', 'name', 'subprocess', 'run')
-               varnames   ('self', 'word_list', 'word_file', 'pdf_file', 'doc', 'e')
+                  'nt'
+                  ('convert',)
+                  'Run pip install docx2pdf for this function to work'
+                  ' Successfully converted '
+                  ' to '
+                  'Error converting '
+                  ': '
+               names      ('preprocess', 'lower', 'endswith', 'print', 'BLUE', 'RESET', 'os', 'name', 'subprocess', 'run', 'PIPE', 'returncode', 'sys', 'exit', 'docx2pdf', 'convert', 'ImportError', 'DMAGENTA', 'Exception')
+               varnames   ('self', 'word_list', 'word_file', 'pdf_file', 'result', 'convert', 'e')
                freevars   ()
                cellvars   ('ls',)
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'word_to_pdf'
-               firstlineno 87
+               firstlineno 89
                lnotab
-                  0x040128010801080102ff12020a014e011c014e011a0202021e012a0222
-                  022a0102ff1a0212011e012c011201020120011a0106ff16021201240102
-                  ff28ff0efb08ee
+                  0x040128010801080102ff12020a014e011c014e011a0202010c0148ff10
+                  02200216011eff120216010c0102ff100228011a0106ff12020802200102
+                  01100112011e012cfe080318010c012aff100208f7060b120144ff08e0
             code
                argcount  : 1
                nlocals   : 5
-               stacksize : 8
+               stacksize : 9
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d01640184007c014400a6000000ab00000000
-                  00000000007d017c0144005ddf7d027c02a0010000000000000000000000
-                  000000000000000000a6000000ab000000000000000000a0020000000000
-                  0000000000000000000000000000006402a6010000ab0100000000000000
-                  00720d7c026400640385021900000000000000000064047a0000007d0309
-                  007407000000000000000000007c027c0364056400ac06a6040000ab0400
-                  00000000000000010074090000000000000000000064076408ac09a60200
-                  00ab0200000000000000000100740a00000000000000000000a006000000
-                  0000000000000000000000000000000000640a7c029b00640b7c039b0064
-                  0c9d05a6010000ab01000000000000000001008c7d2300740e0000000000
-                  0000000000240072260100740900000000000000000000640da6010000ab
-                  01000000000000000001007411000000000000000000006a090000000000
-                  000000640ea6010000ab010000000000000000010059008cac7414000000
-                  00000000000000240072287d04740a00000000000000000000a006000000
-                  0000000000000000000000000000000000640f7c049b00640c9d03a60100
-                  00ab0100000000000000000100590064007d047e048cd864007d047e0477
-                  01770078035900770164005300
-               122           0 RESUME                   0
+                  00000000007d017c01440090015d097d027c02a001000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000a002000000
+                  00000000000000000000000000000000006402a6010000ab010000000000
+                  000000720d7c026400640385021900000000000000000064047a0000007d
+                  0309007407000000000000000000007c027c0364056400ac06a6040000ab
+                  0400000000000000000100740900000000000000000000740a0000000000
+                  00000000009b006407740c000000000000000000009b009d036408ac09a6
+                  020000ab0200000000000000000100740e00000000000000000000a00800
+                  000000000000000000000000000000000000007412000000000000000000
+                  009b00640a7c029b00640b7c039b00740c000000000000000000009b009d
+                  06a6010000ab01000000000000000001008c9a2300741400000000000000
+                  000000240072260100740900000000000000000000640ca6010000ab0100
+                  0000000000000001007417000000000000000000006a0c00000000000000
+                  00640da6010000ab010000000000000000010059008cc9741a0000000000
+                  0000000000240072367d04740e00000000000000000000a0080000000000
+                  000000000000000000000000000000741c000000000000000000009b0064
+                  0e7c049b00740c000000000000000000009b009d04a6010000ab01000000
+                  00000000000100590064007d047e0490018c0364007d047e047701770078
+                  035900770164005300
+               132           0 RESUME                   0
                
-               123           2 LOAD_FAST                0 (self)
+               133           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (preprocess)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (pdf_list)
                
-               124          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 124>)
+               134          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 134>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                1 (pdf_list)
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               1 (pdf_list)
                
-               125          66 LOAD_FAST                1 (pdf_list)
+               135          66 LOAD_FAST                1 (pdf_list)
                             68 GET_ITER
-                       >>   70 FOR_ITER               223 (to 518)
-                            72 STORE_FAST               2 (pdf_file)
+                       >>   70 EXTENDED_ARG             1
+                            72 FOR_ITER               265 (to 604)
+                            74 STORE_FAST               2 (pdf_file)
                
-               126          74 LOAD_FAST                2 (pdf_file)
-                            76 LOAD_METHOD              1 (lower)
-                            98 PRECALL                  0
-                           102 CALL                     0
-                           112 LOAD_METHOD              2 (endswith)
-                           134 LOAD_CONST               2 ('pdf')
-                           136 PRECALL                  1
-                           140 CALL                     1
-                           150 POP_JUMP_FORWARD_IF_FALSE    13 (to 178)
-               
-               127         152 LOAD_FAST                2 (pdf_file)
-                           154 LOAD_CONST               0 (None)
-                           156 LOAD_CONST               3 (-3)
-                           158 BUILD_SLICE              2
-                           160 BINARY_SUBSCR
-                           170 LOAD_CONST               4 ('docx')
-                           172 BINARY_OP                0 (+)
-                           176 STORE_FAST               3 (word_file)
-               
-               129     >>  178 NOP
-               
-               131         180 LOAD_GLOBAL              7 (NULL + parse)
-                           192 LOAD_FAST                2 (pdf_file)
-                           194 LOAD_FAST                3 (word_file)
-                           196 LOAD_CONST               5 (0)
-                           198 LOAD_CONST               0 (None)
-                           200 KW_NAMES                 6
-                           202 PRECALL                  4
-                           206 CALL                     4
-                           216 POP_TOP
+               136          76 LOAD_FAST                2 (pdf_file)
+                            78 LOAD_METHOD              1 (lower)
+                           100 PRECALL                  0
+                           104 CALL                     0
+                           114 LOAD_METHOD              2 (endswith)
+                           136 LOAD_CONST               2 ('pdf')
+                           138 PRECALL                  1
+                           142 CALL                     1
+                           152 POP_JUMP_FORWARD_IF_FALSE    13 (to 180)
                
-               133         218 LOAD_GLOBAL              9 (NULL + print)
-                           230 LOAD_CONST               7 ('\x1b[32mConverting to word..\x1b[0m')
-                           232 LOAD_CONST               8 ('\r')
-                           234 KW_NAMES                 9
-                           236 PRECALL                  2
-                           240 CALL                     2
-                           250 POP_TOP
-               
-               135         252 LOAD_GLOBAL             10 (logger)
-                           264 LOAD_METHOD              6 (info)
-                           286 LOAD_CONST              10 ('\x1b[1;95m Successfully converted')
-                           288 LOAD_FAST                2 (pdf_file)
-                           290 FORMAT_VALUE             0
-                           292 LOAD_CONST              11 (' to ')
-               
-               136         294 LOAD_FAST                3 (word_file)
-               
-               135         296 FORMAT_VALUE             0
-                           298 LOAD_CONST              12 ('\x1b[0m')
-                           300 BUILD_STRING             5
-                           302 PRECALL                  1
-                           306 CALL                     1
-                           316 POP_TOP
-                           318 JUMP_BACKWARD          125 (to 70)
-                       >>  320 PUSH_EXC_INFO
+               137         154 LOAD_FAST                2 (pdf_file)
+                           156 LOAD_CONST               0 (None)
+                           158 LOAD_CONST               3 (-3)
+                           160 BUILD_SLICE              2
+                           162 BINARY_SUBSCR
+                           172 LOAD_CONST               4 ('docx')
+                           174 BINARY_OP                0 (+)
+                           178 STORE_FAST               3 (word_file)
                
-               137         322 LOAD_GLOBAL             14 (KeyboardInterrupt)
-                           334 CHECK_EXC_MATCH
-                           336 POP_JUMP_FORWARD_IF_FALSE    38 (to 414)
-                           338 POP_TOP
+               139     >>  180 NOP
                
-               138         340 LOAD_GLOBAL              9 (NULL + print)
-                           352 LOAD_CONST              13 ('\nExiting..')
-                           354 PRECALL                  1
-                           358 CALL                     1
-                           368 POP_TOP
+               141         182 LOAD_GLOBAL              7 (NULL + parse)
+                           194 LOAD_FAST                2 (pdf_file)
+                           196 LOAD_FAST                3 (word_file)
+                           198 LOAD_CONST               5 (0)
+                           200 LOAD_CONST               0 (None)
+                           202 KW_NAMES                 6
+                           204 PRECALL                  4
+                           208 CALL                     4
+                           218 POP_TOP
                
-               139         370 LOAD_GLOBAL             17 (NULL + sys)
-                           382 LOAD_ATTR                9 (exit)
-                           392 LOAD_CONST              14 (1)
-                           394 PRECALL                  1
-                           398 CALL                     1
-                           408 POP_TOP
-                           410 POP_EXCEPT
-                           412 JUMP_BACKWARD          172 (to 70)
+               143         220 LOAD_GLOBAL              9 (NULL + print)
+                           232 LOAD_GLOBAL             10 (GREEN)
+                           244 FORMAT_VALUE             0
+                           246 LOAD_CONST               7 ('Converting to word..')
+                           248 LOAD_GLOBAL             12 (RESET)
+                           260 FORMAT_VALUE             0
+                           262 BUILD_STRING             3
+                           264 LOAD_CONST               8 ('\r')
+                           266 KW_NAMES                 9
+                           268 PRECALL                  2
+                           272 CALL                     2
+                           282 POP_TOP
+               
+               145         284 LOAD_GLOBAL             14 (logger)
+                           296 LOAD_METHOD              8 (info)
+                           318 LOAD_GLOBAL             18 (DMAGENTA)
+                           330 FORMAT_VALUE             0
+                           332 LOAD_CONST              10 (' Successfully converted')
+                           334 LOAD_FAST                2 (pdf_file)
+                           336 FORMAT_VALUE             0
+                           338 LOAD_CONST              11 (' to ')
+               
+               146         340 LOAD_FAST                3 (word_file)
                
-               140     >>  414 LOAD_GLOBAL             20 (Exception)
-                           426 CHECK_EXC_MATCH
-                           428 POP_JUMP_FORWARD_IF_FALSE    40 (to 510)
-                           430 STORE_FAST               4 (e)
-               
-               141         432 LOAD_GLOBAL             10 (logger)
-                           444 LOAD_METHOD              6 (info)
-                           466 LOAD_CONST              15 ('\x1b[31mAll conversion attempts have failed: ')
-               
-               142         468 LOAD_FAST                4 (e)
-               
-               141         470 FORMAT_VALUE             0
-                           472 LOAD_CONST              12 ('\x1b[0m')
-                           474 BUILD_STRING             3
-                           476 PRECALL                  1
-                           480 CALL                     1
-                           490 POP_TOP
-                           492 POP_EXCEPT
-                           494 LOAD_CONST               0 (None)
-                           496 STORE_FAST               4 (e)
-                           498 DELETE_FAST              4 (e)
-                           500 JUMP_BACKWARD          216 (to 70)
-                       >>  502 LOAD_CONST               0 (None)
-                           504 STORE_FAST               4 (e)
-                           506 DELETE_FAST              4 (e)
-                           508 RERAISE                  1
-               
-               140     >>  510 RERAISE                  0
-                       >>  512 COPY                     3
-                           514 POP_EXCEPT
-                           516 RERAISE                  1
+               145         342 FORMAT_VALUE             0
                
-               125     >>  518 LOAD_CONST               0 (None)
-                           520 RETURN_VALUE
+               146         344 LOAD_GLOBAL             12 (RESET)
+               
+               145         356 FORMAT_VALUE             0
+                           358 BUILD_STRING             6
+                           360 PRECALL                  1
+                           364 CALL                     1
+                           374 POP_TOP
+                           376 JUMP_BACKWARD          154 (to 70)
+                       >>  378 PUSH_EXC_INFO
+               
+               147         380 LOAD_GLOBAL             20 (KeyboardInterrupt)
+                           392 CHECK_EXC_MATCH
+                           394 POP_JUMP_FORWARD_IF_FALSE    38 (to 472)
+                           396 POP_TOP
+               
+               148         398 LOAD_GLOBAL              9 (NULL + print)
+                           410 LOAD_CONST              12 ('\nExiting..')
+                           412 PRECALL                  1
+                           416 CALL                     1
+                           426 POP_TOP
+               
+               149         428 LOAD_GLOBAL             23 (NULL + sys)
+                           440 LOAD_ATTR               12 (exit)
+                           450 LOAD_CONST              13 (1)
+                           452 PRECALL                  1
+                           456 CALL                     1
+                           466 POP_TOP
+                           468 POP_EXCEPT
+                           470 JUMP_BACKWARD          201 (to 70)
+               
+               150     >>  472 LOAD_GLOBAL             26 (Exception)
+                           484 CHECK_EXC_MATCH
+                           486 POP_JUMP_FORWARD_IF_FALSE    54 (to 596)
+                           488 STORE_FAST               4 (e)
+               
+               151         490 LOAD_GLOBAL             14 (logger)
+                           502 LOAD_METHOD              8 (info)
+                           524 LOAD_GLOBAL             28 (DRED)
+                           536 FORMAT_VALUE             0
+                           538 LOAD_CONST              14 ('All conversion attempts have failed: ')
+               
+               152         540 LOAD_FAST                4 (e)
+               
+               151         542 FORMAT_VALUE             0
+               
+               152         544 LOAD_GLOBAL             12 (RESET)
+               
+               151         556 FORMAT_VALUE             0
+                           558 BUILD_STRING             4
+                           560 PRECALL                  1
+                           564 CALL                     1
+                           574 POP_TOP
+                           576 POP_EXCEPT
+                           578 LOAD_CONST               0 (None)
+                           580 STORE_FAST               4 (e)
+                           582 DELETE_FAST              4 (e)
+                           584 EXTENDED_ARG             1
+                           586 JUMP_BACKWARD          259 (to 70)
+                       >>  588 LOAD_CONST               0 (None)
+                           590 STORE_FAST               4 (e)
+                           592 DELETE_FAST              4 (e)
+                           594 RERAISE                  1
+               
+               150     >>  596 RERAISE                  0
+                       >>  598 COPY                     3
+                           600 POP_EXCEPT
+                           602 RERAISE                  1
+               
+               135     >>  604 LOAD_CONST               0 (None)
+                           606 RETURN_VALUE
                ExceptionTable:
-                 180 to 316 -> 320 [1]
-                 320 to 408 -> 512 [2] lasti
-                 414 to 430 -> 512 [2] lasti
-                 432 to 490 -> 502 [2] lasti
-                 502 to 510 -> 512 [2] lasti
+                 182 to 374 -> 378 [1]
+                 378 to 466 -> 598 [2] lasti
+                 472 to 488 -> 598 [2] lasti
+                 490 to 574 -> 588 [2] lasti
+                 588 to 596 -> 598 [2] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d2b7d017c01a000000000000000000000000000000000
                         0000000000a6000000ab000000000000000000a001000000000000000000
                         00000000000000000000006400a6010000ab010000000000000000af297c
                         0191028c2c5300
-                     124           0 RESUME                   0
+                     134           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                43 (to 94)
                                    8 STORE_FAST               1 (item)
                                   10 LOAD_FAST                1 (item)
                                   12 LOAD_METHOD              0 (lower)
                                   34 PRECALL                  0
@@ -1122,42 +1251,41 @@
                              >>   94 RETURN_VALUE
                      consts
                         'pdf'
                      names      ('lower', 'endswith')
                      varnames   ('.0', 'item')
                      freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 124
+                     firstlineno 134
                      lnotab 0x
                   'pdf'
                   -3
                   'docx'
                   0
                   ('start', 'end')
-                  '\x1b[32mConverting to word..\x1b[0m'
+                  'Converting to word..'
                   '\r'
                   ('end',)
-                  '\x1b[1;95m Successfully converted'
+                  ' Successfully converted'
                   ' to '
-                  '\x1b[0m'
                   '\nExiting..'
                   1
-                  '\x1b[31mAll conversion attempts have failed: '
-               names      ('preprocess', 'lower', 'endswith', 'parse', 'print', 'logger', 'info', 'KeyboardInterrupt', 'sys', 'exit', 'Exception')
+                  'All conversion attempts have failed: '
+               names      ('preprocess', 'lower', 'endswith', 'parse', 'print', 'GREEN', 'RESET', 'logger', 'info', 'DMAGENTA', 'KeyboardInterrupt', 'sys', 'exit', 'Exception', 'DRED')
                varnames   ('self', 'pdf_list', 'pdf_file', 'word_file', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'pdf_to_word'
-               firstlineno 122
+               firstlineno 132
                lnotab
-                  0x02012801180108014e011a020202260222022a0102ff1a0212011e012c
-                  011201240102ff28ff08f1
+                  0x0201280118010a014e011a02020226024002380102ff02010cff180212
+                  011e012c011201320102ff02010cff28ff08f1
             code
                argcount  : 2
                nlocals   : 7
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000007c0064016402ac03a6030000ab0300
@@ -1168,33 +1296,33 @@
                   000000ac05a6020000ab0200000000000000007d0467007d057c0344005d
                   387d067c05a0040000000000000000000000000000000000000000740b00
                   0000000000000000007c06a0060000000000000000000000000000000000
                   000000a6000000ab0000000000000000006406ac07a6020000ab02000000
                   0000000000a6010000ab01000000000000000001008c397c04a007000000
                   00000000000000000000000000000000007c05a6010000ab010000000000
                   000000010064045300
-               147           0 RESUME                   0
+               157           0 RESUME                   0
                
-               151           2 LOAD_GLOBAL              1 (NULL + open)
+               161           2 LOAD_GLOBAL              1 (NULL + open)
                             14 LOAD_FAST                0 (input_file)
                             16 LOAD_CONST               1 ('r')
                             18 LOAD_CONST               2 ('utf-8')
                             20 KW_NAMES                 3
                             22 PRECALL                  3
                             26 CALL                     3
                             36 BEFORE_WITH
                             38 STORE_FAST               2 (file)
                
-               152          40 LOAD_FAST                2 (file)
+               162          40 LOAD_FAST                2 (file)
                             42 LOAD_METHOD              1 (readlines)
                             64 PRECALL                  0
                             68 CALL                     0
                             78 STORE_FAST               3 (text_contents)
                
-               151          80 LOAD_CONST               4 (None)
+               161          80 LOAD_CONST               4 (None)
                             82 LOAD_CONST               4 (None)
                             84 LOAD_CONST               4 (None)
                             86 PRECALL                  2
                             90 CALL                     2
                            100 POP_TOP
                            102 JUMP_FORWARD            11 (to 126)
                        >>  104 PUSH_EXC_INFO
@@ -1205,31 +1333,31 @@
                            114 POP_EXCEPT
                            116 RERAISE                  1
                        >>  118 POP_TOP
                            120 POP_EXCEPT
                            122 POP_TOP
                            124 POP_TOP
                
-               155     >>  126 LOAD_GLOBAL              5 (NULL + SimpleDocTemplate)
+               165     >>  126 LOAD_GLOBAL              5 (NULL + SimpleDocTemplate)
                            138 LOAD_FAST                1 (output_file)
                            140 LOAD_GLOBAL              6 (letter)
                            152 KW_NAMES                 5
                            154 PRECALL                  2
                            158 CALL                     2
                            168 STORE_FAST               4 (doc)
                
-               158         170 BUILD_LIST               0
+               168         170 BUILD_LIST               0
                            172 STORE_FAST               5 (story)
                
-               161         174 LOAD_FAST                3 (text_contents)
+               171         174 LOAD_FAST                3 (text_contents)
                            176 GET_ITER
                        >>  178 FOR_ITER                56 (to 292)
                            180 STORE_FAST               6 (line)
                
-               162         182 LOAD_FAST                5 (story)
+               172         182 LOAD_FAST                5 (story)
                            184 LOAD_METHOD              4 (append)
                            206 LOAD_GLOBAL             11 (NULL + Paragraph)
                            218 LOAD_FAST                6 (line)
                            220 LOAD_METHOD              6 (strip)
                            242 PRECALL                  0
                            246 CALL                     0
                            256 LOAD_CONST               6 ('normalText')
@@ -1237,15 +1365,15 @@
                            260 PRECALL                  2
                            264 CALL                     2
                            274 PRECALL                  1
                            278 CALL                     1
                            288 POP_TOP
                            290 JUMP_BACKWARD           57 (to 178)
                
-               165     >>  292 LOAD_FAST                4 (doc)
+               175     >>  292 LOAD_FAST                4 (doc)
                            294 LOAD_METHOD              7 (build)
                            316 LOAD_FAST                5 (story)
                            318 PRECALL                  1
                            322 CALL                     1
                            332 POP_TOP
                            334 LOAD_CONST               4 (None)
                            336 RETURN_VALUE
@@ -1262,1114 +1390,1193 @@
                   ('pagesize',)
                   'normalText'
                   ('style',)
                names      ('open', 'readlines', 'SimpleDocTemplate', 'letter', 'append', 'Paragraph', 'strip', 'build')
                varnames   ('input_file', 'output_file', 'file', 'text_contents', 'doc', 'story', 'line')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'txt_to_pdf'
-               firstlineno 147
+               firstlineno 157
                lnotab 0x0204260128ff2e042c03040308016e03
             code
                argcount  : 1
                nlocals   : 11
-               stacksize : 7
+               stacksize : 10
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d01640184007c014400a6000000ab00000000
-                  00000000007d017c01440090025d227d027c018023740300000000000000
+                  00000000007d017c01440090025d7a7d027c018023740300000000000000
                   0000006402a6010000ab0100000000000000000100740500000000000000
                   0000006a0300000000000000006403a6010000ab01000000000000000001
                   007c02a0040000000000000000000000000000000000000000a6000000ab
                   000000000000000000a00500000000000000000000000000000000000000
                   006404a6010000ab010000000000000000720e7c02640064058502190000
                   0000000000000064067a0000007d036e347c02a004000000000000000000
                   0000000000000000000000a6000000ab000000000000000000a005000000
                   00000000000000000000000000000000006407a6010000ab010000000000
                   000000720d7c026400640885021900000000000000000064067a0000007d
-                  0309007403000000000000000000006409a6010000ab0100000000000000
-                  000100740d000000000000000000007c02a6010000ab0100000000000000
-                  007d04740300000000000000000000640aa6010000ab0100000000000000
-                  000100740f00000000000000000000a6000000ab0000000000000000007d
-                  05740300000000000000000000640b7411000000000000000000007c046a
-                  090000000000000000a6010000ab0100000000000000009b00640c9d03a6
-                  010000ab0100000000000000000100640d7d067c046a0900000000000000
-                  0044005d727d077c0664037a0d00007d067c067411000000000000000000
-                  007c046a090000000000000000a6010000ab0100000000000000007a0b00
-                  00640e7a0500007d08740300000000000000000000640f7c0864109b0464
-                  119d036412ac13a6020000ab02000000000000000001007c056a0a000000
-                  0000000000a00b00000000000000000000000000000000000000007c056a
-                  0c0000000000000000640319000000000000000000a6010000ab01000000
-                  00000000007d097c076a0d00000000000000007c096a0e00000000000000
-                  006a0f00000000000000005f0d00000000000000008c737c05a010000000
-                  00000000000000000000000000000000007c03a6010000ab010000000000
-                  00000001007403000000000000000000006414a6010000ab010000000000
-                  000000010090018c94230074220000000000000000000024007227010074
-                  03000000000000000000006415a6010000ab010000000000000000010074
+                  030900740300000000000000000000740c000000000000000000009b0064
+                  09740e000000000000000000009b009d03a6010000ab0100000000000000
+                  0001007411000000000000000000007c02a6010000ab0100000000000000
+                  007d04740300000000000000000000740c000000000000000000009b0064
+                  0a740e000000000000000000009b009d03a6010000ab0100000000000000
+                  000100741300000000000000000000a6000000ab0000000000000000007d
+                  057403000000000000000000007414000000000000000000009b00640b74
+                  0c000000000000000000009b007417000000000000000000007c046a0c00
+                  00000000000000a6010000ab0100000000000000009b0074140000000000
+                  00000000009b00640c740e000000000000000000009b009d07a6010000ab
+                  0100000000000000000100640d7d067c046a0c000000000000000044005d
+                  807d077c0664037a0d00007d067c067417000000000000000000007c046a
+                  0c0000000000000000a6010000ab0100000000000000007a0b0000640e7a
+                  0500007d08740300000000000000000000741a000000000000000000009b
+                  00640f7c0864109b046411740e000000000000000000009b009d056412ac
+                  13a6020000ab02000000000000000001007c056a0e0000000000000000a0
+                  0f00000000000000000000000000000000000000007c056a100000000000
+                  000000640319000000000000000000a6010000ab0100000000000000007d
+                  097c076a1100000000000000007c096a1200000000000000006a13000000
+                  00000000005f1100000000000000008c817c05a014000000000000000000
+                  00000000000000000000007c03a6010000ab010000000000000000010074
+                  030000000000000000000064147414000000000000000000009b00641574
+                  0e000000000000000000009b009d04a6010000ab01000000000000000001
+                  0090018cec2300742a000000000000000000002400722701007403000000
+                  000000000000006416a6010000ab01000000000000000001007405000000
+                  000000000000006a0300000000000000006403a6010000ab010000000000
+                  0000000100590090028c1c742a0000000000000000000024007227010074
+                  03000000000000000000006417a6010000ab010000000000000000010074
                   05000000000000000000006a0300000000000000006403a6010000ab0100
-                  000000000000000100590090018cc4742200000000000000000000240072
-                  2701007403000000000000000000006416a6010000ab0100000000000000
-                  0001007405000000000000000000006a0300000000000000006403a60100
-                  00ab0100000000000000000100590090018cf37424000000000000000000
-                  00240072257d0a742600000000000000000000a014000000000000000000
-                  00000000000000000000007c0aa6010000ab010000000000000000010059
-                  0064007d0a7e0a90028c1c64007d0a7e0a77017700780359007701640053
-                  00
-               170           0 RESUME                   0
+                  000000000000000100590090028c4b742c00000000000000000000240072
+                  257d0a742e00000000000000000000a01800000000000000000000000000
+                  000000000000007c0aa6010000ab0100000000000000000100590064007d
+                  0a7e0a90028c7464007d0a7e0a7701770078035900770164005300
+               180           0 RESUME                   0
                
-               171           2 LOAD_FAST                0 (self)
+               181           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (preprocess)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (word_list)
                
-               172          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 172>)
+               182          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 182>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                1 (word_list)
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               1 (word_list)
                
-               175          66 LOAD_FAST                1 (word_list)
+               185          66 LOAD_FAST                1 (word_list)
                             68 GET_ITER
                        >>   70 EXTENDED_ARG             2
-                            72 FOR_ITER               546 (to 1166)
+                            72 FOR_ITER               634 (to 1342)
                             74 STORE_FAST               2 (word_file)
                
-               177          76 LOAD_FAST                1 (word_list)
+               187          76 LOAD_FAST                1 (word_list)
                             78 POP_JUMP_FORWARD_IF_NOT_NONE    35 (to 150)
                
-               178          80 LOAD_GLOBAL              3 (NULL + print)
+               188          80 LOAD_GLOBAL              3 (NULL + print)
                             92 LOAD_CONST               2 ('Please provide appropriate file type')
                             94 PRECALL                  1
                             98 CALL                     1
                            108 POP_TOP
                
-               179         110 LOAD_GLOBAL              5 (NULL + sys)
+               189         110 LOAD_GLOBAL              5 (NULL + sys)
                            122 LOAD_ATTR                3 (exit)
                            132 LOAD_CONST               3 (1)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 POP_TOP
                
-               180     >>  150 LOAD_FAST                2 (word_file)
+               190     >>  150 LOAD_FAST                2 (word_file)
                            152 LOAD_METHOD              4 (lower)
                            174 PRECALL                  0
                            178 CALL                     0
                            188 LOAD_METHOD              5 (endswith)
                            210 LOAD_CONST               4 ('docx')
                            212 PRECALL                  1
                            216 CALL                     1
                            226 POP_JUMP_FORWARD_IF_FALSE    14 (to 256)
                
-               181         228 LOAD_FAST                2 (word_file)
+               191         228 LOAD_FAST                2 (word_file)
                            230 LOAD_CONST               0 (None)
                            232 LOAD_CONST               5 (-4)
                            234 BUILD_SLICE              2
                            236 BINARY_SUBSCR
                            246 LOAD_CONST               6 ('pptx')
                            248 BINARY_OP                0 (+)
                            252 STORE_FAST               3 (pptx_file)
                            254 JUMP_FORWARD            52 (to 360)
                
-               182     >>  256 LOAD_FAST                2 (word_file)
+               192     >>  256 LOAD_FAST                2 (word_file)
                            258 LOAD_METHOD              4 (lower)
                            280 PRECALL                  0
                            284 CALL                     0
                            294 LOAD_METHOD              5 (endswith)
                            316 LOAD_CONST               7 ('doc')
                            318 PRECALL                  1
                            322 CALL                     1
                            332 POP_JUMP_FORWARD_IF_FALSE    13 (to 360)
                
-               183         334 LOAD_FAST                2 (word_file)
+               193         334 LOAD_FAST                2 (word_file)
                            336 LOAD_CONST               0 (None)
                            338 LOAD_CONST               8 (-3)
                            340 BUILD_SLICE              2
                            342 BINARY_SUBSCR
                            352 LOAD_CONST               6 ('pptx')
                            354 BINARY_OP                0 (+)
                            358 STORE_FAST               3 (pptx_file)
                
-               184     >>  360 NOP
-               
-               186         362 LOAD_GLOBAL              3 (NULL + print)
-                           374 LOAD_CONST               9 ('\x1b[1;33mLoad the Word document..\x1b[0m')
-                           376 PRECALL                  1
-                           380 CALL                     1
-                           390 POP_TOP
+               194     >>  360 NOP
                
-               187         392 LOAD_GLOBAL             13 (NULL + Document)
-                           404 LOAD_FAST                2 (word_file)
+               196         362 LOAD_GLOBAL              3 (NULL + print)
+                           374 LOAD_GLOBAL             12 (DYELLOW)
+                           386 FORMAT_VALUE             0
+                           388 LOAD_CONST               9 ('Load the Word document..')
+                           390 LOAD_GLOBAL             14 (RESET)
+                           402 FORMAT_VALUE             0
+                           404 BUILD_STRING             3
                            406 PRECALL                  1
                            410 CALL                     1
-                           420 STORE_FAST               4 (doc)
+                           420 POP_TOP
                
-               190         422 LOAD_GLOBAL              3 (NULL + print)
-                           434 LOAD_CONST              10 ('\x1b[1;33mCreate a new PowerPoint presentation..\x1b[0m')
+               197         422 LOAD_GLOBAL             17 (NULL + Document)
+                           434 LOAD_FAST                2 (word_file)
                            436 PRECALL                  1
                            440 CALL                     1
-                           450 POP_TOP
+                           450 STORE_FAST               4 (doc)
                
-               191         452 LOAD_GLOBAL             15 (NULL + Presentation)
-                           464 PRECALL                  0
-                           468 CALL                     0
-                           478 STORE_FAST               5 (prs)
-               
-               194         480 LOAD_GLOBAL              3 (NULL + print)
-               
-               195         492 LOAD_CONST              11 ('\x1b[1;32mPopulating pptx slides with \x1b[1;33m')
-                           494 LOAD_GLOBAL             17 (NULL + len)
-                           506 LOAD_FAST                4 (doc)
-                           508 LOAD_ATTR                9 (paragraphs)
-                           518 PRECALL                  1
-                           522 CALL                     1
-                           532 FORMAT_VALUE             0
-                           534 LOAD_CONST              12 ('\x1b[1;32m entries..\x1b[0m')
-                           536 BUILD_STRING             3
-               
-               194         538 PRECALL                  1
-                           542 CALL                     1
-                           552 POP_TOP
-               
-               196         554 LOAD_CONST              13 (0)
-                           556 STORE_FAST               6 (count)
-               
-               197         558 LOAD_FAST                4 (doc)
-                           560 LOAD_ATTR                9 (paragraphs)
-                           570 GET_ITER
-                       >>  572 FOR_ITER               114 (to 802)
-                           574 STORE_FAST               7 (paragraph)
-               
-               198         576 LOAD_FAST                6 (count)
-                           578 LOAD_CONST               3 (1)
-                           580 BINARY_OP               13 (+=)
-                           584 STORE_FAST               6 (count)
-               
-               199         586 LOAD_FAST                6 (count)
-                           588 LOAD_GLOBAL             17 (NULL + len)
-                           600 LOAD_FAST                4 (doc)
-                           602 LOAD_ATTR                9 (paragraphs)
-                           612 PRECALL                  1
-                           616 CALL                     1
-                           626 BINARY_OP               11 (/)
-                           630 LOAD_CONST              14 (100)
-                           632 BINARY_OP                5 (*)
-                           636 STORE_FAST               8 (perc)
-               
-               200         638 LOAD_GLOBAL              3 (NULL + print)
-               
-               201         650 LOAD_CONST              15 ('\x1b[1;35mProgress:: \x1b[1;36m')
-                           652 LOAD_FAST                8 (perc)
-                           654 LOAD_CONST              16 ('.2f')
-                           656 FORMAT_VALUE             4 (with format)
-                           658 LOAD_CONST              17 ('%\x1b[0m')
-                           660 BUILD_STRING             3
-                           662 LOAD_CONST              18 ('\r')
-               
-               200         664 KW_NAMES                19
-                           666 PRECALL                  2
-                           670 CALL                     2
-                           680 POP_TOP
+               200         452 LOAD_GLOBAL              3 (NULL + print)
+                           464 LOAD_GLOBAL             12 (DYELLOW)
+                           476 FORMAT_VALUE             0
+                           478 LOAD_CONST              10 ('Create a new PowerPoint presentation..')
+                           480 LOAD_GLOBAL             14 (RESET)
+                           492 FORMAT_VALUE             0
+                           494 BUILD_STRING             3
+                           496 PRECALL                  1
+                           500 CALL                     1
+                           510 POP_TOP
+               
+               201         512 LOAD_GLOBAL             19 (NULL + Presentation)
+                           524 PRECALL                  0
+                           528 CALL                     0
+                           538 STORE_FAST               5 (prs)
                
-               203         682 LOAD_FAST                5 (prs)
-                           684 LOAD_ATTR               10 (slides)
-                           694 LOAD_METHOD             11 (add_slide)
-                           716 LOAD_FAST                5 (prs)
-                           718 LOAD_ATTR               12 (slide_layouts)
-                           728 LOAD_CONST               3 (1)
-                           730 BINARY_SUBSCR
-                           740 PRECALL                  1
-                           744 CALL                     1
-                           754 STORE_FAST               9 (slide)
+               204         540 LOAD_GLOBAL              3 (NULL + print)
                
-               206         756 LOAD_FAST                7 (paragraph)
-                           758 LOAD_ATTR               13 (text)
-                           768 LOAD_FAST                9 (slide)
-                           770 LOAD_ATTR               14 (shapes)
-                           780 LOAD_ATTR               15 (title)
-                           790 STORE_ATTR              13 (text)
-                           800 JUMP_BACKWARD          115 (to 572)
-               
-               209     >>  802 LOAD_FAST                5 (prs)
-                           804 LOAD_METHOD             16 (save)
-                           826 LOAD_FAST                3 (pptx_file)
-                           828 PRECALL                  1
-                           832 CALL                     1
-                           842 POP_TOP
-               
-               210         844 LOAD_GLOBAL              3 (NULL + print)
-                           856 LOAD_CONST              20 ('\n\x1b[1;32mDone\x1b[0m')
-                           858 PRECALL                  1
-                           862 CALL                     1
-                           872 POP_TOP
-                           874 EXTENDED_ARG             1
-                           876 JUMP_BACKWARD          404 (to 70)
-                       >>  878 PUSH_EXC_INFO
-               
-               211         880 LOAD_GLOBAL             34 (KeyboardInterrupt)
-                           892 CHECK_EXC_MATCH
-                           894 POP_JUMP_FORWARD_IF_FALSE    39 (to 974)
-                           896 POP_TOP
+               205         552 LOAD_GLOBAL             20 (DGREEN)
+                           564 FORMAT_VALUE             0
+                           566 LOAD_CONST              11 ('Populating pptx slides with ')
+                           568 LOAD_GLOBAL             12 (DYELLOW)
+                           580 FORMAT_VALUE             0
+                           582 LOAD_GLOBAL             23 (NULL + len)
+                           594 LOAD_FAST                4 (doc)
+                           596 LOAD_ATTR               12 (paragraphs)
+                           606 PRECALL                  1
+                           610 CALL                     1
+                           620 FORMAT_VALUE             0
+                           622 LOAD_GLOBAL             20 (DGREEN)
+                           634 FORMAT_VALUE             0
+                           636 LOAD_CONST              12 (' entries..')
+                           638 LOAD_GLOBAL             14 (RESET)
+                           650 FORMAT_VALUE             0
+                           652 BUILD_STRING             7
+               
+               204         654 PRECALL                  1
+                           658 CALL                     1
+                           668 POP_TOP
+               
+               206         670 LOAD_CONST              13 (0)
+                           672 STORE_FAST               6 (count)
+               
+               207         674 LOAD_FAST                4 (doc)
+                           676 LOAD_ATTR               12 (paragraphs)
+                           686 GET_ITER
+                       >>  688 FOR_ITER               128 (to 946)
+                           690 STORE_FAST               7 (paragraph)
+               
+               208         692 LOAD_FAST                6 (count)
+                           694 LOAD_CONST               3 (1)
+                           696 BINARY_OP               13 (+=)
+                           700 STORE_FAST               6 (count)
+               
+               209         702 LOAD_FAST                6 (count)
+                           704 LOAD_GLOBAL             23 (NULL + len)
+                           716 LOAD_FAST                4 (doc)
+                           718 LOAD_ATTR               12 (paragraphs)
+                           728 PRECALL                  1
+                           732 CALL                     1
+                           742 BINARY_OP               11 (/)
+                           746 LOAD_CONST              14 (100)
+                           748 BINARY_OP                5 (*)
+                           752 STORE_FAST               8 (perc)
+               
+               210         754 LOAD_GLOBAL              3 (NULL + print)
+               
+               211         766 LOAD_GLOBAL             26 (DMAGENTA)
+                           778 FORMAT_VALUE             0
+                           780 LOAD_CONST              15 ('Progress:: \x1b[1;36m')
+                           782 LOAD_FAST                8 (perc)
+                           784 LOAD_CONST              16 ('.2f')
+                           786 FORMAT_VALUE             4 (with format)
+                           788 LOAD_CONST              17 ('%')
+                           790 LOAD_GLOBAL             14 (RESET)
+                           802 FORMAT_VALUE             0
+                           804 BUILD_STRING             5
+                           806 LOAD_CONST              18 ('\r')
+               
+               210         808 KW_NAMES                19
+                           810 PRECALL                  2
+                           814 CALL                     2
+                           824 POP_TOP
+               
+               213         826 LOAD_FAST                5 (prs)
+                           828 LOAD_ATTR               14 (slides)
+                           838 LOAD_METHOD             15 (add_slide)
+                           860 LOAD_FAST                5 (prs)
+                           862 LOAD_ATTR               16 (slide_layouts)
+                           872 LOAD_CONST               3 (1)
+                           874 BINARY_SUBSCR
+                           884 PRECALL                  1
+                           888 CALL                     1
+                           898 STORE_FAST               9 (slide)
                
-               212         898 LOAD_GLOBAL              3 (NULL + print)
-                           910 LOAD_CONST              21 ('\nExiting')
-                           912 PRECALL                  1
-                           916 CALL                     1
-                           926 POP_TOP
-               
-               213         928 LOAD_GLOBAL              5 (NULL + sys)
-                           940 LOAD_ATTR                3 (exit)
-                           950 LOAD_CONST               3 (1)
-                           952 PRECALL                  1
-                           956 CALL                     1
-                           966 POP_TOP
-                           968 POP_EXCEPT
-                           970 EXTENDED_ARG             1
-                           972 JUMP_BACKWARD          452 (to 70)
-               
-               214     >>  974 LOAD_GLOBAL             34 (KeyboardInterrupt)
-                           986 CHECK_EXC_MATCH
-                           988 POP_JUMP_FORWARD_IF_FALSE    39 (to 1068)
-                           990 POP_TOP
-               
-               215         992 LOAD_GLOBAL              3 (NULL + print)
-                          1004 LOAD_CONST              22 ('\nExiting..')
-                          1006 PRECALL                  1
-                          1010 CALL                     1
-                          1020 POP_TOP
-               
-               216        1022 LOAD_GLOBAL              5 (NULL + sys)
-                          1034 LOAD_ATTR                3 (exit)
-                          1044 LOAD_CONST               3 (1)
-                          1046 PRECALL                  1
-                          1050 CALL                     1
-                          1060 POP_TOP
-                          1062 POP_EXCEPT
-                          1064 EXTENDED_ARG             1
-                          1066 JUMP_BACKWARD          499 (to 70)
-               
-               217     >> 1068 LOAD_GLOBAL             36 (Exception)
-                          1080 CHECK_EXC_MATCH
-                          1082 POP_JUMP_FORWARD_IF_FALSE    37 (to 1158)
-                          1084 STORE_FAST              10 (e)
-               
-               218        1086 LOAD_GLOBAL             38 (logger)
-                          1098 LOAD_METHOD             20 (error)
-                          1120 LOAD_FAST               10 (e)
-                          1122 PRECALL                  1
-                          1126 CALL                     1
-                          1136 POP_TOP
-                          1138 POP_EXCEPT
-                          1140 LOAD_CONST               0 (None)
-                          1142 STORE_FAST              10 (e)
-                          1144 DELETE_FAST             10 (e)
+               216         900 LOAD_FAST                7 (paragraph)
+                           902 LOAD_ATTR               17 (text)
+                           912 LOAD_FAST                9 (slide)
+                           914 LOAD_ATTR               18 (shapes)
+                           924 LOAD_ATTR               19 (title)
+                           934 STORE_ATTR              17 (text)
+                           944 JUMP_BACKWARD          129 (to 688)
+               
+               219     >>  946 LOAD_FAST                5 (prs)
+                           948 LOAD_METHOD             20 (save)
+                           970 LOAD_FAST                3 (pptx_file)
+                           972 PRECALL                  1
+                           976 CALL                     1
+                           986 POP_TOP
+               
+               220         988 LOAD_GLOBAL              3 (NULL + print)
+                          1000 LOAD_CONST              20 ('\n')
+                          1002 LOAD_GLOBAL             20 (DGREEN)
+                          1014 FORMAT_VALUE             0
+                          1016 LOAD_CONST              21 ('Done')
+                          1018 LOAD_GLOBAL             14 (RESET)
+                          1030 FORMAT_VALUE             0
+                          1032 BUILD_STRING             4
+                          1034 PRECALL                  1
+                          1038 CALL                     1
+                          1048 POP_TOP
+                          1050 EXTENDED_ARG             1
+                          1052 JUMP_BACKWARD          492 (to 70)
+                       >> 1054 PUSH_EXC_INFO
+               
+               221        1056 LOAD_GLOBAL             42 (KeyboardInterrupt)
+                          1068 CHECK_EXC_MATCH
+                          1070 POP_JUMP_FORWARD_IF_FALSE    39 (to 1150)
+                          1072 POP_TOP
+               
+               222        1074 LOAD_GLOBAL              3 (NULL + print)
+                          1086 LOAD_CONST              22 ('\nExiting')
+                          1088 PRECALL                  1
+                          1092 CALL                     1
+                          1102 POP_TOP
+               
+               223        1104 LOAD_GLOBAL              5 (NULL + sys)
+                          1116 LOAD_ATTR                3 (exit)
+                          1126 LOAD_CONST               3 (1)
+                          1128 PRECALL                  1
+                          1132 CALL                     1
+                          1142 POP_TOP
+                          1144 POP_EXCEPT
                           1146 EXTENDED_ARG             2
                           1148 JUMP_BACKWARD          540 (to 70)
-                       >> 1150 LOAD_CONST               0 (None)
-                          1152 STORE_FAST              10 (e)
-                          1154 DELETE_FAST             10 (e)
-                          1156 RERAISE                  1
                
-               217     >> 1158 RERAISE                  0
-                       >> 1160 COPY                     3
-                          1162 POP_EXCEPT
-                          1164 RERAISE                  1
+               224     >> 1150 LOAD_GLOBAL             42 (KeyboardInterrupt)
+                          1162 CHECK_EXC_MATCH
+                          1164 POP_JUMP_FORWARD_IF_FALSE    39 (to 1244)
+                          1166 POP_TOP
+               
+               225        1168 LOAD_GLOBAL              3 (NULL + print)
+                          1180 LOAD_CONST              23 ('\nExiting..')
+                          1182 PRECALL                  1
+                          1186 CALL                     1
+                          1196 POP_TOP
+               
+               226        1198 LOAD_GLOBAL              5 (NULL + sys)
+                          1210 LOAD_ATTR                3 (exit)
+                          1220 LOAD_CONST               3 (1)
+                          1222 PRECALL                  1
+                          1226 CALL                     1
+                          1236 POP_TOP
+                          1238 POP_EXCEPT
+                          1240 EXTENDED_ARG             2
+                          1242 JUMP_BACKWARD          587 (to 70)
+               
+               227     >> 1244 LOAD_GLOBAL             44 (Exception)
+                          1256 CHECK_EXC_MATCH
+                          1258 POP_JUMP_FORWARD_IF_FALSE    37 (to 1334)
+                          1260 STORE_FAST              10 (e)
+               
+               228        1262 LOAD_GLOBAL             46 (logger)
+                          1274 LOAD_METHOD             24 (error)
+                          1296 LOAD_FAST               10 (e)
+                          1298 PRECALL                  1
+                          1302 CALL                     1
+                          1312 POP_TOP
+                          1314 POP_EXCEPT
+                          1316 LOAD_CONST               0 (None)
+                          1318 STORE_FAST              10 (e)
+                          1320 DELETE_FAST             10 (e)
+                          1322 EXTENDED_ARG             2
+                          1324 JUMP_BACKWARD          628 (to 70)
+                       >> 1326 LOAD_CONST               0 (None)
+                          1328 STORE_FAST              10 (e)
+                          1330 DELETE_FAST             10 (e)
+                          1332 RERAISE                  1
+               
+               227     >> 1334 RERAISE                  0
+                       >> 1336 COPY                     3
+                          1338 POP_EXCEPT
+                          1340 RERAISE                  1
                
-               175     >> 1166 LOAD_CONST               0 (None)
-                          1168 RETURN_VALUE
+               185     >> 1342 LOAD_CONST               0 (None)
+                          1344 RETURN_VALUE
                ExceptionTable:
-                 362 to 872 -> 878 [1]
-                 878 to 966 -> 1160 [2] lasti
-                 974 to 1060 -> 1160 [2] lasti
-                 1068 to 1084 -> 1160 [2] lasti
-                 1086 to 1136 -> 1150 [2] lasti
-                 1150 to 1158 -> 1160 [2] lasti
+                 362 to 1048 -> 1054 [1]
+                 1054 to 1142 -> 1336 [2] lasti
+                 1150 to 1236 -> 1336 [2] lasti
+                 1244 to 1260 -> 1336 [2] lasti
+                 1262 to 1312 -> 1326 [2] lasti
+                 1326 to 1334 -> 1336 [2] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d527d017c01a000000000000000000000000000000000
                         0000000000a6000000ab000000000000000000a001000000000000000000
                         00000000000000000000006400a6010000ab01000000000000000073277c
                         01a0000000000000000000000000000000000000000000a6000000ab0000
                         00000000000000a001000000000000000000000000000000000000000064
                         01a6010000ab010000000000000000af507c0191028c535300
-                     172           0 RESUME                   0
+                     182           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                82 (to 172)
                                    8 STORE_FAST               1 (item)
                                   10 LOAD_FAST                1 (item)
                                   12 LOAD_METHOD              0 (lower)
                                   34 PRECALL                  0
                                   38 CALL                     0
                                   48 LOAD_METHOD              1 (endswith)
                      
-                     173          70 LOAD_CONST               0 ('docx')
+                     183          70 LOAD_CONST               0 ('docx')
                      
-                     172          72 PRECALL                  1
+                     182          72 PRECALL                  1
                                   76 CALL                     1
                                   86 POP_JUMP_FORWARD_IF_TRUE    39 (to 166)
                      
-                     173          88 LOAD_FAST                1 (item)
+                     183          88 LOAD_FAST                1 (item)
                                   90 LOAD_METHOD              0 (lower)
                                  112 PRECALL                  0
                                  116 CALL                     0
                                  126 LOAD_METHOD              1 (endswith)
                                  148 LOAD_CONST               1 ('doc')
                                  150 PRECALL                  1
                                  154 CALL                     1
                      
-                     172         164 POP_JUMP_BACKWARD_IF_FALSE    80 (to 6)
+                     182         164 POP_JUMP_BACKWARD_IF_FALSE    80 (to 6)
                              >>  166 LOAD_FAST                1 (item)
                                  168 LIST_APPEND              2
                                  170 JUMP_BACKWARD           83 (to 6)
                              >>  172 RETURN_VALUE
                      consts
                         'docx'
                         'doc'
                      names      ('lower', 'endswith')
                      varnames   ('.0', 'item')
                      freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 172
+                     firstlineno 182
                      lnotab 0x460102ff10014cff
                   'Please provide appropriate file type'
                   1
                   'docx'
                   -4
                   'pptx'
                   'doc'
                   -3
-                  '\x1b[1;33mLoad the Word document..\x1b[0m'
-                  '\x1b[1;33mCreate a new PowerPoint presentation..\x1b[0m'
-                  '\x1b[1;32mPopulating pptx slides with \x1b[1;33m'
-                  '\x1b[1;32m entries..\x1b[0m'
+                  'Load the Word document..'
+                  'Create a new PowerPoint presentation..'
+                  'Populating pptx slides with '
+                  ' entries..'
                   0
                   100
-                  '\x1b[1;35mProgress:: \x1b[1;36m'
+                  'Progress:: \x1b[1;36m'
                   '.2f'
-                  '%\x1b[0m'
+                  '%'
                   '\r'
                   ('end',)
-                  '\n\x1b[1;32mDone\x1b[0m'
+                  '\n'
+                  'Done'
                   '\nExiting'
                   '\nExiting..'
-               names      ('preprocess', 'print', 'sys', 'exit', 'lower', 'endswith', 'Document', 'Presentation', 'len', 'paragraphs', 'slides', 'add_slide', 'slide_layouts', 'text', 'shapes', 'title', 'save', 'KeyboardInterrupt', 'Exception', 'logger', 'error')
+               names      ('preprocess', 'print', 'sys', 'exit', 'lower', 'endswith', 'DYELLOW', 'RESET', 'Document', 'Presentation', 'DGREEN', 'len', 'paragraphs', 'DMAGENTA', 'slides', 'add_slide', 'slide_layouts', 'text', 'shapes', 'title', 'save', 'KeyboardInterrupt', 'Exception', 'logger', 'error')
                varnames   ('self', 'word_list', 'word_file', 'pptx_file', 'doc', 'prs', 'count', 'paragraph', 'perc', 'slide', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'word_to_pptx'
-               firstlineno 170
+               firstlineno 180
                lnotab
-                  0x0201280118030a0204011e0128014e011c014e011a0102021e011e031e
-                  011c030c012eff1002040112010a0134010c010eff12034a032e032a0124
+                  0x0201280118030a0204011e0128014e011c014e011a0102023c011e033c
+                  011c030c0166ff1002040112010a0134010c012aff12034a032e032a0144
                   0112011e012e0112011e012e01120148ff08d6
             code
                argcount  : 1
-               nlocals   : 9
+               nlocals   : 10
                stacksize : 12
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d01640184007c014400a6000000ab00000000
-                  00000000007d017403000000000000000000007c01a6010000ab01000000
-                  000000000001007c01440090015d8a7d027c02a002000000000000000000
-                  0000000000000000000000a6000000ab000000000000000000a003000000
+                  00000000007d017c01440090015dec7d027c02a001000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000a002000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   000000720e7c026400640385021900000000000000000064047a0000007d
-                  036e347c02a0020000000000000000000000000000000000000000a60000
-                  00ab000000000000000000a0030000000000000000000000000000000000
+                  036e347c02a0010000000000000000000000000000000000000000a60000
+                  00ab000000000000000000a0020000000000000000000000000000000000
                   0000006405a6010000ab010000000000000000720d7c0264006406850219
-                  00000000000000000064047a0000007d0309007409000000000000000000
-                  007c02a6010000ab0100000000000000007d04740b000000000000000000
-                  007c0364076408ac09a6030000ab03000000000000000035007d057c046a
-                  06000000000000000044005d397d067c05a0070000000000000000000000
-                  0000000000000000007c066a080000000000000000640a7a000000a60100
-                  00ab0100000000000000000100741200000000000000000000a00a000000
-                  0000000000000000000000000000000000640ba6010000ab010000000000
-                  00000001008c3a741200000000000000000000a00a000000000000000000
-                  0000000000000000000000640c7c029b00640d7c039b00640e9d05a60100
-                  00ab0100000000000000000100640064006400a6020000ab020000000000
-                  00000001006e0b2300310073047702780359007701010059000100010090
-                  018c0a2300741600000000000000000000240072757d0774120000000000
-                  0000000000a00c0000000000000000000000000000000000000000640f7c
-                  029b00640d7c039b0064107c079b009d06a6010000ab0100000000000000
-                  000100740b0000000000000000000064116412a6020000ab020000000000
-                  00000035007d087c08a00700000000000000000000000000000000000000
-                  0064137c029b00640d7c039b0064147c079b00640a9d07a6010000ab0100
-                  000000000000000100640064006400a6020000ab02000000000000000001
-                  006e0b23003100730477027803590077010100590001000100590064007d
-                  077e0790018c8464007d077e077701770078035900770164005300
-               224           0 RESUME                   0
+                  00000000000000000064047a0000007d0309007407000000000000000000
+                  007c02a6010000ab0100000000000000007d047409000000000000000000
+                  006407a6010000ab0100000000000000000100740b000000000000000000
+                  007c0364086409ac0aa6030000ab03000000000000000035007d05640b7d
+                  067c046a06000000000000000044005d5b7d077c05a00700000000000000
+                  000000000000000000000000007c076a080000000000000000640c7a0000
+                  00a6010000ab01000000000000000001007c06640d7a0d00007d06740900
+                  000000000000000000640e7412000000000000000000009b007c069b0064
+                  0f7415000000000000000000007c046a060000000000000000a6010000ab
+                  0100000000000000009b007416000000000000000000009b009d066410ac
+                  11a6020000ab02000000000000000001008c5c7418000000000000000000
+                  00a00d0000000000000000000000000000000000000000741c0000000000
+                  00000000009b0064127416000000000000000000009b009d03a6010000ab
+                  0100000000000000000100640064006400a6020000ab0200000000000000
+                  0001006e0b2300310073047702780359007701010059000100010090018c
+                  452300741e00000000000000000000240072260100740900000000000000
+                  0000006413a6010000ab0100000000000000000100742100000000000000
+                  0000006a110000000000000000a6000000ab000000000000000000010059
+                  0090018c747424000000000000000000002400726e7d0874180000000000
+                  0000000000a013000000000000000000000000000000000000000064147c
+                  089b009d02a6010000ab0100000000000000000100740b00000000000000
+                  00000064156416a6020000ab02000000000000000035007d097c09a00700
+                  0000000000000000000000000000000000000064177c029b0064187c039b
+                  0064197c089b009d06a6010000ab01000000000000000001006400640064
+                  00a6020000ab02000000000000000001006e0b2300310073047702780359
+                  0077010100590001000100590064007d087e0890018ce664007d087e0877
+                  01770078035900770164005300
+               234           0 RESUME                   0
                
-               225           2 LOAD_FAST                0 (self)
+               235           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (preprocess)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (word_list)
                
-               226          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 226>)
+               236          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 236>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                1 (word_list)
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               1 (word_list)
                
-               228          66 LOAD_GLOBAL              3 (NULL + print)
-                            78 LOAD_FAST                1 (word_list)
-                            80 PRECALL                  1
-                            84 CALL                     1
-                            94 POP_TOP
-               
-               229          96 LOAD_FAST                1 (word_list)
-                            98 GET_ITER
-                       >>  100 EXTENDED_ARG             1
-                           102 FOR_ITER               394 (to 892)
-                           104 STORE_FAST               2 (file_path)
-               
-               230         106 LOAD_FAST                2 (file_path)
-                           108 LOAD_METHOD              2 (lower)
-                           130 PRECALL                  0
-                           134 CALL                     0
-                           144 LOAD_METHOD              3 (endswith)
-                           166 LOAD_CONST               2 ('docx')
-                           168 PRECALL                  1
-                           172 CALL                     1
-                           182 POP_JUMP_FORWARD_IF_FALSE    14 (to 212)
-               
-               231         184 LOAD_FAST                2 (file_path)
-                           186 LOAD_CONST               0 (None)
-                           188 LOAD_CONST               3 (-4)
-                           190 BUILD_SLICE              2
-                           192 BINARY_SUBSCR
-                           202 LOAD_CONST               4 ('txt')
-                           204 BINARY_OP                0 (+)
-                           208 STORE_FAST               3 (txt_file)
-                           210 JUMP_FORWARD            52 (to 316)
-               
-               232     >>  212 LOAD_FAST                2 (file_path)
-                           214 LOAD_METHOD              2 (lower)
-                           236 PRECALL                  0
-                           240 CALL                     0
-                           250 LOAD_METHOD              3 (endswith)
-                           272 LOAD_CONST               5 ('doc')
-                           274 PRECALL                  1
-                           278 CALL                     1
-                           288 POP_JUMP_FORWARD_IF_FALSE    13 (to 316)
+               238          66 LOAD_FAST                1 (word_list)
+                            68 GET_ITER
+                       >>   70 EXTENDED_ARG             1
+                            72 FOR_ITER               492 (to 1058)
+                            74 STORE_FAST               2 (file_path)
                
-               233         290 LOAD_FAST                2 (file_path)
-                           292 LOAD_CONST               0 (None)
-                           294 LOAD_CONST               6 (-3)
-                           296 BUILD_SLICE              2
-                           298 BINARY_SUBSCR
-                           308 LOAD_CONST               4 ('txt')
-                           310 BINARY_OP                0 (+)
-                           314 STORE_FAST               3 (txt_file)
+               239          76 LOAD_FAST                2 (file_path)
+                            78 LOAD_METHOD              1 (lower)
+                           100 PRECALL                  0
+                           104 CALL                     0
+                           114 LOAD_METHOD              2 (endswith)
+                           136 LOAD_CONST               2 ('docx')
+                           138 PRECALL                  1
+                           142 CALL                     1
+                           152 POP_JUMP_FORWARD_IF_FALSE    14 (to 182)
+               
+               240         154 LOAD_FAST                2 (file_path)
+                           156 LOAD_CONST               0 (None)
+                           158 LOAD_CONST               3 (-4)
+                           160 BUILD_SLICE              2
+                           162 BINARY_SUBSCR
+                           172 LOAD_CONST               4 ('txt')
+                           174 BINARY_OP                0 (+)
+                           178 STORE_FAST               3 (txt_file)
+                           180 JUMP_FORWARD            52 (to 286)
                
-               234     >>  316 NOP
+               241     >>  182 LOAD_FAST                2 (file_path)
+                           184 LOAD_METHOD              1 (lower)
+                           206 PRECALL                  0
+                           210 CALL                     0
+                           220 LOAD_METHOD              2 (endswith)
+                           242 LOAD_CONST               5 ('doc')
+                           244 PRECALL                  1
+                           248 CALL                     1
+                           258 POP_JUMP_FORWARD_IF_FALSE    13 (to 286)
                
-               235         318 LOAD_GLOBAL              9 (NULL + Document)
-                           330 LOAD_FAST                2 (file_path)
+               242         260 LOAD_FAST                2 (file_path)
+                           262 LOAD_CONST               0 (None)
+                           264 LOAD_CONST               6 (-3)
+                           266 BUILD_SLICE              2
+                           268 BINARY_SUBSCR
+                           278 LOAD_CONST               4 ('txt')
+                           280 BINARY_OP                0 (+)
+                           284 STORE_FAST               3 (txt_file)
+               
+               243     >>  286 NOP
+               
+               244         288 LOAD_GLOBAL              7 (NULL + Document)
+                           300 LOAD_FAST                2 (file_path)
+                           302 PRECALL                  1
+                           306 CALL                     1
+                           316 STORE_FAST               4 (doc)
+               
+               245         318 LOAD_GLOBAL              9 (NULL + print)
+                           330 LOAD_CONST               7 ('INFO Processing...')
                            332 PRECALL                  1
                            336 CALL                     1
-                           346 STORE_FAST               4 (doc)
+                           346 POP_TOP
                
-               236         348 LOAD_GLOBAL             11 (NULL + open)
+               247         348 LOAD_GLOBAL             11 (NULL + open)
                            360 LOAD_FAST                3 (txt_file)
-                           362 LOAD_CONST               7 ('w')
-                           364 LOAD_CONST               8 ('utf-8')
-                           366 KW_NAMES                 9
+                           362 LOAD_CONST               8 ('w')
+                           364 LOAD_CONST               9 ('utf-8')
+                           366 KW_NAMES                10
                            368 PRECALL                  3
                            372 CALL                     3
                            382 BEFORE_WITH
                            384 STORE_FAST               5 (f)
                
-               237         386 LOAD_FAST                4 (doc)
-                           388 LOAD_ATTR                6 (paragraphs)
-                           398 GET_ITER
-                       >>  400 FOR_ITER                57 (to 516)
-                           402 STORE_FAST               6 (paragraph)
-               
-               238         404 LOAD_FAST                5 (f)
-                           406 LOAD_METHOD              7 (write)
-                           428 LOAD_FAST                6 (paragraph)
-                           430 LOAD_ATTR                8 (text)
-                           440 LOAD_CONST              10 ('\n')
-                           442 BINARY_OP                0 (+)
-                           446 PRECALL                  1
-                           450 CALL                     1
-                           460 POP_TOP
+               248         386 LOAD_CONST              11 (0)
+                           388 STORE_FAST               6 (Par)
                
-               239         462 LOAD_GLOBAL             18 (logger)
-                           474 LOAD_METHOD             10 (info)
-                           496 LOAD_CONST              11 ('Processing...')
-                           498 PRECALL                  1
-                           502 CALL                     1
-                           512 POP_TOP
-                           514 JUMP_BACKWARD           58 (to 400)
+               249         390 LOAD_FAST                4 (doc)
+                           392 LOAD_ATTR                6 (paragraphs)
+                           402 GET_ITER
+                       >>  404 FOR_ITER                91 (to 588)
+                           406 STORE_FAST               7 (paragraph)
+               
+               250         408 LOAD_FAST                5 (f)
+                           410 LOAD_METHOD              7 (write)
+                           432 LOAD_FAST                7 (paragraph)
+                           434 LOAD_ATTR                8 (text)
+                           444 LOAD_CONST              12 ('\n')
+                           446 BINARY_OP                0 (+)
+                           450 PRECALL                  1
+                           454 CALL                     1
+                           464 POP_TOP
+               
+               251         466 LOAD_FAST                6 (Par)
+                           468 LOAD_CONST              13 (1)
+                           470 BINARY_OP               13 (+=)
+                           474 STORE_FAST               6 (Par)
+               
+               253         476 LOAD_GLOBAL              9 (NULL + print)
+                           488 LOAD_CONST              14 ('Par:')
+                           490 LOAD_GLOBAL             18 (BLUE)
+                           502 FORMAT_VALUE             0
+                           504 LOAD_FAST                6 (Par)
+                           506 FORMAT_VALUE             0
+                           508 LOAD_CONST              15 ('/')
+                           510 LOAD_GLOBAL             21 (NULL + len)
+                           522 LOAD_FAST                4 (doc)
+                           524 LOAD_ATTR                6 (paragraphs)
+                           534 PRECALL                  1
+                           538 CALL                     1
+                           548 FORMAT_VALUE             0
+                           550 LOAD_GLOBAL             22 (RESET)
+                           562 FORMAT_VALUE             0
+                           564 BUILD_STRING             6
+                           566 LOAD_CONST              16 ('\r')
+                           568 KW_NAMES                17
+                           570 PRECALL                  2
+                           574 CALL                     2
+                           584 POP_TOP
+                           586 JUMP_BACKWARD           92 (to 404)
+               
+               254     >>  588 LOAD_GLOBAL             24 (logger)
+                           600 LOAD_METHOD             13 (info)
+                           622 LOAD_GLOBAL             28 (DMAGENTA)
+                           634 FORMAT_VALUE             0
+                           636 LOAD_CONST              18 ('Conversion of file to txt success')
+                           638 LOAD_GLOBAL             22 (RESET)
+                           650 FORMAT_VALUE             0
+                           652 BUILD_STRING             3
+                           654 PRECALL                  1
+                           658 CALL                     1
+                           668 POP_TOP
+               
+               247         670 LOAD_CONST               0 (None)
+                           672 LOAD_CONST               0 (None)
+                           674 LOAD_CONST               0 (None)
+                           676 PRECALL                  2
+                           680 CALL                     2
+                           690 POP_TOP
+                           692 JUMP_FORWARD            11 (to 716)
+                       >>  694 PUSH_EXC_INFO
+                           696 WITH_EXCEPT_START
+                           698 POP_JUMP_FORWARD_IF_TRUE     4 (to 708)
+                           700 RERAISE                  2
+                       >>  702 COPY                     3
+                           704 POP_EXCEPT
+                           706 RERAISE                  1
+                       >>  708 POP_TOP
+                           710 POP_EXCEPT
+                           712 POP_TOP
+                           714 POP_TOP
+                       >>  716 EXTENDED_ARG             1
+                           718 JUMP_BACKWARD          325 (to 70)
+                       >>  720 PUSH_EXC_INFO
+               
+               256         722 LOAD_GLOBAL             30 (KeyboardInterrupt)
+                           734 CHECK_EXC_MATCH
+                           736 POP_JUMP_FORWARD_IF_FALSE    38 (to 814)
+                           738 POP_TOP
                
-               240     >>  516 LOAD_GLOBAL             18 (logger)
-                           528 LOAD_METHOD             10 (info)
-                           550 LOAD_CONST              12 ('\x1b[1;95mSuccessfully converted ')
-                           552 LOAD_FAST                2 (file_path)
-                           554 FORMAT_VALUE             0
-                           556 LOAD_CONST              13 (' to ')
-               
-               241         558 LOAD_FAST                3 (txt_file)
-               
-               240         560 FORMAT_VALUE             0
-                           562 LOAD_CONST              14 ('\x1b[0m')
-                           564 BUILD_STRING             5
-                           566 PRECALL                  1
-                           570 CALL                     1
-                           580 POP_TOP
-               
-               236         582 LOAD_CONST               0 (None)
-                           584 LOAD_CONST               0 (None)
-                           586 LOAD_CONST               0 (None)
-                           588 PRECALL                  2
-                           592 CALL                     2
-                           602 POP_TOP
-                           604 JUMP_FORWARD            11 (to 628)
-                       >>  606 PUSH_EXC_INFO
-                           608 WITH_EXCEPT_START
-                           610 POP_JUMP_FORWARD_IF_TRUE     4 (to 620)
-                           612 RERAISE                  2
-                       >>  614 COPY                     3
-                           616 POP_EXCEPT
-                           618 RERAISE                  1
-                       >>  620 POP_TOP
-                           622 POP_EXCEPT
-                           624 POP_TOP
-                           626 POP_TOP
-                       >>  628 EXTENDED_ARG             1
-                           630 JUMP_BACKWARD          266 (to 100)
-                       >>  632 PUSH_EXC_INFO
-               
-               242         634 LOAD_GLOBAL             22 (Exception)
-                           646 CHECK_EXC_MATCH
-                           648 POP_JUMP_FORWARD_IF_FALSE   117 (to 884)
-                           650 STORE_FAST               7 (e)
-               
-               243         652 LOAD_GLOBAL             18 (logger)
-                           664 LOAD_METHOD             12 (error)
-               
-               244         686 LOAD_CONST              15 ('Oops something went amiss while attempting to convert ')
-               
-               245         688 LOAD_FAST                2 (file_path)
-               
-               244         690 FORMAT_VALUE             0
-                           692 LOAD_CONST              13 (' to ')
-               
-               245         694 LOAD_FAST                3 (txt_file)
-               
-               244         696 FORMAT_VALUE             0
-                           698 LOAD_CONST              16 (': ')
+               257         740 LOAD_GLOBAL              9 (NULL + print)
+                           752 LOAD_CONST              19 ('\nExit')
+                           754 PRECALL                  1
+                           758 CALL                     1
+                           768 POP_TOP
                
-               245         700 LOAD_FAST                7 (e)
+               258         770 LOAD_GLOBAL             33 (NULL + sys)
+                           782 LOAD_ATTR               17 (exit)
+                           792 PRECALL                  0
+                           796 CALL                     0
+                           806 POP_TOP
+                           808 POP_EXCEPT
+                           810 EXTENDED_ARG             1
+                           812 JUMP_BACKWARD          372 (to 70)
                
-               244         702 FORMAT_VALUE             0
-                           704 BUILD_STRING             6
+               259     >>  814 LOAD_GLOBAL             36 (Exception)
+                           826 CHECK_EXC_MATCH
+                           828 POP_JUMP_FORWARD_IF_FALSE   110 (to 1050)
+                           830 STORE_FAST               8 (e)
+               
+               260         832 LOAD_GLOBAL             24 (logger)
+                           844 LOAD_METHOD             19 (error)
+               
+               261         866 LOAD_CONST              20 ('Dear user something went amiss while attempting the conversion:\n ')
+                           868 LOAD_FAST                8 (e)
+                           870 FORMAT_VALUE             0
+                           872 BUILD_STRING             2
+               
+               260         874 PRECALL                  1
+                           878 CALL                     1
+                           888 POP_TOP
+               
+               262         890 LOAD_GLOBAL             11 (NULL + open)
+                           902 LOAD_CONST              21 ('conversion.log')
+                           904 LOAD_CONST              22 ('a')
+                           906 PRECALL                  2
+                           910 CALL                     2
+                           920 BEFORE_WITH
+                           922 STORE_FAST               9 (log_file)
+               
+               263         924 LOAD_FAST                9 (log_file)
+                           926 LOAD_METHOD              7 (write)
+                           948 LOAD_CONST              23 ("Couldn't convert ")
+                           950 LOAD_FAST                2 (file_path)
+                           952 FORMAT_VALUE             0
+                           954 LOAD_CONST              24 (' to ')
+                           956 LOAD_FAST                3 (txt_file)
+                           958 FORMAT_VALUE             0
+                           960 LOAD_CONST              25 (':REASON->')
                
-               243         706 PRECALL                  1
-                           710 CALL                     1
-                           720 POP_TOP
+               264         962 LOAD_FAST                8 (e)
                
-               246         722 LOAD_GLOBAL             11 (NULL + open)
-                           734 LOAD_CONST              17 ('conversion.log')
-                           736 LOAD_CONST              18 ('a')
-                           738 PRECALL                  2
-                           742 CALL                     2
-                           752 BEFORE_WITH
-                           754 STORE_FAST               8 (log_file)
-               
-               247         756 LOAD_FAST                8 (log_file)
-                           758 LOAD_METHOD              7 (write)
-                           780 LOAD_CONST              19 ('Error converting ')
-                           782 LOAD_FAST                2 (file_path)
-                           784 FORMAT_VALUE             0
-                           786 LOAD_CONST              13 (' to ')
-               
-               248         788 LOAD_FAST                3 (txt_file)
-               
-               247         790 FORMAT_VALUE             0
-                           792 LOAD_CONST              20 (':')
-               
-               248         794 LOAD_FAST                7 (e)
-               
-               247         796 FORMAT_VALUE             0
-                           798 LOAD_CONST              10 ('\n')
-                           800 BUILD_STRING             7
-                           802 PRECALL                  1
-                           806 CALL                     1
-                           816 POP_TOP
+               263         964 FORMAT_VALUE             0
+                           966 BUILD_STRING             6
+                           968 PRECALL                  1
+                           972 CALL                     1
+                           982 POP_TOP
+               
+               262         984 LOAD_CONST               0 (None)
+                           986 LOAD_CONST               0 (None)
+                           988 LOAD_CONST               0 (None)
+                           990 PRECALL                  2
+                           994 CALL                     2
+                          1004 POP_TOP
+                          1006 JUMP_FORWARD            11 (to 1030)
+                       >> 1008 PUSH_EXC_INFO
+                          1010 WITH_EXCEPT_START
+                          1012 POP_JUMP_FORWARD_IF_TRUE     4 (to 1022)
+                          1014 RERAISE                  2
+                       >> 1016 COPY                     3
+                          1018 POP_EXCEPT
+                          1020 RERAISE                  1
+                       >> 1022 POP_TOP
+                          1024 POP_EXCEPT
+                          1026 POP_TOP
+                          1028 POP_TOP
+                       >> 1030 POP_EXCEPT
+                          1032 LOAD_CONST               0 (None)
+                          1034 STORE_FAST               8 (e)
+                          1036 DELETE_FAST              8 (e)
+                          1038 EXTENDED_ARG             1
+                          1040 JUMP_BACKWARD          486 (to 70)
+                       >> 1042 LOAD_CONST               0 (None)
+                          1044 STORE_FAST               8 (e)
+                          1046 DELETE_FAST              8 (e)
+                          1048 RERAISE                  1
                
-               246         818 LOAD_CONST               0 (None)
-                           820 LOAD_CONST               0 (None)
-                           822 LOAD_CONST               0 (None)
-                           824 PRECALL                  2
-                           828 CALL                     2
-                           838 POP_TOP
-                           840 JUMP_FORWARD            11 (to 864)
-                       >>  842 PUSH_EXC_INFO
-                           844 WITH_EXCEPT_START
-                           846 POP_JUMP_FORWARD_IF_TRUE     4 (to 856)
-                           848 RERAISE                  2
-                       >>  850 COPY                     3
-                           852 POP_EXCEPT
-                           854 RERAISE                  1
-                       >>  856 POP_TOP
-                           858 POP_EXCEPT
-                           860 POP_TOP
-                           862 POP_TOP
-                       >>  864 POP_EXCEPT
-                           866 LOAD_CONST               0 (None)
-                           868 STORE_FAST               7 (e)
-                           870 DELETE_FAST              7 (e)
-                           872 EXTENDED_ARG             1
-                           874 JUMP_BACKWARD          388 (to 100)
-                       >>  876 LOAD_CONST               0 (None)
-                           878 STORE_FAST               7 (e)
-                           880 DELETE_FAST              7 (e)
-                           882 RERAISE                  1
-               
-               242     >>  884 RERAISE                  0
-                       >>  886 COPY                     3
-                           888 POP_EXCEPT
-                           890 RERAISE                  1
+               259     >> 1050 RERAISE                  0
+                       >> 1052 COPY                     3
+                          1054 POP_EXCEPT
+                          1056 RERAISE                  1
                
-               229     >>  892 LOAD_CONST               0 (None)
-                           894 RETURN_VALUE
+               238     >> 1058 LOAD_CONST               0 (None)
+                          1060 RETURN_VALUE
                ExceptionTable:
-                 318 to 382 -> 632 [1]
-                 384 to 580 -> 606 [2] lasti
-                 582 to 604 -> 632 [1]
-                 606 to 612 -> 614 [4] lasti
-                 614 to 618 -> 632 [1]
-                 620 to 620 -> 614 [4] lasti
-                 622 to 626 -> 632 [1]
-                 632 to 650 -> 886 [2] lasti
-                 652 to 752 -> 876 [2] lasti
-                 754 to 816 -> 842 [3] lasti
-                 818 to 840 -> 876 [2] lasti
-                 842 to 848 -> 850 [5] lasti
-                 850 to 854 -> 876 [2] lasti
-                 856 to 856 -> 850 [5] lasti
-                 858 to 862 -> 876 [2] lasti
-                 876 to 884 -> 886 [2] lasti
+                 288 to 382 -> 720 [1]
+                 384 to 668 -> 694 [2] lasti
+                 670 to 692 -> 720 [1]
+                 694 to 700 -> 702 [4] lasti
+                 702 to 706 -> 720 [1]
+                 708 to 708 -> 702 [4] lasti
+                 710 to 714 -> 720 [1]
+                 720 to 806 -> 1052 [2] lasti
+                 814 to 830 -> 1052 [2] lasti
+                 832 to 920 -> 1042 [2] lasti
+                 922 to 982 -> 1008 [3] lasti
+                 984 to 1006 -> 1042 [2] lasti
+                 1008 to 1014 -> 1016 [5] lasti
+                 1016 to 1020 -> 1042 [2] lasti
+                 1022 to 1022 -> 1016 [5] lasti
+                 1024 to 1028 -> 1042 [2] lasti
+                 1042 to 1050 -> 1052 [2] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d527d017c01a000000000000000000000000000000000
                         0000000000a6000000ab000000000000000000a001000000000000000000
                         00000000000000000000006400a6010000ab01000000000000000073277c
                         01a0000000000000000000000000000000000000000000a6000000ab0000
                         00000000000000a001000000000000000000000000000000000000000064
                         01a6010000ab010000000000000000af507c0191028c535300
-                     226           0 RESUME                   0
+                     236           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                82 (to 172)
                                    8 STORE_FAST               1 (item)
                                   10 LOAD_FAST                1 (item)
                                   12 LOAD_METHOD              0 (lower)
                                   34 PRECALL                  0
                                   38 CALL                     0
                                   48 LOAD_METHOD              1 (endswith)
                      
-                     227          70 LOAD_CONST               0 ('docx')
+                     237          70 LOAD_CONST               0 ('docx')
                      
-                     226          72 PRECALL                  1
+                     236          72 PRECALL                  1
                                   76 CALL                     1
                                   86 POP_JUMP_FORWARD_IF_TRUE    39 (to 166)
                      
-                     227          88 LOAD_FAST                1 (item)
+                     237          88 LOAD_FAST                1 (item)
                                   90 LOAD_METHOD              0 (lower)
                                  112 PRECALL                  0
                                  116 CALL                     0
                                  126 LOAD_METHOD              1 (endswith)
                                  148 LOAD_CONST               1 ('doc')
                                  150 PRECALL                  1
                                  154 CALL                     1
                      
-                     226         164 POP_JUMP_BACKWARD_IF_FALSE    80 (to 6)
+                     236         164 POP_JUMP_BACKWARD_IF_FALSE    80 (to 6)
                              >>  166 LOAD_FAST                1 (item)
                                  168 LIST_APPEND              2
                                  170 JUMP_BACKWARD           83 (to 6)
                              >>  172 RETURN_VALUE
                      consts
                         'docx'
                         'doc'
                      names      ('lower', 'endswith')
                      varnames   ('.0', 'item')
                      freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 226
+                     firstlineno 236
                      lnotab 0x460102ff10014cff
                   'docx'
                   -4
                   'txt'
                   'doc'
                   -3
+                  'INFO Processing...'
                   'w'
                   'utf-8'
                   ('encoding',)
+                  0
                   '\n'
-                  'Processing...'
-                  '\x1b[1;95mSuccessfully converted '
-                  ' to '
-                  '\x1b[0m'
-                  'Oops something went amiss while attempting to convert '
-                  ': '
+                  1
+                  'Par:'
+                  '/'
+                  '\r'
+                  ('end',)
+                  'Conversion of file to txt success'
+                  '\nExit'
+                  'Dear user something went amiss while attempting the conversion:\n '
                   'conversion.log'
                   'a'
-                  'Error converting '
-                  ':'
-               names      ('preprocess', 'print', 'lower', 'endswith', 'Document', 'open', 'paragraphs', 'write', 'text', 'logger', 'info', 'Exception', 'error')
-               varnames   ('self', 'word_list', 'file_path', 'txt_file', 'doc', 'f', 'paragraph', 'e', 'log_file')
+                  "Couldn't convert "
+                  ' to '
+                  ':REASON->'
+               names      ('preprocess', 'lower', 'endswith', 'Document', 'print', 'open', 'paragraphs', 'write', 'text', 'BLUE', 'len', 'RESET', 'logger', 'info', 'DMAGENTA', 'KeyboardInterrupt', 'sys', 'exit', 'Exception', 'error')
+               varnames   ('self', 'word_list', 'file_path', 'txt_file', 'doc', 'f', 'Par', 'paragraph', 'e', 'log_file')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'word_to_txt'
-               firstlineno 224
+               firstlineno 234
                lnotab
-                  0x0201280118021e010a014e011c014e011a0102011e01260112013a0136
-                  012a0102ff16fc340612012201020102ff040102ff040102ff04ff100322
-                  01200102ff040102ff16ff42fc08f3
+                  0x0201280118020a014e011c014e011a0102011e011e022601040112013a
+                  010a02700152f9340912011e012c011201220108ff10022201260102ff14
+                  ff42fd08eb
             code
                argcount  : 1
                nlocals   : 12
                stacksize : 12
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d01640184007c014400a6000000ab00000000
-                  00000000007d017c01440090015d747d027c026400640285021900000000
+                  00000000007d017c01440090015d877d027c026400640285021900000000
                   000000000064037a0000007d0309007403000000000000000000007c0264
                   04a6020000ab02000000000000000035007d047405000000000000000000
                   006a0300000000000000007c04a6010000ab0100000000000000007d0564
-                  057d067409000000000000000000007c056a050000000000000000a60100
-                  00ab01000000000000000044005d2e7d077c05a006000000000000000000
-                  00000000000000000000007c07a6010000ab0100000000000000007d087c
-                  067c08a0070000000000000000000000000000000000000000a6000000ab
-                  0000000000000000007a0d00007d068c2f0900640064006400a6020000ab
-                  02000000000000000001006e0b2300310073047702780359007701010059
-                  00010001007403000000000000000000007c0364066407ac08a6030000ab
-                  03000000000000000035007d097c09a00800000000000000000000000000
-                  000000000000007c06a6010000ab01000000000000000001007412000000
-                  00000000000000a00a000000000000000000000000000000000000000064
-                  097c029b00640a7c039b00640b9d05a6010000ab01000000000000000001
-                  00640064006400a6020000ab02000000000000000001006e0b2300310073
-                  04770278035900770101005900010001008cf42300741600000000000000
-                  000000240072757d0a741200000000000000000000a00c00000000000000
-                  00000000000000000000000000640c7c029b00640a7c039b00640d7c0a9b
-                  009d06a6010000ab01000000000000000001007403000000000000000000
-                  00640e640fa6020000ab02000000000000000035007d0b7c0ba008000000
-                  000000000000000000000000000000000064107c029b00640a7c039b0064
-                  0d7c0a9b0064119d07a6010000ab01000000000000000001006400640064
-                  00a6020000ab02000000000000000001006e0b2300310073047702780359
-                  0077010100590001000100590064007d0a7e0a90018c6e64007d0a7e0a77
-                  01770078035900770164005300
-               253           0 RESUME                   0
+                  057d06740900000000000000000000740b000000000000000000007c056a
+                  060000000000000000a6010000ab010000000000000000a6010000ab0100
+                  0000000000000044005d267d077c056a0600000000000000007c07190000
+                  000000000000007d087c067c08a007000000000000000000000000000000
+                  0000000000a6000000ab0000000000000000007a0d00007d068c27090064
+                  0064006400a6020000ab02000000000000000001006e0b23003100730477
+                  0278035900770101005900010001007403000000000000000000007c0364
+                  066407ac08a6030000ab03000000000000000035007d097c09a008000000
+                  00000000000000000000000000000000007c06a6010000ab010000000000
+                  0000000100741200000000000000000000a00a0000000000000000000000
+                  0000000000000000007416000000000000000000009b0064097c029b0064
+                  0a7c039b007418000000000000000000009b009d06a6010000ab01000000
+                  00000000000100640064006400a6020000ab02000000000000000001006e
+                  0b2300310073047702780359007701010059000100010090018c07230074
+                  1a00000000000000000000240072757d0a741200000000000000000000a0
+                  0e0000000000000000000000000000000000000000640b7c029b00640a7c
+                  039b00640c7c0a9b009d06a6010000ab0100000000000000000100740300
+                  000000000000000000640d640ea6020000ab02000000000000000035007d
+                  0b7c0ba0080000000000000000000000000000000000000000640f7c029b
+                  00640a7c039b00640c7c0a9b0064109d07a6010000ab0100000000000000
+                  000100640064006400a6020000ab02000000000000000001006e0b230031
+                  00730477027803590077010100590001000100590064007d0a7e0a90018c
+                  8164007d0a7e0a7701770078035900770164005300
+               269           0 RESUME                   0
                
-               254           2 LOAD_FAST                0 (self)
+               270           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (preprocess)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (pdf_list)
                
-               255          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 255>)
+               271          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 271>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                1 (pdf_list)
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               1 (pdf_list)
                
-               256          66 LOAD_FAST                1 (pdf_list)
+               272          66 LOAD_FAST                1 (pdf_list)
                             68 GET_ITER
                        >>   70 EXTENDED_ARG             1
-                            72 FOR_ITER               372 (to 818)
+                            72 FOR_ITER               391 (to 856)
                             74 STORE_FAST               2 (file_path)
                
-               257          76 LOAD_FAST                2 (file_path)
+               273          76 LOAD_FAST                2 (file_path)
                             78 LOAD_CONST               0 (None)
                             80 LOAD_CONST               2 (-3)
                             82 BUILD_SLICE              2
                             84 BINARY_SUBSCR
                             94 LOAD_CONST               3 ('txt')
                             96 BINARY_OP                0 (+)
                            100 STORE_FAST               3 (txt_file)
                
-               258         102 NOP
+               274         102 NOP
                
-               259         104 LOAD_GLOBAL              3 (NULL + open)
+               275         104 LOAD_GLOBAL              3 (NULL + open)
                            116 LOAD_FAST                2 (file_path)
                            118 LOAD_CONST               4 ('rb')
                            120 PRECALL                  2
                            124 CALL                     2
                            134 BEFORE_WITH
                            136 STORE_FAST               4 (file)
                
-               260         138 LOAD_GLOBAL              5 (NULL + PyPDF2)
+               276         138 LOAD_GLOBAL              5 (NULL + PyPDF2)
                            150 LOAD_ATTR                3 (PdfReader)
                            160 LOAD_FAST                4 (file)
                            162 PRECALL                  1
                            166 CALL                     1
                            176 STORE_FAST               5 (pdf_reader)
                
-               261         178 LOAD_CONST               5 ('')
+               277         178 LOAD_CONST               5 ('')
                            180 STORE_FAST               6 (text)
                
-               262         182 LOAD_GLOBAL              9 (NULL + range)
-                           194 LOAD_FAST                5 (pdf_reader)
-                           196 LOAD_ATTR                5 (numPages)
-                           206 PRECALL                  1
-                           210 CALL                     1
-                           220 GET_ITER
-                       >>  222 FOR_ITER                46 (to 316)
-                           224 STORE_FAST               7 (page_num)
-               
-               263         226 LOAD_FAST                5 (pdf_reader)
-                           228 LOAD_METHOD              6 (getPage)
-                           250 LOAD_FAST                7 (page_num)
-                           252 PRECALL                  1
-                           256 CALL                     1
-                           266 STORE_FAST               8 (page)
-               
-               264         268 LOAD_FAST                6 (text)
-                           270 LOAD_FAST                8 (page)
-                           272 LOAD_METHOD              7 (extractText)
-                           294 PRECALL                  0
-                           298 CALL                     0
-                           308 BINARY_OP               13 (+=)
-                           312 STORE_FAST               6 (text)
-                           314 JUMP_BACKWARD           47 (to 222)
-               
-               262     >>  316 NOP
-               
-               259         318 LOAD_CONST               0 (None)
-                           320 LOAD_CONST               0 (None)
-                           322 LOAD_CONST               0 (None)
-                           324 PRECALL                  2
-                           328 CALL                     2
-                           338 POP_TOP
-                           340 JUMP_FORWARD            11 (to 364)
-                       >>  342 PUSH_EXC_INFO
-                           344 WITH_EXCEPT_START
-                           346 POP_JUMP_FORWARD_IF_TRUE     4 (to 356)
-                           348 RERAISE                  2
-                       >>  350 COPY                     3
-                           352 POP_EXCEPT
-                           354 RERAISE                  1
-                       >>  356 POP_TOP
-                           358 POP_EXCEPT
-                           360 POP_TOP
-                           362 POP_TOP
-               
-               265     >>  364 LOAD_GLOBAL              3 (NULL + open)
-                           376 LOAD_FAST                3 (txt_file)
-                           378 LOAD_CONST               6 ('w')
-                           380 LOAD_CONST               7 ('utf-8')
-                           382 KW_NAMES                 8
-                           384 PRECALL                  3
-                           388 CALL                     3
-                           398 BEFORE_WITH
-                           400 STORE_FAST               9 (f)
-               
-               266         402 LOAD_FAST                9 (f)
-                           404 LOAD_METHOD              8 (write)
-                           426 LOAD_FAST                6 (text)
-                           428 PRECALL                  1
-                           432 CALL                     1
-                           442 POP_TOP
-               
-               267         444 LOAD_GLOBAL             18 (logger)
-                           456 LOAD_METHOD             10 (info)
-                           478 LOAD_CONST               9 ('\x1b[1;95mSuccessfully converted ')
-                           480 LOAD_FAST                2 (file_path)
-                           482 FORMAT_VALUE             0
-                           484 LOAD_CONST              10 (' to ')
-               
-               268         486 LOAD_FAST                3 (txt_file)
-               
-               267         488 FORMAT_VALUE             0
-                           490 LOAD_CONST              11 ('\x1b[0m')
-                           492 BUILD_STRING             5
-                           494 PRECALL                  1
-                           498 CALL                     1
-                           508 POP_TOP
-               
-               265         510 LOAD_CONST               0 (None)
-                           512 LOAD_CONST               0 (None)
-                           514 LOAD_CONST               0 (None)
-                           516 PRECALL                  2
-                           520 CALL                     2
-                           530 POP_TOP
-                           532 JUMP_FORWARD            11 (to 556)
-                       >>  534 PUSH_EXC_INFO
-                           536 WITH_EXCEPT_START
-                           538 POP_JUMP_FORWARD_IF_TRUE     4 (to 548)
-                           540 RERAISE                  2
-                       >>  542 COPY                     3
-                           544 POP_EXCEPT
-                           546 RERAISE                  1
-                       >>  548 POP_TOP
-                           550 POP_EXCEPT
-                           552 POP_TOP
-                           554 POP_TOP
-                       >>  556 JUMP_BACKWARD          244 (to 70)
-                       >>  558 PUSH_EXC_INFO
-               
-               269         560 LOAD_GLOBAL             22 (Exception)
-                           572 CHECK_EXC_MATCH
-                           574 POP_JUMP_FORWARD_IF_FALSE   117 (to 810)
-                           576 STORE_FAST              10 (e)
-               
-               270         578 LOAD_GLOBAL             18 (logger)
-                           590 LOAD_METHOD             12 (error)
+               278         182 LOAD_GLOBAL              9 (NULL + range)
+                           194 LOAD_GLOBAL             11 (NULL + len)
+                           206 LOAD_FAST                5 (pdf_reader)
+                           208 LOAD_ATTR                6 (pages)
+                           218 PRECALL                  1
+                           222 CALL                     1
+                           232 PRECALL                  1
+                           236 CALL                     1
+                           246 GET_ITER
+                       >>  248 FOR_ITER                38 (to 326)
+                           250 STORE_FAST               7 (page_num)
+               
+               279         252 LOAD_FAST                5 (pdf_reader)
+                           254 LOAD_ATTR                6 (pages)
+                           264 LOAD_FAST                7 (page_num)
+                           266 BINARY_SUBSCR
+                           276 STORE_FAST               8 (page)
+               
+               280         278 LOAD_FAST                6 (text)
+                           280 LOAD_FAST                8 (page)
+                           282 LOAD_METHOD              7 (extract_text)
+                           304 PRECALL                  0
+                           308 CALL                     0
+                           318 BINARY_OP               13 (+=)
+                           322 STORE_FAST               6 (text)
+                           324 JUMP_BACKWARD           39 (to 248)
+               
+               278     >>  326 NOP
+               
+               275         328 LOAD_CONST               0 (None)
+                           330 LOAD_CONST               0 (None)
+                           332 LOAD_CONST               0 (None)
+                           334 PRECALL                  2
+                           338 CALL                     2
+                           348 POP_TOP
+                           350 JUMP_FORWARD            11 (to 374)
+                       >>  352 PUSH_EXC_INFO
+                           354 WITH_EXCEPT_START
+                           356 POP_JUMP_FORWARD_IF_TRUE     4 (to 366)
+                           358 RERAISE                  2
+                       >>  360 COPY                     3
+                           362 POP_EXCEPT
+                           364 RERAISE                  1
+                       >>  366 POP_TOP
+                           368 POP_EXCEPT
+                           370 POP_TOP
+                           372 POP_TOP
                
-               271         612 LOAD_CONST              12 ('Oops somethin went astray while converting ')
-                           614 LOAD_FAST                2 (file_path)
-                           616 FORMAT_VALUE             0
-                           618 LOAD_CONST              10 (' to ')
+               281     >>  374 LOAD_GLOBAL              3 (NULL + open)
+                           386 LOAD_FAST                3 (txt_file)
+                           388 LOAD_CONST               6 ('w')
+                           390 LOAD_CONST               7 ('utf-8')
+                           392 KW_NAMES                 8
+                           394 PRECALL                  3
+                           398 CALL                     3
+                           408 BEFORE_WITH
+                           410 STORE_FAST               9 (f)
+               
+               282         412 LOAD_FAST                9 (f)
+                           414 LOAD_METHOD              8 (write)
+                           436 LOAD_FAST                6 (text)
+                           438 PRECALL                  1
+                           442 CALL                     1
+                           452 POP_TOP
                
-               272         620 LOAD_FAST                3 (txt_file)
+               283         454 LOAD_GLOBAL             18 (logger)
+                           466 LOAD_METHOD             10 (info)
+                           488 LOAD_GLOBAL             22 (DMAGENTA)
+                           500 FORMAT_VALUE             0
+                           502 LOAD_CONST               9 ('Successfully converted ')
+                           504 LOAD_FAST                2 (file_path)
+                           506 FORMAT_VALUE             0
+                           508 LOAD_CONST              10 (' to ')
+               
+               284         510 LOAD_FAST                3 (txt_file)
+               
+               283         512 FORMAT_VALUE             0
+               
+               284         514 LOAD_GLOBAL             24 (RESET)
+               
+               283         526 FORMAT_VALUE             0
+                           528 BUILD_STRING             6
+                           530 PRECALL                  1
+                           534 CALL                     1
+                           544 POP_TOP
+               
+               281         546 LOAD_CONST               0 (None)
+                           548 LOAD_CONST               0 (None)
+                           550 LOAD_CONST               0 (None)
+                           552 PRECALL                  2
+                           556 CALL                     2
+                           566 POP_TOP
+                           568 JUMP_FORWARD            11 (to 592)
+                       >>  570 PUSH_EXC_INFO
+                           572 WITH_EXCEPT_START
+                           574 POP_JUMP_FORWARD_IF_TRUE     4 (to 584)
+                           576 RERAISE                  2
+                       >>  578 COPY                     3
+                           580 POP_EXCEPT
+                           582 RERAISE                  1
+                       >>  584 POP_TOP
+                           586 POP_EXCEPT
+                           588 POP_TOP
+                           590 POP_TOP
+                       >>  592 EXTENDED_ARG             1
+                           594 JUMP_BACKWARD          263 (to 70)
+                       >>  596 PUSH_EXC_INFO
+               
+               285         598 LOAD_GLOBAL             26 (Exception)
+                           610 CHECK_EXC_MATCH
+                           612 POP_JUMP_FORWARD_IF_FALSE   117 (to 848)
+                           614 STORE_FAST              10 (e)
                
-               271         622 FORMAT_VALUE             0
-                           624 LOAD_CONST              13 (': ')
+               286         616 LOAD_GLOBAL             18 (logger)
+                           628 LOAD_METHOD             14 (error)
                
-               272         626 LOAD_FAST               10 (e)
+               287         650 LOAD_CONST              11 ('Oops somethin went astray while converting ')
+                           652 LOAD_FAST                2 (file_path)
+                           654 FORMAT_VALUE             0
+                           656 LOAD_CONST              10 (' to ')
                
-               271         628 FORMAT_VALUE             0
-                           630 BUILD_STRING             6
+               288         658 LOAD_FAST                3 (txt_file)
                
-               270         632 PRECALL                  1
-                           636 CALL                     1
-                           646 POP_TOP
+               287         660 FORMAT_VALUE             0
+                           662 LOAD_CONST              12 (': ')
                
-               273         648 LOAD_GLOBAL              3 (NULL + open)
-                           660 LOAD_CONST              14 ('conversion.log')
-                           662 LOAD_CONST              15 ('a')
-                           664 PRECALL                  2
-                           668 CALL                     2
-                           678 BEFORE_WITH
-                           680 STORE_FAST              11 (log_file)
+               288         664 LOAD_FAST               10 (e)
                
-               274         682 LOAD_FAST               11 (log_file)
-                           684 LOAD_METHOD              8 (write)
+               287         666 FORMAT_VALUE             0
+                           668 BUILD_STRING             6
+               
+               286         670 PRECALL                  1
+                           674 CALL                     1
+                           684 POP_TOP
+               
+               289         686 LOAD_GLOBAL              3 (NULL + open)
+                           698 LOAD_CONST              13 ('conversion.log')
+                           700 LOAD_CONST              14 ('a')
+                           702 PRECALL                  2
+                           706 CALL                     2
+                           716 BEFORE_WITH
+                           718 STORE_FAST              11 (log_file)
+               
+               290         720 LOAD_FAST               11 (log_file)
+                           722 LOAD_METHOD              8 (write)
+               
+               291         744 LOAD_CONST              15 ('Error converting ')
+                           746 LOAD_FAST                2 (file_path)
+                           748 FORMAT_VALUE             0
+                           750 LOAD_CONST              10 (' to ')
+                           752 LOAD_FAST                3 (txt_file)
+                           754 FORMAT_VALUE             0
+                           756 LOAD_CONST              12 (': ')
+                           758 LOAD_FAST               10 (e)
+                           760 FORMAT_VALUE             0
+                           762 LOAD_CONST              16 ('\n')
+                           764 BUILD_STRING             7
                
-               275         706 LOAD_CONST              16 ('Error converting ')
-                           708 LOAD_FAST                2 (file_path)
-                           710 FORMAT_VALUE             0
-                           712 LOAD_CONST              10 (' to ')
-                           714 LOAD_FAST                3 (txt_file)
-                           716 FORMAT_VALUE             0
-                           718 LOAD_CONST              13 (': ')
-                           720 LOAD_FAST               10 (e)
-                           722 FORMAT_VALUE             0
-                           724 LOAD_CONST              17 ('\n')
-                           726 BUILD_STRING             7
+               290         766 PRECALL                  1
+                           770 CALL                     1
+                           780 POP_TOP
                
-               274         728 PRECALL                  1
-                           732 CALL                     1
-                           742 POP_TOP
+               289         782 LOAD_CONST               0 (None)
+                           784 LOAD_CONST               0 (None)
+                           786 LOAD_CONST               0 (None)
+                           788 PRECALL                  2
+                           792 CALL                     2
+                           802 POP_TOP
+                           804 JUMP_FORWARD            11 (to 828)
+                       >>  806 PUSH_EXC_INFO
+                           808 WITH_EXCEPT_START
+                           810 POP_JUMP_FORWARD_IF_TRUE     4 (to 820)
+                           812 RERAISE                  2
+                       >>  814 COPY                     3
+                           816 POP_EXCEPT
+                           818 RERAISE                  1
+                       >>  820 POP_TOP
+                           822 POP_EXCEPT
+                           824 POP_TOP
+                           826 POP_TOP
+                       >>  828 POP_EXCEPT
+                           830 LOAD_CONST               0 (None)
+                           832 STORE_FAST              10 (e)
+                           834 DELETE_FAST             10 (e)
+                           836 EXTENDED_ARG             1
+                           838 JUMP_BACKWARD          385 (to 70)
+                       >>  840 LOAD_CONST               0 (None)
+                           842 STORE_FAST              10 (e)
+                           844 DELETE_FAST             10 (e)
+                           846 RERAISE                  1
                
-               273         744 LOAD_CONST               0 (None)
-                           746 LOAD_CONST               0 (None)
-                           748 LOAD_CONST               0 (None)
-                           750 PRECALL                  2
-                           754 CALL                     2
-                           764 POP_TOP
-                           766 JUMP_FORWARD            11 (to 790)
-                       >>  768 PUSH_EXC_INFO
-                           770 WITH_EXCEPT_START
-                           772 POP_JUMP_FORWARD_IF_TRUE     4 (to 782)
-                           774 RERAISE                  2
-                       >>  776 COPY                     3
-                           778 POP_EXCEPT
-                           780 RERAISE                  1
-                       >>  782 POP_TOP
-                           784 POP_EXCEPT
-                           786 POP_TOP
-                           788 POP_TOP
-                       >>  790 POP_EXCEPT
-                           792 LOAD_CONST               0 (None)
-                           794 STORE_FAST              10 (e)
-                           796 DELETE_FAST             10 (e)
-                           798 EXTENDED_ARG             1
-                           800 JUMP_BACKWARD          366 (to 70)
-                       >>  802 LOAD_CONST               0 (None)
-                           804 STORE_FAST              10 (e)
-                           806 DELETE_FAST             10 (e)
-                           808 RERAISE                  1
-               
-               269     >>  810 RERAISE                  0
-                       >>  812 COPY                     3
-                           814 POP_EXCEPT
-                           816 RERAISE                  1
+               285     >>  848 RERAISE                  0
+                       >>  850 COPY                     3
+                           852 POP_EXCEPT
+                           854 RERAISE                  1
                
-               256     >>  818 LOAD_CONST               0 (None)
-                           820 RETURN_VALUE
+               272     >>  856 LOAD_CONST               0 (None)
+                           858 RETURN_VALUE
                ExceptionTable:
-                 104 to 134 -> 558 [1]
-                 136 to 314 -> 342 [2] lasti
-                 318 to 340 -> 558 [1]
-                 342 to 348 -> 350 [4] lasti
-                 350 to 354 -> 558 [1]
-                 356 to 356 -> 350 [4] lasti
-                 358 to 398 -> 558 [1]
-                 400 to 508 -> 534 [2] lasti
-                 510 to 532 -> 558 [1]
-                 534 to 540 -> 542 [4] lasti
-                 542 to 546 -> 558 [1]
-                 548 to 548 -> 542 [4] lasti
-                 550 to 554 -> 558 [1]
-                 558 to 576 -> 812 [2] lasti
-                 578 to 678 -> 802 [2] lasti
-                 680 to 742 -> 768 [3] lasti
-                 744 to 766 -> 802 [2] lasti
-                 768 to 774 -> 776 [5] lasti
-                 776 to 780 -> 802 [2] lasti
-                 782 to 782 -> 776 [5] lasti
-                 784 to 788 -> 802 [2] lasti
-                 802 to 810 -> 812 [2] lasti
+                 104 to 134 -> 596 [1]
+                 136 to 324 -> 352 [2] lasti
+                 328 to 350 -> 596 [1]
+                 352 to 358 -> 360 [4] lasti
+                 360 to 364 -> 596 [1]
+                 366 to 366 -> 360 [4] lasti
+                 368 to 408 -> 596 [1]
+                 410 to 544 -> 570 [2] lasti
+                 546 to 568 -> 596 [1]
+                 570 to 576 -> 578 [4] lasti
+                 578 to 582 -> 596 [1]
+                 584 to 584 -> 578 [4] lasti
+                 586 to 590 -> 596 [1]
+                 596 to 614 -> 850 [2] lasti
+                 616 to 716 -> 840 [2] lasti
+                 718 to 780 -> 806 [3] lasti
+                 782 to 804 -> 840 [2] lasti
+                 806 to 812 -> 814 [5] lasti
+                 814 to 818 -> 840 [2] lasti
+                 820 to 820 -> 814 [5] lasti
+                 822 to 826 -> 840 [2] lasti
+                 840 to 848 -> 850 [2] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d2b7d017c01a000000000000000000000000000000000
                         0000000000a6000000ab000000000000000000a001000000000000000000
                         00000000000000000000006400a6010000ab010000000000000000af297c
                         0191028c2c5300
-                     255           0 RESUME                   0
+                     271           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                43 (to 94)
                                    8 STORE_FAST               1 (item)
                                   10 LOAD_FAST                1 (item)
                                   12 LOAD_METHOD              0 (lower)
                                   34 PRECALL                  0
@@ -2385,54 +2592,53 @@
                              >>   94 RETURN_VALUE
                      consts
                         'pdf'
                      names      ('lower', 'endswith')
                      varnames   ('.0', 'item')
                      freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 255
+                     firstlineno 271
                      lnotab 0x
                   -3
                   'txt'
                   'rb'
                   ''
                   'w'
                   'utf-8'
                   ('encoding',)
-                  '\x1b[1;95mSuccessfully converted '
+                  'Successfully converted '
                   ' to '
-                  '\x1b[0m'
                   'Oops somethin went astray while converting '
                   ': '
                   'conversion.log'
                   'a'
                   'Error converting '
                   '\n'
-               names      ('preprocess', 'open', 'PyPDF2', 'PdfReader', 'range', 'numPages', 'getPage', 'extractText', 'write', 'logger', 'info', 'Exception', 'error')
+               names      ('preprocess', 'open', 'PyPDF2', 'PdfReader', 'range', 'len', 'pages', 'extract_text', 'write', 'logger', 'info', 'DMAGENTA', 'RESET', 'Exception', 'error')
                varnames   ('self', 'pdf_list', 'file_path', 'txt_file', 'file', 'pdf_reader', 'text', 'page_num', 'page', 'f', 'e', 'log_file')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'pdf_to_txt'
-               firstlineno 253
+               firstlineno 269
                lnotab
-                  0x0201280118010a011a0102012201280104012c012a0130fe02fd2e0626
-                  012a012a0102ff16fe320412012201080102ff040102ff04ff1003220118
-                  0116ff10ff42fc08f3
+                  0x0201280118010a011a01020122012801040146011a0130fe02fd2e0626
+                  012a01380102ff02010cff14fe340412012201080102ff040102ff04ff10
+                  032201180116ff10ff42fc08f3
             code
                argcount  : 1
                nlocals   : 15
                stacksize : 12
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d01640184007c014400a6000000ab00000000
-                  00000000007d017c01440090025d4c7d027c02a001000000000000000000
+                  00000000007d017c01440090025d597d027c02a001000000000000000000
                   0000000000000000000000a6000000ab000000000000000000a002000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   000000720e7c026400640385021900000000000000000064047a0000007d
                   036e347c02a0010000000000000000000000000000000000000000a60000
                   00ab000000000000000000a0020000000000000000000000000000000000
                   0000006405a6010000ab010000000000000000720d7c0264006406850219
                   00000000000000000064047a0000007d0309007407000000000000000000
@@ -2453,539 +2659,546 @@
                   005f13000000000000000009007c0b6a0e00000000000000006a14000000
                   00000000006a1500000000000000007c0c6a0e00000000000000006a1400
                   000000000000005f1500000000000000008c9d2300742c00000000000000
                   00000024007203010059008ca977007803590077018ccb7c05a00a000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0001008cf790018c037c05a0170000000000000000000000000000000000
                   0000007c03a6010000ab0100000000000000000100743000000000000000
-                  000000a019000000000000000000000000000000000000000064077c029b
-                  0064087c039b0064099d05a6010000ab010000000000000000010090018c
-                  cc2300743400000000000000000000240072757d0d743000000000000000
-                  000000a01b0000000000000000000000000000000000000000640a7c029b
-                  00640b7c039b00640c7c0d9b009d06a6010000ab01000000000000000001
-                  00743900000000000000000000640d640ea6020000ab0200000000000000
-                  0035007d0e7c0ea01d000000000000000000000000000000000000000064
-                  0f7c029b00640b7c039b0064107c0d9b0064119d07a6010000ab01000000
-                  00000000000100640064006400a6020000ab02000000000000000001006e
-                  0b23003100730477027803590077010100590001000100590064007d0d7e
-                  0d90028c4664007d0d7e0d7701770078035900770164005300
-               280           0 RESUME                   0
+                  000000a01900000000000000000000000000000000000000007434000000
+                  000000000000009b0064077c029b0064087c039b00743600000000000000
+                  0000009b009d06a6010000ab010000000000000000010090018cd9230074
+                  3800000000000000000000240072757d0d743000000000000000000000a0
+                  1d000000000000000000000000000000000000000064097c029b00640a7c
+                  039b00640b7c0d9b009d06a6010000ab0100000000000000000100743d00
+                  000000000000000000640c640da6020000ab02000000000000000035007d
+                  0e7c0ea01f0000000000000000000000000000000000000000640e7c029b
+                  00640a7c039b00640f7c0d9b0064109d07a6010000ab0100000000000000
+                  000100640064006400a6020000ab02000000000000000001006e0b230031
+                  00730477027803590077010100590001000100590064007d0d7e0d90028c
+                  5364007d0d7e0d7701770078035900770164005300
+               296           0 RESUME                   0
                
-               281           2 LOAD_FAST                0 (self)
+               297           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (preprocess)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (ppt_list)
                
-               282          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 282>)
+               298          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 298>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                1 (ppt_list)
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               1 (ppt_list)
                
-               284          66 LOAD_FAST                1 (ppt_list)
+               300          66 LOAD_FAST                1 (ppt_list)
                             68 GET_ITER
                        >>   70 EXTENDED_ARG             2
-                            72 FOR_ITER               588 (to 1250)
+                            72 FOR_ITER               601 (to 1276)
                             74 STORE_FAST               2 (file_path)
                
-               285          76 LOAD_FAST                2 (file_path)
+               301          76 LOAD_FAST                2 (file_path)
                             78 LOAD_METHOD              1 (lower)
                            100 PRECALL                  0
                            104 CALL                     0
                            114 LOAD_METHOD              2 (endswith)
                            136 LOAD_CONST               2 ('pptx')
                            138 PRECALL                  1
                            142 CALL                     1
                            152 POP_JUMP_FORWARD_IF_FALSE    14 (to 182)
                
-               286         154 LOAD_FAST                2 (file_path)
+               302         154 LOAD_FAST                2 (file_path)
                            156 LOAD_CONST               0 (None)
                            158 LOAD_CONST               3 (-4)
                            160 BUILD_SLICE              2
                            162 BINARY_SUBSCR
                            172 LOAD_CONST               4 ('docx')
                            174 BINARY_OP                0 (+)
                            178 STORE_FAST               3 (word_file)
                            180 JUMP_FORWARD            52 (to 286)
                
-               287     >>  182 LOAD_FAST                2 (file_path)
+               303     >>  182 LOAD_FAST                2 (file_path)
                            184 LOAD_METHOD              1 (lower)
                            206 PRECALL                  0
                            210 CALL                     0
                            220 LOAD_METHOD              2 (endswith)
                            242 LOAD_CONST               5 ('ppt')
                            244 PRECALL                  1
                            248 CALL                     1
                            258 POP_JUMP_FORWARD_IF_FALSE    13 (to 286)
                
-               288         260 LOAD_FAST                2 (file_path)
+               304         260 LOAD_FAST                2 (file_path)
                            262 LOAD_CONST               0 (None)
                            264 LOAD_CONST               6 (-3)
                            266 BUILD_SLICE              2
                            268 BINARY_SUBSCR
                            278 LOAD_CONST               4 ('docx')
                            280 BINARY_OP                0 (+)
                            284 STORE_FAST               3 (word_file)
                
-               289     >>  286 NOP
+               305     >>  286 NOP
                
-               290         288 LOAD_GLOBAL              7 (NULL + Presentation)
+               306         288 LOAD_GLOBAL              7 (NULL + Presentation)
                            300 LOAD_FAST                2 (file_path)
                            302 PRECALL                  1
                            306 CALL                     1
                            316 STORE_FAST               4 (presentation)
                
-               291         318 LOAD_GLOBAL              9 (NULL + Document)
+               307         318 LOAD_GLOBAL              9 (NULL + Document)
                            330 PRECALL                  0
                            334 CALL                     0
                            344 STORE_FAST               5 (document)
                
-               293         346 LOAD_FAST                4 (presentation)
+               309         346 LOAD_FAST                4 (presentation)
                            348 LOAD_ATTR                5 (slides)
                            358 GET_ITER
                        >>  360 EXTENDED_ARG             1
                            362 FOR_ITER               257 (to 878)
                            364 STORE_FAST               6 (slide)
                
-               294         366 LOAD_FAST                6 (slide)
+               310         366 LOAD_FAST                6 (slide)
                            368 LOAD_ATTR                6 (shapes)
                            378 GET_ITER
                        >>  380 FOR_ITER               246 (to 874)
                            382 STORE_FAST               7 (shape)
                
-               295         384 LOAD_FAST                7 (shape)
+               311         384 LOAD_FAST                7 (shape)
                            386 LOAD_ATTR                7 (has_text_frame)
                            396 POP_JUMP_FORWARD_IF_FALSE   237 (to 872)
                
-               296         398 LOAD_FAST                7 (shape)
+               312         398 LOAD_FAST                7 (shape)
                            400 LOAD_ATTR                8 (text_frame)
                            410 STORE_FAST               8 (text_frame)
                
-               297         412 LOAD_FAST                8 (text_frame)
+               313         412 LOAD_FAST                8 (text_frame)
                            414 LOAD_ATTR                9 (paragraphs)
                            424 GET_ITER
                        >>  426 FOR_ITER               202 (to 832)
                            428 STORE_FAST               9 (paragraph)
                
-               298         430 LOAD_FAST                5 (document)
+               314         430 LOAD_FAST                5 (document)
                            432 LOAD_METHOD             10 (add_paragraph)
                            454 PRECALL                  0
                            458 CALL                     0
                            468 STORE_FAST              10 (new_paragraph)
                
-               299         470 LOAD_FAST                9 (paragraph)
+               315         470 LOAD_FAST                9 (paragraph)
                            472 LOAD_ATTR               11 (runs)
                            482 GET_ITER
                        >>  484 FOR_ITER               172 (to 830)
                            486 STORE_FAST              11 (run)
                
-               300         488 LOAD_FAST               10 (new_paragraph)
+               316         488 LOAD_FAST               10 (new_paragraph)
                            490 LOAD_METHOD             12 (add_run)
                            512 LOAD_FAST               11 (run)
                            514 LOAD_ATTR               13 (text)
                            524 PRECALL                  1
                            528 CALL                     1
                            538 STORE_FAST              12 (new_run)
                
-               302         540 LOAD_FAST               11 (run)
+               318         540 LOAD_FAST               11 (run)
                            542 LOAD_ATTR               14 (font)
                            552 LOAD_ATTR               15 (bold)
                            562 LOAD_FAST               12 (new_run)
                            564 STORE_ATTR              15 (bold)
                
-               304         574 LOAD_FAST               11 (run)
+               320         574 LOAD_FAST               11 (run)
                            576 LOAD_ATTR               14 (font)
                            586 LOAD_ATTR               16 (italic)
                            596 LOAD_FAST               12 (new_run)
                            598 STORE_ATTR              16 (italic)
                
-               306         608 LOAD_FAST               11 (run)
+               322         608 LOAD_FAST               11 (run)
                            610 LOAD_ATTR               14 (font)
                            620 LOAD_ATTR               17 (underline)
                            630 LOAD_FAST               12 (new_run)
                            632 STORE_ATTR              17 (underline)
                
-               308         642 LOAD_FAST               11 (run)
+               324         642 LOAD_FAST               11 (run)
                            644 LOAD_ATTR               14 (font)
                            654 LOAD_ATTR               18 (name)
                            664 LOAD_FAST               12 (new_run)
                            666 LOAD_ATTR               14 (font)
                            676 STORE_ATTR              18 (name)
                
-               310         686 LOAD_FAST               11 (run)
+               326         686 LOAD_FAST               11 (run)
                            688 LOAD_ATTR               14 (font)
                            698 LOAD_ATTR               19 (size)
                            708 LOAD_FAST               12 (new_run)
                            710 LOAD_ATTR               14 (font)
                            720 STORE_ATTR              19 (size)
                
-               311         730 NOP
+               327         730 NOP
                
-               313         732 LOAD_FAST               11 (run)
+               329         732 LOAD_FAST               11 (run)
                            734 LOAD_ATTR               14 (font)
                            744 LOAD_ATTR               20 (color)
                            754 LOAD_ATTR               21 (rgb)
                            764 LOAD_FAST               12 (new_run)
                            766 LOAD_ATTR               14 (font)
                            776 LOAD_ATTR               20 (color)
                            786 STORE_ATTR              21 (rgb)
                            796 JUMP_BACKWARD          157 (to 484)
                        >>  798 PUSH_EXC_INFO
                
-               314         800 LOAD_GLOBAL             44 (AttributeError)
+               330         800 LOAD_GLOBAL             44 (AttributeError)
                            812 CHECK_EXC_MATCH
                            814 POP_JUMP_FORWARD_IF_FALSE     3 (to 822)
                            816 POP_TOP
                
-               317         818 POP_EXCEPT
+               333         818 POP_EXCEPT
                            820 JUMP_BACKWARD          169 (to 484)
                
-               314     >>  822 RERAISE                  0
+               330     >>  822 RERAISE                  0
                        >>  824 COPY                     3
                            826 POP_EXCEPT
                            828 RERAISE                  1
                
-               299     >>  830 JUMP_BACKWARD          203 (to 426)
+               315     >>  830 JUMP_BACKWARD          203 (to 426)
                
-               319     >>  832 LOAD_FAST                5 (document)
+               335     >>  832 LOAD_FAST                5 (document)
                            834 LOAD_METHOD             10 (add_paragraph)
                            856 PRECALL                  0
                            860 CALL                     0
                            870 POP_TOP
                        >>  872 JUMP_BACKWARD          247 (to 380)
                
-               294     >>  874 EXTENDED_ARG             1
+               310     >>  874 EXTENDED_ARG             1
                            876 JUMP_BACKWARD          259 (to 360)
                
-               320     >>  878 LOAD_FAST                5 (document)
+               336     >>  878 LOAD_FAST                5 (document)
                            880 LOAD_METHOD             23 (save)
                            902 LOAD_FAST                3 (word_file)
                            904 PRECALL                  1
                            908 CALL                     1
                            918 POP_TOP
                
-               321         920 LOAD_GLOBAL             48 (logger)
+               337         920 LOAD_GLOBAL             48 (logger)
                            932 LOAD_METHOD             25 (info)
-                           954 LOAD_CONST               7 ('\x1b[1;95mSuccessfully converted ')
-                           956 LOAD_FAST                2 (file_path)
-                           958 FORMAT_VALUE             0
-                           960 LOAD_CONST               8 (' to         ')
-               
-               322         962 LOAD_FAST                3 (word_file)
-               
-               321         964 FORMAT_VALUE             0
-                           966 LOAD_CONST               9 ('\x1b[0m')
-                           968 BUILD_STRING             5
-                           970 PRECALL                  1
-                           974 CALL                     1
-                           984 POP_TOP
-                           986 EXTENDED_ARG             1
-                           988 JUMP_BACKWARD          460 (to 70)
-                       >>  990 PUSH_EXC_INFO
-               
-               323         992 LOAD_GLOBAL             52 (Exception)
-                          1004 CHECK_EXC_MATCH
-                          1006 POP_JUMP_FORWARD_IF_FALSE   117 (to 1242)
-                          1008 STORE_FAST              13 (e)
-               
-               324        1010 LOAD_GLOBAL             48 (logger)
-                          1022 LOAD_METHOD             27 (error)
-               
-               325        1044 LOAD_CONST              10 ('Oops somethin gwent awry while attempting to convert         ')
-               
-               326        1046 LOAD_FAST                2 (file_path)
-               
-               325        1048 FORMAT_VALUE             0
-                          1050 LOAD_CONST              11 (' to ')
-               
-               326        1052 LOAD_FAST                3 (word_file)
-               
-               325        1054 FORMAT_VALUE             0
-                          1056 LOAD_CONST              12 (':\n>>>')
-               
-               326        1058 LOAD_FAST               13 (e)
-               
-               325        1060 FORMAT_VALUE             0
-                          1062 BUILD_STRING             6
-               
-               324        1064 PRECALL                  1
-                          1068 CALL                     1
-                          1078 POP_TOP
-               
-               327        1080 LOAD_GLOBAL             57 (NULL + open)
-                          1092 LOAD_CONST              13 ('conversion.log')
-                          1094 LOAD_CONST              14 ('a')
-                          1096 PRECALL                  2
-                          1100 CALL                     2
-                          1110 BEFORE_WITH
-                          1112 STORE_FAST              14 (log_file)
-               
-               328        1114 LOAD_FAST               14 (log_file)
-                          1116 LOAD_METHOD             29 (write)
-               
-               329        1138 LOAD_CONST              15 ('Oops something went astray while attempting         convert ')
-               
-               330        1140 LOAD_FAST                2 (file_path)
+                           954 LOAD_GLOBAL             52 (DMAGENTA)
+                           966 FORMAT_VALUE             0
+                           968 LOAD_CONST               7 ('Successfully converted ')
+                           970 LOAD_FAST                2 (file_path)
+                           972 FORMAT_VALUE             0
+                           974 LOAD_CONST               8 (' to         ')
+               
+               338         976 LOAD_FAST                3 (word_file)
+               
+               337         978 FORMAT_VALUE             0
+               
+               338         980 LOAD_GLOBAL             54 (RESET)
+               
+               337         992 FORMAT_VALUE             0
+                           994 BUILD_STRING             6
+                           996 PRECALL                  1
+                          1000 CALL                     1
+                          1010 POP_TOP
+                          1012 EXTENDED_ARG             1
+                          1014 JUMP_BACKWARD          473 (to 70)
+                       >> 1016 PUSH_EXC_INFO
+               
+               339        1018 LOAD_GLOBAL             56 (Exception)
+                          1030 CHECK_EXC_MATCH
+                          1032 POP_JUMP_FORWARD_IF_FALSE   117 (to 1268)
+                          1034 STORE_FAST              13 (e)
+               
+               340        1036 LOAD_GLOBAL             48 (logger)
+                          1048 LOAD_METHOD             29 (error)
+               
+               341        1070 LOAD_CONST               9 ('Oops somethin gwent awry while attempting to convert         ')
+               
+               342        1072 LOAD_FAST                2 (file_path)
+               
+               341        1074 FORMAT_VALUE             0
+                          1076 LOAD_CONST              10 (' to ')
+               
+               342        1078 LOAD_FAST                3 (word_file)
+               
+               341        1080 FORMAT_VALUE             0
+                          1082 LOAD_CONST              11 (':\n>>>')
+               
+               342        1084 LOAD_FAST               13 (e)
+               
+               341        1086 FORMAT_VALUE             0
+                          1088 BUILD_STRING             6
+               
+               340        1090 PRECALL                  1
+                          1094 CALL                     1
+                          1104 POP_TOP
+               
+               343        1106 LOAD_GLOBAL             61 (NULL + open)
+                          1118 LOAD_CONST              12 ('conversion.log')
+                          1120 LOAD_CONST              13 ('a')
+                          1122 PRECALL                  2
+                          1126 CALL                     2
+                          1136 BEFORE_WITH
+                          1138 STORE_FAST              14 (log_file)
+               
+               344        1140 LOAD_FAST               14 (log_file)
+                          1142 LOAD_METHOD             31 (write)
+               
+               345        1164 LOAD_CONST              14 ('Oops something went astray while attempting         convert ')
+               
+               346        1166 LOAD_FAST                2 (file_path)
+               
+               345        1168 FORMAT_VALUE             0
+                          1170 LOAD_CONST              10 (' to ')
+               
+               346        1172 LOAD_FAST                3 (word_file)
+               
+               345        1174 FORMAT_VALUE             0
+                          1176 LOAD_CONST              15 (':')
+               
+               346        1178 LOAD_FAST               13 (e)
+               
+               345        1180 FORMAT_VALUE             0
+                          1182 LOAD_CONST              16 ('\n')
+                          1184 BUILD_STRING             7
+               
+               344        1186 PRECALL                  1
+                          1190 CALL                     1
+                          1200 POP_TOP
+               
+               343        1202 LOAD_CONST               0 (None)
+                          1204 LOAD_CONST               0 (None)
+                          1206 LOAD_CONST               0 (None)
+                          1208 PRECALL                  2
+                          1212 CALL                     2
+                          1222 POP_TOP
+                          1224 JUMP_FORWARD            11 (to 1248)
+                       >> 1226 PUSH_EXC_INFO
+                          1228 WITH_EXCEPT_START
+                          1230 POP_JUMP_FORWARD_IF_TRUE     4 (to 1240)
+                          1232 RERAISE                  2
+                       >> 1234 COPY                     3
+                          1236 POP_EXCEPT
+                          1238 RERAISE                  1
+                       >> 1240 POP_TOP
+                          1242 POP_EXCEPT
+                          1244 POP_TOP
+                          1246 POP_TOP
+                       >> 1248 POP_EXCEPT
+                          1250 LOAD_CONST               0 (None)
+                          1252 STORE_FAST              13 (e)
+                          1254 DELETE_FAST             13 (e)
+                          1256 EXTENDED_ARG             2
+                          1258 JUMP_BACKWARD          595 (to 70)
+                       >> 1260 LOAD_CONST               0 (None)
+                          1262 STORE_FAST              13 (e)
+                          1264 DELETE_FAST             13 (e)
+                          1266 RERAISE                  1
+               
+               339     >> 1268 RERAISE                  0
+                       >> 1270 COPY                     3
+                          1272 POP_EXCEPT
+                          1274 RERAISE                  1
                
-               329        1142 FORMAT_VALUE             0
-                          1144 LOAD_CONST              11 (' to ')
-               
-               330        1146 LOAD_FAST                3 (word_file)
-               
-               329        1148 FORMAT_VALUE             0
-                          1150 LOAD_CONST              16 (':')
-               
-               330        1152 LOAD_FAST               13 (e)
-               
-               329        1154 FORMAT_VALUE             0
-                          1156 LOAD_CONST              17 ('\n')
-                          1158 BUILD_STRING             7
-               
-               328        1160 PRECALL                  1
-                          1164 CALL                     1
-                          1174 POP_TOP
-               
-               327        1176 LOAD_CONST               0 (None)
-                          1178 LOAD_CONST               0 (None)
-                          1180 LOAD_CONST               0 (None)
-                          1182 PRECALL                  2
-                          1186 CALL                     2
-                          1196 POP_TOP
-                          1198 JUMP_FORWARD            11 (to 1222)
-                       >> 1200 PUSH_EXC_INFO
-                          1202 WITH_EXCEPT_START
-                          1204 POP_JUMP_FORWARD_IF_TRUE     4 (to 1214)
-                          1206 RERAISE                  2
-                       >> 1208 COPY                     3
-                          1210 POP_EXCEPT
-                          1212 RERAISE                  1
-                       >> 1214 POP_TOP
-                          1216 POP_EXCEPT
-                          1218 POP_TOP
-                          1220 POP_TOP
-                       >> 1222 POP_EXCEPT
-                          1224 LOAD_CONST               0 (None)
-                          1226 STORE_FAST              13 (e)
-                          1228 DELETE_FAST             13 (e)
-                          1230 EXTENDED_ARG             2
-                          1232 JUMP_BACKWARD          582 (to 70)
-                       >> 1234 LOAD_CONST               0 (None)
-                          1236 STORE_FAST              13 (e)
-                          1238 DELETE_FAST             13 (e)
-                          1240 RERAISE                  1
-               
-               323     >> 1242 RERAISE                  0
-                       >> 1244 COPY                     3
-                          1246 POP_EXCEPT
-                          1248 RERAISE                  1
-               
-               284     >> 1250 LOAD_CONST               0 (None)
-                          1252 RETURN_VALUE
+               300     >> 1276 LOAD_CONST               0 (None)
+                          1278 RETURN_VALUE
                ExceptionTable:
-                 288 to 728 -> 990 [1]
+                 288 to 728 -> 1016 [1]
                  732 to 794 -> 798 [5]
-                 796 to 796 -> 990 [1]
+                 796 to 796 -> 1016 [1]
                  798 to 816 -> 824 [6] lasti
-                 818 to 820 -> 990 [1]
+                 818 to 820 -> 1016 [1]
                  822 to 822 -> 824 [6] lasti
-                 824 to 984 -> 990 [1]
-                 990 to 1008 -> 1244 [2] lasti
-                 1010 to 1110 -> 1234 [2] lasti
-                 1112 to 1174 -> 1200 [3] lasti
-                 1176 to 1198 -> 1234 [2] lasti
-                 1200 to 1206 -> 1208 [5] lasti
-                 1208 to 1212 -> 1234 [2] lasti
-                 1214 to 1214 -> 1208 [5] lasti
-                 1216 to 1220 -> 1234 [2] lasti
-                 1234 to 1242 -> 1244 [2] lasti
+                 824 to 1010 -> 1016 [1]
+                 1016 to 1034 -> 1270 [2] lasti
+                 1036 to 1136 -> 1260 [2] lasti
+                 1138 to 1200 -> 1226 [3] lasti
+                 1202 to 1224 -> 1260 [2] lasti
+                 1226 to 1232 -> 1234 [5] lasti
+                 1234 to 1238 -> 1260 [2] lasti
+                 1240 to 1240 -> 1234 [5] lasti
+                 1242 to 1246 -> 1260 [2] lasti
+                 1260 to 1268 -> 1270 [2] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d527d017c01a000000000000000000000000000000000
                         0000000000a6000000ab000000000000000000a001000000000000000000
                         00000000000000000000006400a6010000ab01000000000000000073277c
                         01a0000000000000000000000000000000000000000000a6000000ab0000
                         00000000000000a001000000000000000000000000000000000000000064
                         01a6010000ab010000000000000000af507c0191028c535300
-                     282           0 RESUME                   0
+                     298           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                82 (to 172)
                                    8 STORE_FAST               1 (item)
                                   10 LOAD_FAST                1 (item)
                                   12 LOAD_METHOD              0 (lower)
                                   34 PRECALL                  0
                                   38 CALL                     0
                                   48 LOAD_METHOD              1 (endswith)
                      
-                     283          70 LOAD_CONST               0 ('pptx')
+                     299          70 LOAD_CONST               0 ('pptx')
                      
-                     282          72 PRECALL                  1
+                     298          72 PRECALL                  1
                                   76 CALL                     1
                                   86 POP_JUMP_FORWARD_IF_TRUE    39 (to 166)
                      
-                     283          88 LOAD_FAST                1 (item)
+                     299          88 LOAD_FAST                1 (item)
                                   90 LOAD_METHOD              0 (lower)
                                  112 PRECALL                  0
                                  116 CALL                     0
                                  126 LOAD_METHOD              1 (endswith)
                                  148 LOAD_CONST               1 ('ppt')
                                  150 PRECALL                  1
                                  154 CALL                     1
                      
-                     282         164 POP_JUMP_BACKWARD_IF_FALSE    80 (to 6)
+                     298         164 POP_JUMP_BACKWARD_IF_FALSE    80 (to 6)
                              >>  166 LOAD_FAST                1 (item)
                                  168 LIST_APPEND              2
                                  170 JUMP_BACKWARD           83 (to 6)
                              >>  172 RETURN_VALUE
                      consts
                         'pptx'
                         'ppt'
                      names      ('lower', 'endswith')
                      varnames   ('.0', 'item')
                      freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 282
+                     firstlineno 298
                      lnotab 0x460102ff10014cff
                   'pptx'
                   -4
                   'docx'
                   'ppt'
                   -3
-                  '\x1b[1;95mSuccessfully converted '
+                  'Successfully converted '
                   ' to         '
-                  '\x1b[0m'
                   'Oops somethin gwent awry while attempting to convert         '
                   ' to '
                   ':\n>>>'
                   'conversion.log'
                   'a'
                   'Oops something went astray while attempting         convert '
                   ':'
                   '\n'
-               names      ('preprocess', 'lower', 'endswith', 'Presentation', 'Document', 'slides', 'shapes', 'has_text_frame', 'text_frame', 'paragraphs', 'add_paragraph', 'runs', 'add_run', 'text', 'font', 'bold', 'italic', 'underline', 'name', 'size', 'color', 'rgb', 'AttributeError', 'save', 'logger', 'info', 'Exception', 'error', 'open', 'write')
+               names      ('preprocess', 'lower', 'endswith', 'Presentation', 'Document', 'slides', 'shapes', 'has_text_frame', 'text_frame', 'paragraphs', 'add_paragraph', 'runs', 'add_run', 'text', 'font', 'bold', 'italic', 'underline', 'name', 'size', 'color', 'rgb', 'AttributeError', 'save', 'logger', 'info', 'DMAGENTA', 'RESET', 'Exception', 'error', 'open', 'write')
                varnames   ('self', 'ppt_list', 'file_path', 'word_file', 'presentation', 'document', 'slide', 'shape', 'text_frame', 'paragraph', 'new_paragraph', 'run', 'new_run', 'e', 'log_file')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'ppt_to_word'
-               firstlineno 280
+               firstlineno 296
                lnotab
                   0x0201280118020a014e011c014e011a0102011e011c02140112010e010e
                   0112012801120134022202220222022c022c0102024401120304fd08f102
-                  142ae7041a2a012a0102ff1c0212012201020102ff040102ff040102ff04
-                  ff100322011801020102ff040102ff040102ff06ff10ff42fc08d9
+                  142ae7041a2a01380102ff02010cff1a0212012201020102ff040102ff04
+                  0102ff04ff100322011801020102ff040102ff040102ff06ff10ff42fc08
+                  d9
             code
                argcount  : 1
                nlocals   : 10
                stacksize : 12
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d01640184007c014400a6000000ab00000000
-                  00000000007d017c01440090015d9d7d027c02a001000000000000000000
+                  00000000007d017c01440090015daa7d027c02a001000000000000000000
                   0000000000000000000000a6000000ab000000000000000000a002000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   000000720d7c026400640385021900000000000000000064047a0000007d
                   0309007407000000000000000000007c02640564066407ac08a6040000ab
                   04000000000000000035007d047c04a00400000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d05640064006400a6
                   020000ab02000000000000000001006e0b23003100730477027803590077
                   010100590001000100740b000000000000000000006a0600000000000000
                   006409640a7c05a6030000ab0300000000000000007d06740f0000000000
                   0000000000a6000000ab0000000000000000007d077c07a0080000000000
                   0000000000000000000000000000007c06a6010000ab0100000000000000
                   0001007c07a00900000000000000000000000000000000000000007c03a6
                   010000ab0100000000000000000100741400000000000000000000a00b00
-                  00000000000000000000000000000000000000640b7c029b00640c7c039b
-                  00640d9d05a6010000ab01000000000000000001008ce723007418000000
-                  00000000000000240072337d08741400000000000000000000a00d000000
-                  0000000000000000000000000000000000741d000000000000000000007c
-                  08a6010000ab0100000000000000009b00a6010000ab0100000000000000
-                  000100590064007d087e0890018c1f64007d087e087701741e0000000000
-                  0000000000240072707d08741400000000000000000000a00d0000000000
-                  000000000000000000000000000000640e7c089b00640f9d03a6010000ab
-                  010000000000000000010074070000000000000000000064106411a60200
-                  00ab02000000000000000035007d097c09a0100000000000000000000000
-                  00000000000000000064127c029b0064137c039b0064147c089b00640f9d
-                  07a6010000ab0100000000000000000100640064006400a6020000ab0200
-                  0000000000000001006e0b23003100730477027803590077010100590001
-                  000100590064007d087e0890018c9764007d087e08770177007803590077
-                  0164005300
-               335           0 RESUME                   0
+                  000000000000000000000000000000000000007418000000000000000000
+                  009b00640b7c029b00640c7c039b00741a000000000000000000009b009d
+                  06a6010000ab01000000000000000001008cf42300741c00000000000000
+                  000000240072337d08741400000000000000000000a00f00000000000000
+                  000000000000000000000000007421000000000000000000007c08a60100
+                  00ab0100000000000000009b00a6010000ab010000000000000000010059
+                  0064007d087e0890018c2c64007d087e0877017422000000000000000000
+                  00240072707d08741400000000000000000000a00f000000000000000000
+                  0000000000000000000000640d7c089b00640e9d03a6010000ab01000000
+                  00000000000100740700000000000000000000640f6410a6020000ab0200
+                  0000000000000035007d097c09a012000000000000000000000000000000
+                  000000000064117c029b0064127c039b0064137c089b00640e9d07a60100
+                  00ab0100000000000000000100640064006400a6020000ab020000000000
+                  00000001006e0b2300310073047702780359007701010059000100010059
+                  0064007d087e0890018ca464007d087e0877017700780359007701640053
+                  00
+               351           0 RESUME                   0
                
-               336           2 LOAD_FAST                0 (self)
+               352           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (preprocess)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (flist)
                
-               337          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 337>)
+               353          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 353>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                1 (flist)
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               1 (flist)
                
-               338          66 LOAD_FAST                1 (flist)
+               354          66 LOAD_FAST                1 (flist)
                             68 GET_ITER
                        >>   70 EXTENDED_ARG             1
-                            72 FOR_ITER               413 (to 900)
+                            72 FOR_ITER               426 (to 926)
                             74 STORE_FAST               2 (file_path)
                
-               339          76 LOAD_FAST                2 (file_path)
+               355          76 LOAD_FAST                2 (file_path)
                             78 LOAD_METHOD              1 (lower)
                            100 PRECALL                  0
                            104 CALL                     0
                            114 LOAD_METHOD              2 (endswith)
                            136 LOAD_CONST               2 ('txt')
                            138 PRECALL                  1
                            142 CALL                     1
                            152 POP_JUMP_FORWARD_IF_FALSE    13 (to 180)
                
-               340         154 LOAD_FAST                2 (file_path)
+               356         154 LOAD_FAST                2 (file_path)
                            156 LOAD_CONST               0 (None)
                            158 LOAD_CONST               3 (-3)
                            160 BUILD_SLICE              2
                            162 BINARY_SUBSCR
                            172 LOAD_CONST               4 ('docx')
                            174 BINARY_OP                0 (+)
                            178 STORE_FAST               3 (word_file)
                
-               342     >>  180 NOP
+               358     >>  180 NOP
                
-               344         182 LOAD_GLOBAL              7 (NULL + open)
+               360         182 LOAD_GLOBAL              7 (NULL + open)
                            194 LOAD_FAST                2 (file_path)
                            196 LOAD_CONST               5 ('r')
                            198 LOAD_CONST               6 ('utf-8')
                            200 LOAD_CONST               7 ('ignore')
                            202 KW_NAMES                 8
                            204 PRECALL                  4
                            208 CALL                     4
                            218 BEFORE_WITH
                            220 STORE_FAST               4 (file)
                
-               345         222 LOAD_FAST                4 (file)
+               361         222 LOAD_FAST                4 (file)
                            224 LOAD_METHOD              4 (read)
                            246 PRECALL                  0
                            250 CALL                     0
                            260 STORE_FAST               5 (text_content)
                
-               344         262 LOAD_CONST               0 (None)
+               360         262 LOAD_CONST               0 (None)
                            264 LOAD_CONST               0 (None)
                            266 LOAD_CONST               0 (None)
                            268 PRECALL                  2
                            272 CALL                     2
                            282 POP_TOP
                            284 JUMP_FORWARD            11 (to 308)
                        >>  286 PUSH_EXC_INFO
@@ -2996,203 +3209,208 @@
                            296 POP_EXCEPT
                            298 RERAISE                  1
                        >>  300 POP_TOP
                            302 POP_EXCEPT
                            304 POP_TOP
                            306 POP_TOP
                
-               348     >>  308 LOAD_GLOBAL             11 (NULL + re)
+               364     >>  308 LOAD_GLOBAL             11 (NULL + re)
                            320 LOAD_ATTR                6 (sub)
                
-               349         330 LOAD_CONST               9 ('[^\\x09\\x0A\\x0D\\x20-\\uD7FF\\uE000-\\uFFFD]+')
+               365         330 LOAD_CONST               9 ('[^\\x09\\x0A\\x0D\\x20-\\uD7FF\\uE000-\\uFFFD]+')
                            332 LOAD_CONST              10 ('')
                            334 LOAD_FAST                5 (text_content)
                
-               348         336 PRECALL                  3
+               364         336 PRECALL                  3
                            340 CALL                     3
                            350 STORE_FAST               6 (filtered_content)
                
-               352         352 LOAD_GLOBAL             15 (NULL + Document)
+               368         352 LOAD_GLOBAL             15 (NULL + Document)
                            364 PRECALL                  0
                            368 CALL                     0
                            378 STORE_FAST               7 (doc)
                
-               354         380 LOAD_FAST                7 (doc)
+               370         380 LOAD_FAST                7 (doc)
                            382 LOAD_METHOD              8 (add_paragraph)
                            404 LOAD_FAST                6 (filtered_content)
                            406 PRECALL                  1
                            410 CALL                     1
                            420 POP_TOP
                
-               357         422 LOAD_FAST                7 (doc)
+               373         422 LOAD_FAST                7 (doc)
                            424 LOAD_METHOD              9 (save)
                            446 LOAD_FAST                3 (word_file)
                            448 PRECALL                  1
                            452 CALL                     1
                            462 POP_TOP
                
-               358         464 LOAD_GLOBAL             20 (logger)
+               374         464 LOAD_GLOBAL             20 (logger)
                            476 LOAD_METHOD             11 (info)
-                           498 LOAD_CONST              11 ('\x1b[1;95mSuccessfully converted ')
-                           500 LOAD_FAST                2 (file_path)
-                           502 FORMAT_VALUE             0
-                           504 LOAD_CONST              12 (' to         ')
+                           498 LOAD_GLOBAL             24 (DMAGENTA)
+                           510 FORMAT_VALUE             0
+                           512 LOAD_CONST              11 ('Successfully converted ')
+                           514 LOAD_FAST                2 (file_path)
+                           516 FORMAT_VALUE             0
+                           518 LOAD_CONST              12 (' to         ')
                
-               359         506 LOAD_FAST                3 (word_file)
+               375         520 LOAD_FAST                3 (word_file)
                
-               358         508 FORMAT_VALUE             0
-                           510 LOAD_CONST              13 ('\x1b[0m')
-                           512 BUILD_STRING             5
-                           514 PRECALL                  1
-                           518 CALL                     1
-                           528 POP_TOP
-                           530 JUMP_BACKWARD          231 (to 70)
-                       >>  532 PUSH_EXC_INFO
-               
-               360         534 LOAD_GLOBAL             24 (FileExistsError)
-                           546 CHECK_EXC_MATCH
-                           548 POP_JUMP_FORWARD_IF_FALSE    51 (to 652)
-                           550 STORE_FAST               8 (e)
-               
-               361         552 LOAD_GLOBAL             20 (logger)
-                           564 LOAD_METHOD             13 (error)
-                           586 LOAD_GLOBAL             29 (NULL + str)
-                           598 LOAD_FAST                8 (e)
-                           600 PRECALL                  1
-                           604 CALL                     1
-                           614 FORMAT_VALUE             0
-                           616 PRECALL                  1
-                           620 CALL                     1
-                           630 POP_TOP
-                           632 POP_EXCEPT
-                           634 LOAD_CONST               0 (None)
-                           636 STORE_FAST               8 (e)
-                           638 DELETE_FAST              8 (e)
-                           640 EXTENDED_ARG             1
-                           642 JUMP_BACKWARD          287 (to 70)
-                       >>  644 LOAD_CONST               0 (None)
-                           646 STORE_FAST               8 (e)
-                           648 DELETE_FAST              8 (e)
-                           650 RERAISE                  1
-               
-               362     >>  652 LOAD_GLOBAL             30 (Exception)
-                           664 CHECK_EXC_MATCH
-                           666 POP_JUMP_FORWARD_IF_FALSE   112 (to 892)
-                           668 STORE_FAST               8 (e)
-               
-               363         670 LOAD_GLOBAL             20 (logger)
-                           682 LOAD_METHOD             13 (error)
-               
-               364         704 LOAD_CONST              14 ('Oops Unable to perfom requested conversion: ')
-                           706 LOAD_FAST                8 (e)
-                           708 FORMAT_VALUE             0
-                           710 LOAD_CONST              15 ('\n')
-                           712 BUILD_STRING             3
-               
-               363         714 PRECALL                  1
-                           718 CALL                     1
-                           728 POP_TOP
-               
-               365         730 LOAD_GLOBAL              7 (NULL + open)
-                           742 LOAD_CONST              16 ('conversion.log')
-                           744 LOAD_CONST              17 ('a')
-                           746 PRECALL                  2
-                           750 CALL                     2
-                           760 BEFORE_WITH
-                           762 STORE_FAST               9 (log_file)
-               
-               366         764 LOAD_FAST                9 (log_file)
-                           766 LOAD_METHOD             16 (write)
-               
-               367         788 LOAD_CONST              18 ('Error converting ')
-                           790 LOAD_FAST                2 (file_path)
-                           792 FORMAT_VALUE             0
-                           794 LOAD_CONST              19 (' to ')
-                           796 LOAD_FAST                3 (word_file)
-                           798 FORMAT_VALUE             0
-                           800 LOAD_CONST              20 (': ')
-               
-               368         802 LOAD_FAST                8 (e)
-               
-               367         804 FORMAT_VALUE             0
-                           806 LOAD_CONST              15 ('\n')
-                           808 BUILD_STRING             7
+               374         522 FORMAT_VALUE             0
                
-               366         810 PRECALL                  1
-                           814 CALL                     1
-                           824 POP_TOP
+               375         524 LOAD_GLOBAL             26 (RESET)
                
-               365         826 LOAD_CONST               0 (None)
-                           828 LOAD_CONST               0 (None)
-                           830 LOAD_CONST               0 (None)
-                           832 PRECALL                  2
-                           836 CALL                     2
-                           846 POP_TOP
-                           848 JUMP_FORWARD            11 (to 872)
-                       >>  850 PUSH_EXC_INFO
-                           852 WITH_EXCEPT_START
-                           854 POP_JUMP_FORWARD_IF_TRUE     4 (to 864)
-                           856 RERAISE                  2
-                       >>  858 COPY                     3
-                           860 POP_EXCEPT
-                           862 RERAISE                  1
-                       >>  864 POP_TOP
-                           866 POP_EXCEPT
-                           868 POP_TOP
-                           870 POP_TOP
-                       >>  872 POP_EXCEPT
-                           874 LOAD_CONST               0 (None)
-                           876 STORE_FAST               8 (e)
-                           878 DELETE_FAST              8 (e)
-                           880 EXTENDED_ARG             1
-                           882 JUMP_BACKWARD          407 (to 70)
-                       >>  884 LOAD_CONST               0 (None)
-                           886 STORE_FAST               8 (e)
-                           888 DELETE_FAST              8 (e)
-                           890 RERAISE                  1
+               374         536 FORMAT_VALUE             0
+                           538 BUILD_STRING             6
+                           540 PRECALL                  1
+                           544 CALL                     1
+                           554 POP_TOP
+                           556 JUMP_BACKWARD          244 (to 70)
+                       >>  558 PUSH_EXC_INFO
                
-               362     >>  892 RERAISE                  0
-                       >>  894 COPY                     3
-                           896 POP_EXCEPT
-                           898 RERAISE                  1
+               376         560 LOAD_GLOBAL             28 (FileExistsError)
+                           572 CHECK_EXC_MATCH
+                           574 POP_JUMP_FORWARD_IF_FALSE    51 (to 678)
+                           576 STORE_FAST               8 (e)
                
-               338     >>  900 LOAD_CONST               0 (None)
-                           902 RETURN_VALUE
+               377         578 LOAD_GLOBAL             20 (logger)
+                           590 LOAD_METHOD             15 (error)
+                           612 LOAD_GLOBAL             33 (NULL + str)
+                           624 LOAD_FAST                8 (e)
+                           626 PRECALL                  1
+                           630 CALL                     1
+                           640 FORMAT_VALUE             0
+                           642 PRECALL                  1
+                           646 CALL                     1
+                           656 POP_TOP
+                           658 POP_EXCEPT
+                           660 LOAD_CONST               0 (None)
+                           662 STORE_FAST               8 (e)
+                           664 DELETE_FAST              8 (e)
+                           666 EXTENDED_ARG             1
+                           668 JUMP_BACKWARD          300 (to 70)
+                       >>  670 LOAD_CONST               0 (None)
+                           672 STORE_FAST               8 (e)
+                           674 DELETE_FAST              8 (e)
+                           676 RERAISE                  1
+               
+               378     >>  678 LOAD_GLOBAL             34 (Exception)
+                           690 CHECK_EXC_MATCH
+                           692 POP_JUMP_FORWARD_IF_FALSE   112 (to 918)
+                           694 STORE_FAST               8 (e)
+               
+               379         696 LOAD_GLOBAL             20 (logger)
+                           708 LOAD_METHOD             15 (error)
+               
+               380         730 LOAD_CONST              13 ('Oops Unable to perfom requested conversion: ')
+                           732 LOAD_FAST                8 (e)
+                           734 FORMAT_VALUE             0
+                           736 LOAD_CONST              14 ('\n')
+                           738 BUILD_STRING             3
+               
+               379         740 PRECALL                  1
+                           744 CALL                     1
+                           754 POP_TOP
+               
+               381         756 LOAD_GLOBAL              7 (NULL + open)
+                           768 LOAD_CONST              15 ('conversion.log')
+                           770 LOAD_CONST              16 ('a')
+                           772 PRECALL                  2
+                           776 CALL                     2
+                           786 BEFORE_WITH
+                           788 STORE_FAST               9 (log_file)
+               
+               382         790 LOAD_FAST                9 (log_file)
+                           792 LOAD_METHOD             18 (write)
+               
+               383         814 LOAD_CONST              17 ('Error converting ')
+                           816 LOAD_FAST                2 (file_path)
+                           818 FORMAT_VALUE             0
+                           820 LOAD_CONST              18 (' to ')
+                           822 LOAD_FAST                3 (word_file)
+                           824 FORMAT_VALUE             0
+                           826 LOAD_CONST              19 (': ')
+               
+               384         828 LOAD_FAST                8 (e)
+               
+               383         830 FORMAT_VALUE             0
+                           832 LOAD_CONST              14 ('\n')
+                           834 BUILD_STRING             7
+               
+               382         836 PRECALL                  1
+                           840 CALL                     1
+                           850 POP_TOP
+               
+               381         852 LOAD_CONST               0 (None)
+                           854 LOAD_CONST               0 (None)
+                           856 LOAD_CONST               0 (None)
+                           858 PRECALL                  2
+                           862 CALL                     2
+                           872 POP_TOP
+                           874 JUMP_FORWARD            11 (to 898)
+                       >>  876 PUSH_EXC_INFO
+                           878 WITH_EXCEPT_START
+                           880 POP_JUMP_FORWARD_IF_TRUE     4 (to 890)
+                           882 RERAISE                  2
+                       >>  884 COPY                     3
+                           886 POP_EXCEPT
+                           888 RERAISE                  1
+                       >>  890 POP_TOP
+                           892 POP_EXCEPT
+                           894 POP_TOP
+                           896 POP_TOP
+                       >>  898 POP_EXCEPT
+                           900 LOAD_CONST               0 (None)
+                           902 STORE_FAST               8 (e)
+                           904 DELETE_FAST              8 (e)
+                           906 EXTENDED_ARG             1
+                           908 JUMP_BACKWARD          420 (to 70)
+                       >>  910 LOAD_CONST               0 (None)
+                           912 STORE_FAST               8 (e)
+                           914 DELETE_FAST              8 (e)
+                           916 RERAISE                  1
+               
+               378     >>  918 RERAISE                  0
+                       >>  920 COPY                     3
+                           922 POP_EXCEPT
+                           924 RERAISE                  1
+               
+               354     >>  926 LOAD_CONST               0 (None)
+                           928 RETURN_VALUE
                ExceptionTable:
-                 182 to 218 -> 532 [1]
+                 182 to 218 -> 558 [1]
                  220 to 260 -> 286 [2] lasti
-                 262 to 284 -> 532 [1]
+                 262 to 284 -> 558 [1]
                  286 to 292 -> 294 [4] lasti
-                 294 to 298 -> 532 [1]
+                 294 to 298 -> 558 [1]
                  300 to 300 -> 294 [4] lasti
-                 302 to 528 -> 532 [1]
-                 532 to 550 -> 894 [2] lasti
-                 552 to 630 -> 644 [2] lasti
-                 644 to 668 -> 894 [2] lasti
-                 670 to 760 -> 884 [2] lasti
-                 762 to 824 -> 850 [3] lasti
-                 826 to 848 -> 884 [2] lasti
-                 850 to 856 -> 858 [5] lasti
-                 858 to 862 -> 884 [2] lasti
-                 864 to 864 -> 858 [5] lasti
-                 866 to 870 -> 884 [2] lasti
-                 884 to 892 -> 894 [2] lasti
+                 302 to 554 -> 558 [1]
+                 558 to 576 -> 920 [2] lasti
+                 578 to 656 -> 670 [2] lasti
+                 670 to 694 -> 920 [2] lasti
+                 696 to 786 -> 910 [2] lasti
+                 788 to 850 -> 876 [3] lasti
+                 852 to 874 -> 910 [2] lasti
+                 876 to 882 -> 884 [5] lasti
+                 884 to 888 -> 910 [2] lasti
+                 890 to 890 -> 884 [5] lasti
+                 892 to 896 -> 910 [2] lasti
+                 910 to 918 -> 920 [2] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d2b7d017c01a000000000000000000000000000000000
                         0000000000a6000000ab000000000000000000a001000000000000000000
                         00000000000000000000006400a6010000ab010000000000000000af297c
                         0191028c2c5300
-                     337           0 RESUME                   0
+                     353           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                43 (to 94)
                                    8 STORE_FAST               1 (item)
                                   10 LOAD_FAST                1 (item)
                                   12 LOAD_METHOD              0 (lower)
                                   34 PRECALL                  0
@@ -3208,339 +3426,367 @@
                              >>   94 RETURN_VALUE
                      consts
                         'txt'
                      names      ('lower', 'endswith')
                      varnames   ('.0', 'item')
                      freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 337
+                     firstlineno 353
                      lnotab 0x
                   'txt'
                   -3
                   'docx'
                   'r'
                   'utf-8'
                   'ignore'
                   ('encoding', 'errors')
                   '[^\\x09\\x0A\\x0D\\x20-\\uD7FF\\uE000-\\uFFFD]+'
                   ''
-                  '\x1b[1;95mSuccessfully converted '
+                  'Successfully converted '
                   ' to         '
-                  '\x1b[0m'
                   'Oops Unable to perfom requested conversion: '
                   '\n'
                   'conversion.log'
                   'a'
                   'Error converting '
                   ' to '
                   ': '
-               names      ('preprocess', 'lower', 'endswith', 'open', 'read', 're', 'sub', 'Document', 'add_paragraph', 'save', 'logger', 'info', 'FileExistsError', 'error', 'str', 'Exception', 'write')
+               names      ('preprocess', 'lower', 'endswith', 'open', 'read', 're', 'sub', 'Document', 'add_paragraph', 'save', 'logger', 'info', 'DMAGENTA', 'RESET', 'FileExistsError', 'error', 'str', 'Exception', 'write')
                varnames   ('self', 'flist', 'file_path', 'word_file', 'file', 'text_content', 'filtered_content', 'doc', 'e', 'log_file')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'text_to_word'
-               firstlineno 335
+               firstlineno 351
                lnotab
                   0x0201280118010a014e011a020202280128ff2e04160106ff10041c022a
-                  032a012a0102ff1a0212016401120122010aff1002220118010e0102ff06
-                  ff10ff42fd08e8
+                  032a01380102ff02010cff180212016401120122010aff1002220118010e
+                  0102ff06ff10ff42fd08e8
             code
                argcount  : 1
                nlocals   : 13
-               stacksize : 11
+               stacksize : 14
                flags     : 3
                code
                   0x870d97007c00a0000000000000000000000000000000000000000000a6
                   000000ab0000000000000000007d016401640267028a0d880d6601640384
                   087c014400a6000000ab0000000000000000007d01740300000000000000
-                  0000006404a6010000ab01000000000000000001007c01440090015db17d
-                  027c02a0020000000000000000000000000000000000000000a6000000ab
-                  000000000000000000a00300000000000000000000000000000000000000
+                  0000007404000000000000000000009b0064047406000000000000000000
+                  009b009d03a6010000ab01000000000000000001007c01440090015de37d
+                  027c02a0040000000000000000000000000000000000000000a6000000ab
+                  000000000000000000a00500000000000000000000000000000000000000
                   006401a6010000ab010000000000000000720e7c02640064058502190000
-                  0000000000000064067a0000007d036e347c02a002000000000000000000
-                  0000000000000000000000a6000000ab000000000000000000a003000000
+                  0000000000000064067a0000007d036e347c02a004000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000a005000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   000000720d7c026400640785021900000000000000000064067a0000007d
-                  03090009007409000000000000000000006a0500000000000000007c02a6
-                  010000ab0100000000000000007d040900740d00000000000000000000a6
-                  000000ab0000000000000000007d050900740e00000000000000000000a0
-                  08000000000000000000000000000000000000000064087c029b0064099d
-                  03a6010000ab01000000000000000001007c046a09000000000000000064
-                  0a190000000000000000007d067c04a00a00000000000000000000000000
-                  00000000000000a6000000ab00000000000000000044005d555c0200007d
-                  077d087c07640b7a0000007d097c097c067a0b0000640c7a0500007d0a7c
-                  0844005d247d0b7c05a00b00000000000000000000000000000000000000
-                  007419000000000000000000007c0ba6010000ab010000000000000000a6
-                  010000ab01000000000000000001008c2574030000000000000000000064
-                  0d7c099b00640e7c069b00640f7c0a64109b0464119d076412ac13a60200
-                  00ab02000000000000000001008c567c05a00d0000000000000000000000
-                  0000000000000000007c03a6010000ab0100000000000000000100740300
-                  00000000000000000064146415ac13a6020000ab02000000000000000001
-                  0090018c4f2300741c000000000000000000002400722701007403000000
-                  000000000000006416a6010000ab0100000000000000000100741f000000
-                  000000000000006a100000000000000000640ba6010000ab010000000000
-                  0000000100590090018c7f742200000000000000000000240072287d0c74
-                  030000000000000000000064177419000000000000000000007c0ca60100
-                  00ab010000000000000000a6020000ab0200000000000000000100590064
-                  007d0c7e0c90018cab64007d0c7e0c7701770078035900770164005300
+                  0309000900740d000000000000000000006a0700000000000000007c02a6
+                  010000ab0100000000000000007d040900741100000000000000000000a6
+                  000000ab0000000000000000007d050900741200000000000000000000a0
+                  0a0000000000000000000000000000000000000000741600000000000000
+                  0000009b0064087c029b0064097406000000000000000000009b009d05a6
+                  010000ab01000000000000000001007c046a0c0000000000000000640a19
+                  0000000000000000007d067c04a00d000000000000000000000000000000
+                  0000000000a6000000ab00000000000000000044005d6a5c0200007d077d
+                  087c07640b7a0000007d097c097c067a0b0000640c7a0500007d0a7c0844
+                  005d247d0b7c05a00e000000000000000000000000000000000000000074
+                  1f000000000000000000007c0ba6010000ab010000000000000000a60100
+                  00ab01000000000000000001008c25740300000000000000000000640d74
+                  20000000000000000000009b007c099b00640e7c069b00640f7422000000
+                  000000000000009b007c0a64109b0464117406000000000000000000009b
+                  009d0a6412ac13a6020000ab02000000000000000001008c6b7c05a01200
+                  000000000000000000000000000000000000007c03a6010000ab01000000
+                  000000000001007403000000000000000000007404000000000000000000
+                  009b0064147406000000000000000000009b009d036415ac13a6020000ab
+                  020000000000000000010090018c81230074260000000000000000000024
+                  00722701007403000000000000000000006416a6010000ab010000000000
+                  00000001007429000000000000000000006a150000000000000000640ba6
+                  010000ab0100000000000000000100590090018cb1742c00000000000000
+                  000000240072287d0c7403000000000000000000006417741f0000000000
+                  00000000007c0ca6010000ab010000000000000000a6020000ab02000000
+                  00000000000100590064007d0c7e0c90018cdd64007d0c7e0c7701770078
+                  035900770164005300
                              0 MAKE_CELL               13 (ls)
                
-               373           2 RESUME                   0
+               389           2 RESUME                   0
                
-               374           4 LOAD_FAST                0 (self)
+               390           4 LOAD_FAST                0 (self)
                              6 LOAD_METHOD              0 (preprocess)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 STORE_FAST               1 (xls_list)
                
-               375          44 LOAD_CONST               1 ('xlsx')
+               391          44 LOAD_CONST               1 ('xlsx')
                             46 LOAD_CONST               2 ('xls')
                             48 BUILD_LIST               2
                             50 STORE_DEREF             13 (ls)
                
-               376          52 LOAD_CLOSURE            13 (ls)
+               392          52 LOAD_CLOSURE            13 (ls)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 376>)
+                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 392>)
                             58 MAKE_FUNCTION            8 (closure)
                             60 LOAD_FAST                1 (xls_list)
                             62 GET_ITER
                             64 PRECALL                  0
                             68 CALL                     0
                             78 STORE_FAST               1 (xls_list)
                
-               378          80 LOAD_GLOBAL              3 (NULL + print)
-                            92 LOAD_CONST               4 ('\x1b[1;32mInitializing conversion sequence\x1b[0m')
-                            94 PRECALL                  1
-                            98 CALL                     1
-                           108 POP_TOP
+               394          80 LOAD_GLOBAL              3 (NULL + print)
+                            92 LOAD_GLOBAL              4 (DGREEN)
+                           104 FORMAT_VALUE             0
+                           106 LOAD_CONST               4 ('Initializing conversion sequence')
+                           108 LOAD_GLOBAL              6 (RESET)
+                           120 FORMAT_VALUE             0
+                           122 BUILD_STRING             3
+                           124 PRECALL                  1
+                           128 CALL                     1
+                           138 POP_TOP
+               
+               395         140 LOAD_FAST                1 (xls_list)
+                           142 GET_ITER
+                       >>  144 EXTENDED_ARG             1
+                           146 FOR_ITER               483 (to 1114)
+                           148 STORE_FAST               2 (xls_file)
                
-               379         110 LOAD_FAST                1 (xls_list)
-                           112 GET_ITER
-                       >>  114 EXTENDED_ARG             1
-                           116 FOR_ITER               433 (to 984)
-                           118 STORE_FAST               2 (xls_file)
-               
-               380         120 LOAD_FAST                2 (xls_file)
-                           122 LOAD_METHOD              2 (lower)
-                           144 PRECALL                  0
-                           148 CALL                     0
-                           158 LOAD_METHOD              3 (endswith)
-                           180 LOAD_CONST               1 ('xlsx')
-                           182 PRECALL                  1
-                           186 CALL                     1
-                           196 POP_JUMP_FORWARD_IF_FALSE    14 (to 226)
+               396         150 LOAD_FAST                2 (xls_file)
+                           152 LOAD_METHOD              4 (lower)
+                           174 PRECALL                  0
+                           178 CALL                     0
+                           188 LOAD_METHOD              5 (endswith)
+                           210 LOAD_CONST               1 ('xlsx')
+                           212 PRECALL                  1
+                           216 CALL                     1
+                           226 POP_JUMP_FORWARD_IF_FALSE    14 (to 256)
                
-               381         198 LOAD_FAST                2 (xls_file)
-                           200 LOAD_CONST               0 (None)
-                           202 LOAD_CONST               5 (-4)
-                           204 BUILD_SLICE              2
-                           206 BINARY_SUBSCR
-                           216 LOAD_CONST               6 ('docx')
-                           218 BINARY_OP                0 (+)
-                           222 STORE_FAST               3 (word_file)
-                           224 JUMP_FORWARD            52 (to 330)
-               
-               382     >>  226 LOAD_FAST                2 (xls_file)
-                           228 LOAD_METHOD              2 (lower)
-                           250 PRECALL                  0
-                           254 CALL                     0
-                           264 LOAD_METHOD              3 (endswith)
-                           286 LOAD_CONST               2 ('xls')
-                           288 PRECALL                  1
-                           292 CALL                     1
-                           302 POP_JUMP_FORWARD_IF_FALSE    13 (to 330)
+               397         228 LOAD_FAST                2 (xls_file)
+                           230 LOAD_CONST               0 (None)
+                           232 LOAD_CONST               5 (-4)
+                           234 BUILD_SLICE              2
+                           236 BINARY_SUBSCR
+                           246 LOAD_CONST               6 ('docx')
+                           248 BINARY_OP                0 (+)
+                           252 STORE_FAST               3 (word_file)
+                           254 JUMP_FORWARD            52 (to 360)
                
-               383         304 LOAD_FAST                2 (xls_file)
-                           306 LOAD_CONST               0 (None)
-                           308 LOAD_CONST               7 (-3)
-                           310 BUILD_SLICE              2
-                           312 BINARY_SUBSCR
-                           322 LOAD_CONST               6 ('docx')
-                           324 BINARY_OP                0 (+)
-                           328 STORE_FAST               3 (word_file)
+               398     >>  256 LOAD_FAST                2 (xls_file)
+                           258 LOAD_METHOD              4 (lower)
+                           280 PRECALL                  0
+                           284 CALL                     0
+                           294 LOAD_METHOD              5 (endswith)
+                           316 LOAD_CONST               2 ('xls')
+                           318 PRECALL                  1
+                           322 CALL                     1
+                           332 POP_JUMP_FORWARD_IF_FALSE    13 (to 360)
                
-               384     >>  330 NOP
+               399         334 LOAD_FAST                2 (xls_file)
+                           336 LOAD_CONST               0 (None)
+                           338 LOAD_CONST               7 (-3)
+                           340 BUILD_SLICE              2
+                           342 BINARY_SUBSCR
+                           352 LOAD_CONST               6 ('docx')
+                           354 BINARY_OP                0 (+)
+                           358 STORE_FAST               3 (word_file)
                
-               385         332 NOP
+               400     >>  360 NOP
                
-               387         334 LOAD_GLOBAL              9 (NULL + pd)
-                           346 LOAD_ATTR                5 (read_excel)
-                           356 LOAD_FAST                2 (xls_file)
-                           358 PRECALL                  1
-                           362 CALL                     1
-                           372 STORE_FAST               4 (df)
+               401         362 NOP
                
-               389         374 NOP
+               403         364 LOAD_GLOBAL             13 (NULL + pd)
+                           376 LOAD_ATTR                7 (read_excel)
+                           386 LOAD_FAST                2 (xls_file)
+                           388 PRECALL                  1
+                           392 CALL                     1
+                           402 STORE_FAST               4 (df)
                
-               390         376 LOAD_GLOBAL             13 (NULL + Document)
-                           388 PRECALL                  0
-                           392 CALL                     0
-                           402 STORE_FAST               5 (doc)
-               
-               392         404 NOP
-               
-               394         406 LOAD_GLOBAL             14 (logger)
-                           418 LOAD_METHOD              8 (info)
-                           440 LOAD_CONST               8 ('\x1b[3;36mConverting ')
-                           442 LOAD_FAST                2 (xls_file)
-                           444 FORMAT_VALUE             0
-                           446 LOAD_CONST               9 ('..\x1b[0m')
-                           448 BUILD_STRING             3
-                           450 PRECALL                  1
-                           454 CALL                     1
-                           464 POP_TOP
+               405         404 NOP
                
-               396         466 LOAD_FAST                4 (df)
-                           468 LOAD_ATTR                9 (shape)
-                           478 LOAD_CONST              10 (0)
-                           480 BINARY_SUBSCR
-                           490 STORE_FAST               6 (total_rows)
-               
-               397         492 LOAD_FAST                4 (df)
-                           494 LOAD_METHOD             10 (iterrows)
-                           516 PRECALL                  0
-                           520 CALL                     0
-                           530 GET_ITER
-                       >>  532 FOR_ITER                85 (to 704)
-                           534 UNPACK_SEQUENCE          2
-                           538 STORE_FAST               7 (_)
-                           540 STORE_FAST               8 (row)
-               
-               398         542 LOAD_FAST                7 (_)
-                           544 LOAD_CONST              11 (1)
-                           546 BINARY_OP                0 (+)
-                           550 STORE_FAST               9 (current_row)
-               
-               399         552 LOAD_FAST                9 (current_row)
-                           554 LOAD_FAST                6 (total_rows)
-                           556 BINARY_OP               11 (/)
-                           560 LOAD_CONST              12 (100)
-                           562 BINARY_OP                5 (*)
-                           566 STORE_FAST              10 (percentage)
-               
-               400         568 LOAD_FAST                8 (row)
-                           570 GET_ITER
-                       >>  572 FOR_ITER                36 (to 646)
-                           574 STORE_FAST              11 (value)
-               
-               401         576 LOAD_FAST                5 (doc)
-                           578 LOAD_METHOD             11 (add_paragraph)
-                           600 LOAD_GLOBAL             25 (NULL + str)
-                           612 LOAD_FAST               11 (value)
-                           614 PRECALL                  1
-                           618 CALL                     1
-                           628 PRECALL                  1
-                           632 CALL                     1
-                           642 POP_TOP
-                           644 JUMP_BACKWARD           37 (to 572)
+               406         406 LOAD_GLOBAL             17 (NULL + Document)
+                           418 PRECALL                  0
+                           422 CALL                     0
+                           432 STORE_FAST               5 (doc)
                
-               402     >>  646 LOAD_GLOBAL              3 (NULL + print)
-                           658 LOAD_CONST              13 ('Row \x1b[1;33m')
-                           660 LOAD_FAST                9 (current_row)
-                           662 FORMAT_VALUE             0
-                           664 LOAD_CONST              14 ('/')
-                           666 LOAD_FAST                6 (total_rows)
-                           668 FORMAT_VALUE             0
-                           670 LOAD_CONST              15 (' \x1b[1;34m')
-               
-               403         672 LOAD_FAST               10 (percentage)
-               
-               402         674 LOAD_CONST              16 ('.1f')
-                           676 FORMAT_VALUE             4 (with format)
-                           678 LOAD_CONST              17 ('%\x1b[0m')
-                           680 BUILD_STRING             7
-               
-               403         682 LOAD_CONST              18 ('\r')
-               
-               402         684 KW_NAMES                19
-                           686 PRECALL                  2
-                           690 CALL                     2
+               408         434 NOP
+               
+               410         436 LOAD_GLOBAL             18 (logger)
+                           448 LOAD_METHOD             10 (info)
+                           470 LOAD_GLOBAL             22 (ICYAN)
+                           482 FORMAT_VALUE             0
+                           484 LOAD_CONST               8 ('Converting ')
+                           486 LOAD_FAST                2 (xls_file)
+                           488 FORMAT_VALUE             0
+                           490 LOAD_CONST               9 ('..')
+                           492 LOAD_GLOBAL              6 (RESET)
+                           504 FORMAT_VALUE             0
+                           506 BUILD_STRING             5
+                           508 PRECALL                  1
+                           512 CALL                     1
+                           522 POP_TOP
+               
+               412         524 LOAD_FAST                4 (df)
+                           526 LOAD_ATTR               12 (shape)
+                           536 LOAD_CONST              10 (0)
+                           538 BINARY_SUBSCR
+                           548 STORE_FAST               6 (total_rows)
+               
+               413         550 LOAD_FAST                4 (df)
+                           552 LOAD_METHOD             13 (iterrows)
+                           574 PRECALL                  0
+                           578 CALL                     0
+                           588 GET_ITER
+                       >>  590 FOR_ITER               106 (to 804)
+                           592 UNPACK_SEQUENCE          2
+                           596 STORE_FAST               7 (_)
+                           598 STORE_FAST               8 (row)
+               
+               414         600 LOAD_FAST                7 (_)
+                           602 LOAD_CONST              11 (1)
+                           604 BINARY_OP                0 (+)
+                           608 STORE_FAST               9 (current_row)
+               
+               415         610 LOAD_FAST                9 (current_row)
+                           612 LOAD_FAST                6 (total_rows)
+                           614 BINARY_OP               11 (/)
+                           618 LOAD_CONST              12 (100)
+                           620 BINARY_OP                5 (*)
+                           624 STORE_FAST              10 (percentage)
+               
+               416         626 LOAD_FAST                8 (row)
+                           628 GET_ITER
+                       >>  630 FOR_ITER                36 (to 704)
+                           632 STORE_FAST              11 (value)
+               
+               417         634 LOAD_FAST                5 (doc)
+                           636 LOAD_METHOD             14 (add_paragraph)
+                           658 LOAD_GLOBAL             31 (NULL + str)
+                           670 LOAD_FAST               11 (value)
+                           672 PRECALL                  1
+                           676 CALL                     1
+                           686 PRECALL                  1
+                           690 CALL                     1
                            700 POP_TOP
-                           702 JUMP_BACKWARD           86 (to 532)
+                           702 JUMP_BACKWARD           37 (to 630)
                
-               407     >>  704 LOAD_FAST                5 (doc)
-                           706 LOAD_METHOD             13 (save)
-                           728 LOAD_FAST                3 (word_file)
-                           730 PRECALL                  1
-                           734 CALL                     1
-                           744 POP_TOP
+               418     >>  704 LOAD_GLOBAL              3 (NULL + print)
+                           716 LOAD_CONST              13 ('Row ')
+                           718 LOAD_GLOBAL             32 (DYELLOW)
+                           730 FORMAT_VALUE             0
+                           732 LOAD_FAST                9 (current_row)
+                           734 FORMAT_VALUE             0
+                           736 LOAD_CONST              14 ('/')
+                           738 LOAD_FAST                6 (total_rows)
+                           740 FORMAT_VALUE             0
+                           742 LOAD_CONST              15 (' ')
                
-               408         746 LOAD_GLOBAL              3 (NULL + print)
-                           758 LOAD_CONST              20 ('\x1b[1;32mConversion successful!\x1b[0m')
-                           760 LOAD_CONST              21 ('\n')
-                           762 KW_NAMES                19
-                           764 PRECALL                  2
-                           768 CALL                     2
-                           778 POP_TOP
-                           780 EXTENDED_ARG             1
-                           782 JUMP_BACKWARD          335 (to 114)
-                       >>  784 PUSH_EXC_INFO
-               
-               409         786 LOAD_GLOBAL             28 (KeyboardInterrupt)
-                           798 CHECK_EXC_MATCH
-                           800 POP_JUMP_FORWARD_IF_FALSE    39 (to 880)
-                           802 POP_TOP
+               419         744 LOAD_GLOBAL             34 (DBLUE)
                
-               410         804 LOAD_GLOBAL              3 (NULL + print)
-                           816 LOAD_CONST              22 ('\nExiting')
-                           818 PRECALL                  1
-                           822 CALL                     1
-                           832 POP_TOP
-               
-               411         834 LOAD_GLOBAL             31 (NULL + sys)
-                           846 LOAD_ATTR               16 (exit)
-                           856 LOAD_CONST              11 (1)
-                           858 PRECALL                  1
-                           862 CALL                     1
-                           872 POP_TOP
-                           874 POP_EXCEPT
-                           876 EXTENDED_ARG             1
-                           878 JUMP_BACKWARD          383 (to 114)
-               
-               412     >>  880 LOAD_GLOBAL             34 (Exception)
-                           892 CHECK_EXC_MATCH
-                           894 POP_JUMP_FORWARD_IF_FALSE    40 (to 976)
-                           896 STORE_FAST              12 (e)
-               
-               413         898 LOAD_GLOBAL              3 (NULL + print)
-                           910 LOAD_CONST              23 ('Oops Conversion failed:')
-                           912 LOAD_GLOBAL             25 (NULL + str)
-                           924 LOAD_FAST               12 (e)
-                           926 PRECALL                  1
-                           930 CALL                     1
-                           940 PRECALL                  2
-                           944 CALL                     2
-                           954 POP_TOP
-                           956 POP_EXCEPT
-                           958 LOAD_CONST               0 (None)
-                           960 STORE_FAST              12 (e)
-                           962 DELETE_FAST             12 (e)
-                           964 EXTENDED_ARG             1
-                           966 JUMP_BACKWARD          427 (to 114)
-                       >>  968 LOAD_CONST               0 (None)
-                           970 STORE_FAST              12 (e)
-                           972 DELETE_FAST             12 (e)
-                           974 RERAISE                  1
-               
-               412     >>  976 RERAISE                  0
-                       >>  978 COPY                     3
-                           980 POP_EXCEPT
-                           982 RERAISE                  1
+               418         756 FORMAT_VALUE             0
+               
+               419         758 LOAD_FAST               10 (percentage)
+               
+               418         760 LOAD_CONST              16 ('.1f')
+                           762 FORMAT_VALUE             4 (with format)
+                           764 LOAD_CONST              17 ('%')
+               
+               419         766 LOAD_GLOBAL              6 (RESET)
                
-               379     >>  984 LOAD_CONST               0 (None)
-                           986 RETURN_VALUE
+               418         778 FORMAT_VALUE             0
+                           780 BUILD_STRING            10
+               
+               419         782 LOAD_CONST              18 ('\r')
+               
+               418         784 KW_NAMES                19
+                           786 PRECALL                  2
+                           790 CALL                     2
+                           800 POP_TOP
+                           802 JUMP_BACKWARD          107 (to 590)
+               
+               423     >>  804 LOAD_FAST                5 (doc)
+                           806 LOAD_METHOD             18 (save)
+                           828 LOAD_FAST                3 (word_file)
+                           830 PRECALL                  1
+                           834 CALL                     1
+                           844 POP_TOP
+               
+               424         846 LOAD_GLOBAL              3 (NULL + print)
+                           858 LOAD_GLOBAL              4 (DGREEN)
+                           870 FORMAT_VALUE             0
+                           872 LOAD_CONST              20 ('Conversion successful!')
+                           874 LOAD_GLOBAL              6 (RESET)
+                           886 FORMAT_VALUE             0
+                           888 BUILD_STRING             3
+                           890 LOAD_CONST              21 ('\n')
+                           892 KW_NAMES                19
+                           894 PRECALL                  2
+                           898 CALL                     2
+                           908 POP_TOP
+                           910 EXTENDED_ARG             1
+                           912 JUMP_BACKWARD          385 (to 144)
+                       >>  914 PUSH_EXC_INFO
+               
+               425         916 LOAD_GLOBAL             38 (KeyboardInterrupt)
+                           928 CHECK_EXC_MATCH
+                           930 POP_JUMP_FORWARD_IF_FALSE    39 (to 1010)
+                           932 POP_TOP
+               
+               426         934 LOAD_GLOBAL              3 (NULL + print)
+                           946 LOAD_CONST              22 ('\nExiting')
+                           948 PRECALL                  1
+                           952 CALL                     1
+                           962 POP_TOP
+               
+               427         964 LOAD_GLOBAL             41 (NULL + sys)
+                           976 LOAD_ATTR               21 (exit)
+                           986 LOAD_CONST              11 (1)
+                           988 PRECALL                  1
+                           992 CALL                     1
+                          1002 POP_TOP
+                          1004 POP_EXCEPT
+                          1006 EXTENDED_ARG             1
+                          1008 JUMP_BACKWARD          433 (to 144)
+               
+               428     >> 1010 LOAD_GLOBAL             44 (Exception)
+                          1022 CHECK_EXC_MATCH
+                          1024 POP_JUMP_FORWARD_IF_FALSE    40 (to 1106)
+                          1026 STORE_FAST              12 (e)
+               
+               429        1028 LOAD_GLOBAL              3 (NULL + print)
+                          1040 LOAD_CONST              23 ('Oops Conversion failed:')
+                          1042 LOAD_GLOBAL             31 (NULL + str)
+                          1054 LOAD_FAST               12 (e)
+                          1056 PRECALL                  1
+                          1060 CALL                     1
+                          1070 PRECALL                  2
+                          1074 CALL                     2
+                          1084 POP_TOP
+                          1086 POP_EXCEPT
+                          1088 LOAD_CONST               0 (None)
+                          1090 STORE_FAST              12 (e)
+                          1092 DELETE_FAST             12 (e)
+                          1094 EXTENDED_ARG             1
+                          1096 JUMP_BACKWARD          477 (to 144)
+                       >> 1098 LOAD_CONST               0 (None)
+                          1100 STORE_FAST              12 (e)
+                          1102 DELETE_FAST             12 (e)
+                          1104 RERAISE                  1
+               
+               428     >> 1106 RERAISE                  0
+                       >> 1108 COPY                     3
+                          1110 POP_EXCEPT
+                          1112 RERAISE                  1
+               
+               395     >> 1114 LOAD_CONST               0 (None)
+                          1116 RETURN_VALUE
                ExceptionTable:
-                 332 to 778 -> 784 [1]
-                 784 to 872 -> 978 [2] lasti
-                 880 to 896 -> 978 [2] lasti
-                 898 to 954 -> 968 [2] lasti
-                 968 to 976 -> 978 [2] lasti
+                 362 to 908 -> 914 [1]
+                 914 to 1002 -> 1108 [2] lasti
+                 1010 to 1026 -> 1108 [2] lasti
+                 1028 to 1084 -> 1098 [2] lasti
+                 1098 to 1106 -> 1108 [2] lasti
                consts
                   None
                   'xlsx'
                   'xls'
                   code
                      argcount  : 1
                      nlocals   : 1
@@ -3549,28 +3795,28 @@
                      code
                         0x95018701970067007c005d1f8a01740100000000000000000000880166
                         016400840889024400a6000000ab000000000000000000a6010000ab0100
                         00000000000000af1d890191028c205300
                                    0 COPY_FREE_VARS           1
                                    2 MAKE_CELL                1 (item)
                      
-                     376           4 RESUME                   0
+                     392           4 RESUME                   0
                                    6 BUILD_LIST               0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                31 (to 74)
                                   12 STORE_DEREF              1 (item)
                                   14 LOAD_GLOBAL              1 (NULL + any)
                                   26 LOAD_CLOSURE             1 (item)
                                   28 BUILD_TUPLE              1
-                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 376>)
+                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 392>)
                                   32 MAKE_FUNCTION            8 (closure)
                      
-                     377          34 LOAD_DEREF               2 (ls)
+                     393          34 LOAD_DEREF               2 (ls)
                      
-                     376          36 GET_ITER
+                     392          36 GET_ITER
                                   38 PRECALL                  0
                                   42 CALL                     0
                                   52 PRECALL                  1
                                   56 CALL                     1
                                   66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
                                   68 LOAD_DEREF               1 (item)
                                   70 LIST_APPEND              2
@@ -3585,392 +3831,421 @@
                            code
                               0x95014b00010097007c005d2b7d018902a0000000000000000000000000
                               000000000000000000a6000000ab000000000000000000a0010000000000
                               0000000000000000000000000000007c01a6010000ab0100000000000000
                               005600970101008c2c64005300
                                          0 COPY_FREE_VARS           1
                            
-                           376           2 RETURN_GENERATOR
+                           392           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                43 (to 98)
                            
-                           377          12 STORE_FAST               1 (ext)
+                           393          12 STORE_FAST               1 (ext)
                                         14 LOAD_DEREF               2 (item)
                                         16 LOAD_METHOD              0 (lower)
                                         38 PRECALL                  0
                                         42 CALL                     0
                                         52 LOAD_METHOD              1 (endswith)
                                         74 LOAD_FAST                1 (ext)
                                         76 PRECALL                  1
                                         80 CALL                     1
                            
-                           376          90 YIELD_VALUE
+                           392          90 YIELD_VALUE
                                         92 RESUME                   1
                                         94 POP_TOP
                                         96 JUMP_BACKWARD           44 (to 10)
                                    >>   98 LOAD_CONST               0 (None)
                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('lower', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                            name       '<genexpr>'
-                           firstlineno 376
+                           firstlineno 392
                            lnotab 0x0c014eff
                      names      ('any',)
                      varnames   ('.0',)
                      freevars   ('ls',)
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 376
+                     firstlineno 392
                      lnotab 0x220102ff
-                  '\x1b[1;32mInitializing conversion sequence\x1b[0m'
+                  'Initializing conversion sequence'
                   -4
                   'docx'
                   -3
-                  '\x1b[3;36mConverting '
-                  '..\x1b[0m'
+                  'Converting '
+                  '..'
                   0
                   1
                   100
-                  'Row \x1b[1;33m'
+                  'Row '
                   '/'
-                  ' \x1b[1;34m'
+                  ' '
                   '.1f'
-                  '%\x1b[0m'
+                  '%'
                   '\r'
                   ('end',)
-                  '\x1b[1;32mConversion successful!\x1b[0m'
+                  'Conversion successful!'
                   '\n'
                   '\nExiting'
                   'Oops Conversion failed:'
-               names      ('preprocess', 'print', 'lower', 'endswith', 'pd', 'read_excel', 'Document', 'logger', 'info', 'shape', 'iterrows', 'add_paragraph', 'str', 'save', 'KeyboardInterrupt', 'sys', 'exit', 'Exception')
+               names      ('preprocess', 'print', 'DGREEN', 'RESET', 'lower', 'endswith', 'pd', 'read_excel', 'Document', 'logger', 'info', 'ICYAN', 'shape', 'iterrows', 'add_paragraph', 'str', 'DYELLOW', 'DBLUE', 'save', 'KeyboardInterrupt', 'sys', 'exit', 'Exception')
                varnames   ('self', 'xls_list', 'xls_file', 'word_file', 'df', 'doc', 'total_rows', '_', 'row', 'current_row', 'percentage', 'value', 'e')
                freevars   ()
                cellvars   ('ls',)
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'convert_xls_to_word'
-               firstlineno 373
+               firstlineno 389
                lnotab
-                  0x0401280108011c021e010a014e011c014e011a0102010202280202011c
-                  0202023c021a0132010a011001080146011a0102ff080102ff14052a0128
-                  0112011e012e0112014eff08df
+                  0x0401280108011c023c010a014e011c014e011a0102010202280202011c
+                  02020258021a0132010a0110010801460128010cff020102ff06010cff04
+                  0102ff14052a01460112011e012e0112014eff08df
             code
                argcount  : 1
                nlocals   : 11
-               stacksize : 10
+               stacksize : 15
                flags     : 3
                code
                   0x870b97007c00a0000000000000000000000000000000000000000000a6
                   000000ab0000000000000000007d016401640267028a0b880b6601640384
                   087c014400a6000000ab0000000000000000007d01740300000000000000
-                  0000006404a6010000ab01000000000000000001007c01440090015dd37d
-                  027c02a0020000000000000000000000000000000000000000a6000000ab
-                  000000000000000000a00300000000000000000000000000000000000000
+                  0000007404000000000000000000009b0064047406000000000000000000
+                  009b009d03a6010000ab01000000000000000001007c01440090015dff7d
+                  027c02a0040000000000000000000000000000000000000000a6000000ab
+                  000000000000000000a00500000000000000000000000000000000000000
                   006401a6010000ab010000000000000000720e7c02640064058502190000
-                  0000000000000064067a0000007d036e347c02a002000000000000000000
-                  0000000000000000000000a6000000ab000000000000000000a003000000
+                  0000000000000064067a0000007d036e347c02a004000000000000000000
+                  0000000000000000000000a6000000ab000000000000000000a005000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   000000720d7c026400640785021900000000000000000064067a0000007d
-                  030900740800000000000000000000a00500000000000000000000000000
+                  030900740c00000000000000000000a00700000000000000000000000000
                   0000000000000064087c029b0064099d03a6010000ab0100000000000000
-                  000100740d000000000000000000006a0700000000000000007c02a60100
-                  00ab0100000000000000007d047c04a00800000000000000000000000000
-                  00000000000000640aac0ba6010000ab0100000000000000007d05741300
-                  0000000000000000007c05a6010000ab0100000000000000007d06741300
-                  0000000000000000007c05a00a0000000000000000000000000000000000
+                  0001007411000000000000000000006a0900000000000000007c02a60100
+                  00ab0100000000000000007d047c04a00a00000000000000000000000000
+                  00000000000000640aac0ba6010000ab0100000000000000007d05741700
+                  0000000000000000007c05a6010000ab0100000000000000007d06741700
+                  0000000000000000007c05a00c0000000000000000000000000000000000
                   000000a6000000ab000000000000000000a6010000ab0100000000000000
-                  007d077413000000000000000000007c05a00b0000000000000000000000
+                  007d077417000000000000000000007c05a00d0000000000000000000000
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
-                  000000000000007d08740300000000000000000000640c7c069b00640d7c
-                  079b00640e7c089b00640f9d076410ac11a6020000ab0200000000000000
-                  0001007419000000000000000000007c036412a6020000ab020000000000
-                  00000035007d097c09a00d00000000000000000000000000000000000000
-                  007c05a6010000ab0100000000000000000100640064006400a6020000ab
-                  02000000000000000001006e0b2300310073047702780359007701010059
-                  000100010074030000000000000000000064136410ac11a6020000ab0200
-                  00000000000000010090018c712300741c00000000000000000000240072
-                  2701007403000000000000000000006414a6010000ab0100000000000000
-                  000100741f000000000000000000006a1000000000000000006415a60100
-                  00ab0100000000000000000100590090018ca17422000000000000000000
-                  00240072287d0a7403000000000000000000006416742500000000000000
-                  0000007c0aa6010000ab010000000000000000a6020000ab020000000000
-                  0000000100590064007d0a7e0a90018ccd64007d0a7e0a77017700780359
-                  00770164005300
+                  000000000000007d08740300000000000000000000640c741c0000000000
+                  00000000009b007c069b00640d741c000000000000000000009b00640e7c
+                  079b00640f741c000000000000000000009b007c089b0064107406000000
+                  000000000000009b009d0c6411ac12a6020000ab02000000000000000001
+                  00741f000000000000000000007c036413a6020000ab0200000000000000
+                  0035007d097c09a01000000000000000000000000000000000000000007c
+                  05a6010000ab0100000000000000000100640064006400a6020000ab0200
+                  0000000000000001006e0b23003100730477027803590077010100590001
+                  0001007403000000000000000000007404000000000000000000009b0064
+                  147406000000000000000000009b009d036411ac12a6020000ab02000000
+                  0000000000010090018c9d23007422000000000000000000002400722701
+                  007403000000000000000000006415a6010000ab01000000000000000001
+                  007425000000000000000000006a1300000000000000006416a6010000ab
+                  0100000000000000000100590090018ccd74280000000000000000000024
+                  0072287d0a7403000000000000000000006417742b000000000000000000
+                  007c0aa6010000ab010000000000000000a6020000ab0200000000000000
+                  000100590064007d0a7e0a90018cf964007d0a7e0a770177007803590077
+                  0164005300
                              0 MAKE_CELL               11 (ls)
                
-               419           2 RESUME                   0
+               435           2 RESUME                   0
                
-               420           4 LOAD_FAST                0 (self)
+               436           4 LOAD_FAST                0 (self)
                              6 LOAD_METHOD              0 (preprocess)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 STORE_FAST               1 (xls_list)
                
-               421          44 LOAD_CONST               1 ('xlsx')
+               437          44 LOAD_CONST               1 ('xlsx')
                             46 LOAD_CONST               2 ('xls')
                             48 BUILD_LIST               2
                             50 STORE_DEREF             11 (ls)
                
-               422          52 LOAD_CLOSURE            11 (ls)
+               438          52 LOAD_CLOSURE            11 (ls)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 422>)
+                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 438>)
                             58 MAKE_FUNCTION            8 (closure)
                
-               423          60 LOAD_FAST                1 (xls_list)
+               439          60 LOAD_FAST                1 (xls_list)
                
-               422          62 GET_ITER
+               438          62 GET_ITER
                             64 PRECALL                  0
                             68 CALL                     0
                             78 STORE_FAST               1 (xls_list)
                
-               425          80 LOAD_GLOBAL              3 (NULL + print)
-                            92 LOAD_CONST               4 ('\x1b[1;32mInitializing conversion sequence\x1b[0m')
-                            94 PRECALL                  1
-                            98 CALL                     1
-                           108 POP_TOP
+               441          80 LOAD_GLOBAL              3 (NULL + print)
+                            92 LOAD_GLOBAL              4 (DGREEN)
+                           104 FORMAT_VALUE             0
+                           106 LOAD_CONST               4 ('Initializing conversion sequence')
+                           108 LOAD_GLOBAL              6 (RESET)
+                           120 FORMAT_VALUE             0
+                           122 BUILD_STRING             3
+                           124 PRECALL                  1
+                           128 CALL                     1
+                           138 POP_TOP
+               
+               442         140 LOAD_FAST                1 (xls_list)
+                           142 GET_ITER
+                       >>  144 EXTENDED_ARG             1
+                           146 FOR_ITER               511 (to 1170)
+                           148 STORE_FAST               2 (xls_file)
                
-               426         110 LOAD_FAST                1 (xls_list)
-                           112 GET_ITER
-                       >>  114 EXTENDED_ARG             1
-                           116 FOR_ITER               467 (to 1052)
-                           118 STORE_FAST               2 (xls_file)
-               
-               427         120 LOAD_FAST                2 (xls_file)
-                           122 LOAD_METHOD              2 (lower)
-                           144 PRECALL                  0
-                           148 CALL                     0
-                           158 LOAD_METHOD              3 (endswith)
-                           180 LOAD_CONST               1 ('xlsx')
-                           182 PRECALL                  1
-                           186 CALL                     1
-                           196 POP_JUMP_FORWARD_IF_FALSE    14 (to 226)
+               443         150 LOAD_FAST                2 (xls_file)
+                           152 LOAD_METHOD              4 (lower)
+                           174 PRECALL                  0
+                           178 CALL                     0
+                           188 LOAD_METHOD              5 (endswith)
+                           210 LOAD_CONST               1 ('xlsx')
+                           212 PRECALL                  1
+                           216 CALL                     1
+                           226 POP_JUMP_FORWARD_IF_FALSE    14 (to 256)
                
-               428         198 LOAD_FAST                2 (xls_file)
-                           200 LOAD_CONST               0 (None)
-                           202 LOAD_CONST               5 (-4)
-                           204 BUILD_SLICE              2
-                           206 BINARY_SUBSCR
-                           216 LOAD_CONST               6 ('txt')
-                           218 BINARY_OP                0 (+)
-                           222 STORE_FAST               3 (txt_file)
-                           224 JUMP_FORWARD            52 (to 330)
-               
-               429     >>  226 LOAD_FAST                2 (xls_file)
-                           228 LOAD_METHOD              2 (lower)
-                           250 PRECALL                  0
-                           254 CALL                     0
-                           264 LOAD_METHOD              3 (endswith)
-                           286 LOAD_CONST               2 ('xls')
-                           288 PRECALL                  1
-                           292 CALL                     1
-                           302 POP_JUMP_FORWARD_IF_FALSE    13 (to 330)
+               444         228 LOAD_FAST                2 (xls_file)
+                           230 LOAD_CONST               0 (None)
+                           232 LOAD_CONST               5 (-4)
+                           234 BUILD_SLICE              2
+                           236 BINARY_SUBSCR
+                           246 LOAD_CONST               6 ('txt')
+                           248 BINARY_OP                0 (+)
+                           252 STORE_FAST               3 (txt_file)
+                           254 JUMP_FORWARD            52 (to 360)
                
-               430         304 LOAD_FAST                2 (xls_file)
-                           306 LOAD_CONST               0 (None)
-                           308 LOAD_CONST               7 (-3)
-                           310 BUILD_SLICE              2
-                           312 BINARY_SUBSCR
-                           322 LOAD_CONST               6 ('txt')
-                           324 BINARY_OP                0 (+)
-                           328 STORE_FAST               3 (txt_file)
-               
-               431     >>  330 NOP
-               
-               433         332 LOAD_GLOBAL              8 (logger)
-                           344 LOAD_METHOD              5 (info)
-                           366 LOAD_CONST               8 ('Converting ')
-                           368 LOAD_FAST                2 (xls_file)
-                           370 FORMAT_VALUE             0
-                           372 LOAD_CONST               9 ('..')
-                           374 BUILD_STRING             3
-                           376 PRECALL                  1
-                           380 CALL                     1
-                           390 POP_TOP
+               445     >>  256 LOAD_FAST                2 (xls_file)
+                           258 LOAD_METHOD              4 (lower)
+                           280 PRECALL                  0
+                           284 CALL                     0
+                           294 LOAD_METHOD              5 (endswith)
+                           316 LOAD_CONST               2 ('xls')
+                           318 PRECALL                  1
+                           322 CALL                     1
+                           332 POP_JUMP_FORWARD_IF_FALSE    13 (to 360)
+               
+               446         334 LOAD_FAST                2 (xls_file)
+                           336 LOAD_CONST               0 (None)
+                           338 LOAD_CONST               7 (-3)
+                           340 BUILD_SLICE              2
+                           342 BINARY_SUBSCR
+                           352 LOAD_CONST               6 ('txt')
+                           354 BINARY_OP                0 (+)
+                           358 STORE_FAST               3 (txt_file)
                
-               434         392 LOAD_GLOBAL             13 (NULL + pd)
-                           404 LOAD_ATTR                7 (read_excel)
-                           414 LOAD_FAST                2 (xls_file)
-                           416 PRECALL                  1
-                           420 CALL                     1
-                           430 STORE_FAST               4 (df)
-               
-               437         432 LOAD_FAST                4 (df)
-                           434 LOAD_METHOD              8 (to_string)
-                           456 LOAD_CONST              10 (False)
-                           458 KW_NAMES                11
-                           460 PRECALL                  1
-                           464 CALL                     1
-                           474 STORE_FAST               5 (text)
+               447     >>  360 NOP
                
-               438         476 LOAD_GLOBAL             19 (NULL + len)
-                           488 LOAD_FAST                5 (text)
+               449         362 LOAD_GLOBAL             12 (logger)
+                           374 LOAD_METHOD              7 (info)
+                           396 LOAD_CONST               8 ('Converting ')
+                           398 LOAD_FAST                2 (xls_file)
+                           400 FORMAT_VALUE             0
+                           402 LOAD_CONST               9 ('..')
+                           404 BUILD_STRING             3
+                           406 PRECALL                  1
+                           410 CALL                     1
+                           420 POP_TOP
+               
+               450         422 LOAD_GLOBAL             17 (NULL + pd)
+                           434 LOAD_ATTR                9 (read_excel)
+                           444 LOAD_FAST                2 (xls_file)
+                           446 PRECALL                  1
+                           450 CALL                     1
+                           460 STORE_FAST               4 (df)
+               
+               453         462 LOAD_FAST                4 (df)
+                           464 LOAD_METHOD             10 (to_string)
+                           486 LOAD_CONST              10 (False)
+                           488 KW_NAMES                11
                            490 PRECALL                  1
                            494 CALL                     1
-                           504 STORE_FAST               6 (chars)
+                           504 STORE_FAST               5 (text)
                
-               439         506 LOAD_GLOBAL             19 (NULL + len)
+               454         506 LOAD_GLOBAL             23 (NULL + len)
                            518 LOAD_FAST                5 (text)
-                           520 LOAD_METHOD             10 (split)
-                           542 PRECALL                  0
-                           546 CALL                     0
-                           556 PRECALL                  1
-                           560 CALL                     1
-                           570 STORE_FAST               7 (words)
+                           520 PRECALL                  1
+                           524 CALL                     1
+                           534 STORE_FAST               6 (chars)
+               
+               455         536 LOAD_GLOBAL             23 (NULL + len)
+                           548 LOAD_FAST                5 (text)
+                           550 LOAD_METHOD             12 (split)
+                           572 PRECALL                  0
+                           576 CALL                     0
+                           586 PRECALL                  1
+                           590 CALL                     1
+                           600 STORE_FAST               7 (words)
+               
+               456         602 LOAD_GLOBAL             23 (NULL + len)
+                           614 LOAD_FAST                5 (text)
+                           616 LOAD_METHOD             13 (splitlines)
+                           638 PRECALL                  0
+                           642 CALL                     0
+                           652 PRECALL                  1
+                           656 CALL                     1
+                           666 STORE_FAST               8 (lines)
                
-               440         572 LOAD_GLOBAL             19 (NULL + len)
-                           584 LOAD_FAST                5 (text)
-                           586 LOAD_METHOD             11 (splitlines)
-                           608 PRECALL                  0
-                           612 CALL                     0
-                           622 PRECALL                  1
-                           626 CALL                     1
-                           636 STORE_FAST               8 (lines)
+               458         668 LOAD_GLOBAL              3 (NULL + print)
                
-               442         638 LOAD_GLOBAL              3 (NULL + print)
+               459         680 LOAD_CONST              12 ('Preparing to write: ')
+                           682 LOAD_GLOBAL             28 (DYELLOW)
+                           694 FORMAT_VALUE             0
+                           696 LOAD_FAST                6 (chars)
+                           698 FORMAT_VALUE             0
+                           700 LOAD_CONST              13 (' \x1b[1;30m characters')
                
-               443         650 LOAD_CONST              12 ('Preparing to write: \x1b[1;33m')
-                           652 LOAD_FAST                6 (chars)
-                           654 FORMAT_VALUE             0
-                           656 LOAD_CONST              13 (' \x1b[1;30m characters\x1b[1;33m ')
+               460         702 LOAD_GLOBAL             28 (DYELLOW)
                
-               444         658 LOAD_FAST                7 (words)
+               459         714 FORMAT_VALUE             0
+                           716 LOAD_CONST              14 (' ')
                
-               443         660 FORMAT_VALUE             0
-                           662 LOAD_CONST              14 ('\x1b[1;30m words \x1b[1;33m')
+               460         718 LOAD_FAST                7 (words)
                
-               444         664 LOAD_FAST                8 (lines)
+               459         720 FORMAT_VALUE             0
+                           722 LOAD_CONST              15 ('\x1b[1;30m words ')
                
-               443         666 FORMAT_VALUE             0
-                           668 LOAD_CONST              15 ('\x1b[1;30m lines \x1b[0m')
-                           670 BUILD_STRING             7
+               460         724 LOAD_GLOBAL             28 (DYELLOW)
                
-               445         672 LOAD_CONST              16 ('\n')
+               459         736 FORMAT_VALUE             0
                
-               442         674 KW_NAMES                17
-                           676 PRECALL                  2
-                           680 CALL                     2
-                           690 POP_TOP
+               460         738 LOAD_FAST                8 (lines)
                
-               447         692 LOAD_GLOBAL             25 (NULL + open)
-                           704 LOAD_FAST                3 (txt_file)
-                           706 LOAD_CONST              18 ('w')
-                           708 PRECALL                  2
-                           712 CALL                     2
-                           722 BEFORE_WITH
-                           724 STORE_FAST               9 (file)
-               
-               448         726 LOAD_FAST                9 (file)
-                           728 LOAD_METHOD             13 (write)
-                           750 LOAD_FAST                5 (text)
-                           752 PRECALL                  1
-                           756 CALL                     1
-                           766 POP_TOP
-               
-               447         768 LOAD_CONST               0 (None)
-                           770 LOAD_CONST               0 (None)
-                           772 LOAD_CONST               0 (None)
-                           774 PRECALL                  2
-                           778 CALL                     2
-                           788 POP_TOP
-                           790 JUMP_FORWARD            11 (to 814)
-                       >>  792 PUSH_EXC_INFO
-                           794 WITH_EXCEPT_START
-                           796 POP_JUMP_FORWARD_IF_TRUE     4 (to 806)
-                           798 RERAISE                  2
-                       >>  800 COPY                     3
-                           802 POP_EXCEPT
-                           804 RERAISE                  1
-                       >>  806 POP_TOP
-                           808 POP_EXCEPT
-                           810 POP_TOP
-                           812 POP_TOP
+               459         740 FORMAT_VALUE             0
+                           742 LOAD_CONST              16 ('\x1b[1;30m lines ')
                
-               450     >>  814 LOAD_GLOBAL              3 (NULL + print)
-                           826 LOAD_CONST              19 ('\x1b[1;32mConversion successful!\x1b[0m')
-                           828 LOAD_CONST              16 ('\n')
-                           830 KW_NAMES                17
-                           832 PRECALL                  2
-                           836 CALL                     2
-                           846 POP_TOP
-                           848 EXTENDED_ARG             1
-                           850 JUMP_BACKWARD          369 (to 114)
-                       >>  852 PUSH_EXC_INFO
-               
-               451         854 LOAD_GLOBAL             28 (KeyboardInterrupt)
-                           866 CHECK_EXC_MATCH
-                           868 POP_JUMP_FORWARD_IF_FALSE    39 (to 948)
-                           870 POP_TOP
+               461         744 LOAD_GLOBAL              6 (RESET)
+               
+               459         756 FORMAT_VALUE             0
+                           758 BUILD_STRING            12
+               
+               461         760 LOAD_CONST              17 ('\n')
+               
+               458         762 KW_NAMES                18
+                           764 PRECALL                  2
+                           768 CALL                     2
+                           778 POP_TOP
                
-               452         872 LOAD_GLOBAL              3 (NULL + print)
-                           884 LOAD_CONST              20 ('\nExiting')
-                           886 PRECALL                  1
-                           890 CALL                     1
+               463         780 LOAD_GLOBAL             31 (NULL + open)
+                           792 LOAD_FAST                3 (txt_file)
+                           794 LOAD_CONST              19 ('w')
+                           796 PRECALL                  2
+                           800 CALL                     2
+                           810 BEFORE_WITH
+                           812 STORE_FAST               9 (file)
+               
+               464         814 LOAD_FAST                9 (file)
+                           816 LOAD_METHOD             16 (write)
+                           838 LOAD_FAST                5 (text)
+                           840 PRECALL                  1
+                           844 CALL                     1
+                           854 POP_TOP
+               
+               463         856 LOAD_CONST               0 (None)
+                           858 LOAD_CONST               0 (None)
+                           860 LOAD_CONST               0 (None)
+                           862 PRECALL                  2
+                           866 CALL                     2
+                           876 POP_TOP
+                           878 JUMP_FORWARD            11 (to 902)
+                       >>  880 PUSH_EXC_INFO
+                           882 WITH_EXCEPT_START
+                           884 POP_JUMP_FORWARD_IF_TRUE     4 (to 894)
+                           886 RERAISE                  2
+                       >>  888 COPY                     3
+                           890 POP_EXCEPT
+                           892 RERAISE                  1
+                       >>  894 POP_TOP
+                           896 POP_EXCEPT
+                           898 POP_TOP
                            900 POP_TOP
                
-               453         902 LOAD_GLOBAL             31 (NULL + sys)
-                           914 LOAD_ATTR               16 (exit)
-                           924 LOAD_CONST              21 (1)
-                           926 PRECALL                  1
-                           930 CALL                     1
-                           940 POP_TOP
-                           942 POP_EXCEPT
-                           944 EXTENDED_ARG             1
-                           946 JUMP_BACKWARD          417 (to 114)
-               
-               454     >>  948 LOAD_GLOBAL             34 (Exception)
-                           960 CHECK_EXC_MATCH
-                           962 POP_JUMP_FORWARD_IF_FALSE    40 (to 1044)
-                           964 STORE_FAST              10 (e)
-               
-               455         966 LOAD_GLOBAL              3 (NULL + print)
-                           978 LOAD_CONST              22 ('Oops Conversion failed:')
-                           980 LOAD_GLOBAL             37 (NULL + str)
-                           992 LOAD_FAST               10 (e)
-                           994 PRECALL                  1
-                           998 CALL                     1
-                          1008 PRECALL                  2
-                          1012 CALL                     2
-                          1022 POP_TOP
-                          1024 POP_EXCEPT
-                          1026 LOAD_CONST               0 (None)
-                          1028 STORE_FAST              10 (e)
-                          1030 DELETE_FAST             10 (e)
-                          1032 EXTENDED_ARG             1
-                          1034 JUMP_BACKWARD          461 (to 114)
-                       >> 1036 LOAD_CONST               0 (None)
-                          1038 STORE_FAST              10 (e)
-                          1040 DELETE_FAST             10 (e)
-                          1042 RERAISE                  1
-               
-               454     >> 1044 RERAISE                  0
-                       >> 1046 COPY                     3
-                          1048 POP_EXCEPT
-                          1050 RERAISE                  1
+               466     >>  902 LOAD_GLOBAL              3 (NULL + print)
+                           914 LOAD_GLOBAL              4 (DGREEN)
+                           926 FORMAT_VALUE             0
+                           928 LOAD_CONST              20 ('Conversion successful!')
+                           930 LOAD_GLOBAL              6 (RESET)
+                           942 FORMAT_VALUE             0
+                           944 BUILD_STRING             3
+                           946 LOAD_CONST              17 ('\n')
+                           948 KW_NAMES                18
+                           950 PRECALL                  2
+                           954 CALL                     2
+                           964 POP_TOP
+                           966 EXTENDED_ARG             1
+                           968 JUMP_BACKWARD          413 (to 144)
+                       >>  970 PUSH_EXC_INFO
+               
+               467         972 LOAD_GLOBAL             34 (KeyboardInterrupt)
+                           984 CHECK_EXC_MATCH
+                           986 POP_JUMP_FORWARD_IF_FALSE    39 (to 1066)
+                           988 POP_TOP
+               
+               468         990 LOAD_GLOBAL              3 (NULL + print)
+                          1002 LOAD_CONST              21 ('\nExiting')
+                          1004 PRECALL                  1
+                          1008 CALL                     1
+                          1018 POP_TOP
+               
+               469        1020 LOAD_GLOBAL             37 (NULL + sys)
+                          1032 LOAD_ATTR               19 (exit)
+                          1042 LOAD_CONST              22 (1)
+                          1044 PRECALL                  1
+                          1048 CALL                     1
+                          1058 POP_TOP
+                          1060 POP_EXCEPT
+                          1062 EXTENDED_ARG             1
+                          1064 JUMP_BACKWARD          461 (to 144)
+               
+               470     >> 1066 LOAD_GLOBAL             40 (Exception)
+                          1078 CHECK_EXC_MATCH
+                          1080 POP_JUMP_FORWARD_IF_FALSE    40 (to 1162)
+                          1082 STORE_FAST              10 (e)
+               
+               471        1084 LOAD_GLOBAL              3 (NULL + print)
+                          1096 LOAD_CONST              23 ('Oops Conversion failed:')
+                          1098 LOAD_GLOBAL             43 (NULL + str)
+                          1110 LOAD_FAST               10 (e)
+                          1112 PRECALL                  1
+                          1116 CALL                     1
+                          1126 PRECALL                  2
+                          1130 CALL                     2
+                          1140 POP_TOP
+                          1142 POP_EXCEPT
+                          1144 LOAD_CONST               0 (None)
+                          1146 STORE_FAST              10 (e)
+                          1148 DELETE_FAST             10 (e)
+                          1150 EXTENDED_ARG             1
+                          1152 JUMP_BACKWARD          505 (to 144)
+                       >> 1154 LOAD_CONST               0 (None)
+                          1156 STORE_FAST              10 (e)
+                          1158 DELETE_FAST             10 (e)
+                          1160 RERAISE                  1
+               
+               470     >> 1162 RERAISE                  0
+                       >> 1164 COPY                     3
+                          1166 POP_EXCEPT
+                          1168 RERAISE                  1
                
-               426     >> 1052 LOAD_CONST               0 (None)
-                          1054 RETURN_VALUE
+               442     >> 1170 LOAD_CONST               0 (None)
+                          1172 RETURN_VALUE
                ExceptionTable:
-                 332 to 722 -> 852 [1]
-                 724 to 766 -> 792 [2] lasti
-                 768 to 790 -> 852 [1]
-                 792 to 798 -> 800 [4] lasti
-                 800 to 804 -> 852 [1]
-                 806 to 806 -> 800 [4] lasti
-                 808 to 846 -> 852 [1]
-                 852 to 940 -> 1046 [2] lasti
-                 948 to 964 -> 1046 [2] lasti
-                 966 to 1022 -> 1036 [2] lasti
-                 1036 to 1044 -> 1046 [2] lasti
+                 362 to 810 -> 970 [1]
+                 812 to 854 -> 880 [2] lasti
+                 856 to 878 -> 970 [1]
+                 880 to 886 -> 888 [4] lasti
+                 888 to 892 -> 970 [1]
+                 894 to 894 -> 888 [4] lasti
+                 896 to 964 -> 970 [1]
+                 970 to 1058 -> 1164 [2] lasti
+                 1066 to 1082 -> 1164 [2] lasti
+                 1084 to 1140 -> 1154 [2] lasti
+                 1154 to 1162 -> 1164 [2] lasti
                consts
                   None
                   'xlsx'
                   'xls'
                   code
                      argcount  : 1
                      nlocals   : 1
@@ -3979,39 +4254,39 @@
                      code
                         0x95018701970067007c005d1f8a01740100000000000000000000880166
                         016400840889024400a6000000ab000000000000000000a6010000ab0100
                         00000000000000af1d890191028c205300
                                    0 COPY_FREE_VARS           1
                                    2 MAKE_CELL                1 (item)
                      
-                     422           4 RESUME                   0
+                     438           4 RESUME                   0
                                    6 BUILD_LIST               0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                31 (to 74)
                      
-                     423          12 STORE_DEREF              1 (item)
+                     439          12 STORE_DEREF              1 (item)
                                   14 LOAD_GLOBAL              1 (NULL + any)
                                   26 LOAD_CLOSURE             1 (item)
                                   28 BUILD_TUPLE              1
-                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 423>)
+                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 439>)
                                   32 MAKE_FUNCTION            8 (closure)
                      
-                     424          34 LOAD_DEREF               2 (ls)
+                     440          34 LOAD_DEREF               2 (ls)
                      
-                     423          36 GET_ITER
+                     439          36 GET_ITER
                                   38 PRECALL                  0
                                   42 CALL                     0
                                   52 PRECALL                  1
                                   56 CALL                     1
                      
-                     422          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
+                     438          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
                      
-                     423          68 LOAD_DEREF               1 (item)
+                     439          68 LOAD_DEREF               1 (item)
                      
-                     422          70 LIST_APPEND              2
+                     438          70 LIST_APPEND              2
                                   72 JUMP_BACKWARD           32 (to 10)
                              >>   74 RETURN_VALUE
                      consts
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
@@ -4019,23 +4294,23 @@
                            code
                               0x95014b00010097007c005d2b7d018902a0000000000000000000000000
                               000000000000000000a6000000ab000000000000000000a0010000000000
                               0000000000000000000000000000007c01a6010000ab0100000000000000
                               005600970101008c2c64005300
                                          0 COPY_FREE_VARS           1
                            
-                           423           2 RETURN_GENERATOR
+                           439           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                43 (to 98)
                            
-                           424          12 STORE_FAST               1 (ext)
+                           440          12 STORE_FAST               1 (ext)
                            
-                           423          14 LOAD_DEREF               2 (item)
+                           439          14 LOAD_DEREF               2 (item)
                                         16 LOAD_METHOD              0 (lower)
                                         38 PRECALL                  0
                                         42 CALL                     0
                                         52 LOAD_METHOD              1 (endswith)
                                         74 LOAD_FAST                1 (ext)
                                         76 PRECALL                  1
                                         80 CALL                     1
@@ -4047,304 +4322,322 @@
                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('lower', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                            name       '<genexpr>'
-                           firstlineno 423
+                           firstlineno 439
                            lnotab 0x0c0102ff
                      names      ('any',)
                      varnames   ('.0',)
                      freevars   ('ls',)
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 422
+                     firstlineno 438
                      lnotab 0x0c01160102ff1eff020102ff
-                  '\x1b[1;32mInitializing conversion sequence\x1b[0m'
+                  'Initializing conversion sequence'
                   -4
                   'txt'
                   -3
                   'Converting '
                   '..'
                   False
                   ('index',)
-                  'Preparing to write: \x1b[1;33m'
-                  ' \x1b[1;30m characters\x1b[1;33m '
-                  '\x1b[1;30m words \x1b[1;33m'
-                  '\x1b[1;30m lines \x1b[0m'
+                  'Preparing to write: '
+                  ' \x1b[1;30m characters'
+                  ' '
+                  '\x1b[1;30m words '
+                  '\x1b[1;30m lines '
                   '\n'
                   ('end',)
                   'w'
-                  '\x1b[1;32mConversion successful!\x1b[0m'
+                  'Conversion successful!'
                   '\nExiting'
                   1
                   'Oops Conversion failed:'
-               names      ('preprocess', 'print', 'lower', 'endswith', 'logger', 'info', 'pd', 'read_excel', 'to_string', 'len', 'split', 'splitlines', 'open', 'write', 'KeyboardInterrupt', 'sys', 'exit', 'Exception', 'str')
+               names      ('preprocess', 'print', 'DGREEN', 'RESET', 'lower', 'endswith', 'logger', 'info', 'pd', 'read_excel', 'to_string', 'len', 'split', 'splitlines', 'DYELLOW', 'open', 'write', 'KeyboardInterrupt', 'sys', 'exit', 'Exception', 'str')
                varnames   ('self', 'xls_list', 'xls_file', 'txt_file', 'df', 'text', 'chars', 'words', 'lines', 'file', 'e')
                freevars   ()
                cellvars   ('ls',)
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'convert_xls_to_text'
-               firstlineno 419
+               firstlineno 435
                lnotab
-                  0x040128010801080102ff12031e010a014e011c014e011a0102023c0128
-                  032c011e01420142020c01080102ff040102ff060202fd120522012aff2e
-                  03280112011e012e0112014eff08e4
+                  0x040128010801080102ff12033c010a014e011c014e011a0102023c0128
+                  032c011e01420142020c0116010cff040102ff04010cff020102ff04020c
+                  fe040202fd120522012aff2e03460112011e012e0112014eff08e4
             code
                argcount  : 1
                nlocals   : 8
-               stacksize : 7
+               stacksize : 8
                flags     : 3
                code
                   0x870897007c00a0000000000000000000000000000000000000000000a6
                   000000ab0000000000000000007d016401640267028a0888086601640384
-                  087c014400a6000000ab0000000000000000007d017c01440090015d757d
+                  087c014400a6000000ab0000000000000000007d017c01440090015da17d
                   027c02a0010000000000000000000000000000000000000000a6000000ab
                   000000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab010000000000000000720e7c02640064048502190000
                   0000000000000064057a0000007d036e347c02a001000000000000000000
                   0000000000000000000000a6000000ab000000000000000000a002000000
                   00000000000000000000000000000000006402a6010000ab010000000000
                   000000720d7c026400640685021900000000000000000064057a0000007d
-                  03090009007407000000000000000000006407a6010000ab010000000000
-                  00000001007409000000000000000000006a0500000000000000007c02a6
-                  010000ab0100000000000000007d04740c00000000000000000000a00700
+                  03090009007407000000000000000000007408000000000000000000009b
+                  006407740a000000000000000000009b009d03a6010000ab010000000000
+                  0000000100740d000000000000000000006a0700000000000000007c02a6
+                  010000ab0100000000000000007d04741000000000000000000000a00900
                   0000000000000000000000000000000000000064087c029b0064099d03a6
-                  010000ab01000000000000000001007c046a080000000000000000640a19
-                  0000000000000000007d05740700000000000000000000640b7c059b0064
-                  0c9d03640dac0ea6020000ab020000000000000000010074130000000000
-                  0000000000640fa6010000ab01000000000000000044005d177d06740700
-                  00000000000000000064107c069b0064119d036412ac0ea6020000ab0200
-                  0000000000000001008c1809007c04a00a00000000000000000000000000
-                  000000000000007c036413ac14a6020000ab020000000000000000010074
-                  07000000000000000000006415a6010000ab010000000000000000010090
-                  018c21230074160000000000000000000024007227010074070000000000
-                  00000000006416a6010000ab010000000000000000010074190000000000
-                  00000000006a0d00000000000000006417a6010000ab0100000000000000
-                  000100590090018c51741c000000000000000000002400721a7d07740700
-                  0000000000000000007c07a6010000ab0100000000000000000100590064
-                  007d077e0790018c6f64007d077e077701770078035900770164005300
+                  010000ab01000000000000000001007c046a0a0000000000000000640a19
+                  0000000000000000007d05740700000000000000000000640b7416000000
+                  000000000000009b007c059b00640c740a000000000000000000009b009d
+                  05640dac0ea6020000ab0200000000000000000100741900000000000000
+                  000000640fa6010000ab01000000000000000044005d177d067407000000
+                  0000000000000064107c069b0064119d036412ac0ea6020000ab02000000
+                  000000000001008c1809007c04a00d000000000000000000000000000000
+                  00000000007c036413ac14a6020000ab0200000000000000000100740700
+                  000000000000000000741c000000000000000000009b006415740a000000
+                  000000000000009b009d03a6010000ab010000000000000000010090018c
+                  4d2300741e00000000000000000000240072270100740700000000000000
+                  0000006416a6010000ab0100000000000000000100742100000000000000
+                  0000006a1100000000000000006417a6010000ab01000000000000000001
+                  00590090018c7d7424000000000000000000002400721a7d077407000000
+                  000000000000007c07a6010000ab0100000000000000000100590064007d
+                  077e0790018c9b64007d077e077701770078035900770164005300
                              0 MAKE_CELL                8 (ls)
                
-               461           2 RESUME                   0
+               477           2 RESUME                   0
                
-               462           4 LOAD_FAST                0 (self)
+               478           4 LOAD_FAST                0 (self)
                              6 LOAD_METHOD              0 (preprocess)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 STORE_FAST               1 (xls_list)
                
-               463          44 LOAD_CONST               1 ('xlsx')
+               479          44 LOAD_CONST               1 ('xlsx')
                             46 LOAD_CONST               2 ('xls')
                             48 BUILD_LIST               2
                             50 STORE_DEREF              8 (ls)
                
-               464          52 LOAD_CLOSURE             8 (ls)
+               480          52 LOAD_CLOSURE             8 (ls)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 464>)
+                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 480>)
                             58 MAKE_FUNCTION            8 (closure)
                
-               465          60 LOAD_FAST                1 (xls_list)
+               481          60 LOAD_FAST                1 (xls_list)
                
-               464          62 GET_ITER
+               480          62 GET_ITER
                             64 PRECALL                  0
                             68 CALL                     0
                             78 STORE_FAST               1 (xls_list)
                
-               467          80 LOAD_FAST                1 (xls_list)
+               483          80 LOAD_FAST                1 (xls_list)
                             82 GET_ITER
                        >>   84 EXTENDED_ARG             1
-                            86 FOR_ITER               373 (to 834)
+                            86 FOR_ITER               417 (to 922)
                             88 STORE_FAST               2 (xls_file)
                
-               468          90 LOAD_FAST                2 (xls_file)
+               484          90 LOAD_FAST                2 (xls_file)
                             92 LOAD_METHOD              1 (lower)
                            114 PRECALL                  0
                            118 CALL                     0
                            128 LOAD_METHOD              2 (endswith)
                            150 LOAD_CONST               1 ('xlsx')
                            152 PRECALL                  1
                            156 CALL                     1
                            166 POP_JUMP_FORWARD_IF_FALSE    14 (to 196)
                
-               469         168 LOAD_FAST                2 (xls_file)
+               485         168 LOAD_FAST                2 (xls_file)
                            170 LOAD_CONST               0 (None)
                            172 LOAD_CONST               4 (-4)
                            174 BUILD_SLICE              2
                            176 BINARY_SUBSCR
                            186 LOAD_CONST               5 ('csv')
                            188 BINARY_OP                0 (+)
                            192 STORE_FAST               3 (csv_file)
                            194 JUMP_FORWARD            52 (to 300)
                
-               470     >>  196 LOAD_FAST                2 (xls_file)
+               486     >>  196 LOAD_FAST                2 (xls_file)
                            198 LOAD_METHOD              1 (lower)
                            220 PRECALL                  0
                            224 CALL                     0
                            234 LOAD_METHOD              2 (endswith)
                            256 LOAD_CONST               2 ('xls')
                            258 PRECALL                  1
                            262 CALL                     1
                            272 POP_JUMP_FORWARD_IF_FALSE    13 (to 300)
                
-               471         274 LOAD_FAST                2 (xls_file)
+               487         274 LOAD_FAST                2 (xls_file)
                            276 LOAD_CONST               0 (None)
                            278 LOAD_CONST               6 (-3)
                            280 BUILD_SLICE              2
                            282 BINARY_SUBSCR
                            292 LOAD_CONST               5 ('csv')
                            294 BINARY_OP                0 (+)
                            298 STORE_FAST               3 (csv_file)
                
-               472     >>  300 NOP
+               488     >>  300 NOP
                
-               473         302 NOP
+               489         302 NOP
                
-               474         304 LOAD_GLOBAL              7 (NULL + print)
-                           316 LOAD_CONST               7 ('\x1b[1;32mInitializing conversion sequence\x1b[0m')
-                           318 PRECALL                  1
-                           322 CALL                     1
-                           332 POP_TOP
+               490         304 LOAD_GLOBAL              7 (NULL + print)
+                           316 LOAD_GLOBAL              8 (DGREEN)
+                           328 FORMAT_VALUE             0
+                           330 LOAD_CONST               7 ('Initializing conversion sequence')
+                           332 LOAD_GLOBAL             10 (RESET)
+                           344 FORMAT_VALUE             0
+                           346 BUILD_STRING             3
+                           348 PRECALL                  1
+                           352 CALL                     1
+                           362 POP_TOP
                
-               475         334 LOAD_GLOBAL              9 (NULL + pd)
-                           346 LOAD_ATTR                5 (read_excel)
-                           356 LOAD_FAST                2 (xls_file)
-                           358 PRECALL                  1
-                           362 CALL                     1
-                           372 STORE_FAST               4 (df)
+               491         364 LOAD_GLOBAL             13 (NULL + pd)
+                           376 LOAD_ATTR                7 (read_excel)
+                           386 LOAD_FAST                2 (xls_file)
+                           388 PRECALL                  1
+                           392 CALL                     1
+                           402 STORE_FAST               4 (df)
+               
+               492         404 LOAD_GLOBAL             16 (logger)
+                           416 LOAD_METHOD              9 (info)
+                           438 LOAD_CONST               8 ('Converting ')
+                           440 LOAD_FAST                2 (xls_file)
+                           442 FORMAT_VALUE             0
+                           444 LOAD_CONST               9 ('..')
+                           446 BUILD_STRING             3
+                           448 PRECALL                  1
+                           452 CALL                     1
+                           462 POP_TOP
                
-               476         374 LOAD_GLOBAL             12 (logger)
-                           386 LOAD_METHOD              7 (info)
-                           408 LOAD_CONST               8 ('Converting ')
-                           410 LOAD_FAST                2 (xls_file)
-                           412 FORMAT_VALUE             0
-                           414 LOAD_CONST               9 ('..')
-                           416 BUILD_STRING             3
-                           418 PRECALL                  1
-                           422 CALL                     1
-                           432 POP_TOP
+               493         464 LOAD_FAST                4 (df)
+                           466 LOAD_ATTR               10 (shape)
+                           476 LOAD_CONST              10 (0)
+                           478 BINARY_SUBSCR
+                           488 STORE_FAST               5 (total_rows)
+               
+               494         490 LOAD_GLOBAL              7 (NULL + print)
+                           502 LOAD_CONST              11 ('Writing ')
+                           504 LOAD_GLOBAL             22 (DYELLOW)
+                           516 FORMAT_VALUE             0
+                           518 LOAD_FAST                5 (total_rows)
+                           520 FORMAT_VALUE             0
+                           522 LOAD_CONST              12 (' rows ')
+                           524 LOAD_GLOBAL             10 (RESET)
+                           536 FORMAT_VALUE             0
+                           538 BUILD_STRING             5
+                           540 LOAD_CONST              13 ('\n')
+                           542 KW_NAMES                14
+                           544 PRECALL                  2
+                           548 CALL                     2
+                           558 POP_TOP
+               
+               495         560 LOAD_GLOBAL             25 (NULL + range)
+                           572 LOAD_CONST              15 (101)
+                           574 PRECALL                  1
+                           578 CALL                     1
+                           588 GET_ITER
+                       >>  590 FOR_ITER                23 (to 638)
+                           592 STORE_FAST               6 (i)
+               
+               496         594 LOAD_GLOBAL              7 (NULL + print)
+                           606 LOAD_CONST              16 ('Progress: ')
+                           608 LOAD_FAST                6 (i)
+                           610 FORMAT_VALUE             0
+                           612 LOAD_CONST              17 ('%')
+                           614 BUILD_STRING             3
+                           616 LOAD_CONST              18 ('\r')
+                           618 KW_NAMES                14
+                           620 PRECALL                  2
+                           624 CALL                     2
+                           634 POP_TOP
+                           636 JUMP_BACKWARD           24 (to 590)
+               
+               497     >>  638 NOP
+               
+               498         640 LOAD_FAST                4 (df)
+                           642 LOAD_METHOD             13 (to_csv)
+                           664 LOAD_FAST                3 (csv_file)
+                           666 LOAD_CONST              19 (False)
+                           668 KW_NAMES                20
+                           670 PRECALL                  2
+                           674 CALL                     2
+                           684 POP_TOP
                
-               477         434 LOAD_FAST                4 (df)
-                           436 LOAD_ATTR                8 (shape)
-                           446 LOAD_CONST              10 (0)
-                           448 BINARY_SUBSCR
-                           458 STORE_FAST               5 (total_rows)
-               
-               478         460 LOAD_GLOBAL              7 (NULL + print)
-                           472 LOAD_CONST              11 ('Writing \x1b[1;33m')
-                           474 LOAD_FAST                5 (total_rows)
-                           476 FORMAT_VALUE             0
-                           478 LOAD_CONST              12 (' rows \x1b[0m')
-                           480 BUILD_STRING             3
-                           482 LOAD_CONST              13 ('\n')
-                           484 KW_NAMES                14
-                           486 PRECALL                  2
-                           490 CALL                     2
-                           500 POP_TOP
-               
-               479         502 LOAD_GLOBAL             19 (NULL + range)
-                           514 LOAD_CONST              15 (101)
-                           516 PRECALL                  1
-                           520 CALL                     1
-                           530 GET_ITER
-                       >>  532 FOR_ITER                23 (to 580)
-                           534 STORE_FAST               6 (i)
-               
-               480         536 LOAD_GLOBAL              7 (NULL + print)
-                           548 LOAD_CONST              16 ('Progress: ')
-                           550 LOAD_FAST                6 (i)
-                           552 FORMAT_VALUE             0
-                           554 LOAD_CONST              17 ('%')
-                           556 BUILD_STRING             3
-                           558 LOAD_CONST              18 ('\r')
-                           560 KW_NAMES                14
-                           562 PRECALL                  2
-                           566 CALL                     2
-                           576 POP_TOP
-                           578 JUMP_BACKWARD           24 (to 532)
-               
-               481     >>  580 NOP
-               
-               482         582 LOAD_FAST                4 (df)
-                           584 LOAD_METHOD             10 (to_csv)
-                           606 LOAD_FAST                3 (csv_file)
-                           608 LOAD_CONST              19 (False)
-                           610 KW_NAMES                20
-                           612 PRECALL                  2
-                           616 CALL                     2
-                           626 POP_TOP
+               499         686 LOAD_GLOBAL              7 (NULL + print)
+                           698 LOAD_GLOBAL             28 (DMAGENTA)
+                           710 FORMAT_VALUE             0
+                           712 LOAD_CONST              21 (' Conversion successful')
+                           714 LOAD_GLOBAL             10 (RESET)
+                           726 FORMAT_VALUE             0
+                           728 BUILD_STRING             3
+                           730 PRECALL                  1
+                           734 CALL                     1
+                           744 POP_TOP
+                           746 EXTENDED_ARG             1
+                           748 JUMP_BACKWARD          333 (to 84)
+                       >>  750 PUSH_EXC_INFO
+               
+               500         752 LOAD_GLOBAL             30 (KeyboardInterrupt)
+                           764 CHECK_EXC_MATCH
+                           766 POP_JUMP_FORWARD_IF_FALSE    39 (to 846)
+                           768 POP_TOP
+               
+               501         770 LOAD_GLOBAL              7 (NULL + print)
+                           782 LOAD_CONST              22 ('Exiting')
+                           784 PRECALL                  1
+                           788 CALL                     1
+                           798 POP_TOP
                
-               483         628 LOAD_GLOBAL              7 (NULL + print)
-                           640 LOAD_CONST              21 ('\x1b[1;95m Conversion successful\x1b[0m')
-                           642 PRECALL                  1
-                           646 CALL                     1
-                           656 POP_TOP
-                           658 EXTENDED_ARG             1
-                           660 JUMP_BACKWARD          289 (to 84)
-                       >>  662 PUSH_EXC_INFO
+               502         800 LOAD_GLOBAL             33 (NULL + sys)
+                           812 LOAD_ATTR               17 (exit)
+                           822 LOAD_CONST              23 (1)
+                           824 PRECALL                  1
+                           828 CALL                     1
+                           838 POP_TOP
+                           840 POP_EXCEPT
+                           842 EXTENDED_ARG             1
+                           844 JUMP_BACKWARD          381 (to 84)
                
-               484         664 LOAD_GLOBAL             22 (KeyboardInterrupt)
-                           676 CHECK_EXC_MATCH
-                           678 POP_JUMP_FORWARD_IF_FALSE    39 (to 758)
-                           680 POP_TOP
+               503     >>  846 LOAD_GLOBAL             36 (Exception)
+                           858 CHECK_EXC_MATCH
+                           860 POP_JUMP_FORWARD_IF_FALSE    26 (to 914)
+                           862 STORE_FAST               7 (e)
                
-               485         682 LOAD_GLOBAL              7 (NULL + print)
-                           694 LOAD_CONST              22 ('Exiting')
-                           696 PRECALL                  1
-                           700 CALL                     1
-                           710 POP_TOP
-               
-               486         712 LOAD_GLOBAL             25 (NULL + sys)
-                           724 LOAD_ATTR               13 (exit)
-                           734 LOAD_CONST              23 (1)
-                           736 PRECALL                  1
-                           740 CALL                     1
-                           750 POP_TOP
-                           752 POP_EXCEPT
-                           754 EXTENDED_ARG             1
-                           756 JUMP_BACKWARD          337 (to 84)
-               
-               487     >>  758 LOAD_GLOBAL             28 (Exception)
-                           770 CHECK_EXC_MATCH
-                           772 POP_JUMP_FORWARD_IF_FALSE    26 (to 826)
-                           774 STORE_FAST               7 (e)
-               
-               488         776 LOAD_GLOBAL              7 (NULL + print)
-                           788 LOAD_FAST                7 (e)
-                           790 PRECALL                  1
-                           794 CALL                     1
-                           804 POP_TOP
-                           806 POP_EXCEPT
-                           808 LOAD_CONST               0 (None)
-                           810 STORE_FAST               7 (e)
-                           812 DELETE_FAST              7 (e)
-                           814 EXTENDED_ARG             1
-                           816 JUMP_BACKWARD          367 (to 84)
-                       >>  818 LOAD_CONST               0 (None)
-                           820 STORE_FAST               7 (e)
-                           822 DELETE_FAST              7 (e)
-                           824 RERAISE                  1
-               
-               487     >>  826 RERAISE                  0
-                       >>  828 COPY                     3
-                           830 POP_EXCEPT
-                           832 RERAISE                  1
+               504         864 LOAD_GLOBAL              7 (NULL + print)
+                           876 LOAD_FAST                7 (e)
+                           878 PRECALL                  1
+                           882 CALL                     1
+                           892 POP_TOP
+                           894 POP_EXCEPT
+                           896 LOAD_CONST               0 (None)
+                           898 STORE_FAST               7 (e)
+                           900 DELETE_FAST              7 (e)
+                           902 EXTENDED_ARG             1
+                           904 JUMP_BACKWARD          411 (to 84)
+                       >>  906 LOAD_CONST               0 (None)
+                           908 STORE_FAST               7 (e)
+                           910 DELETE_FAST              7 (e)
+                           912 RERAISE                  1
+               
+               503     >>  914 RERAISE                  0
+                       >>  916 COPY                     3
+                           918 POP_EXCEPT
+                           920 RERAISE                  1
                
-               467     >>  834 LOAD_CONST               0 (None)
-                           836 RETURN_VALUE
+               483     >>  922 LOAD_CONST               0 (None)
+                           924 RETURN_VALUE
                ExceptionTable:
-                 302 to 656 -> 662 [1]
-                 662 to 750 -> 828 [2] lasti
-                 758 to 774 -> 828 [2] lasti
-                 776 to 804 -> 818 [2] lasti
-                 818 to 826 -> 828 [2] lasti
+                 302 to 744 -> 750 [1]
+                 750 to 838 -> 916 [2] lasti
+                 846 to 862 -> 916 [2] lasti
+                 864 to 892 -> 906 [2] lasti
+                 906 to 914 -> 916 [2] lasti
                consts
                   None
                   'xlsx'
                   'xls'
                   code
                      argcount  : 1
                      nlocals   : 1
@@ -4353,39 +4646,39 @@
                      code
                         0x95018701970067007c005d1f8a01740100000000000000000000880166
                         016400840889024400a6000000ab000000000000000000a6010000ab0100
                         00000000000000af1d890191028c205300
                                    0 COPY_FREE_VARS           1
                                    2 MAKE_CELL                1 (item)
                      
-                     464           4 RESUME                   0
+                     480           4 RESUME                   0
                                    6 BUILD_LIST               0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                31 (to 74)
                      
-                     465          12 STORE_DEREF              1 (item)
+                     481          12 STORE_DEREF              1 (item)
                                   14 LOAD_GLOBAL              1 (NULL + any)
                                   26 LOAD_CLOSURE             1 (item)
                                   28 BUILD_TUPLE              1
-                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 465>)
+                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 481>)
                                   32 MAKE_FUNCTION            8 (closure)
                      
-                     466          34 LOAD_DEREF               2 (ls)
+                     482          34 LOAD_DEREF               2 (ls)
                      
-                     465          36 GET_ITER
+                     481          36 GET_ITER
                                   38 PRECALL                  0
                                   42 CALL                     0
                                   52 PRECALL                  1
                                   56 CALL                     1
                      
-                     464          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
+                     480          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
                      
-                     465          68 LOAD_DEREF               1 (item)
+                     481          68 LOAD_DEREF               1 (item)
                      
-                     464          70 LIST_APPEND              2
+                     480          70 LIST_APPEND              2
                                   72 JUMP_BACKWARD           32 (to 10)
                              >>   74 RETURN_VALUE
                      consts
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
@@ -4393,23 +4686,23 @@
                            code
                               0x95014b00010097007c005d2b7d018902a0000000000000000000000000
                               000000000000000000a6000000ab000000000000000000a0010000000000
                               0000000000000000000000000000007c01a6010000ab0100000000000000
                               005600970101008c2c64005300
                                          0 COPY_FREE_VARS           1
                            
-                           465           2 RETURN_GENERATOR
+                           481           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                43 (to 98)
                            
-                           466          12 STORE_FAST               1 (ext)
+                           482          12 STORE_FAST               1 (ext)
                            
-                           465          14 LOAD_DEREF               2 (item)
+                           481          14 LOAD_DEREF               2 (item)
                                         16 LOAD_METHOD              0 (lower)
                                         38 PRECALL                  0
                                         42 CALL                     0
                                         52 LOAD_METHOD              1 (endswith)
                                         74 LOAD_FAST                1 (ext)
                                         76 PRECALL                  1
                                         80 CALL                     1
@@ -4421,362 +4714,391 @@
                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('lower', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                            name       '<genexpr>'
-                           firstlineno 465
+                           firstlineno 481
                            lnotab 0x0c0102ff
                      names      ('any',)
                      varnames   ('.0',)
                      freevars   ('ls',)
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 464
+                     firstlineno 480
                      lnotab 0x0c01160102ff1eff020102ff
                   -4
                   'csv'
                   -3
-                  '\x1b[1;32mInitializing conversion sequence\x1b[0m'
+                  'Initializing conversion sequence'
                   'Converting '
                   '..'
                   0
-                  'Writing \x1b[1;33m'
-                  ' rows \x1b[0m'
+                  'Writing '
+                  ' rows '
                   '\n'
                   ('end',)
                   101
                   'Progress: '
                   '%'
                   '\r'
                   False
                   ('index',)
-                  '\x1b[1;95m Conversion successful\x1b[0m'
+                  ' Conversion successful'
                   'Exiting'
                   1
-               names      ('preprocess', 'lower', 'endswith', 'print', 'pd', 'read_excel', 'logger', 'info', 'shape', 'range', 'to_csv', 'KeyboardInterrupt', 'sys', 'exit', 'Exception')
+               names      ('preprocess', 'lower', 'endswith', 'print', 'DGREEN', 'RESET', 'pd', 'read_excel', 'logger', 'info', 'shape', 'DYELLOW', 'range', 'to_csv', 'DMAGENTA', 'KeyboardInterrupt', 'sys', 'exit', 'Exception')
                varnames   ('self', 'xls_list', 'xls_file', 'csv_file', 'df', 'total_rows', 'i', 'e')
                freevars   ()
                cellvars   ('ls',)
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'convert_xlsx_to_csv'
-               firstlineno 461
+               firstlineno 477
                lnotab
-                  0x040128010801080102ff12030a014e011c014e011a01020102011e0128
-                  013c011a012a0122012c0102012e01240112011e012e01120132ff08ec
+                  0x040128010801080102ff12030a014e011c014e011a01020102013c0128
+                  013c011a01460122012c0102012e01420112011e012e01120132ff08ec
             code
                argcount  : 1
                nlocals   : 11
                stacksize : 8
                flags     : 3
                code
                   0x870b97007c00a0000000000000000000000000000000000000000000a6
                   000000ab0000000000000000007d016401640267028a0b880b6601640384
-                  087c014400a6000000ab0000000000000000007d017c01440090015ddd7d
+                  087c014400a6000000ab0000000000000000007d017c01440090025d277d
                   027c02a0010000000000000000000000000000000000000000a6000000ab
                   000000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab010000000000000000720b7c02640064048502190000
                   000000000000007d036e317c02a001000000000000000000000000000000
                   0000000000a6000000ab000000000000000000a002000000000000000000
                   00000000000000000000006402a6010000ab010000000000000000720a7c
                   02640064058502190000000000000000007d030900740700000000000000
-                  0000006406a6010000ab0100000000000000007d04740700000000000000
-                  0000006407a6010000ab0100000000000000007d05740900000000000000
+                  0000007408000000000000000000009b006406740a000000000000000000
+                  009b009d03a6010000ab0100000000000000007d04740700000000000000
+                  0000006407a6010000ab0100000000000000007d05740d00000000000000
                   0000007c04a6010000ab01000000000000000064086b020000000072077c
                   0364097a0000007d047c037d057c04a00200000000000000000000000000
                   00000000000000640aa6010000ab01000000000000000073057c04640a7a
-                  0000007d04640b7d06740b00000000000000000000640ca6010000ab0100
-                  0000000000000044005d077d077c06640b7a0d00007d068c08740d000000
+                  0000007d04640b7d06740f00000000000000000000640ca6010000ab0100
+                  0000000000000044005d077d077c06640b7a0d00007d068c087411000000
                   00000000000000640d7c029b00640e9d03a6010000ab0100000000000000
-                  000100740f000000000000000000006a0800000000000000007c02a60100
-                  00ab0100000000000000007d08740d00000000000000000000640fa60100
-                  00ab0100000000000000000100740d000000000000000000006410a60100
-                  00ab01000000000000000001007413000000000000000000006a0a000000
-                  00000000007c04a6010000ab0100000000000000007d09740d0000000000
-                  00000000006411a6010000ab01000000000000000001007c08a00b000000
+                  0001007413000000000000000000006a0a00000000000000007c02a60100
+                  00ab0100000000000000007d087411000000000000000000007416000000
+                  000000000000009b00640f740a000000000000000000009b009d03a60100
+                  00ab01000000000000000001007411000000000000000000007416000000
+                  000000000000009b006410740a000000000000000000009b009d03a60100
+                  00ab01000000000000000001007419000000000000000000006a0d000000
+                  00000000007c04a6010000ab0100000000000000007d0974110000000000
+                  0000000000741c000000000000000000009b006411740a00000000000000
+                  0000009b009d03a6010000ab01000000000000000001007c08a00f000000
                   00000000000000000000000000000000007c057c067c0964126413ac14a6
-                  050000ab0500000000000000000100740d0000000000000000000064157c
-                  049b0064169d03a6010000ab01000000000000000001007c09a00c000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  00010090018c7d2300741a00000000000000000000240072270100740d00
-                  0000000000000000006417a6010000ab0100000000000000000100741d00
-                  0000000000000000006a0f00000000000000006418a6010000ab01000000
-                  00000000000100590090018cad742000000000000000000000240072267d
-                  0a742200000000000000000000a012000000000000000000000000000000
-                  00000000007c0a9b00a6010000ab0100000000000000000100590064007d
-                  0a7e0a90018cd764007d0a7e0a7701770078035900770164005300
+                  050000ab0500000000000000000100741100000000000000000000641574
+                  0a000000000000000000009b0064167c049b00740a000000000000000000
+                  009b009d05a6010000ab01000000000000000001007c09a0100000000000
+                  000000000000000000000000000000a6000000ab00000000000000000001
+                  0090018cc723007422000000000000000000002400722701007411000000
+                  000000000000006417a6010000ab01000000000000000001007425000000
+                  000000000000006a1300000000000000006418a6010000ab010000000000
+                  0000000100590090018cf7742800000000000000000000240072267d0a74
+                  2a00000000000000000000a0160000000000000000000000000000000000
+                  0000007c0a9b00a6010000ab0100000000000000000100590064007d0a7e
+                  0a90028c2164007d0a7e0a7701770078035900770164005300
                              0 MAKE_CELL               11 (ls)
                
-               494           2 RESUME                   0
+               510           2 RESUME                   0
                
-               495           4 LOAD_FAST                0 (self)
+               511           4 LOAD_FAST                0 (self)
                              6 LOAD_METHOD              0 (preprocess)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 STORE_FAST               1 (xlsx_list)
                
-               496          44 LOAD_CONST               1 ('xlsx')
+               512          44 LOAD_CONST               1 ('xlsx')
                             46 LOAD_CONST               2 ('xls')
                             48 BUILD_LIST               2
                             50 STORE_DEREF             11 (ls)
                
-               497          52 LOAD_CLOSURE            11 (ls)
+               513          52 LOAD_CLOSURE            11 (ls)
                             54 BUILD_TUPLE              1
-                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 497>)
+                            56 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 513>)
                             58 MAKE_FUNCTION            8 (closure)
                
-               498          60 LOAD_FAST                1 (xlsx_list)
+               514          60 LOAD_FAST                1 (xlsx_list)
                
-               497          62 GET_ITER
+               513          62 GET_ITER
                             64 PRECALL                  0
                             68 CALL                     0
                             78 STORE_FAST               1 (xlsx_list)
                
-               500          80 LOAD_FAST                1 (xlsx_list)
+               516          80 LOAD_FAST                1 (xlsx_list)
                             82 GET_ITER
-                       >>   84 EXTENDED_ARG             1
-                            86 FOR_ITER               477 (to 1042)
+                       >>   84 EXTENDED_ARG             2
+                            86 FOR_ITER               551 (to 1190)
                             88 STORE_FAST               2 (xlsx_file)
                
-               501          90 LOAD_FAST                2 (xlsx_file)
+               517          90 LOAD_FAST                2 (xlsx_file)
                             92 LOAD_METHOD              1 (lower)
                            114 PRECALL                  0
                            118 CALL                     0
                            128 LOAD_METHOD              2 (endswith)
                            150 LOAD_CONST               1 ('xlsx')
                            152 PRECALL                  1
                            156 CALL                     1
                            166 POP_JUMP_FORWARD_IF_FALSE    11 (to 190)
                
-               502         168 LOAD_FAST                2 (xlsx_file)
+               518         168 LOAD_FAST                2 (xlsx_file)
                            170 LOAD_CONST               0 (None)
                            172 LOAD_CONST               4 (-4)
                            174 BUILD_SLICE              2
                            176 BINARY_SUBSCR
                            186 STORE_FAST               3 (sqlfile)
                            188 JUMP_FORWARD            49 (to 288)
                
-               503     >>  190 LOAD_FAST                2 (xlsx_file)
+               519     >>  190 LOAD_FAST                2 (xlsx_file)
                            192 LOAD_METHOD              1 (lower)
                            214 PRECALL                  0
                            218 CALL                     0
                            228 LOAD_METHOD              2 (endswith)
                            250 LOAD_CONST               2 ('xls')
                            252 PRECALL                  1
                            256 CALL                     1
                            266 POP_JUMP_FORWARD_IF_FALSE    10 (to 288)
                
-               504         268 LOAD_FAST                2 (xlsx_file)
+               520         268 LOAD_FAST                2 (xlsx_file)
                            270 LOAD_CONST               0 (None)
                            272 LOAD_CONST               5 (-3)
                            274 BUILD_SLICE              2
                            276 BINARY_SUBSCR
                            286 STORE_FAST               3 (sqlfile)
                
-               505     >>  288 NOP
-               
-               506         290 LOAD_GLOBAL              7 (NULL + input)
-               
-               507         302 LOAD_CONST               6 ('\x1b[1;34m Please enter desired sql filename: \x1b[0m')
+               521     >>  288 NOP
                
-               506         304 PRECALL                  1
-                           308 CALL                     1
-                           318 STORE_FAST               4 (db_file)
+               522         290 LOAD_GLOBAL              7 (NULL + input)
                
-               508         320 LOAD_GLOBAL              7 (NULL + input)
+               523         302 LOAD_GLOBAL              8 (DBLUE)
+                           314 FORMAT_VALUE             0
+                           316 LOAD_CONST               6 ('Please enter desired sql filename: ')
+                           318 LOAD_GLOBAL             10 (RESET)
+                           330 FORMAT_VALUE             0
+                           332 BUILD_STRING             3
                
-               509         332 LOAD_CONST               7 ('\x1b[1;37m Please enter desired table name: \x1b[0m')
-               
-               508         334 PRECALL                  1
+               522         334 PRECALL                  1
                            338 CALL                     1
-                           348 STORE_FAST               5 (table_name)
+                           348 STORE_FAST               4 (db_file)
                
-               511         350 LOAD_GLOBAL              9 (NULL + any)
-                           362 LOAD_FAST                4 (db_file)
-                           364 PRECALL                  1
-                           368 CALL                     1
-                           378 LOAD_CONST               8 ('')
-                           380 COMPARE_OP               2 (==)
-                           386 POP_JUMP_FORWARD_IF_FALSE     7 (to 402)
-               
-               512         388 LOAD_FAST                3 (sqlfile)
-                           390 LOAD_CONST               9 ('sql')
-                           392 BINARY_OP                0 (+)
-                           396 STORE_FAST               4 (db_file)
-               
-               513         398 LOAD_FAST                3 (sqlfile)
-                           400 STORE_FAST               5 (table_name)
-               
-               514     >>  402 LOAD_FAST                4 (db_file)
-                           404 LOAD_METHOD              2 (endswith)
-                           426 LOAD_CONST              10 ('.sql')
-                           428 PRECALL                  1
-                           432 CALL                     1
-                           442 POP_JUMP_FORWARD_IF_TRUE     5 (to 454)
-               
-               515         444 LOAD_FAST                4 (db_file)
-                           446 LOAD_CONST              10 ('.sql')
-                           448 BINARY_OP                0 (+)
-                           452 STORE_FAST               4 (db_file)
-               
-               516     >>  454 LOAD_CONST              11 (0)
-                           456 STORE_FAST               6 (column)
-               
-               517         458 LOAD_GLOBAL             11 (NULL + range)
-                           470 LOAD_CONST              12 (20)
-                           472 PRECALL                  1
-                           476 CALL                     1
-                           486 GET_ITER
-                       >>  488 FOR_ITER                 7 (to 504)
-                           490 STORE_FAST               7 (i)
-               
-               518         492 LOAD_FAST                6 (column)
-                           494 LOAD_CONST              11 (0)
-                           496 BINARY_OP               13 (+=)
-                           500 STORE_FAST               6 (column)
-                           502 JUMP_BACKWARD            8 (to 488)
-               
-               520     >>  504 LOAD_GLOBAL             13 (NULL + print)
-                           516 LOAD_CONST              13 ('Reading ')
-                           518 LOAD_FAST                2 (xlsx_file)
-                           520 FORMAT_VALUE             0
-                           522 LOAD_CONST              14 ('...')
-                           524 BUILD_STRING             3
-                           526 PRECALL                  1
-                           530 CALL                     1
-                           540 POP_TOP
-               
-               521         542 LOAD_GLOBAL             15 (NULL + pd)
-                           554 LOAD_ATTR                8 (read_excel)
-                           564 LOAD_FAST                2 (xlsx_file)
-                           566 PRECALL                  1
-                           570 CALL                     1
-                           580 STORE_FAST               8 (df)
+               524         350 LOAD_GLOBAL              7 (NULL + input)
                
-               522         582 LOAD_GLOBAL             13 (NULL + print)
-                           594 LOAD_CONST              15 ('\x1b[1;32mInitializing conversion sequence\x1b[0m')
-                           596 PRECALL                  1
-                           600 CALL                     1
-                           610 POP_TOP
+               525         362 LOAD_CONST               7 ('Please enter desired table name: ')
                
-               523         612 LOAD_GLOBAL             13 (NULL + print)
-                           624 LOAD_CONST              16 ('\x1b[1;32m Connected to sqlite3 database::\x1b[0m')
-                           626 PRECALL                  1
-                           630 CALL                     1
-                           640 POP_TOP
+               524         364 PRECALL                  1
+                           368 CALL                     1
+                           378 STORE_FAST               5 (table_name)
                
-               525         642 LOAD_GLOBAL             19 (NULL + sqlite3)
-                           654 LOAD_ATTR               10 (connect)
-                           664 LOAD_FAST                4 (db_file)
-                           666 PRECALL                  1
-                           670 CALL                     1
-                           680 STORE_FAST               9 (conn)
-               
-               526         682 LOAD_GLOBAL             13 (NULL + print)
-                           694 LOAD_CONST              17 ('\x1b[1;33m Creating database table::\x1b[0m')
-                           696 PRECALL                  1
-                           700 CALL                     1
-                           710 POP_TOP
-               
-               528         712 LOAD_FAST                8 (df)
-                           714 LOAD_METHOD             11 (to_sql)
-                           736 LOAD_FAST                5 (table_name)
-                           738 LOAD_FAST                6 (column)
-                           740 LOAD_FAST                9 (conn)
-               
-               529         742 LOAD_CONST              18 ('replace')
-                           744 LOAD_CONST              19 (False)
-               
-               528         746 KW_NAMES                20
-                           748 PRECALL                  5
-                           752 CALL                     5
-                           762 POP_TOP
-               
-               530         764 LOAD_GLOBAL             13 (NULL + print)
-               
-               531         776 LOAD_CONST              21 ('Operation successful\x1b[0m file saved as \x1b[32')
-                           778 LOAD_FAST                4 (db_file)
-                           780 FORMAT_VALUE             0
-                           782 LOAD_CONST              22 ('\x1b[0m')
-                           784 BUILD_STRING             3
+               527         380 LOAD_GLOBAL             13 (NULL + any)
+                           392 LOAD_FAST                4 (db_file)
+                           394 PRECALL                  1
+                           398 CALL                     1
+                           408 LOAD_CONST               8 ('')
+                           410 COMPARE_OP               2 (==)
+                           416 POP_JUMP_FORWARD_IF_FALSE     7 (to 432)
+               
+               528         418 LOAD_FAST                3 (sqlfile)
+                           420 LOAD_CONST               9 ('sql')
+                           422 BINARY_OP                0 (+)
+                           426 STORE_FAST               4 (db_file)
+               
+               529         428 LOAD_FAST                3 (sqlfile)
+                           430 STORE_FAST               5 (table_name)
+               
+               530     >>  432 LOAD_FAST                4 (db_file)
+                           434 LOAD_METHOD              2 (endswith)
+                           456 LOAD_CONST              10 ('.sql')
+                           458 PRECALL                  1
+                           462 CALL                     1
+                           472 POP_JUMP_FORWARD_IF_TRUE     5 (to 484)
                
-               530         786 PRECALL                  1
-                           790 CALL                     1
-                           800 POP_TOP
+               531         474 LOAD_FAST                4 (db_file)
+                           476 LOAD_CONST              10 ('.sql')
+                           478 BINARY_OP                0 (+)
+                           482 STORE_FAST               4 (db_file)
+               
+               532     >>  484 LOAD_CONST              11 (0)
+                           486 STORE_FAST               6 (column)
+               
+               533         488 LOAD_GLOBAL             15 (NULL + range)
+                           500 LOAD_CONST              12 (20)
+                           502 PRECALL                  1
+                           506 CALL                     1
+                           516 GET_ITER
+                       >>  518 FOR_ITER                 7 (to 534)
+                           520 STORE_FAST               7 (i)
+               
+               534         522 LOAD_FAST                6 (column)
+                           524 LOAD_CONST              11 (0)
+                           526 BINARY_OP               13 (+=)
+                           530 STORE_FAST               6 (column)
+                           532 JUMP_BACKWARD            8 (to 518)
+               
+               536     >>  534 LOAD_GLOBAL             17 (NULL + print)
+                           546 LOAD_CONST              13 ('Reading ')
+                           548 LOAD_FAST                2 (xlsx_file)
+                           550 FORMAT_VALUE             0
+                           552 LOAD_CONST              14 ('...')
+                           554 BUILD_STRING             3
+                           556 PRECALL                  1
+                           560 CALL                     1
+                           570 POP_TOP
                
-               533         802 LOAD_FAST                9 (conn)
-                           804 LOAD_METHOD             12 (close)
-                           826 PRECALL                  0
-                           830 CALL                     0
-                           840 POP_TOP
-                           842 EXTENDED_ARG             1
-                           844 JUMP_BACKWARD          381 (to 84)
-                       >>  846 PUSH_EXC_INFO
+               537         572 LOAD_GLOBAL             19 (NULL + pd)
+                           584 LOAD_ATTR               10 (read_excel)
+                           594 LOAD_FAST                2 (xlsx_file)
+                           596 PRECALL                  1
+                           600 CALL                     1
+                           610 STORE_FAST               8 (df)
                
-               534         848 LOAD_GLOBAL             26 (KeyboardInterrupt)
-                           860 CHECK_EXC_MATCH
-                           862 POP_JUMP_FORWARD_IF_FALSE    39 (to 942)
-                           864 POP_TOP
-               
-               535         866 LOAD_GLOBAL             13 (NULL + print)
-                           878 LOAD_CONST              23 ('\nExiting')
-                           880 PRECALL                  1
-                           884 CALL                     1
-                           894 POP_TOP
+               538         612 LOAD_GLOBAL             17 (NULL + print)
+                           624 LOAD_GLOBAL             22 (DGREEN)
+                           636 FORMAT_VALUE             0
+                           638 LOAD_CONST              15 ('Initializing conversion sequence')
+                           640 LOAD_GLOBAL             10 (RESET)
+                           652 FORMAT_VALUE             0
+                           654 BUILD_STRING             3
+                           656 PRECALL                  1
+                           660 CALL                     1
+                           670 POP_TOP
                
-               536         896 LOAD_GLOBAL             29 (NULL + sys)
-                           908 LOAD_ATTR               15 (exit)
-                           918 LOAD_CONST              24 (1)
-                           920 PRECALL                  1
-                           924 CALL                     1
-                           934 POP_TOP
-                           936 POP_EXCEPT
-                           938 EXTENDED_ARG             1
-                           940 JUMP_BACKWARD          429 (to 84)
-               
-               537     >>  942 LOAD_GLOBAL             32 (Exception)
-                           954 CHECK_EXC_MATCH
-                           956 POP_JUMP_FORWARD_IF_FALSE    38 (to 1034)
-                           958 STORE_FAST              10 (e)
-               
-               538         960 LOAD_GLOBAL             34 (logger)
-                           972 LOAD_METHOD             18 (error)
-                           994 LOAD_FAST               10 (e)
-                           996 FORMAT_VALUE             0
-                           998 PRECALL                  1
-                          1002 CALL                     1
+               539         672 LOAD_GLOBAL             17 (NULL + print)
+                           684 LOAD_GLOBAL             22 (DGREEN)
+                           696 FORMAT_VALUE             0
+                           698 LOAD_CONST              16 (' Connected to sqlite3 database::')
+                           700 LOAD_GLOBAL             10 (RESET)
+                           712 FORMAT_VALUE             0
+                           714 BUILD_STRING             3
+                           716 PRECALL                  1
+                           720 CALL                     1
+                           730 POP_TOP
+               
+               541         732 LOAD_GLOBAL             25 (NULL + sqlite3)
+                           744 LOAD_ATTR               13 (connect)
+                           754 LOAD_FAST                4 (db_file)
+                           756 PRECALL                  1
+                           760 CALL                     1
+                           770 STORE_FAST               9 (conn)
+               
+               542         772 LOAD_GLOBAL             17 (NULL + print)
+                           784 LOAD_GLOBAL             28 (DYELLOW)
+                           796 FORMAT_VALUE             0
+                           798 LOAD_CONST              17 (' Creating database table::')
+                           800 LOAD_GLOBAL             10 (RESET)
+                           812 FORMAT_VALUE             0
+                           814 BUILD_STRING             3
+                           816 PRECALL                  1
+                           820 CALL                     1
+                           830 POP_TOP
+               
+               544         832 LOAD_FAST                8 (df)
+                           834 LOAD_METHOD             15 (to_sql)
+                           856 LOAD_FAST                5 (table_name)
+                           858 LOAD_FAST                6 (column)
+                           860 LOAD_FAST                9 (conn)
+               
+               545         862 LOAD_CONST              18 ('replace')
+                           864 LOAD_CONST              19 (False)
+               
+               544         866 KW_NAMES                20
+                           868 PRECALL                  5
+                           872 CALL                     5
+                           882 POP_TOP
+               
+               546         884 LOAD_GLOBAL             17 (NULL + print)
+               
+               547         896 LOAD_CONST              21 ('Operation successful')
+                           898 LOAD_GLOBAL             10 (RESET)
+                           910 FORMAT_VALUE             0
+                           912 LOAD_CONST              22 (' file saved as \x1b[32')
+                           914 LOAD_FAST                4 (db_file)
+                           916 FORMAT_VALUE             0
+                           918 LOAD_GLOBAL             10 (RESET)
+                           930 FORMAT_VALUE             0
+                           932 BUILD_STRING             5
+               
+               546         934 PRECALL                  1
+                           938 CALL                     1
+                           948 POP_TOP
+               
+               549         950 LOAD_FAST                9 (conn)
+                           952 LOAD_METHOD             16 (close)
+                           974 PRECALL                  0
+                           978 CALL                     0
+                           988 POP_TOP
+                           990 EXTENDED_ARG             1
+                           992 JUMP_BACKWARD          455 (to 84)
+                       >>  994 PUSH_EXC_INFO
+               
+               550         996 LOAD_GLOBAL             34 (KeyboardInterrupt)
+                          1008 CHECK_EXC_MATCH
+                          1010 POP_JUMP_FORWARD_IF_FALSE    39 (to 1090)
                           1012 POP_TOP
-                          1014 POP_EXCEPT
-                          1016 LOAD_CONST               0 (None)
-                          1018 STORE_FAST              10 (e)
-                          1020 DELETE_FAST             10 (e)
-                          1022 EXTENDED_ARG             1
-                          1024 JUMP_BACKWARD          471 (to 84)
-                       >> 1026 LOAD_CONST               0 (None)
-                          1028 STORE_FAST              10 (e)
-                          1030 DELETE_FAST             10 (e)
-                          1032 RERAISE                  1
-               
-               537     >> 1034 RERAISE                  0
-                       >> 1036 COPY                     3
-                          1038 POP_EXCEPT
-                          1040 RERAISE                  1
                
-               500     >> 1042 LOAD_CONST               0 (None)
-                          1044 RETURN_VALUE
+               551        1014 LOAD_GLOBAL             17 (NULL + print)
+                          1026 LOAD_CONST              23 ('\nExiting')
+                          1028 PRECALL                  1
+                          1032 CALL                     1
+                          1042 POP_TOP
+               
+               552        1044 LOAD_GLOBAL             37 (NULL + sys)
+                          1056 LOAD_ATTR               19 (exit)
+                          1066 LOAD_CONST              24 (1)
+                          1068 PRECALL                  1
+                          1072 CALL                     1
+                          1082 POP_TOP
+                          1084 POP_EXCEPT
+                          1086 EXTENDED_ARG             1
+                          1088 JUMP_BACKWARD          503 (to 84)
+               
+               553     >> 1090 LOAD_GLOBAL             40 (Exception)
+                          1102 CHECK_EXC_MATCH
+                          1104 POP_JUMP_FORWARD_IF_FALSE    38 (to 1182)
+                          1106 STORE_FAST              10 (e)
+               
+               554        1108 LOAD_GLOBAL             42 (logger)
+                          1120 LOAD_METHOD             22 (error)
+                          1142 LOAD_FAST               10 (e)
+                          1144 FORMAT_VALUE             0
+                          1146 PRECALL                  1
+                          1150 CALL                     1
+                          1160 POP_TOP
+                          1162 POP_EXCEPT
+                          1164 LOAD_CONST               0 (None)
+                          1166 STORE_FAST              10 (e)
+                          1168 DELETE_FAST             10 (e)
+                          1170 EXTENDED_ARG             2
+                          1172 JUMP_BACKWARD          545 (to 84)
+                       >> 1174 LOAD_CONST               0 (None)
+                          1176 STORE_FAST              10 (e)
+                          1178 DELETE_FAST             10 (e)
+                          1180 RERAISE                  1
+               
+               553     >> 1182 RERAISE                  0
+                       >> 1184 COPY                     3
+                          1186 POP_EXCEPT
+                          1188 RERAISE                  1
+               
+               516     >> 1190 LOAD_CONST               0 (None)
+                          1192 RETURN_VALUE
                ExceptionTable:
-                 290 to 840 -> 846 [1]
-                 846 to 934 -> 1036 [2] lasti
-                 942 to 958 -> 1036 [2] lasti
-                 960 to 1012 -> 1026 [2] lasti
-                 1026 to 1034 -> 1036 [2] lasti
+                 290 to 988 -> 994 [1]
+                 994 to 1082 -> 1184 [2] lasti
+                 1090 to 1106 -> 1184 [2] lasti
+                 1108 to 1160 -> 1174 [2] lasti
+                 1174 to 1182 -> 1184 [2] lasti
                consts
                   None
                   'xlsx'
                   'xls'
                   code
                      argcount  : 1
                      nlocals   : 1
@@ -4785,39 +5107,39 @@
                      code
                         0x95018701970067007c005d1f8a01740100000000000000000000880166
                         016400840889024400a6000000ab000000000000000000a6010000ab0100
                         00000000000000af1d890191028c205300
                                    0 COPY_FREE_VARS           1
                                    2 MAKE_CELL                1 (item)
                      
-                     497           4 RESUME                   0
+                     513           4 RESUME                   0
                                    6 BUILD_LIST               0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                31 (to 74)
                      
-                     498          12 STORE_DEREF              1 (item)
+                     514          12 STORE_DEREF              1 (item)
                                   14 LOAD_GLOBAL              1 (NULL + any)
                                   26 LOAD_CLOSURE             1 (item)
                                   28 BUILD_TUPLE              1
-                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 498>)
+                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 514>)
                                   32 MAKE_FUNCTION            8 (closure)
                      
-                     499          34 LOAD_DEREF               2 (ls)
+                     515          34 LOAD_DEREF               2 (ls)
                      
-                     498          36 GET_ITER
+                     514          36 GET_ITER
                                   38 PRECALL                  0
                                   42 CALL                     0
                                   52 PRECALL                  1
                                   56 CALL                     1
                      
-                     497          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
+                     513          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
                      
-                     498          68 LOAD_DEREF               1 (item)
+                     514          68 LOAD_DEREF               1 (item)
                      
-                     497          70 LIST_APPEND              2
+                     513          70 LIST_APPEND              2
                                   72 JUMP_BACKWARD           32 (to 10)
                              >>   74 RETURN_VALUE
                      consts
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
@@ -4825,23 +5147,23 @@
                            code
                               0x95014b00010097007c005d2b7d018902a0000000000000000000000000
                               000000000000000000a6000000ab000000000000000000a0010000000000
                               0000000000000000000000000000007c01a6010000ab0100000000000000
                               005600970101008c2c64005300
                                          0 COPY_FREE_VARS           1
                            
-                           498           2 RETURN_GENERATOR
+                           514           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                43 (to 98)
                            
-                           499          12 STORE_FAST               1 (ext)
+                           515          12 STORE_FAST               1 (ext)
                            
-                           498          14 LOAD_DEREF               2 (item)
+                           514          14 LOAD_DEREF               2 (item)
                                         16 LOAD_METHOD              0 (lower)
                                         38 PRECALL                  0
                                         42 CALL                     0
                                         52 LOAD_METHOD              1 (endswith)
                                         74 LOAD_FAST                1 (ext)
                                         76 PRECALL                  1
                                         80 CALL                     1
@@ -4853,176 +5175,444 @@
                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('lower', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                            name       '<genexpr>'
-                           firstlineno 498
+                           firstlineno 514
                            lnotab 0x0c0102ff
                      names      ('any',)
                      varnames   ('.0',)
                      freevars   ('ls',)
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 497
+                     firstlineno 513
                      lnotab 0x0c01160102ff1eff020102ff
                   -4
                   -3
-                  '\x1b[1;34m Please enter desired sql filename: \x1b[0m'
-                  '\x1b[1;37m Please enter desired table name: \x1b[0m'
+                  'Please enter desired sql filename: '
+                  'Please enter desired table name: '
                   ''
                   'sql'
                   '.sql'
                   0
                   20
                   'Reading '
                   '...'
-                  '\x1b[1;32mInitializing conversion sequence\x1b[0m'
-                  '\x1b[1;32m Connected to sqlite3 database::\x1b[0m'
-                  '\x1b[1;33m Creating database table::\x1b[0m'
+                  'Initializing conversion sequence'
+                  ' Connected to sqlite3 database::'
+                  ' Creating database table::'
                   'replace'
                   False
                   ('if_exists', 'index')
-                  'Operation successful\x1b[0m file saved as \x1b[32'
-                  '\x1b[0m'
+                  'Operation successful'
+                  ' file saved as \x1b[32'
                   '\nExiting'
                   1
-               names      ('preprocess', 'lower', 'endswith', 'input', 'any', 'range', 'print', 'pd', 'read_excel', 'sqlite3', 'connect', 'to_sql', 'close', 'KeyboardInterrupt', 'sys', 'exit', 'Exception', 'logger', 'error')
+               names      ('preprocess', 'lower', 'endswith', 'input', 'DBLUE', 'RESET', 'any', 'range', 'print', 'pd', 'read_excel', 'DGREEN', 'sqlite3', 'connect', 'DYELLOW', 'to_sql', 'close', 'KeyboardInterrupt', 'sys', 'exit', 'Exception', 'logger', 'error')
                varnames   ('self', 'xlsx_list', 'xlsx_file', 'sqlfile', 'db_file', 'table_name', 'column', 'i', 'df', 'conn', 'e')
                freevars   ()
                cellvars   ('ls',)
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'convert_xlsx_to_database'
-               firstlineno 494
+               firstlineno 510
                lnotab
-                  0x040128010801080102ff12030a014e0116014e01140102010c0102ff10
-                  020c0102ff100326010a0104012a010a01040122010c02260128011e011e
-                  0228011e021e0104ff12020c010aff10032e0112011e012e0112014aff08
+                  0x040128010801080102ff12030a014e0116014e01140102010c0120ff10
+                  020c0102ff100326010a0104012a010a01040122010c02260128013c013c
+                  0228013c021e0104ff12020c0126ff10032e0112011e012e0112014aff08
                   db
+            'png'
+            code
+               argcount  : 2
+               nlocals   : 12
+               stacksize : 10
+               flags     : 3
+               code
+                  0x870c97006401640267027d027c017c027601720264017d017c00a00000
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  0000007d0367006403a2018a0c880c6601640484087c034400a6000000ab
+                  0000000000000000007d0467007d057c04440090015d127d067c06a00100
+                  00000000000000000000000000000000000000a6000000ab000000000000
+                  000000a00200000000000000000000000000000000000000006405a60100
+                  00ab01000000000000000072ca7407000000000000000000006406a60100
+                  00ab01000000000000000001007409000000000000000000007c06a60100
+                  00ab0100000000000000007d077c06640064078502190000000000000000
+                  007d08740700000000000000000000740a000000000000000000009b0064
+                  08740c000000000000000000009b006409740f000000000000000000007c
+                  07a6010000ab0100000000000000009b007410000000000000000000009b
+                  009d06a6010000ab01000000000000000001007413000000000000000000
+                  007c07a6010000ab01000000000000000044005d5d5c0200007d097d0a74
+                  07000000000000000000007414000000000000000000009b007c099b0074
+                  10000000000000000000009b009d03640aac0ba6020000ab020000000000
+                  00000001007c089b00640c7c09640d7a0000009b00640e7c019b009d057d
+                  0b7c0aa00b00000000000000000000000000000000000000007c0ba60100
+                  00ab01000000000000000001007c05a00c00000000000000000000000000
+                  000000000000007c0ba6010000ab01000000000000000001008c5e740700
+                  000000000000000000741a000000000000000000009b00640f7410000000
+                  000000000000009b009d03a6010000ab010000000000000000010090018c
+                  147c055300
+                             0 MAKE_CELL               12 (ls)
+               
+               559           2 RESUME                   0
+               
+               560           4 LOAD_CONST               1 ('png')
+                             6 LOAD_CONST               2 ('jpg')
+                             8 BUILD_LIST               2
+                            10 STORE_FAST               2 (outf_list)
+               
+               561          12 LOAD_FAST                1 (outf)
+                            14 LOAD_FAST                2 (outf_list)
+                            16 CONTAINS_OP              1
+                            18 POP_JUMP_FORWARD_IF_FALSE     2 (to 24)
+               
+               562          20 LOAD_CONST               1 ('png')
+                            22 STORE_FAST               1 (outf)
+               
+               563     >>   24 LOAD_FAST                0 (self)
+                            26 LOAD_METHOD              0 (preprocess)
+                            48 PRECALL                  0
+                            52 CALL                     0
+                            62 STORE_FAST               3 (path_list)
+               
+               564          64 BUILD_LIST               0
+                            66 LOAD_CONST               3 (('pdf', 'doc', 'docx'))
+                            68 LIST_EXTEND              1
+                            70 STORE_DEREF             12 (ls)
+               
+               565          72 LOAD_CLOSURE            12 (ls)
+                            74 BUILD_TUPLE              1
+                            76 LOAD_CONST               4 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 565>)
+                            78 MAKE_FUNCTION            8 (closure)
+               
+               566          80 LOAD_FAST                3 (path_list)
+               
+               565          82 GET_ITER
+                            84 PRECALL                  0
+                            88 CALL                     0
+                            98 STORE_FAST               4 (file_list)
+               
+               568         100 BUILD_LIST               0
+                           102 STORE_FAST               5 (imgs)
+               
+               569         104 LOAD_FAST                4 (file_list)
+                           106 GET_ITER
+                       >>  108 EXTENDED_ARG             1
+                           110 FOR_ITER               274 (to 660)
+                           112 STORE_FAST               6 (file)
+               
+               570         114 LOAD_FAST                6 (file)
+                           116 LOAD_METHOD              1 (lower)
+                           138 PRECALL                  0
+                           142 CALL                     0
+                           152 LOAD_METHOD              2 (endswith)
+                           174 LOAD_CONST               5 ('pdf')
+                           176 PRECALL                  1
+                           180 CALL                     1
+                           190 POP_JUMP_FORWARD_IF_FALSE   202 (to 596)
+               
+               572         192 LOAD_GLOBAL              7 (NULL + print)
+                           204 LOAD_CONST               6 ('Generate image objects ..')
+                           206 PRECALL                  1
+                           210 CALL                     1
+                           220 POP_TOP
+               
+               573         222 LOAD_GLOBAL              9 (NULL + convert_from_path)
+                           234 LOAD_FAST                6 (file)
+                           236 PRECALL                  1
+                           240 CALL                     1
+                           250 STORE_FAST               7 (images)
+               
+               576         252 LOAD_FAST                6 (file)
+                           254 LOAD_CONST               0 (None)
+                           256 LOAD_CONST               7 (-4)
+                           258 BUILD_SLICE              2
+                           260 BINARY_SUBSCR
+                           270 STORE_FAST               8 (fname)
+               
+               577         272 LOAD_GLOBAL              7 (NULL + print)
+                           284 LOAD_GLOBAL             10 (YELLOW)
+                           296 FORMAT_VALUE             0
+                           298 LOAD_CONST               8 ('Target images')
+                           300 LOAD_GLOBAL             12 (BLUE)
+                           312 FORMAT_VALUE             0
+                           314 LOAD_CONST               9 (' ')
+                           316 LOAD_GLOBAL             15 (NULL + len)
+                           328 LOAD_FAST                7 (images)
+                           330 PRECALL                  1
+                           334 CALL                     1
+                           344 FORMAT_VALUE             0
+                           346 LOAD_GLOBAL             16 (RESET)
+                           358 FORMAT_VALUE             0
+                           360 BUILD_STRING             6
+                           362 PRECALL                  1
+                           366 CALL                     1
+                           376 POP_TOP
+               
+               578         378 LOAD_GLOBAL             19 (NULL + enumerate)
+                           390 LOAD_FAST                7 (images)
+                           392 PRECALL                  1
+                           396 CALL                     1
+                           406 GET_ITER
+                       >>  408 FOR_ITER                93 (to 596)
+                           410 UNPACK_SEQUENCE          2
+                           414 STORE_FAST               9 (i)
+                           416 STORE_FAST              10 (image)
+               
+               579         418 LOAD_GLOBAL              7 (NULL + print)
+                           430 LOAD_GLOBAL             20 (DBLUE)
+                           442 FORMAT_VALUE             0
+                           444 LOAD_FAST                9 (i)
+                           446 FORMAT_VALUE             0
+                           448 LOAD_GLOBAL             16 (RESET)
+                           460 FORMAT_VALUE             0
+                           462 BUILD_STRING             3
+                           464 LOAD_CONST              10 ('\r')
+                           466 KW_NAMES                11
+                           468 PRECALL                  2
+                           472 CALL                     2
+                           482 POP_TOP
+               
+               580         484 LOAD_FAST                8 (fname)
+                           486 FORMAT_VALUE             0
+                           488 LOAD_CONST              12 ('_')
+                           490 LOAD_FAST                9 (i)
+                           492 LOAD_CONST              13 (1)
+                           494 BINARY_OP                0 (+)
+                           498 FORMAT_VALUE             0
+                           500 LOAD_CONST              14 ('.')
+                           502 LOAD_FAST                1 (outf)
+                           504 FORMAT_VALUE             0
+                           506 BUILD_STRING             5
+                           508 STORE_FAST              11 (yd)
+               
+               581         510 LOAD_FAST               10 (image)
+                           512 LOAD_METHOD             11 (save)
+                           534 LOAD_FAST               11 (yd)
+                           536 PRECALL                  1
+                           540 CALL                     1
+                           550 POP_TOP
+               
+               582         552 LOAD_FAST                5 (imgs)
+                           554 LOAD_METHOD             12 (append)
+                           576 LOAD_FAST               11 (yd)
+                           578 PRECALL                  1
+                           582 CALL                     1
+                           592 POP_TOP
+                           594 JUMP_BACKWARD           94 (to 408)
+               
+               583     >>  596 LOAD_GLOBAL              7 (NULL + print)
+                           608 LOAD_GLOBAL             26 (GREEN)
+                           620 FORMAT_VALUE             0
+                           622 LOAD_CONST              15 ('Ok')
+                           624 LOAD_GLOBAL             16 (RESET)
+                           636 FORMAT_VALUE             0
+                           638 BUILD_STRING             3
+                           640 PRECALL                  1
+                           644 CALL                     1
+                           654 POP_TOP
+                           656 EXTENDED_ARG             1
+                           658 JUMP_BACKWARD          276 (to 108)
+               
+               585     >>  660 LOAD_FAST                5 (imgs)
+                           662 RETURN_VALUE
+               consts
+                  None
+                  'png'
+                  'jpg'
+                  ('pdf', 'doc', 'docx')
+                  code
+                     argcount  : 1
+                     nlocals   : 1
+                     stacksize : 6
+                     flags     : 19
+                     code
+                        0x95018701970067007c005d1f8a01740100000000000000000000880166
+                        016400840889024400a6000000ab000000000000000000a6010000ab0100
+                        00000000000000af1d890191028c205300
+                                   0 COPY_FREE_VARS           1
+                                   2 MAKE_CELL                1 (item)
+                     
+                     565           4 RESUME                   0
+                                   6 BUILD_LIST               0
+                                   8 LOAD_FAST                0 (.0)
+                             >>   10 FOR_ITER                31 (to 74)
+                     
+                     566          12 STORE_DEREF              1 (item)
+                                  14 LOAD_GLOBAL              1 (NULL + any)
+                                  26 LOAD_CLOSURE             1 (item)
+                                  28 BUILD_TUPLE              1
+                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 566>)
+                                  32 MAKE_FUNCTION            8 (closure)
+                     
+                     567          34 LOAD_DEREF               2 (ls)
+                     
+                     566          36 GET_ITER
+                                  38 PRECALL                  0
+                                  42 CALL                     0
+                                  52 PRECALL                  1
+                                  56 CALL                     1
+                     
+                     565          66 POP_JUMP_BACKWARD_IF_FALSE    29 (to 10)
+                     
+                     566          68 LOAD_DEREF               1 (item)
+                     
+                     565          70 LIST_APPEND              2
+                                  72 JUMP_BACKWARD           32 (to 10)
+                             >>   74 RETURN_VALUE
+                     consts
+                        code
+                           argcount  : 1
+                           nlocals   : 2
+                           stacksize : 4
+                           flags     : 51
+                           code
+                              0x95014b00010097007c005d2b7d018902a0000000000000000000000000
+                              000000000000000000a6000000ab000000000000000000a0010000000000
+                              0000000000000000000000000000007c01a6010000ab0100000000000000
+                              005600970101008c2c64005300
+                                         0 COPY_FREE_VARS           1
+                           
+                           566           2 RETURN_GENERATOR
+                                         4 POP_TOP
+                                         6 RESUME                   0
+                                         8 LOAD_FAST                0 (.0)
+                                   >>   10 FOR_ITER                43 (to 98)
+                           
+                           567          12 STORE_FAST               1 (ext)
+                           
+                           566          14 LOAD_DEREF               2 (item)
+                                        16 LOAD_METHOD              0 (lower)
+                                        38 PRECALL                  0
+                                        42 CALL                     0
+                                        52 LOAD_METHOD              1 (endswith)
+                                        74 LOAD_FAST                1 (ext)
+                                        76 PRECALL                  1
+                                        80 CALL                     1
+                                        90 YIELD_VALUE
+                                        92 RESUME                   1
+                                        94 POP_TOP
+                                        96 JUMP_BACKWARD           44 (to 10)
+                                   >>   98 LOAD_CONST               0 (None)
+                                       100 RETURN_VALUE
+                           consts
+                              None
+                           names      ('lower', 'endswith')
+                           varnames   ('.0', 'ext')
+                           freevars   ('item',)
+                           cellvars   ()
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+                           name       '<genexpr>'
+                           firstlineno 566
+                           lnotab 0x0c0102ff
+                     names      ('any',)
+                     varnames   ('.0',)
+                     freevars   ('ls',)
+                     cellvars   ('item',)
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+                     name       '<listcomp>'
+                     firstlineno 565
+                     lnotab 0x0c01160102ff1eff020102ff
+                  'pdf'
+                  'Generate image objects ..'
+                  -4
+                  'Target images'
+                  ' '
+                  '\r'
+                  ('end',)
+                  '_'
+                  1
+                  '.'
+                  'Ok'
+               names      ('preprocess', 'lower', 'endswith', 'print', 'convert_from_path', 'YELLOW', 'BLUE', 'len', 'RESET', 'enumerate', 'DBLUE', 'save', 'append', 'GREEN')
+               varnames   ('self', 'outf', 'outf_list', 'path_list', 'file_list', 'imgs', 'file', 'images', 'fname', 'i', 'image', 'yd')
+               freevars   ()
+               cellvars   ('ls',)
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+               name       'doc2image'
+               firstlineno 559
+               lnotab
+                  0x040108010801040128010801080102ff120304010a014e021e011e0314
+                  016a01280142011a012a012c014002
             None
-         names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'preprocess', 'word_to_pdf', 'pdf_to_word', 'txt_to_pdf', 'word_to_pptx', 'word_to_txt', 'pdf_to_txt', 'ppt_to_word', 'text_to_word', 'convert_xls_to_word', 'convert_xls_to_text', 'convert_xlsx_to_csv', 'convert_xlsx_to_database')
+            ('png',)
+         names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'preprocess', 'word_to_pdf', 'pdf_to_word', 'txt_to_pdf', 'word_to_pptx', 'word_to_txt', 'pdf_to_txt', 'ppt_to_word', 'text_to_word', 'convert_xls_to_word', 'convert_xls_to_text', 'convert_xlsx_to_csv', 'convert_xlsx_to_database', 'doc2image')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+         filename   '/media/skye/skye/FileMAC/filemac/converter.py'
          name       'MakeConversion'
-         firstlineno 49
+         firstlineno 51
          lnotab
-            0x0a0204020603020906160623061906170636061d061b06370626062b02
-            03062702030621
+            0x0a020402060302090616062b0619061706360623061b06370626062b02
+            030627020306210631
       'MakeConversion'
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 11
+         stacksize : 1
          flags     : 0
          code
-            0x970065005a0164005a02640184005a03640284005a0464146404650565
-            061900000000000000000064056507640665086606640784055a09641564
-            0a650a640b650a640c650a640d65076406640e660a640f84055a0b641084
-            005a0c641184005a0d641284005a0e0900641384005a0f640e5300
-         541           0 RESUME                   0
+            0x970065005a0164005a02640184005a03640284005a04640384005a0564
+            0484005a06640584005a0764065300
+         588           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('FileSynthesis')
+                       6 LOAD_CONST               0 ('Scanner')
                        8 STORE_NAME               2 (__qualname__)
          
-         543          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 543>)
+         590          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/skye/FileMAC/filemac/converter.py", line 590>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-         547          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 547>)
+         593          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/skye/FileMAC/filemac/converter.py", line 593>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (preprocess)
          
-         560          22 LOAD_CONST              20 ((16000,))
-                      24 LOAD_CONST               4 ('segments')
-                      26 LOAD_NAME                5 (Iterable)
-                      28 LOAD_NAME                6 (bytes)
-                      30 BINARY_SUBSCR
-                      40 LOAD_CONST               5 ('sample_rate')
-                      42 LOAD_NAME                7 (int)
-                      44 LOAD_CONST               6 ('return')
-                      46 LOAD_NAME                8 (AudioSegment)
-                      48 BUILD_TUPLE              6
-                      50 LOAD_CONST               7 (<code object join_audios, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 560>)
-                      52 MAKE_FUNCTION            5 (defaults, annotations)
-                      54 STORE_NAME               9 (join_audios)
-         
-         566          56 LOAD_CONST              21 (('tempfile', 3))
-                      58 LOAD_CONST              10 ('text')
-                      60 LOAD_NAME               10 (str)
-                      62 LOAD_CONST              11 ('output_file')
-                      64 LOAD_NAME               10 (str)
-                      66 LOAD_CONST              12 ('ogg_folder')
-                      68 LOAD_NAME               10 (str)
-                      70 LOAD_CONST              13 ('retries')
-                      72 LOAD_NAME                7 (int)
-                      74 LOAD_CONST               6 ('return')
-                      76 LOAD_CONST              14 (None)
-                      78 BUILD_TUPLE             10
-                      80 LOAD_CONST              15 (<code object Synthesise, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 566>)
-                      82 MAKE_FUNCTION            5 (defaults, annotations)
-                      84 STORE_NAME              11 (Synthesise)
-         
-         638          86 LOAD_CONST              16 (<code object pdf_to_text, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 638>)
-                      88 MAKE_FUNCTION            0
-                      90 STORE_NAME              12 (pdf_to_text)
-         
-         653          92 LOAD_CONST              17 (<code object text_file, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 653>)
-                      94 MAKE_FUNCTION            0
-                      96 STORE_NAME              13 (text_file)
-         
-         658          98 LOAD_CONST              18 (<code object docx_to_text, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 658>)
-                     100 MAKE_FUNCTION            0
-                     102 STORE_NAME              14 (docx_to_text)
+         606          22 LOAD_CONST               3 (<code object scanPDF, file "/media/skye/skye/FileMAC/filemac/converter.py", line 606>)
+                      24 MAKE_FUNCTION            0
+                      26 STORE_NAME               5 (scanPDF)
          
-         668         104 NOP
+         634          28 LOAD_CONST               4 (<code object scanAsImgs, file "/media/skye/skye/FileMAC/filemac/converter.py", line 634>)
+                      30 MAKE_FUNCTION            0
+                      32 STORE_NAME               6 (scanAsImgs)
          
-         670         106 LOAD_CONST              19 (<code object audiofy, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 670>)
-                     108 MAKE_FUNCTION            0
-                     110 STORE_NAME              15 (audiofy)
-                     112 LOAD_CONST              14 (None)
-                     114 RETURN_VALUE
+         650          34 LOAD_CONST               5 (<code object scanAsLongImg, file "/media/skye/skye/FileMAC/filemac/converter.py", line 650>)
+                      36 MAKE_FUNCTION            0
+                      38 STORE_NAME               7 (scanAsLongImg)
+                      40 LOAD_CONST               6 (None)
+                      42 RETURN_VALUE
          consts
-            'FileSynthesis'
+            'Scanner'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
-               code
-                  0x97007c017c005f00000000000000000064017c005f0100000000000000
-                  0064005300
-               543           0 RESUME                   0
+               code 0x97007c017c005f00000000000000000064005300
+               590           0 RESUME                   0
                
-               544           2 LOAD_FAST                1 (input_file)
+               591           2 LOAD_FAST                1 (input_file)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (input_file)
-               
-               545          16 LOAD_CONST               1 (20000)
-                            18 LOAD_FAST                0 (self)
-                            20 STORE_ATTR               1 (CHUNK_SIZE)
-                            30 LOAD_CONST               0 (None)
-                            32 RETURN_VALUE
+                            16 LOAD_CONST               0 (None)
+                            18 RETURN_VALUE
                consts
                   None
-                  20000
-               names      ('input_file', 'CHUNK_SIZE')
+               names      ('input_file',)
                varnames   ('self', 'input_file')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       '__init__'
-               firstlineno 543
-               lnotab 0x02010e01
+               firstlineno 590
+               lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x970067007d017400000000000000000000006a010000000000000000a0
@@ -5036,1928 +5626,2541 @@
                   010000ab01000000000000000044005d5b7d027400000000000000000000
                   006a010000000000000000a0070000000000000000000000000000000000
                   0000007c006a0300000000000000007c02a6020000ab0200000000000000
                   007d037400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c03a6010000ab010000000000
                   00000072157c01a00400000000000000000000000000000000000000007c
                   03a6010000ab01000000000000000001008c5c7c015300
-               547           0 RESUME                   0
+               593           0 RESUME                   0
                
-               548           2 BUILD_LIST               0
+               594           2 BUILD_LIST               0
                              4 STORE_FAST               1 (files_to_process)
                
-               550           6 LOAD_GLOBAL              0 (os)
+               596           6 LOAD_GLOBAL              0 (os)
                             18 LOAD_ATTR                1 (path)
                             28 LOAD_METHOD              2 (isfile)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                3 (input_file)
                             62 PRECALL                  1
                             66 CALL                     1
                             76 POP_JUMP_FORWARD_IF_FALSE    27 (to 132)
                
-               551          78 LOAD_FAST                1 (files_to_process)
+               597          78 LOAD_FAST                1 (files_to_process)
                             80 LOAD_METHOD              4 (append)
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                3 (input_file)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                            130 JUMP_FORWARD           153 (to 438)
                
-               552     >>  132 LOAD_GLOBAL              0 (os)
+               598     >>  132 LOAD_GLOBAL              0 (os)
                            144 LOAD_ATTR                1 (path)
                            154 LOAD_METHOD              5 (isdir)
                            176 LOAD_FAST                0 (self)
                            178 LOAD_ATTR                3 (input_file)
                            188 PRECALL                  1
                            192 CALL                     1
                            202 POP_JUMP_FORWARD_IF_FALSE   117 (to 438)
                
-               553         204 LOAD_GLOBAL              1 (NULL + os)
+               599         204 LOAD_GLOBAL              1 (NULL + os)
                            216 LOAD_ATTR                6 (listdir)
                            226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                3 (input_file)
                            238 PRECALL                  1
                            242 CALL                     1
                            252 GET_ITER
                        >>  254 FOR_ITER                91 (to 438)
                            256 STORE_FAST               2 (file)
                
-               554         258 LOAD_GLOBAL              0 (os)
+               600         258 LOAD_GLOBAL              0 (os)
                            270 LOAD_ATTR                1 (path)
                            280 LOAD_METHOD              7 (join)
                            302 LOAD_FAST                0 (self)
                            304 LOAD_ATTR                3 (input_file)
                            314 LOAD_FAST                2 (file)
                            316 PRECALL                  2
                            320 CALL                     2
                            330 STORE_FAST               3 (file_path)
                
-               555         332 LOAD_GLOBAL              0 (os)
+               601         332 LOAD_GLOBAL              0 (os)
                            344 LOAD_ATTR                1 (path)
                            354 LOAD_METHOD              2 (isfile)
                            376 LOAD_FAST                3 (file_path)
                            378 PRECALL                  1
                            382 CALL                     1
                            392 POP_JUMP_FORWARD_IF_FALSE    21 (to 436)
                
-               556         394 LOAD_FAST                1 (files_to_process)
+               602         394 LOAD_FAST                1 (files_to_process)
                            396 LOAD_METHOD              4 (append)
                            418 LOAD_FAST                3 (file_path)
                            420 PRECALL                  1
                            424 CALL                     1
                            434 POP_TOP
                        >>  436 JUMP_BACKWARD           92 (to 254)
                
-               558     >>  438 LOAD_FAST                1 (files_to_process)
+               604     >>  438 LOAD_FAST                1 (files_to_process)
                            440 RETURN_VALUE
                consts
                   None
                names      ('os', 'path', 'isfile', 'input_file', 'append', 'isdir', 'listdir', 'join')
                varnames   ('self', 'files_to_process', 'file', 'file_path')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'preprocess'
-               firstlineno 547
+               firstlineno 593
                lnotab 0x0201040248013601480136014a013e012c02
-            16000
-            'segments'
-            'sample_rate'
-            'return'
             code
-               argcount  : 2
-               nlocals   : 3
-               stacksize : 3
+               argcount  : 1
+               nlocals   : 10
+               stacksize : 11
                flags     : 3
                code
-                  0x8701970088016601640184087c004400a6000000ab0000000000000000
-                  007d027401000000000000000000006a0100000000000000007c028e0053
-                  00
-                             0 MAKE_CELL                1 (sample_rate)
+                  0x97007c00a0000000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007d01640184007c014400a6000000ab00000000
+                  00000000007d017c01440090015da77d027c026400640285021900000000
+                  000000000064037a0000007d037403000000000000000000007404000000
+                  000000000000009b0064047406000000000000000000009b009d03a60100
+                  00ab01000000000000000001007409000000000000000000007c026405a6
+                  020000ab02000000000000000035007d04740b000000000000000000006a
+                  0600000000000000007c04a6010000ab0100000000000000007d0564067d
+                  0664077d07740f000000000000000000007411000000000000000000007c
+                  056a090000000000000000a6010000ab010000000000000000a6010000ab
+                  01000000000000000044005d817d087c0764087a0d00007d077403000000
+                  000000000000007414000000000000000000009b00640974060000000000
+                  00000000009b009d036406ac0aa6020000ab020000000000000000010074
+                  03000000000000000000007416000000000000000000009b007c079b0064
+                  0b7411000000000000000000007c056a090000000000000000a6010000ab
+                  0100000000000000009b007406000000000000000000009b009d05640cac
+                  0aa6020000ab02000000000000000001007c056a0900000000000000007c
+                  08190000000000000000007d097c067c09a00c0000000000000000000000
+                  000000000000000000a6000000ab0000000000000000007a0d00007d068c
+                  820900640064006400a6020000ab02000000000000000001006e0b230031
+                  007304770278035900770101005900010001007403000000000000000000
+                  00640d7c069b009d02a6010000ab01000000000000000001007403000000
+                  00000000000000640d7404000000000000000000009b00640e741a000000
+                  000000000000009b007c039b007406000000000000000000009b009d06a6
+                  010000ab01000000000000000001007409000000000000000000007c0364
+                  0fa6020000ab02000000000000000035007d047c04a00e00000000000000
+                  000000000000000000000000007c06a6010000ab01000000000000000001
+                  00640064006400a6020000ab02000000000000000001006e0b2300310073
+                  047702780359007701010059000100010074030000000000000000000074
+                  1e000000000000000000009b0064107406000000000000000000009b009d
+                  03a6010000ab010000000000000000010090018ca964005300
+               606           0 RESUME                   0
+               
+               607           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (preprocess)
+                            26 PRECALL                  0
+                            30 CALL                     0
+                            40 STORE_FAST               1 (pdf_list)
+               
+               608          42 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 608>)
+                            44 MAKE_FUNCTION            0
+                            46 LOAD_FAST                1 (pdf_list)
+                            48 GET_ITER
+                            50 PRECALL                  0
+                            54 CALL                     0
+                            64 STORE_FAST               1 (pdf_list)
+               
+               610          66 LOAD_FAST                1 (pdf_list)
+                            68 GET_ITER
+                       >>   70 EXTENDED_ARG             1
+                            72 FOR_ITER               423 (to 920)
+                            74 STORE_FAST               2 (pdf)
+               
+               611          76 LOAD_FAST                2 (pdf)
+                            78 LOAD_CONST               0 (None)
+                            80 LOAD_CONST               2 (-3)
+                            82 BUILD_SLICE              2
+                            84 BINARY_SUBSCR
+                            94 LOAD_CONST               3 ('txt')
+                            96 BINARY_OP                0 (+)
+                           100 STORE_FAST               3 (out_f)
+               
+               612         102 LOAD_GLOBAL              3 (NULL + print)
+                           114 LOAD_GLOBAL              4 (YELLOW)
+                           126 FORMAT_VALUE             0
+                           128 LOAD_CONST               4 ('Read pdf ..')
+                           130 LOAD_GLOBAL              6 (RESET)
+                           142 FORMAT_VALUE             0
+                           144 BUILD_STRING             3
+                           146 PRECALL                  1
+                           150 CALL                     1
+                           160 POP_TOP
+               
+               614         162 LOAD_GLOBAL              9 (NULL + open)
+                           174 LOAD_FAST                2 (pdf)
+                           176 LOAD_CONST               5 ('rb')
+                           178 PRECALL                  2
+                           182 CALL                     2
+                           192 BEFORE_WITH
+                           194 STORE_FAST               4 (f)
+               
+               615         196 LOAD_GLOBAL             11 (NULL + PyPDF2)
+                           208 LOAD_ATTR                6 (PdfReader)
+                           218 LOAD_FAST                4 (f)
+                           220 PRECALL                  1
+                           224 CALL                     1
+                           234 STORE_FAST               5 (reader)
+               
+               616         236 LOAD_CONST               6 ('')
+                           238 STORE_FAST               6 (text)
+               
+               618         240 LOAD_CONST               7 (0)
+                           242 STORE_FAST               7 (pg)
+               
+               619         244 LOAD_GLOBAL             15 (NULL + range)
+                           256 LOAD_GLOBAL             17 (NULL + len)
+                           268 LOAD_FAST                5 (reader)
+                           270 LOAD_ATTR                9 (pages)
+                           280 PRECALL                  1
+                           284 CALL                     1
+                           294 PRECALL                  1
+                           298 CALL                     1
+                           308 GET_ITER
+                       >>  310 FOR_ITER               129 (to 570)
+                           312 STORE_FAST               8 (page_num)
+               
+               620         314 LOAD_FAST                7 (pg)
+                           316 LOAD_CONST               8 (1)
+                           318 BINARY_OP               13 (+=)
+                           322 STORE_FAST               7 (pg)
+               
+               622         324 LOAD_GLOBAL              3 (NULL + print)
+                           336 LOAD_GLOBAL             20 (DYELLOW)
+                           348 FORMAT_VALUE             0
+                           350 LOAD_CONST               9 ('Progress:')
+                           352 LOAD_GLOBAL              6 (RESET)
+                           364 FORMAT_VALUE             0
+                           366 BUILD_STRING             3
+                           368 LOAD_CONST               6 ('')
+                           370 KW_NAMES                10
+                           372 PRECALL                  2
+                           376 CALL                     2
+                           386 POP_TOP
+               
+               623         388 LOAD_GLOBAL              3 (NULL + print)
+                           400 LOAD_GLOBAL             22 (CYAN)
+                           412 FORMAT_VALUE             0
+                           414 LOAD_FAST                7 (pg)
+                           416 FORMAT_VALUE             0
+                           418 LOAD_CONST              11 ('/')
+                           420 LOAD_GLOBAL             17 (NULL + len)
+                           432 LOAD_FAST                5 (reader)
+                           434 LOAD_ATTR                9 (pages)
+                           444 PRECALL                  1
+                           448 CALL                     1
+                           458 FORMAT_VALUE             0
+                           460 LOAD_GLOBAL              6 (RESET)
+                           472 FORMAT_VALUE             0
+                           474 BUILD_STRING             5
+                           476 LOAD_CONST              12 ('\r')
+                           478 KW_NAMES                10
+                           480 PRECALL                  2
+                           484 CALL                     2
+                           494 POP_TOP
+               
+               624         496 LOAD_FAST                5 (reader)
+                           498 LOAD_ATTR                9 (pages)
+                           508 LOAD_FAST                8 (page_num)
+                           510 BINARY_SUBSCR
+                           520 STORE_FAST               9 (page)
+               
+               625         522 LOAD_FAST                6 (text)
+                           524 LOAD_FAST                9 (page)
+                           526 LOAD_METHOD             12 (extract_text)
+                           548 PRECALL                  0
+                           552 CALL                     0
+                           562 BINARY_OP               13 (+=)
+                           566 STORE_FAST               6 (text)
+                           568 JUMP_BACKWARD          130 (to 310)
+               
+               619     >>  570 NOP
+               
+               614         572 LOAD_CONST               0 (None)
+                           574 LOAD_CONST               0 (None)
+                           576 LOAD_CONST               0 (None)
+                           578 PRECALL                  2
+                           582 CALL                     2
+                           592 POP_TOP
+                           594 JUMP_FORWARD            11 (to 618)
+                       >>  596 PUSH_EXC_INFO
+                           598 WITH_EXCEPT_START
+                           600 POP_JUMP_FORWARD_IF_TRUE     4 (to 610)
+                           602 RERAISE                  2
+                       >>  604 COPY                     3
+                           606 POP_EXCEPT
+                           608 RERAISE                  1
+                       >>  610 POP_TOP
+                           612 POP_EXCEPT
+                           614 POP_TOP
+                           616 POP_TOP
+               
+               627     >>  618 LOAD_GLOBAL              3 (NULL + print)
+                           630 LOAD_CONST              13 ('\n')
+                           632 LOAD_FAST                6 (text)
+                           634 FORMAT_VALUE             0
+                           636 BUILD_STRING             2
+                           638 PRECALL                  1
+                           642 CALL                     1
+                           652 POP_TOP
+               
+               628         654 LOAD_GLOBAL              3 (NULL + print)
+                           666 LOAD_CONST              13 ('\n')
+                           668 LOAD_GLOBAL              4 (YELLOW)
+                           680 FORMAT_VALUE             0
+                           682 LOAD_CONST              14 ('Write text to ')
+                           684 LOAD_GLOBAL             26 (GREEN)
+                           696 FORMAT_VALUE             0
+                           698 LOAD_FAST                3 (out_f)
+                           700 FORMAT_VALUE             0
+                           702 LOAD_GLOBAL              6 (RESET)
+                           714 FORMAT_VALUE             0
+                           716 BUILD_STRING             6
+                           718 PRECALL                  1
+                           722 CALL                     1
+                           732 POP_TOP
+               
+               629         734 LOAD_GLOBAL              9 (NULL + open)
+                           746 LOAD_FAST                3 (out_f)
+                           748 LOAD_CONST              15 ('w')
+                           750 PRECALL                  2
+                           754 CALL                     2
+                           764 BEFORE_WITH
+                           766 STORE_FAST               4 (f)
                
-               560           2 RESUME                   0
+               630         768 LOAD_FAST                4 (f)
+                           770 LOAD_METHOD             14 (write)
+                           792 LOAD_FAST                6 (text)
+                           794 PRECALL                  1
+                           798 CALL                     1
+                           808 POP_TOP
+               
+               629         810 LOAD_CONST               0 (None)
+                           812 LOAD_CONST               0 (None)
+                           814 LOAD_CONST               0 (None)
+                           816 PRECALL                  2
+                           820 CALL                     2
+                           830 POP_TOP
+                           832 JUMP_FORWARD            11 (to 856)
+                       >>  834 PUSH_EXC_INFO
+                           836 WITH_EXCEPT_START
+                           838 POP_JUMP_FORWARD_IF_TRUE     4 (to 848)
+                           840 RERAISE                  2
+                       >>  842 COPY                     3
+                           844 POP_EXCEPT
+                           846 RERAISE                  1
+                       >>  848 POP_TOP
+                           850 POP_EXCEPT
+                           852 POP_TOP
+                           854 POP_TOP
                
-               562           4 LOAD_CLOSURE             1 (sample_rate)
-                             6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 562>)
-                            10 MAKE_FUNCTION            8 (closure)
-               
-               563          12 LOAD_FAST                0 (segments)
-               
-               562          14 GET_ITER
-                            16 PRECALL                  0
-                            20 CALL                     0
-                            30 STORE_FAST               2 (chunks)
-               
-               564          32 LOAD_GLOBAL              1 (NULL + pydub)
-                            44 LOAD_ATTR                1 (concat)
-                            54 LOAD_FAST                2 (chunks)
-                            56 CALL_FUNCTION_EX         0
-                            58 RETURN_VALUE
+               632     >>  856 LOAD_GLOBAL              3 (NULL + print)
+                           868 LOAD_GLOBAL             30 (DGREEN)
+                           880 FORMAT_VALUE             0
+                           882 LOAD_CONST              16 ('Ok')
+                           884 LOAD_GLOBAL              6 (RESET)
+                           896 FORMAT_VALUE             0
+                           898 BUILD_STRING             3
+                           900 PRECALL                  1
+                           904 CALL                     1
+                           914 POP_TOP
+                           916 EXTENDED_ARG             1
+                           918 JUMP_BACKWARD          425 (to 70)
+               
+               610     >>  920 LOAD_CONST               0 (None)
+                           922 RETURN_VALUE
+               ExceptionTable:
+                 194 to 568 -> 596 [2] lasti
+                 596 to 602 -> 604 [4] lasti
+                 610 to 610 -> 604 [4] lasti
+                 766 to 808 -> 834 [2] lasti
+                 834 to 840 -> 842 [4] lasti
+                 848 to 848 -> 842 [4] lasti
                consts
-                  'Join multiple audio segments together'
+                  None
                   code
                      argcount  : 1
                      nlocals   : 2
-                     stacksize : 6
+                     stacksize : 5
                      flags     : 19
                      code
-                        0x9501970067007c005d187d017401000000000000000000006a01000000
-                        00000000007c018902ac00a6020000ab02000000000000000091028c1953
-                        00
-                                   0 COPY_FREE_VARS           1
-                     
-                     562           2 RESUME                   0
-                                   4 BUILD_LIST               0
-                                   6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                24 (to 58)
-                     
-                     563          10 STORE_FAST               1 (segment)
-                     
-                     562          12 LOAD_GLOBAL              1 (NULL + AudioSegment)
-                                  24 LOAD_ATTR                1 (from_buffer)
-                                  34 LOAD_FAST                1 (segment)
-                                  36 LOAD_DEREF               2 (sample_rate)
-                                  38 KW_NAMES                 0
-                                  40 PRECALL                  2
-                                  44 CALL                     2
-                                  54 LIST_APPEND              2
-                                  56 JUMP_BACKWARD           25 (to 8)
-                             >>   58 RETURN_VALUE
+                        0x970067007c005d2b7d017c01a000000000000000000000000000000000
+                        0000000000a6000000ab000000000000000000a001000000000000000000
+                        00000000000000000000006400a6010000ab010000000000000000af297c
+                        0191028c2c5300
+                     608           0 RESUME                   0
+                                   2 BUILD_LIST               0
+                                   4 LOAD_FAST                0 (.0)
+                             >>    6 FOR_ITER                43 (to 94)
+                                   8 STORE_FAST               1 (item)
+                                  10 LOAD_FAST                1 (item)
+                                  12 LOAD_METHOD              0 (lower)
+                                  34 PRECALL                  0
+                                  38 CALL                     0
+                                  48 LOAD_METHOD              1 (endswith)
+                                  70 LOAD_CONST               0 ('pdf')
+                                  72 PRECALL                  1
+                                  76 CALL                     1
+                                  86 POP_JUMP_BACKWARD_IF_FALSE    41 (to 6)
+                                  88 LOAD_FAST                1 (item)
+                                  90 LIST_APPEND              2
+                                  92 JUMP_BACKWARD           44 (to 6)
+                             >>   94 RETURN_VALUE
                      consts
-                        ('frame_rate',)
-                     names      ('AudioSegment', 'from_buffer')
-                     varnames   ('.0', 'segment')
-                     freevars   ('sample_rate',)
+                        'pdf'
+                     names      ('lower', 'endswith')
+                     varnames   ('.0', 'item')
+                     freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 562
-                     lnotab 0x0a0102ff
-               names      ('pydub', 'concat')
-               varnames   ('segments', 'sample_rate', 'chunks')
+                     firstlineno 608
+                     lnotab 0x
+                  -3
+                  'txt'
+                  'Read pdf ..'
+                  'rb'
+                  ''
+                  0
+                  1
+                  'Progress:'
+                  ('end',)
+                  '/'
+                  '\r'
+                  '\n'
+                  'Write text to '
+                  'w'
+                  'Ok'
+               names      ('preprocess', 'print', 'YELLOW', 'RESET', 'open', 'PyPDF2', 'PdfReader', 'range', 'len', 'pages', 'DYELLOW', 'CYAN', 'extract_text', 'GREEN', 'write', 'DGREEN')
+               varnames   ('self', 'pdf_list', 'pdf', 'out_f', 'f', 'reader', 'text', 'pg', 'page_num', 'page')
                freevars   ()
-               cellvars   ('sample_rate',)
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               cellvars   ()
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+               name       'scanPDF'
+               firstlineno 606
+               lnotab
+                  0x0201280118020a011a013c02220128010402040146010a0240016c011a
+                  0130fa02fb2e0d2401500122012aff2e0340ea
+            code
+               argcount  : 1
+               nlocals   : 9
+               stacksize : 5
+               flags     : 3
+               code
+                  0x97007c006a0000000000000000007d017403000000000000000000007c
+                  01a6010000ab0100000000000000007d027c02a002000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000007d03640164
+                  026c036d047d04010064037d057c0344005d287d0602007c047c06a60100
+                  00ab0100000000000000007d077c07a00500000000000000000000000000
+                  00000000000000a6000000ab0000000000000000007d087c0881057c057c
+                  087a0d00007d058c29740d000000000000000000007c05a6010000ab0100
+                  000000000000000100740d00000000000000000000740e00000000000000
+                  0000009b0064047410000000000000000000009b009d03a6010000ab0100
+                  0000000000000001007c055300
+               634           0 RESUME                   0
+               
+               635           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (input_file)
+                            14 STORE_FAST               1 (file)
+               
+               636          16 LOAD_GLOBAL              3 (NULL + MakeConversion)
+                            28 LOAD_FAST                1 (file)
+                            30 PRECALL                  1
+                            34 CALL                     1
+                            44 STORE_FAST               2 (mc)
+               
+               637          46 LOAD_FAST                2 (mc)
+                            48 LOAD_METHOD              2 (doc2image)
+                            70 PRECALL                  0
+                            74 CALL                     0
+                            84 STORE_FAST               3 (img_objs)
+               
+               639          86 LOAD_CONST               1 (1)
+                            88 LOAD_CONST               2 (('ExtractText',))
+                            90 IMPORT_NAME              3 (OCRTextExtractor)
+                            92 IMPORT_FROM              4 (ExtractText)
+                            94 STORE_FAST               4 (ExtractText)
+                            96 POP_TOP
+               
+               640          98 LOAD_CONST               3 ('')
+                           100 STORE_FAST               5 (text)
+               
+               641         102 LOAD_FAST                3 (img_objs)
+                           104 GET_ITER
+                       >>  106 FOR_ITER                40 (to 188)
+                           108 STORE_FAST               6 (i)
+               
+               642         110 PUSH_NULL
+                           112 LOAD_FAST                4 (ExtractText)
+                           114 LOAD_FAST                6 (i)
+                           116 PRECALL                  1
+                           120 CALL                     1
+                           130 STORE_FAST               7 (extract)
+               
+               643         132 LOAD_FAST                7 (extract)
+                           134 LOAD_METHOD              5 (OCR)
+                           156 PRECALL                  0
+                           160 CALL                     0
+                           170 STORE_FAST               8 (tx)
+               
+               644         172 LOAD_FAST                8 (tx)
+                           174 POP_JUMP_FORWARD_IF_NONE     5 (to 186)
+               
+               645         176 LOAD_FAST                5 (text)
+                           178 LOAD_FAST                8 (tx)
+                           180 BINARY_OP               13 (+=)
+                           184 STORE_FAST               5 (text)
+                       >>  186 JUMP_BACKWARD           41 (to 106)
+               
+               646     >>  188 LOAD_GLOBAL             13 (NULL + print)
+                           200 LOAD_FAST                5 (text)
+                           202 PRECALL                  1
+                           206 CALL                     1
+                           216 POP_TOP
+               
+               647         218 LOAD_GLOBAL             13 (NULL + print)
+                           230 LOAD_GLOBAL             14 (GREEN)
+                           242 FORMAT_VALUE             0
+                           244 LOAD_CONST               4 ('Ok')
+                           246 LOAD_GLOBAL             16 (RESET)
+                           258 FORMAT_VALUE             0
+                           260 BUILD_STRING             3
+                           262 PRECALL                  1
+                           266 CALL                     1
+                           276 POP_TOP
+               
+               648         278 LOAD_FAST                5 (text)
+                           280 RETURN_VALUE
+               consts
+                  None
+                  1
+                  ('ExtractText',)
+                  ''
+                  'Ok'
+               names      ('input_file', 'MakeConversion', 'doc2image', 'OCRTextExtractor', 'ExtractText', 'OCR', 'print', 'GREEN', 'RESET')
+               varnames   ('self', 'file', 'mc', 'img_objs', 'ExtractText', 'text', 'i', 'extract', 'tx')
+               freevars   ()
+               cellvars   ()
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+               name       'scanAsImgs'
+               firstlineno 634
+               lnotab 0x02010e011e0128020c01040108011601280104010c011e013c01
+            code
+               argcount  : 1
+               nlocals   : 6
+               stacksize : 5
+               flags     : 3
+               code
+                  0x97007c006a0000000000000000007d01640164026c016d027d02010002
+                  007c027c01a6010000ab0100000000000000007d03640164036c036d047d
+                  04010002007c047c03a6010000ab0100000000000000007d05740b000000
+                  000000000000007c05a6010000ab0100000000000000000100740b000000
+                  00000000000000740c000000000000000000009b006404740e0000000000
+                  00000000009b009d03a6010000ab01000000000000000001007c055300
+               650           0 RESUME                   0
+               
+               651           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (input_file)
+                            14 STORE_FAST               1 (file)
+               
+               652          16 LOAD_CONST               1 (1)
+                            18 LOAD_CONST               2 (('pdf_2L_Img',))
+                            20 IMPORT_NAME              1 (longImg)
+                            22 IMPORT_FROM              2 (pdf_2L_Img)
+                            24 STORE_FAST               2 (pdf_2L_Img)
+                            26 POP_TOP
+               
+               653          28 PUSH_NULL
+                            30 LOAD_FAST                2 (pdf_2L_Img)
+                            32 LOAD_FAST                1 (file)
+                            34 PRECALL                  1
+                            38 CALL                     1
+                            48 STORE_FAST               3 (LImg)
+               
+               654          50 LOAD_CONST               1 (1)
+                            52 LOAD_CONST               3 (('ExtractText',))
+                            54 IMPORT_NAME              3 (OCRTextExtractor)
+                            56 IMPORT_FROM              4 (ExtractText)
+                            58 STORE_FAST               4 (ExtractText)
+                            60 POP_TOP
+               
+               655          62 PUSH_NULL
+                            64 LOAD_FAST                4 (ExtractText)
+                            66 LOAD_FAST                3 (LImg)
+                            68 PRECALL                  1
+                            72 CALL                     1
+                            82 STORE_FAST               5 (text)
+               
+               656          84 LOAD_GLOBAL             11 (NULL + print)
+                            96 LOAD_FAST                5 (text)
+                            98 PRECALL                  1
+                           102 CALL                     1
+                           112 POP_TOP
+               
+               657         114 LOAD_GLOBAL             11 (NULL + print)
+                           126 LOAD_GLOBAL             12 (GREEN)
+                           138 FORMAT_VALUE             0
+                           140 LOAD_CONST               4 ('Ok')
+                           142 LOAD_GLOBAL             14 (RESET)
+                           154 FORMAT_VALUE             0
+                           156 BUILD_STRING             3
+                           158 PRECALL                  1
+                           162 CALL                     1
+                           172 POP_TOP
+               
+               658         174 LOAD_FAST                5 (text)
+                           176 RETURN_VALUE
+               consts
+                  None
+                  1
+                  ('pdf_2L_Img',)
+                  ('ExtractText',)
+                  'Ok'
+               names      ('input_file', 'longImg', 'pdf_2L_Img', 'OCRTextExtractor', 'ExtractText', 'print', 'GREEN', 'RESET')
+               varnames   ('self', 'file', 'pdf_2L_Img', 'LImg', 'ExtractText', 'text')
+               freevars   ()
+               cellvars   ()
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+               name       'scanAsLongImg'
+               firstlineno 650
+               lnotab 0x02010e010c0116010c0116011e013c01
+            None
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'preprocess', 'scanPDF', 'scanAsImgs', 'scanAsLongImg')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+         name       'Scanner'
+         firstlineno 588
+         lnotab 0x0a020603060d061c0610
+      'Scanner'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 13
+         flags     : 0
+         code
+            0x970065005a0164005a02640184005a03640284005a04650564038400a6
+            000000ab0000000000000000005a06641364076507640865076409650864
+            0a6507640b6508640c640d660c640e84055a096505640f8400a6000000ab
+            0000000000000000005a0a650564108400a6000000ab0000000000000000
+            005a0b650564118400a6000000ab0000000000000000005a0c0900641284
+            005a0d640d5300
+         661           0 RESUME                   0
+                       2 LOAD_NAME                0 (__name__)
+                       4 STORE_NAME               1 (__module__)
+                       6 LOAD_CONST               0 ('FileSynthesis')
+                       8 STORE_NAME               2 (__qualname__)
+         
+         663          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/skye/FileMAC/filemac/converter.py", line 663>)
+                      12 MAKE_FUNCTION            0
+                      14 STORE_NAME               3 (__init__)
+         
+         667          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/skye/FileMAC/filemac/converter.py", line 667>)
+                      18 MAKE_FUNCTION            0
+                      20 STORE_NAME               4 (preprocess)
+         
+         680          22 LOAD_NAME                5 (staticmethod)
+         
+         681          24 LOAD_CONST               3 (<code object join_audios, file "/media/skye/skye/FileMAC/filemac/converter.py", line 680>)
+                      26 MAKE_FUNCTION            0
+         
+         680          28 PRECALL                  0
+                      32 CALL                     0
+         
+         681          42 STORE_NAME               6 (join_audios)
+         
+         704          44 LOAD_CONST              19 ((20000, 'tempfile', 5))
+                      46 LOAD_CONST               7 ('text')
+                      48 LOAD_NAME                7 (str)
+                      50 LOAD_CONST               8 ('output_file')
+                      52 LOAD_NAME                7 (str)
+                      54 LOAD_CONST               9 ('CHUNK_SIZE')
+                      56 LOAD_NAME                8 (int)
+                      58 LOAD_CONST              10 ('ogg_folder')
+                      60 LOAD_NAME                7 (str)
+                      62 LOAD_CONST              11 ('retries')
+                      64 LOAD_NAME                8 (int)
+                      66 LOAD_CONST              12 ('return')
+                      68 LOAD_CONST              13 (None)
+                      70 BUILD_TUPLE             12
+                      72 LOAD_CONST              14 (<code object Synthesise, file "/media/skye/skye/FileMAC/filemac/converter.py", line 704>)
+                      74 MAKE_FUNCTION            5 (defaults, annotations)
+                      76 STORE_NAME               9 (Synthesise)
+         
+         774          78 LOAD_NAME                5 (staticmethod)
+         
+         775          80 LOAD_CONST              15 (<code object pdf_to_text, file "/media/skye/skye/FileMAC/filemac/converter.py", line 774>)
+                      82 MAKE_FUNCTION            0
+         
+         774          84 PRECALL                  0
+                      88 CALL                     0
+         
+         775          98 STORE_NAME              10 (pdf_to_text)
+         
+         792         100 LOAD_NAME                5 (staticmethod)
+         
+         793         102 LOAD_CONST              16 (<code object text_file, file "/media/skye/skye/FileMAC/filemac/converter.py", line 792>)
+                     104 MAKE_FUNCTION            0
+         
+         792         106 PRECALL                  0
+                     110 CALL                     0
+         
+         793         120 STORE_NAME              11 (text_file)
+         
+         805         122 LOAD_NAME                5 (staticmethod)
+         
+         806         124 LOAD_CONST              17 (<code object docx_to_text, file "/media/skye/skye/FileMAC/filemac/converter.py", line 805>)
+                     126 MAKE_FUNCTION            0
+         
+         805         128 PRECALL                  0
+                     132 CALL                     0
+         
+         806         142 STORE_NAME              12 (docx_to_text)
+         
+         819         144 NOP
+         
+         821         146 LOAD_CONST              18 (<code object audiofy, file "/media/skye/skye/FileMAC/filemac/converter.py", line 821>)
+                     148 MAKE_FUNCTION            0
+                     150 STORE_NAME              13 (audiofy)
+                     152 LOAD_CONST              13 (None)
+                     154 RETURN_VALUE
+         consts
+            'FileSynthesis'
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 2
+               flags     : 3
+               code 0x97007c017c005f00000000000000000064005300
+               663           0 RESUME                   0
+               
+               664           2 LOAD_FAST                1 (input_file)
+                             4 LOAD_FAST                0 (self)
+                             6 STORE_ATTR               0 (input_file)
+                            16 LOAD_CONST               0 (None)
+                            18 RETURN_VALUE
+               consts
+                  None
+               names      ('input_file',)
+               varnames   ('self', 'input_file')
+               freevars   ()
+               cellvars   ()
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+               name       '__init__'
+               firstlineno 663
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 4
+               stacksize : 5
+               flags     : 3
+               code
+                  0x970067007d017400000000000000000000006a010000000000000000a0
+                  0200000000000000000000000000000000000000007c006a030000000000
+                  000000a6010000ab010000000000000000721b7c01a00400000000000000
+                  000000000000000000000000007c006a030000000000000000a6010000ab
+                  01000000000000000001006e997400000000000000000000006a01000000
+                  0000000000a00500000000000000000000000000000000000000007c006a
+                  030000000000000000a6010000ab01000000000000000072757401000000
+                  000000000000006a0600000000000000007c006a030000000000000000a6
+                  010000ab01000000000000000044005d5b7d027400000000000000000000
+                  006a010000000000000000a0070000000000000000000000000000000000
+                  0000007c006a0300000000000000007c02a6020000ab0200000000000000
+                  007d037400000000000000000000006a010000000000000000a002000000
+                  00000000000000000000000000000000007c03a6010000ab010000000000
+                  00000072157c01a00400000000000000000000000000000000000000007c
+                  03a6010000ab01000000000000000001008c5c7c015300
+               667           0 RESUME                   0
+               
+               668           2 BUILD_LIST               0
+                             4 STORE_FAST               1 (files_to_process)
+               
+               670           6 LOAD_GLOBAL              0 (os)
+                            18 LOAD_ATTR                1 (path)
+                            28 LOAD_METHOD              2 (isfile)
+                            50 LOAD_FAST                0 (self)
+                            52 LOAD_ATTR                3 (input_file)
+                            62 PRECALL                  1
+                            66 CALL                     1
+                            76 POP_JUMP_FORWARD_IF_FALSE    27 (to 132)
+               
+               671          78 LOAD_FAST                1 (files_to_process)
+                            80 LOAD_METHOD              4 (append)
+                           102 LOAD_FAST                0 (self)
+                           104 LOAD_ATTR                3 (input_file)
+                           114 PRECALL                  1
+                           118 CALL                     1
+                           128 POP_TOP
+                           130 JUMP_FORWARD           153 (to 438)
+               
+               672     >>  132 LOAD_GLOBAL              0 (os)
+                           144 LOAD_ATTR                1 (path)
+                           154 LOAD_METHOD              5 (isdir)
+                           176 LOAD_FAST                0 (self)
+                           178 LOAD_ATTR                3 (input_file)
+                           188 PRECALL                  1
+                           192 CALL                     1
+                           202 POP_JUMP_FORWARD_IF_FALSE   117 (to 438)
+               
+               673         204 LOAD_GLOBAL              1 (NULL + os)
+                           216 LOAD_ATTR                6 (listdir)
+                           226 LOAD_FAST                0 (self)
+                           228 LOAD_ATTR                3 (input_file)
+                           238 PRECALL                  1
+                           242 CALL                     1
+                           252 GET_ITER
+                       >>  254 FOR_ITER                91 (to 438)
+                           256 STORE_FAST               2 (file)
+               
+               674         258 LOAD_GLOBAL              0 (os)
+                           270 LOAD_ATTR                1 (path)
+                           280 LOAD_METHOD              7 (join)
+                           302 LOAD_FAST                0 (self)
+                           304 LOAD_ATTR                3 (input_file)
+                           314 LOAD_FAST                2 (file)
+                           316 PRECALL                  2
+                           320 CALL                     2
+                           330 STORE_FAST               3 (file_path)
+               
+               675         332 LOAD_GLOBAL              0 (os)
+                           344 LOAD_ATTR                1 (path)
+                           354 LOAD_METHOD              2 (isfile)
+                           376 LOAD_FAST                3 (file_path)
+                           378 PRECALL                  1
+                           382 CALL                     1
+                           392 POP_JUMP_FORWARD_IF_FALSE    21 (to 436)
+               
+               676         394 LOAD_FAST                1 (files_to_process)
+                           396 LOAD_METHOD              4 (append)
+                           418 LOAD_FAST                3 (file_path)
+                           420 PRECALL                  1
+                           424 CALL                     1
+                           434 POP_TOP
+                       >>  436 JUMP_BACKWARD           92 (to 254)
+               
+               678     >>  438 LOAD_FAST                1 (files_to_process)
+                           440 RETURN_VALUE
+               consts
+                  None
+               names      ('os', 'path', 'isfile', 'input_file', 'append', 'isdir', 'listdir', 'join')
+               varnames   ('self', 'files_to_process', 'file', 'file_path')
+               freevars   ()
+               cellvars   ()
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
+               name       'preprocess'
+               firstlineno 667
+               lnotab 0x0201040248013601480136014a013e012c02
+            code
+               argcount  : 2
+               nlocals   : 7
+               stacksize : 8
+               flags     : 3
+               code
+                  0x97007c0164017a0000007d027401000000000000000000007402000000
+                  000000000000009b0064027404000000000000000000009b007c029b0074
+                  06000000000000000000009b009d056403ac04a6020000ab020000000000
+                  000000010067007d037401000000000000000000007c00a6010000ab0100
+                  0000000000000001007c0044005d577d0474010000000000000000000064
+                  057402000000000000000000009b007409000000000000000000007c00a6
+                  010000ab0100000000000000009b007406000000000000000000009b0064
+                  069d05a6010000ab01000000000000000001007c03a00500000000000000
+                  00000000000000000000000000740d000000000000000000006a07000000
+                  00000000007c04a6010000ab010000000000000000a6010000ab01000000
+                  000000000001008c587c036407190000000000000000007d057411000000
+                  0000000000000064087409000000000000000000007c00a6010000ab0100
+                  00000000000000a6020000ab02000000000000000044005d0d7d067c057c
+                  037c06190000000000000000007a0d00007d058c0e7c05a0090000000000
+                  0000000000000000000000000000007c0164097a000000640aac0ba60200
+                  00ab02000000000000000001007401000000000000000000007414000000
+                  000000000000009b00640c7406000000000000000000009b009d03a60100
+                  00ab010000000000000000010064005300
+               680           0 RESUME                   0
+               
+               682           2 LOAD_FAST                1 (output_file)
+                             4 LOAD_CONST               1 ('_master.mp3')
+                             6 BINARY_OP                0 (+)
+                            10 STORE_FAST               2 (masterfile)
+               
+               683          12 LOAD_GLOBAL              1 (NULL + print)
+               
+               684          24 LOAD_GLOBAL              2 (DBLUE)
+                            36 FORMAT_VALUE             0
+                            38 LOAD_CONST               2 ('Create a master file ')
+                            40 LOAD_GLOBAL              4 (DMAGENTA)
+                            52 FORMAT_VALUE             0
+                            54 LOAD_FAST                2 (masterfile)
+                            56 FORMAT_VALUE             0
+                            58 LOAD_GLOBAL              6 (RESET)
+                            70 FORMAT_VALUE             0
+                            72 BUILD_STRING             5
+                            74 LOAD_CONST               3 ('\r')
+               
+               683          76 KW_NAMES                 4
+                            78 PRECALL                  2
+                            82 CALL                     2
+                            92 POP_TOP
+               
+               686          94 BUILD_LIST               0
+                            96 STORE_FAST               3 (ogg_files)
+               
+               688          98 LOAD_GLOBAL              1 (NULL + print)
+                           110 LOAD_FAST                0 (files)
+                           112 PRECALL                  1
+                           116 CALL                     1
+                           126 POP_TOP
+               
+               689         128 LOAD_FAST                0 (files)
+                           130 GET_ITER
+                       >>  132 FOR_ITER                87 (to 308)
+                           134 STORE_FAST               4 (filename)
+               
+               690         136 LOAD_GLOBAL              1 (NULL + print)
+                           148 LOAD_CONST               5 ('Join ')
+                           150 LOAD_GLOBAL              2 (DBLUE)
+                           162 FORMAT_VALUE             0
+                           164 LOAD_GLOBAL              9 (NULL + len)
+                           176 LOAD_FAST                0 (files)
+                           178 PRECALL                  1
+                           182 CALL                     1
+                           192 FORMAT_VALUE             0
+                           194 LOAD_GLOBAL              6 (RESET)
+                           206 FORMAT_VALUE             0
+                           208 LOAD_CONST               6 (' files')
+                           210 BUILD_STRING             5
+                           212 PRECALL                  1
+                           216 CALL                     1
+                           226 POP_TOP
+               
+               693         228 LOAD_FAST                3 (ogg_files)
+                           230 LOAD_METHOD              5 (append)
+                           252 LOAD_GLOBAL             13 (NULL + AudioSegment)
+                           264 LOAD_ATTR                7 (from_file)
+                           274 LOAD_FAST                4 (filename)
+                           276 PRECALL                  1
+                           280 CALL                     1
+                           290 PRECALL                  1
+                           294 CALL                     1
+                           304 POP_TOP
+                           306 JUMP_BACKWARD           88 (to 132)
+               
+               696     >>  308 LOAD_FAST                3 (ogg_files)
+                           310 LOAD_CONST               7 (0)
+                           312 BINARY_SUBSCR
+                           322 STORE_FAST               5 (combined_ogg)
+               
+               697         324 LOAD_GLOBAL             17 (NULL + range)
+                           336 LOAD_CONST               8 (1)
+                           338 LOAD_GLOBAL              9 (NULL + len)
+                           350 LOAD_FAST                0 (files)
+                           352 PRECALL                  1
+                           356 CALL                     1
+                           366 PRECALL                  2
+                           370 CALL                     2
+                           380 GET_ITER
+                       >>  382 FOR_ITER                13 (to 410)
+                           384 STORE_FAST               6 (i)
+               
+               698         386 LOAD_FAST                5 (combined_ogg)
+                           388 LOAD_FAST                3 (ogg_files)
+                           390 LOAD_FAST                6 (i)
+                           392 BINARY_SUBSCR
+                           402 BINARY_OP               13 (+=)
+                           406 STORE_FAST               5 (combined_ogg)
+                           408 JUMP_BACKWARD           14 (to 382)
+               
+               701     >>  410 LOAD_FAST                5 (combined_ogg)
+                           412 LOAD_METHOD              9 (export)
+                           434 LOAD_FAST                1 (output_file)
+                           436 LOAD_CONST               9 ('_master.ogg')
+                           438 BINARY_OP                0 (+)
+                           442 LOAD_CONST              10 ('ogg')
+                           444 KW_NAMES                11
+                           446 PRECALL                  2
+                           450 CALL                     2
+                           460 POP_TOP
+               
+               702         462 LOAD_GLOBAL              1 (NULL + print)
+                           474 LOAD_GLOBAL             20 (DGREEN)
+                           486 FORMAT_VALUE             0
+                           488 LOAD_CONST              12 ('Master file:Ok                                                                             ')
+                           490 LOAD_GLOBAL              6 (RESET)
+                           502 FORMAT_VALUE             0
+                           504 BUILD_STRING             3
+                           506 PRECALL                  1
+                           510 CALL                     1
+                           520 POP_TOP
+                           522 LOAD_CONST               0 (None)
+                           524 RETURN_VALUE
+               consts
+                  None
+                  '_master.mp3'
+                  'Create a master file '
+                  '\r'
+                  ('end',)
+                  'Join '
+                  ' files'
+                  0
+                  1
+                  '_master.ogg'
+                  'ogg'
+                  ('format',)
+                  'Master file:Ok                                                                             '
+               names      ('print', 'DBLUE', 'DMAGENTA', 'RESET', 'len', 'append', 'AudioSegment', 'from_file', 'range', 'export', 'DGREEN')
+               varnames   ('files', 'output_file', 'masterfile', 'ogg_files', 'filename', 'combined_ogg', 'i')
+               freevars   ()
+               cellvars   ()
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'join_audios'
-               firstlineno 560
-               lnotab 0x0402080102ff1202
+               firstlineno 680
+               lnotab 0x02020a010c0134ff120304021e0108015c03500310013e0118033401
+            20000
             'tempfile'
-            3
+            5
             'text'
             'output_file'
+            'CHUNK_SIZE'
             'ogg_folder'
             'retries'
+            'return'
             None
             code
-               argcount  : 5
+               argcount  : 6
                nlocals   : 17
-               stacksize : 11
+               stacksize : 12
                flags     : 3
                code
-                  0x970009007400000000000000000000006a010000000000000000a00200
-                  000000000000000000000000000000000000007c03a6010000ab01000000
-                  000000000073147401000000000000000000006a0300000000000000007c
-                  03a6010000ab01000000000000000001007409000000000000000000006a
-                  050000000000000000a6000000ab0000000000000000007d057c05a00600
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  00000001007c05a0070000000000000000000000000000000000000000a6
-                  000000ab0000000000000000007d06741000000000000000000000a00900
-                  0000000000000000000000000000000000000064017c0664027a0b000064
-                  039b0464049d03a6010000ab010000000000000000010074150000000000
-                  00000000007c04a6010000ab010000000000000000440090025df67d0709
-                  00090074150000000000000000000064057417000000000000000000007c
-                  01a6010000ab0100000000000000007c006a0c0000000000000000a60300
-                  00ab03000000000000000044005d7d7d087c017c087c087c006a0c000000
-                  00000000007a0000008502190000000000000000007d0974150000000000
-                  00000000006405741b000000000000000000006a0e000000000000000074
-                  17000000000000000000007c01a6010000ab0100000000000000007c006a
-                  0c00000000000000007a0b0000a6010000ab010000000000000000a60200
-                  00ab02000000000000000044005d0a7d087c029b0064067c089b0064079d
-                  047d0a8c0b741f000000000000000000007c0964086409ac0aa6030000ab
-                  0300000000000000007d0b7c0ba010000000000000000000000000000000
-                  00000000007c0aa6010000ab01000000000000000001008c7e7423000000
-                  000000000000007401000000000000000000006a1200000000000000007c
-                  03a6010000ab010000000000000000a6010000ab0100000000000000007d
-                  0c742700000000000000000000640b84007c0c4400a6000000ab00000000
-                  0000000000a6010000ab0100000000000000007d0d7c0da0140000000000
-                  0000000000000000000000000000007c02640cac0da6020000ab02000000
-                  00000000000100742b00000000000000000000742d000000000000000000
-                  007401000000000000000000006a1200000000000000007c03a6010000ab
-                  010000000000000000a6010000ab010000000000000000a6010000ab0100
-                  0000000000000044005d497d0e7c0ea01700000000000000000000000000
-                  00000000000000640ea6010000ab01000000000000000072327401000000
-                  000000000000006a1800000000000000007400000000000000000000006a
-                  010000000000000000a01900000000000000000000000000000000000000
-                  007c037c0ea6020000ab020000000000000000a6010000ab010000000000
-                  00000001008c4a741000000000000000000000a009000000000000000000
-                  0000000000000000000000640f7c029b0064109d03a6010000ab01000000
-                  00000000000100010090016e682300743400000000000000000000743600
-                  000000000000000000743800000000000000000000743a00000000000000
-                  000000743c0000000000000000000066047600240072467d0f7410000000
-                  00000000000000a01f000000000000000000000000000000000000000064
-                  117c0f9b0064127c0764137a0000009b0064147c049b0064159d07a60100
-                  00ab01000000000000000001007441000000000000000000006a21000000
-                  00000000006416a6010000ab0100000000000000000100590064177d0f7e
-                  0f90018cf564177d0f7e0f77017444000000000000000000006a23000000
-                  00000000006a240000000000000000240072267d0f741000000000000000
-                  000000a01f00000000000000000000000000000000000000007c0f9b00a6
-                  010000ab0100000000000000000100590064177d0f7e0f90028c2d64177d
-                  0f7e0f7701743400000000000000000000240072bb7d0f74100000000000
-                  0000000000a01f000000000000000000000000000000000000000064187c
-                  0764137a0000009b0064147c049b0064157c0f9b0064109d07a6010000ab
-                  0100000000000000000100744b000000000000000000006a260000000000
-                  000000744f000000000000000000006a280000000000000000a6000000ab
-                  000000000000000000641919000000000000000000a6010000ab01000000
-                  00000000007d10741000000000000000000000a009000000000000000000
-                  0000000000000000000000641aa019000000000000000000000000000000
-                  0000000000641b8400745300000000000000000000745400000000000000
-                  0000007c10a6020000ab0200000000000000004400a6000000ab00000000
-                  0000000000a6010000ab010000000000000000a6010000ab010000000000
-                  00000001007441000000000000000000006a210000000000000000641ca6
-                  010000ab0100000000000000000100590064177d0f7e0f90028cf064177d
-                  0f7e0f770177007803590077017c077c046b0500000000721e7410000000
-                  00000000000000a01f000000000000000000000000000000000000000064
-                  1d7c049b00641e9d03a6010000ab01000000000000000001007409000000
-                  000000000000006a050000000000000000a6000000ab0000000000000000
-                  007d05741000000000000000000000a00900000000000000000000000000
-                  00000000000000641fa6010000ab01000000000000000001007410000000
-                  00000000000000a009000000000000000000000000000000000000000064
-                  207c05a0070000000000000000000000000000000000000000a6000000ab
-                  00000000000000000064027a0b000064039b0464219d03a6010000ab0100
-                  0000000000000001006417530023007409000000000000000000006a0500
-                  00000000000000a6000000ab0000000000000000007d0574100000000000
-                  0000000000a0090000000000000000000000000000000000000000641fa6
-                  010000ab0100000000000000000100741000000000000000000000a00900
-                  0000000000000000000000000000000000000064207c05a0070000000000
+                  0x970067007d0609007400000000000000000000006a0100000000000000
+                  00a00200000000000000000000000000000000000000007c04a6010000ab
+                  01000000000000000073147401000000000000000000006a030000000000
+                  0000007c04a6010000ab0100000000000000000100740900000000000000
+                  000000740a000000000000000000009b006401740c000000000000000000
+                  009b009d03a6010000ab0100000000000000000100740f00000000000000
+                  0000006a080000000000000000a6000000ab0000000000000000007d077c
+                  07a0090000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000001007c07a00a0000000000000000000000000000000000
+                  000000a6000000ab0000000000000000007d087416000000000000000000
+                  00a00c0000000000000000000000000000000000000000741a0000000000
+                  00000000009b006402741c000000000000000000009b007c0864037a0b00
+                  0064049b046405740c000000000000000000009b009d06a6010000ab0100
+                  000000000000000100741f000000000000000000007c05a6010000ab0100
+                  00000000000000440090025d1e7d090900090064067d0a741f0000000000
+                  000000000064067421000000000000000000007c01a6010000ab01000000
+                  00000000007c03a6030000ab03000000000000000044005d827d0b7c017c
+                  0b7c0b7c037a0000008502190000000000000000007d0c7c029b0064077c
+                  0a9b0064089d047d0d7c0a64097a0d00007d0a7400000000000000000000
+                  006a010000000000000000a0020000000000000000000000000000000000
+                  0000007c0da6010000ab010000000000000000720b7c029b0064077c0a64
+                  097a0000009b0064089d047d0d7423000000000000000000007c0c640a64
+                  0bac0ca6030000ab0300000000000000007d0e7c0ea01200000000000000
+                  000000000000000000000000007c0da6010000ab01000000000000000001
+                  007c06a01300000000000000000000000000000000000000007c0da60100
+                  00ab01000000000000000001008c83010090016e75230074280000000000
+                  0000000000742a00000000000000000000742c0000000000000000000074
+                  2e0000000000000000000074300000000000000000000066047600240072
+                  467d0f741600000000000000000000a01900000000000000000000000000
+                  00000000000000640d7c0f9b00640e7c0964097a0000009b00640f7c059b
+                  0064109d07a6010000ab0100000000000000000100743500000000000000
+                  0000006a1b00000000000000006411a6010000ab01000000000000000001
+                  00590064127d0f7e0f90018c1064127d0f7e0f7701743800000000000000
+                  0000006a1d00000000000000006a1e0000000000000000240072267d0f74
+                  1600000000000000000000a0190000000000000000000000000000000000
+                  0000007c0f9b00a6010000ab0100000000000000000100590064127d0f7e
+                  0f90018c4864127d0f7e0f7701742800000000000000000000240072c87d
+                  0f741600000000000000000000a019000000000000000000000000000000
+                  0000000000743e000000000000000000009b0064137c0964097a0000009b
+                  00640f7c059b0064107c0f9b00740c000000000000000000009b009d08a6
+                  010000ab01000000000000000001007441000000000000000000006a2100
+                  000000000000007445000000000000000000006a230000000000000000a6
+                  000000ab000000000000000000641419000000000000000000a6010000ab
+                  0100000000000000007d10741600000000000000000000a00c0000000000
+                  0000000000000000000000000000006415a0240000000000000000000000
+                  00000000000000000064168400744b00000000000000000000744c000000
+                  000000000000007c10a6020000ab0200000000000000004400a6000000ab
+                  000000000000000000a6010000ab010000000000000000a6010000ab0100
+                  0000000000000001007435000000000000000000006a1b00000000000000
+                  006417a6010000ab0100000000000000000100590064127d0f7e0f90028c
+                  1864127d0f7e0f770177007803590077017c097c056b0500000000723274
+                  1600000000000000000000a0190000000000000000000000000000000000
+                  00000064187c059b0064199d03a6010000ab010000000000000000010074
+                  45000000000000000000006a2700000000000000006414a6010000ab0100
+                  0000000000000001007421000000000000000000007c06a6010000ab0100
+                  0000000000000064096b0500000000721b745000000000000000000000a0
+                  2900000000000000000000000000000000000000007c067c02a6020000ab
+                  0200000000000000000100740f000000000000000000006a080000000000
+                  000000a6000000ab0000000000000000007d077416000000000000000000
+                  00a00c0000000000000000000000000000000000000000641aa6010000ab
+                  0100000000000000000100740900000000000000000000641ba6010000ab
+                  0100000000000000000100741600000000000000000000a00c0000000000
+                  0000000000000000000000000000007454000000000000000000009b0064
+                  1c7c07a00a0000000000000000000000000000000000000000a6000000ab
+                  00000000000000000064037a0b000064049b04641d740c00000000000000
+                  0000009b009d05a6010000ab010000000000000000010064125300230074
+                  21000000000000000000007c06a6010000ab01000000000000000064096b
+                  0500000000721b745000000000000000000000a029000000000000000000
+                  00000000000000000000007c067c02a6020000ab02000000000000000001
+                  00740f000000000000000000006a080000000000000000a6000000ab0000
+                  000000000000007d07741600000000000000000000a00c00000000000000
+                  00000000000000000000000000641aa6010000ab01000000000000000001
+                  00740900000000000000000000641ba6010000ab01000000000000000001
+                  00741600000000000000000000a00c000000000000000000000000000000
+                  00000000007454000000000000000000009b00641c7c07a00a0000000000
                   000000000000000000000000000000a6000000ab00000000000000000064
-                  027a0b000064039b0464219d03a6010000ab010000000000000000010077
-                  00780359007701
-               566           0 RESUME                   0
-               
-               568           2 NOP
-               
-               569           4 LOAD_GLOBAL              0 (os)
-                            16 LOAD_ATTR                1 (path)
-                            26 LOAD_METHOD              2 (exists)
-                            48 LOAD_FAST                3 (ogg_folder)
-                            50 PRECALL                  1
-                            54 CALL                     1
-                            64 POP_JUMP_FORWARD_IF_TRUE    20 (to 106)
-               
-               570          66 LOAD_GLOBAL              1 (NULL + os)
-                            78 LOAD_ATTR                3 (mkdir)
-                            88 LOAD_FAST                3 (ogg_folder)
-                            90 PRECALL                  1
-                            94 CALL                     1
-                           104 POP_TOP
-               
-               572     >>  106 LOAD_GLOBAL              9 (NULL + speedtest)
-                           118 LOAD_ATTR                5 (Speedtest)
-                           128 PRECALL                  0
-                           132 CALL                     0
-                           142 STORE_FAST               5 (st)
-               
-               573         144 LOAD_FAST                5 (st)
-                           146 LOAD_METHOD              6 (get_best_server)
-                           168 PRECALL                  0
-                           172 CALL                     0
-                           182 POP_TOP
-               
-               574         184 LOAD_FAST                5 (st)
-                           186 LOAD_METHOD              7 (download)
-                           208 PRECALL                  0
-                           212 CALL                     0
-                           222 STORE_FAST               6 (download_speed)
-               
-               575         224 LOAD_GLOBAL             16 (logger)
-                           236 LOAD_METHOD              9 (info)
-               
-               576         258 LOAD_CONST               1 ('\x1b[32m Conversion to mp3 sequence initialized startspeed \x1b[36m')
-               
-               577         260 LOAD_FAST                6 (download_speed)
-                           262 LOAD_CONST               2 (1000000)
-                           264 BINARY_OP               11 (/)
-               
-               576         268 LOAD_CONST               3 ('.2f')
-                           270 FORMAT_VALUE             4 (with format)
-                           272 LOAD_CONST               4 ('Mbps\x1b[0m')
-                           274 BUILD_STRING             3
+                  037a0b000064049b04641d740c000000000000000000009b009d05a60100
+                  00ab01000000000000000001007700780359007701
+               704           0 RESUME                   0
                
-               575         276 PRECALL                  1
-                           280 CALL                     1
-                           290 POP_TOP
+               706           2 BUILD_LIST               0
+                             4 STORE_FAST               6 (out_ls)
                
-               579         292 LOAD_GLOBAL             21 (NULL + range)
-                           304 LOAD_FAST                4 (retries)
-                           306 PRECALL                  1
-                           310 CALL                     1
-                           320 GET_ITER
-                       >>  322 EXTENDED_ARG             2
-                           324 FOR_ITER               758 (to 1842)
-                           326 STORE_FAST               7 (attempt)
-               
-               580         328 NOP
-               
-               581         330 NOP
-               
-               583         332 LOAD_GLOBAL             21 (NULL + range)
-                           344 LOAD_CONST               5 (0)
-                           346 LOAD_GLOBAL             23 (NULL + len)
-                           358 LOAD_FAST                1 (text)
-                           360 PRECALL                  1
-                           364 CALL                     1
-                           374 LOAD_FAST                0 (self)
-                           376 LOAD_ATTR               12 (CHUNK_SIZE)
-                           386 PRECALL                  3
-                           390 CALL                     3
-                           400 GET_ITER
-                       >>  402 FOR_ITER               125 (to 654)
-                           404 STORE_FAST               8 (i)
-               
-               584         406 LOAD_FAST                1 (text)
-                           408 LOAD_FAST                8 (i)
-                           410 LOAD_FAST                8 (i)
-                           412 LOAD_FAST                0 (self)
-                           414 LOAD_ATTR               12 (CHUNK_SIZE)
-                           424 BINARY_OP                0 (+)
-                           428 BUILD_SLICE              2
-                           430 BINARY_SUBSCR
-                           440 STORE_FAST               9 (chunk)
-               
-               585         442 LOAD_GLOBAL             21 (NULL + range)
-                           454 LOAD_CONST               5 (0)
-                           456 LOAD_GLOBAL             27 (NULL + math)
-                           468 LOAD_ATTR               14 (ceil)
-                           478 LOAD_GLOBAL             23 (NULL + len)
-                           490 LOAD_FAST                1 (text)
-                           492 PRECALL                  1
-                           496 CALL                     1
-                           506 LOAD_FAST                0 (self)
-                           508 LOAD_ATTR               12 (CHUNK_SIZE)
-                           518 BINARY_OP               11 (/)
-                           522 PRECALL                  1
-                           526 CALL                     1
-                           536 PRECALL                  2
-                           540 CALL                     2
-                           550 GET_ITER
-                       >>  552 FOR_ITER                10 (to 574)
-                           554 STORE_FAST               8 (i)
-               
-               586         556 LOAD_FAST                2 (output_file)
-                           558 FORMAT_VALUE             0
-                           560 LOAD_CONST               6 ('_')
-                           562 LOAD_FAST                8 (i)
-                           564 FORMAT_VALUE             0
-                           566 LOAD_CONST               7 ('.ogg')
-                           568 BUILD_STRING             4
-                           570 STORE_FAST              10 (output_filename)
-                           572 JUMP_BACKWARD           11 (to 552)
-               
-               587     >>  574 LOAD_GLOBAL             31 (NULL + gTTS)
-                           586 LOAD_FAST                9 (chunk)
-                           588 LOAD_CONST               8 ('en')
-                           590 LOAD_CONST               9 (False)
-                           592 KW_NAMES                10
-                           594 PRECALL                  3
-                           598 CALL                     3
-                           608 STORE_FAST              11 (tts)
-               
-               588         610 LOAD_FAST               11 (tts)
-                           612 LOAD_METHOD             16 (save)
-                           634 LOAD_FAST               10 (output_filename)
-                           636 PRECALL                  1
-                           640 CALL                     1
-                           650 POP_TOP
-                           652 JUMP_BACKWARD          126 (to 402)
+               707           6 NOP
+               
+               708           8 LOAD_GLOBAL              0 (os)
+                            20 LOAD_ATTR                1 (path)
+                            30 LOAD_METHOD              2 (exists)
+                            52 LOAD_FAST                4 (ogg_folder)
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 POP_JUMP_FORWARD_IF_TRUE    20 (to 110)
+               
+               709          70 LOAD_GLOBAL              1 (NULL + os)
+                            82 LOAD_ATTR                3 (mkdir)
+                            92 LOAD_FAST                4 (ogg_folder)
+                            94 PRECALL                  1
+                            98 CALL                     1
+                           108 POP_TOP
+               
+               710     >>  110 LOAD_GLOBAL              9 (NULL + print)
+                           122 LOAD_GLOBAL             10 (DYELLOW)
+                           134 FORMAT_VALUE             0
+                           136 LOAD_CONST               1 ('Get initial net speed..')
+                           138 LOAD_GLOBAL             12 (RESET)
+                           150 FORMAT_VALUE             0
+                           152 BUILD_STRING             3
+                           154 PRECALL                  1
+                           158 CALL                     1
+                           168 POP_TOP
+               
+               711         170 LOAD_GLOBAL             15 (NULL + speedtest)
+                           182 LOAD_ATTR                8 (Speedtest)
+                           192 PRECALL                  0
+                           196 CALL                     0
+                           206 STORE_FAST               7 (st)
+               
+               712         208 LOAD_FAST                7 (st)
+                           210 LOAD_METHOD              9 (get_best_server)
+                           232 PRECALL                  0
+                           236 CALL                     0
+                           246 POP_TOP
                
-               591     >>  654 LOAD_GLOBAL             35 (NULL + sorted)
-                           666 LOAD_GLOBAL              1 (NULL + os)
-                           678 LOAD_ATTR               18 (listdir)
-                           688 LOAD_FAST                3 (ogg_folder)
-                           690 PRECALL                  1
-                           694 CALL                     1
+               713         248 LOAD_FAST                7 (st)
+                           250 LOAD_METHOD             10 (download)
+                           272 PRECALL                  0
+                           276 CALL                     0
+                           286 STORE_FAST               8 (download_speed)
+               
+               714         288 LOAD_GLOBAL             22 (logger)
+                           300 LOAD_METHOD             12 (info)
+               
+               716         322 LOAD_GLOBAL             26 (GREEN)
+                           334 FORMAT_VALUE             0
+                           336 LOAD_CONST               2 (' Conversion to mp3 sequence initialized startspeed ')
+               
+               717         338 LOAD_GLOBAL             28 (CYAN)
+               
+               716         350 FORMAT_VALUE             0
+               
+               717         352 LOAD_FAST                8 (download_speed)
+                           354 LOAD_CONST               3 (1000000)
+                           356 BINARY_OP               11 (/)
+               
+               716         360 LOAD_CONST               4 ('.2f')
+                           362 FORMAT_VALUE             4 (with format)
+                           364 LOAD_CONST               5 ('Kbps')
+               
+               717         366 LOAD_GLOBAL             12 (RESET)
+               
+               716         378 FORMAT_VALUE             0
+                           380 BUILD_STRING             6
+               
+               714         382 PRECALL                  1
+                           386 CALL                     1
+                           396 POP_TOP
+               
+               719         398 LOAD_GLOBAL             31 (NULL + range)
+                           410 LOAD_FAST                5 (retries)
+                           412 PRECALL                  1
+                           416 CALL                     1
+                           426 GET_ITER
+                       >>  428 EXTENDED_ARG             2
+                           430 FOR_ITER               542 (to 1516)
+                           432 STORE_FAST               9 (attempt)
+               
+               720         434 NOP
+               
+               721         436 NOP
+               
+               723         438 LOAD_CONST               6 (0)
+                           440 STORE_FAST              10 (counter)
+               
+               724         442 LOAD_GLOBAL             31 (NULL + range)
+                           454 LOAD_CONST               6 (0)
+                           456 LOAD_GLOBAL             33 (NULL + len)
+                           468 LOAD_FAST                1 (text)
+                           470 PRECALL                  1
+                           474 CALL                     1
+                           484 LOAD_FAST                3 (CHUNK_SIZE)
+                           486 PRECALL                  3
+                           490 CALL                     3
+                           500 GET_ITER
+                       >>  502 FOR_ITER               130 (to 764)
+                           504 STORE_FAST              11 (i)
+               
+               725         506 LOAD_FAST                1 (text)
+                           508 LOAD_FAST               11 (i)
+                           510 LOAD_FAST               11 (i)
+                           512 LOAD_FAST                3 (CHUNK_SIZE)
+                           514 BINARY_OP                0 (+)
+                           518 BUILD_SLICE              2
+                           520 BINARY_SUBSCR
+                           530 STORE_FAST              12 (chunk)
+               
+               726         532 LOAD_FAST                2 (output_file)
+                           534 FORMAT_VALUE             0
+                           536 LOAD_CONST               7 ('_')
+                           538 LOAD_FAST               10 (counter)
+                           540 FORMAT_VALUE             0
+                           542 LOAD_CONST               8 ('.ogg')
+                           544 BUILD_STRING             4
+                           546 STORE_FAST              13 (output_filename)
+               
+               727         548 LOAD_FAST               10 (counter)
+                           550 LOAD_CONST               9 (1)
+                           552 BINARY_OP               13 (+=)
+                           556 STORE_FAST              10 (counter)
+               
+               729         558 LOAD_GLOBAL              0 (os)
+                           570 LOAD_ATTR                1 (path)
+                           580 LOAD_METHOD              2 (exists)
+                           602 LOAD_FAST               13 (output_filename)
+                           604 PRECALL                  1
+                           608 CALL                     1
+                           618 POP_JUMP_FORWARD_IF_FALSE    11 (to 642)
+               
+               730         620 LOAD_FAST                2 (output_file)
+                           622 FORMAT_VALUE             0
+                           624 LOAD_CONST               7 ('_')
+                           626 LOAD_FAST               10 (counter)
+                           628 LOAD_CONST               9 (1)
+                           630 BINARY_OP                0 (+)
+                           634 FORMAT_VALUE             0
+                           636 LOAD_CONST               8 ('.ogg')
+                           638 BUILD_STRING             4
+                           640 STORE_FAST              13 (output_filename)
+               
+               732     >>  642 LOAD_GLOBAL             35 (NULL + gTTS)
+                           654 LOAD_FAST               12 (chunk)
+                           656 LOAD_CONST              10 ('en')
+                           658 LOAD_CONST              11 (False)
+                           660 KW_NAMES                12
+                           662 PRECALL                  3
+                           666 CALL                     3
+                           676 STORE_FAST              14 (tts)
+               
+               733         678 LOAD_FAST               14 (tts)
+                           680 LOAD_METHOD             18 (save)
+                           702 LOAD_FAST               13 (output_filename)
                            704 PRECALL                  1
                            708 CALL                     1
-                           718 STORE_FAST              12 (combined_files)
-               
-               593         720 LOAD_GLOBAL             39 (NULL + join_audios)
-                           732 LOAD_CONST              11 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 593>)
-                           734 MAKE_FUNCTION            0
+                           718 POP_TOP
                
-               594         736 LOAD_FAST               12 (combined_files)
+               734         720 LOAD_FAST                6 (out_ls)
+                           722 LOAD_METHOD             19 (append)
+                           744 LOAD_FAST               13 (output_filename)
+                           746 PRECALL                  1
+                           750 CALL                     1
+                           760 POP_TOP
+                           762 JUMP_BACKWARD          131 (to 502)
+               
+               735     >>  764 POP_TOP
+                           766 EXTENDED_ARG             1
+                           768 JUMP_FORWARD           373 (to 1516)
+                       >>  770 PUSH_EXC_INFO
+               
+               738         772 LOAD_GLOBAL             40 (Exception)
+                           784 LOAD_GLOBAL             42 (ConnectionError)
+                           796 LOAD_GLOBAL             44 (ConnectionAbortedError)
+               
+               739         808 LOAD_GLOBAL             46 (ConnectionRefusedError)
+               
+               740         820 LOAD_GLOBAL             48 (ConnectionResetError)
+               
+               738         832 BUILD_TUPLE              4
+                           834 CONTAINS_OP              0
+                           836 CHECK_EXC_MATCH
+                           838 POP_JUMP_FORWARD_IF_FALSE    70 (to 980)
+                           840 STORE_FAST              15 (e)
+               
+               741         842 LOAD_GLOBAL             22 (logger)
+                           854 LOAD_METHOD             25 (error)
+                           876 LOAD_CONST              13 ('Sorry boss connection problem encountered: ')
+                           878 LOAD_FAST               15 (e)
+                           880 FORMAT_VALUE             0
+                           882 LOAD_CONST              14 (' in ')
+                           884 LOAD_FAST                9 (attempt)
+                           886 LOAD_CONST               9 (1)
+                           888 BINARY_OP                0 (+)
+                           892 FORMAT_VALUE             0
+                           894 LOAD_CONST              15 ('/')
+                           896 LOAD_FAST                5 (retries)
+                           898 FORMAT_VALUE             0
+                           900 LOAD_CONST              16 (':')
+                           902 BUILD_STRING             7
+                           904 PRECALL                  1
+                           908 CALL                     1
+                           918 POP_TOP
                
-               593         738 GET_ITER
-                           740 PRECALL                  0
-                           744 CALL                     0
-                           754 PRECALL                  1
-                           758 CALL                     1
-                           768 STORE_FAST              13 (combined_audio)
+               742         920 LOAD_GLOBAL             53 (NULL + time)
+                           932 LOAD_ATTR               27 (sleep)
+                           942 LOAD_CONST              17 (5)
+                           944 PRECALL                  1
+                           948 CALL                     1
+                           958 POP_TOP
+                           960 POP_EXCEPT
+                           962 LOAD_CONST              18 (None)
+                           964 STORE_FAST              15 (e)
+                           966 DELETE_FAST             15 (e)
+                           968 EXTENDED_ARG             1
+                           970 JUMP_BACKWARD          272 (to 428)
+                       >>  972 LOAD_CONST              18 (None)
+                           974 STORE_FAST              15 (e)
+                           976 DELETE_FAST             15 (e)
+                           978 RERAISE                  1
+               
+               745     >>  980 LOAD_GLOBAL             56 (requests)
+                           992 LOAD_ATTR               29 (exceptions)
+                          1002 LOAD_ATTR               30 (RequestException)
+                          1012 CHECK_EXC_MATCH
+                          1014 POP_JUMP_FORWARD_IF_FALSE    38 (to 1092)
+                          1016 STORE_FAST              15 (e)
+               
+               746        1018 LOAD_GLOBAL             22 (logger)
+                          1030 LOAD_METHOD             25 (error)
+                          1052 LOAD_FAST               15 (e)
+                          1054 FORMAT_VALUE             0
+                          1056 PRECALL                  1
+                          1060 CALL                     1
+                          1070 POP_TOP
+                          1072 POP_EXCEPT
+                          1074 LOAD_CONST              18 (None)
+                          1076 STORE_FAST              15 (e)
+                          1078 DELETE_FAST             15 (e)
+                          1080 EXTENDED_ARG             1
+                          1082 JUMP_BACKWARD          328 (to 428)
+                       >> 1084 LOAD_CONST              18 (None)
+                          1086 STORE_FAST              15 (e)
+                          1088 DELETE_FAST             15 (e)
+                          1090 RERAISE                  1
+               
+               747     >> 1092 LOAD_GLOBAL             40 (Exception)
+                          1104 CHECK_EXC_MATCH
+                          1106 POP_JUMP_FORWARD_IF_FALSE   200 (to 1508)
+                          1108 STORE_FAST              15 (e)
+               
+               748        1110 LOAD_GLOBAL             22 (logger)
+                          1122 LOAD_METHOD             25 (error)
+                          1144 LOAD_GLOBAL             62 (DRED)
+                          1156 FORMAT_VALUE             0
+                          1158 LOAD_CONST              19 (' Error during conversion attempt ')
+               
+               749        1160 LOAD_FAST                9 (attempt)
+                          1162 LOAD_CONST               9 (1)
+                          1164 BINARY_OP                0 (+)
+               
+               748        1168 FORMAT_VALUE             0
+                          1170 LOAD_CONST              15 ('/')
+               
+               749        1172 LOAD_FAST                5 (retries)
+               
+               748        1174 FORMAT_VALUE             0
+                          1176 LOAD_CONST              16 (':')
+               
+               749        1178 LOAD_FAST               15 (e)
+               
+               748        1180 FORMAT_VALUE             0
+               
+               749        1182 LOAD_GLOBAL             12 (RESET)
+               
+               748        1194 FORMAT_VALUE             0
+                          1196 BUILD_STRING             8
+                          1198 PRECALL                  1
+                          1202 CALL                     1
+                          1212 POP_TOP
+               
+               750        1214 LOAD_GLOBAL             65 (NULL + traceback)
+                          1226 LOAD_ATTR               33 (extract_tb)
+                          1236 LOAD_GLOBAL             69 (NULL + sys)
+                          1248 LOAD_ATTR               35 (exc_info)
+                          1258 PRECALL                  0
+                          1262 CALL                     0
+                          1272 LOAD_CONST              20 (2)
+                          1274 BINARY_SUBSCR
+                          1284 PRECALL                  1
+                          1288 CALL                     1
+                          1298 STORE_FAST              16 (tb)
+               
+               751        1300 LOAD_GLOBAL             22 (logger)
+                          1312 LOAD_METHOD             12 (info)
+                          1334 LOAD_CONST              21 ('\n')
+                          1336 LOAD_METHOD             36 (join)
+                          1358 LOAD_CONST              22 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 751>)
+                          1360 MAKE_FUNCTION            0
+               
+               752        1362 LOAD_GLOBAL             75 (NULL + map)
+                          1374 LOAD_GLOBAL             76 (str)
+                          1386 LOAD_FAST               16 (tb)
+                          1388 PRECALL                  2
+                          1392 CALL                     2
+               
+               751        1402 GET_ITER
+                          1404 PRECALL                  0
+                          1408 CALL                     0
+                          1418 PRECALL                  1
+                          1422 CALL                     1
+                          1432 PRECALL                  1
+                          1436 CALL                     1
+                          1446 POP_TOP
+               
+               753        1448 LOAD_GLOBAL             53 (NULL + time)
+                          1460 LOAD_ATTR               27 (sleep)
+                          1470 LOAD_CONST              23 (3)
+                          1472 PRECALL                  1
+                          1476 CALL                     1
+                          1486 POP_TOP
+               
+               754        1488 POP_EXCEPT
+                          1490 LOAD_CONST              18 (None)
+                          1492 STORE_FAST              15 (e)
+                          1494 DELETE_FAST             15 (e)
+                          1496 EXTENDED_ARG             2
+                          1498 JUMP_BACKWARD          536 (to 428)
+                       >> 1500 LOAD_CONST              18 (None)
+                          1502 STORE_FAST              15 (e)
+                          1504 DELETE_FAST             15 (e)
+                          1506 RERAISE                  1
+               
+               747     >> 1508 RERAISE                  0
+                       >> 1510 COPY                     3
+                          1512 POP_EXCEPT
+                          1514 RERAISE                  1
+               
+               756     >> 1516 LOAD_FAST                9 (attempt)
+                          1518 LOAD_FAST                5 (retries)
+                          1520 COMPARE_OP               5 (>=)
+                          1526 POP_JUMP_FORWARD_IF_FALSE    50 (to 1628)
+               
+               757        1528 LOAD_GLOBAL             22 (logger)
+                          1540 LOAD_METHOD             25 (error)
+               
+               758        1562 LOAD_CONST              24 ('Conversion unsuccessful after ')
+                          1564 LOAD_FAST                5 (retries)
+                          1566 FORMAT_VALUE             0
+                          1568 LOAD_CONST              25 (' attempts.')
+                          1570 BUILD_STRING             3
+               
+               757        1572 PRECALL                  1
+                          1576 CALL                     1
+                          1586 POP_TOP
+               
+               759        1588 LOAD_GLOBAL             69 (NULL + sys)
+                          1600 LOAD_ATTR               39 (exit)
+                          1610 LOAD_CONST              20 (2)
+                          1612 PRECALL                  1
+                          1616 CALL                     1
+                          1626 POP_TOP
+               
+               764     >> 1628 LOAD_GLOBAL             33 (NULL + len)
+                          1640 LOAD_FAST                6 (out_ls)
+                          1642 PRECALL                  1
+                          1646 CALL                     1
+                          1656 LOAD_CONST               9 (1)
+                          1658 COMPARE_OP               5 (>=)
+                          1664 POP_JUMP_FORWARD_IF_FALSE    27 (to 1720)
+               
+               765        1666 LOAD_GLOBAL             80 (FileSynthesis)
+                          1678 LOAD_METHOD             41 (join_audios)
+                          1700 LOAD_FAST                6 (out_ls)
+                          1702 LOAD_FAST                2 (output_file)
+                          1704 PRECALL                  2
+                          1708 CALL                     2
+                          1718 POP_TOP
                
-               597         770 LOAD_FAST               13 (combined_audio)
-                           772 LOAD_METHOD             20 (export)
-                           794 LOAD_FAST                2 (output_file)
-                           796 LOAD_CONST              12 ('mp3')
-                           798 KW_NAMES                13
-                           800 PRECALL                  2
-                           804 CALL                     2
-                           814 POP_TOP
-               
-               600         816 LOAD_GLOBAL             43 (NULL + reversed)
-                           828 LOAD_GLOBAL             45 (NULL + list)
-                           840 LOAD_GLOBAL              1 (NULL + os)
-                           852 LOAD_ATTR               18 (listdir)
-                           862 LOAD_FAST                3 (ogg_folder)
-                           864 PRECALL                  1
-                           868 CALL                     1
-                           878 PRECALL                  1
-                           882 CALL                     1
-                           892 PRECALL                  1
-                           896 CALL                     1
-                           906 GET_ITER
-                       >>  908 FOR_ITER                73 (to 1056)
-                           910 STORE_FAST              14 (fname)
-               
-               601         912 LOAD_FAST               14 (fname)
-                           914 LOAD_METHOD             23 (startswith)
-                           936 LOAD_CONST              14 ('chunk')
-                           938 PRECALL                  1
-                           942 CALL                     1
-                           952 POP_JUMP_FORWARD_IF_FALSE    50 (to 1054)
-               
-               602         954 LOAD_GLOBAL              1 (NULL + os)
-                           966 LOAD_ATTR               24 (remove)
-                           976 LOAD_GLOBAL              0 (os)
-                           988 LOAD_ATTR                1 (path)
-                           998 LOAD_METHOD             25 (join)
-                          1020 LOAD_FAST                3 (ogg_folder)
-                          1022 LOAD_FAST               14 (fname)
-                          1024 PRECALL                  2
-                          1028 CALL                     2
-                          1038 PRECALL                  1
-                          1042 CALL                     1
-                          1052 POP_TOP
-                       >> 1054 JUMP_BACKWARD           74 (to 908)
-               
-               604     >> 1056 LOAD_GLOBAL             16 (logger)
-                          1068 LOAD_METHOD              9 (info)
-               
-               605        1090 LOAD_CONST              15 ('\x1b[32m Conversion successful! Output file: ')
-               
-               606        1092 LOAD_FAST                2 (output_file)
-               
-               605        1094 FORMAT_VALUE             0
-                          1096 LOAD_CONST              16 ('\x1b[0m')
-                          1098 BUILD_STRING             3
-               
-               604        1100 PRECALL                  1
-                          1104 CALL                     1
-                          1114 POP_TOP
-               
-               607        1116 POP_TOP
-                          1118 EXTENDED_ARG             1
-                          1120 JUMP_FORWARD           360 (to 1842)
-                       >> 1122 PUSH_EXC_INFO
-               
-               610        1124 LOAD_GLOBAL             52 (Exception)
-                          1136 LOAD_GLOBAL             54 (ConnectionError)
-                          1148 LOAD_GLOBAL             56 (ConnectionAbortedError)
-                          1160 LOAD_GLOBAL             58 (ConnectionRefusedError)
-                          1172 LOAD_GLOBAL             60 (ConnectionResetError)
-                          1184 BUILD_TUPLE              4
-                          1186 CONTAINS_OP              0
-                          1188 CHECK_EXC_MATCH
-                          1190 POP_JUMP_FORWARD_IF_FALSE    70 (to 1332)
-                          1192 STORE_FAST              15 (e)
-               
-               611        1194 LOAD_GLOBAL             16 (logger)
-                          1206 LOAD_METHOD             31 (error)
-                          1228 LOAD_CONST              17 ('Sorry boss we are sad to note the followingconnection issue arised: ')
-               
-               612        1230 LOAD_FAST               15 (e)
-               
-               611        1232 FORMAT_VALUE             0
-                          1234 LOAD_CONST              18 (' in ')
-               
-               612        1236 LOAD_FAST                7 (attempt)
-                          1238 LOAD_CONST              19 (1)
-                          1240 BINARY_OP                0 (+)
-               
-               611        1244 FORMAT_VALUE             0
-                          1246 LOAD_CONST              20 ('/')
-               
-               612        1248 LOAD_FAST                4 (retries)
-               
-               611        1250 FORMAT_VALUE             0
-                          1252 LOAD_CONST              21 (':')
-                          1254 BUILD_STRING             7
-                          1256 PRECALL                  1
-                          1260 CALL                     1
-                          1270 POP_TOP
-               
-               613        1272 LOAD_GLOBAL             65 (NULL + time)
-                          1284 LOAD_ATTR               33 (sleep)
-                          1294 LOAD_CONST              22 (5)
-                          1296 PRECALL                  1
-                          1300 CALL                     1
-                          1310 POP_TOP
-                          1312 POP_EXCEPT
-                          1314 LOAD_CONST              23 (None)
-                          1316 STORE_FAST              15 (e)
-                          1318 DELETE_FAST             15 (e)
-                          1320 EXTENDED_ARG             1
-                          1322 JUMP_BACKWARD          501 (to 322)
-                       >> 1324 LOAD_CONST              23 (None)
-                          1326 STORE_FAST              15 (e)
-                          1328 DELETE_FAST             15 (e)
-                          1330 RERAISE                  1
-               
-               616     >> 1332 LOAD_GLOBAL             68 (requests)
-                          1344 LOAD_ATTR               35 (exceptions)
-                          1354 LOAD_ATTR               36 (RequestException)
-                          1364 CHECK_EXC_MATCH
-                          1366 POP_JUMP_FORWARD_IF_FALSE    38 (to 1444)
-                          1368 STORE_FAST              15 (e)
-               
-               617        1370 LOAD_GLOBAL             16 (logger)
-                          1382 LOAD_METHOD             31 (error)
-                          1404 LOAD_FAST               15 (e)
-                          1406 FORMAT_VALUE             0
-                          1408 PRECALL                  1
-                          1412 CALL                     1
-                          1422 POP_TOP
-                          1424 POP_EXCEPT
-                          1426 LOAD_CONST              23 (None)
-                          1428 STORE_FAST              15 (e)
-                          1430 DELETE_FAST             15 (e)
-                          1432 EXTENDED_ARG             2
-                          1434 JUMP_BACKWARD          557 (to 322)
-                       >> 1436 LOAD_CONST              23 (None)
-                          1438 STORE_FAST              15 (e)
-                          1440 DELETE_FAST             15 (e)
-                          1442 RERAISE                  1
-               
-               618     >> 1444 LOAD_GLOBAL             52 (Exception)
-                          1456 CHECK_EXC_MATCH
-                          1458 POP_JUMP_FORWARD_IF_FALSE   187 (to 1834)
-                          1460 STORE_FAST              15 (e)
-               
-               619        1462 LOAD_GLOBAL             16 (logger)
-                          1474 LOAD_METHOD             31 (error)
-                          1496 LOAD_CONST              24 ('\x1b[31m Error during conversion attempt ')
-               
-               620        1498 LOAD_FAST                7 (attempt)
-                          1500 LOAD_CONST              19 (1)
-                          1502 BINARY_OP                0 (+)
-               
-               619        1506 FORMAT_VALUE             0
-                          1508 LOAD_CONST              20 ('/')
-               
-               620        1510 LOAD_FAST                4 (retries)
-               
-               619        1512 FORMAT_VALUE             0
-                          1514 LOAD_CONST              21 (':')
-               
-               620        1516 LOAD_FAST               15 (e)
-               
-               619        1518 FORMAT_VALUE             0
-                          1520 LOAD_CONST              16 ('\x1b[0m')
-                          1522 BUILD_STRING             7
-                          1524 PRECALL                  1
-                          1528 CALL                     1
-                          1538 POP_TOP
-               
-               621        1540 LOAD_GLOBAL             75 (NULL + traceback)
-                          1552 LOAD_ATTR               38 (extract_tb)
-                          1562 LOAD_GLOBAL             79 (NULL + sys)
-                          1574 LOAD_ATTR               40 (exc_info)
-                          1584 PRECALL                  0
-                          1588 CALL                     0
-                          1598 LOAD_CONST              25 (2)
-                          1600 BINARY_SUBSCR
-                          1610 PRECALL                  1
-                          1614 CALL                     1
-                          1624 STORE_FAST              16 (tb)
-               
-               622        1626 LOAD_GLOBAL             16 (logger)
-                          1638 LOAD_METHOD              9 (info)
-                          1660 LOAD_CONST              26 ('\n')
-                          1662 LOAD_METHOD             25 (join)
-                          1684 LOAD_CONST              27 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 622>)
-                          1686 MAKE_FUNCTION            0
-               
-               623        1688 LOAD_GLOBAL             83 (NULL + map)
-                          1700 LOAD_GLOBAL             84 (str)
-                          1712 LOAD_FAST               16 (tb)
-                          1714 PRECALL                  2
-                          1718 CALL                     2
-               
-               622        1728 GET_ITER
-                          1730 PRECALL                  0
-                          1734 CALL                     0
-                          1744 PRECALL                  1
-                          1748 CALL                     1
-                          1758 PRECALL                  1
-                          1762 CALL                     1
-                          1772 POP_TOP
-               
-               624        1774 LOAD_GLOBAL             65 (NULL + time)
-                          1786 LOAD_ATTR               33 (sleep)
-                          1796 LOAD_CONST              28 (3)
-                          1798 PRECALL                  1
-                          1802 CALL                     1
-                          1812 POP_TOP
-               
-               625        1814 POP_EXCEPT
-                          1816 LOAD_CONST              23 (None)
-                          1818 STORE_FAST              15 (e)
-                          1820 DELETE_FAST             15 (e)
-                          1822 EXTENDED_ARG             2
-                          1824 JUMP_BACKWARD          752 (to 322)
-                       >> 1826 LOAD_CONST              23 (None)
-                          1828 STORE_FAST              15 (e)
-                          1830 DELETE_FAST             15 (e)
-                          1832 RERAISE                  1
-               
-               618     >> 1834 RERAISE                  0
-                       >> 1836 COPY                     3
-                          1838 POP_EXCEPT
-                          1840 RERAISE                  1
-               
-               627     >> 1842 LOAD_FAST                7 (attempt)
-                          1844 LOAD_FAST                4 (retries)
-                          1846 COMPARE_OP               5 (>=)
-                          1852 POP_JUMP_FORWARD_IF_FALSE    30 (to 1914)
-               
-               628        1854 LOAD_GLOBAL             16 (logger)
-                          1866 LOAD_METHOD             31 (error)
-               
-               629        1888 LOAD_CONST              29 ('Conversion unsuccessful after ')
-                          1890 LOAD_FAST                4 (retries)
-                          1892 FORMAT_VALUE             0
-                          1894 LOAD_CONST              30 (' \x07ttempts.')
-                          1896 BUILD_STRING             3
-               
-               628        1898 PRECALL                  1
-                          1902 CALL                     1
-                          1912 POP_TOP
-               
-               632     >> 1914 LOAD_GLOBAL              9 (NULL + speedtest)
-                          1926 LOAD_ATTR                5 (Speedtest)
-                          1936 PRECALL                  0
-                          1940 CALL                     0
-                          1950 STORE_FAST               5 (st)
-               
-               633        1952 LOAD_GLOBAL             16 (logger)
-                          1964 LOAD_METHOD              9 (info)
-                          1986 LOAD_CONST              31 ('Done')
-                          1988 PRECALL                  1
-                          1992 CALL                     1
-                          2002 POP_TOP
-               
-               634        2004 LOAD_GLOBAL             16 (logger)
-                          2016 LOAD_METHOD              9 (info)
-               
-               635        2038 LOAD_CONST              32 ('\x1b[33m Final Network Speed: ')
-                          2040 LOAD_FAST                5 (st)
-                          2042 LOAD_METHOD              7 (download)
-                          2064 PRECALL                  0
-                          2068 CALL                     0
-                          2078 LOAD_CONST               2 (1000000)
-                          2080 BINARY_OP               11 (/)
-                          2084 LOAD_CONST               3 ('.2f')
-                          2086 FORMAT_VALUE             4 (with format)
-                          2088 LOAD_CONST              33 (' Mbps\x1b[0m')
-                          2090 BUILD_STRING             3
-               
-               634        2092 PRECALL                  1
-                          2096 CALL                     1
-                          2106 POP_TOP
-                          2108 LOAD_CONST              23 (None)
-                          2110 RETURN_VALUE
-                       >> 2112 PUSH_EXC_INFO
-               
-               632        2114 LOAD_GLOBAL              9 (NULL + speedtest)
-                          2126 LOAD_ATTR                5 (Speedtest)
-                          2136 PRECALL                  0
-                          2140 CALL                     0
-                          2150 STORE_FAST               5 (st)
-               
-               633        2152 LOAD_GLOBAL             16 (logger)
-                          2164 LOAD_METHOD              9 (info)
-                          2186 LOAD_CONST              31 ('Done')
-                          2188 PRECALL                  1
-                          2192 CALL                     1
-                          2202 POP_TOP
-               
-               634        2204 LOAD_GLOBAL             16 (logger)
-                          2216 LOAD_METHOD              9 (info)
-               
-               635        2238 LOAD_CONST              32 ('\x1b[33m Final Network Speed: ')
-                          2240 LOAD_FAST                5 (st)
-                          2242 LOAD_METHOD              7 (download)
+               767     >> 1720 LOAD_GLOBAL             15 (NULL + speedtest)
+                          1732 LOAD_ATTR                8 (Speedtest)
+                          1742 PRECALL                  0
+                          1746 CALL                     0
+                          1756 STORE_FAST               7 (st)
+               
+               768        1758 LOAD_GLOBAL             22 (logger)
+                          1770 LOAD_METHOD             12 (info)
+                          1792 LOAD_CONST              26 ('Done')
+                          1794 PRECALL                  1
+                          1798 CALL                     1
+                          1808 POP_TOP
+               
+               769        1810 LOAD_GLOBAL              9 (NULL + print)
+                          1822 LOAD_CONST              27 ('Get final speed ...')
+                          1824 PRECALL                  1
+                          1828 CALL                     1
+                          1838 POP_TOP
+               
+               770        1840 LOAD_GLOBAL             22 (logger)
+                          1852 LOAD_METHOD             12 (info)
+               
+               772        1874 LOAD_GLOBAL             84 (YELLOW)
+                          1886 FORMAT_VALUE             0
+                          1888 LOAD_CONST              28 ('Final Network Speed: ')
+                          1890 LOAD_FAST                7 (st)
+                          1892 LOAD_METHOD             10 (download)
+                          1914 PRECALL                  0
+                          1918 CALL                     0
+                          1928 LOAD_CONST               3 (1000000)
+                          1930 BINARY_OP               11 (/)
+                          1934 LOAD_CONST               4 ('.2f')
+                          1936 FORMAT_VALUE             4 (with format)
+                          1938 LOAD_CONST              29 (' Kbps')
+                          1940 LOAD_GLOBAL             12 (RESET)
+                          1952 FORMAT_VALUE             0
+                          1954 BUILD_STRING             5
+               
+               770        1956 PRECALL                  1
+                          1960 CALL                     1
+                          1970 POP_TOP
+                          1972 LOAD_CONST              18 (None)
+                          1974 RETURN_VALUE
+                       >> 1976 PUSH_EXC_INFO
+               
+               764        1978 LOAD_GLOBAL             33 (NULL + len)
+                          1990 LOAD_FAST                6 (out_ls)
+                          1992 PRECALL                  1
+                          1996 CALL                     1
+                          2006 LOAD_CONST               9 (1)
+                          2008 COMPARE_OP               5 (>=)
+                          2014 POP_JUMP_FORWARD_IF_FALSE    27 (to 2070)
+               
+               765        2016 LOAD_GLOBAL             80 (FileSynthesis)
+                          2028 LOAD_METHOD             41 (join_audios)
+                          2050 LOAD_FAST                6 (out_ls)
+                          2052 LOAD_FAST                2 (output_file)
+                          2054 PRECALL                  2
+                          2058 CALL                     2
+                          2068 POP_TOP
+               
+               767     >> 2070 LOAD_GLOBAL             15 (NULL + speedtest)
+                          2082 LOAD_ATTR                8 (Speedtest)
+                          2092 PRECALL                  0
+                          2096 CALL                     0
+                          2106 STORE_FAST               7 (st)
+               
+               768        2108 LOAD_GLOBAL             22 (logger)
+                          2120 LOAD_METHOD             12 (info)
+                          2142 LOAD_CONST              26 ('Done')
+                          2144 PRECALL                  1
+                          2148 CALL                     1
+                          2158 POP_TOP
+               
+               769        2160 LOAD_GLOBAL              9 (NULL + print)
+                          2172 LOAD_CONST              27 ('Get final speed ...')
+                          2174 PRECALL                  1
+                          2178 CALL                     1
+                          2188 POP_TOP
+               
+               770        2190 LOAD_GLOBAL             22 (logger)
+                          2202 LOAD_METHOD             12 (info)
+               
+               772        2224 LOAD_GLOBAL             84 (YELLOW)
+                          2236 FORMAT_VALUE             0
+                          2238 LOAD_CONST              28 ('Final Network Speed: ')
+                          2240 LOAD_FAST                7 (st)
+                          2242 LOAD_METHOD             10 (download)
                           2264 PRECALL                  0
                           2268 CALL                     0
-                          2278 LOAD_CONST               2 (1000000)
+                          2278 LOAD_CONST               3 (1000000)
                           2280 BINARY_OP               11 (/)
-                          2284 LOAD_CONST               3 ('.2f')
+                          2284 LOAD_CONST               4 ('.2f')
                           2286 FORMAT_VALUE             4 (with format)
-                          2288 LOAD_CONST              33 (' Mbps\x1b[0m')
-                          2290 BUILD_STRING             3
-               
-               634        2292 PRECALL                  1
-                          2296 CALL                     1
-                          2306 POP_TOP
-                          2308 RERAISE                  0
-                       >> 2310 COPY                     3
-                          2312 POP_EXCEPT
-                          2314 RERAISE                  1
+                          2288 LOAD_CONST              29 (' Kbps')
+                          2290 LOAD_GLOBAL             12 (RESET)
+                          2302 FORMAT_VALUE             0
+                          2304 BUILD_STRING             5
+               
+               770        2306 PRECALL                  1
+                          2310 CALL                     1
+                          2320 POP_TOP
+                          2322 RERAISE                  0
+                       >> 2324 COPY                     3
+                          2326 POP_EXCEPT
+                          2328 RERAISE                  1
                ExceptionTable:
-                 4 to 326 -> 2112 [0]
-                 330 to 1114 -> 1122 [1]
-                 1116 to 1120 -> 2112 [0]
-                 1122 to 1192 -> 1836 [2] lasti
-                 1194 to 1310 -> 1324 [2] lasti
-                 1312 to 1322 -> 2112 [0]
-                 1324 to 1368 -> 1836 [2] lasti
-                 1370 to 1422 -> 1436 [2] lasti
-                 1424 to 1434 -> 2112 [0]
-                 1436 to 1460 -> 1836 [2] lasti
-                 1462 to 1812 -> 1826 [2] lasti
-                 1814 to 1824 -> 2112 [0]
-                 1826 to 1834 -> 1836 [2] lasti
-                 1836 to 1912 -> 2112 [0]
-                 2112 to 2308 -> 2310 [1] lasti
+                 8 to 432 -> 1976 [0]
+                 436 to 762 -> 770 [1]
+                 764 to 768 -> 1976 [0]
+                 770 to 840 -> 1510 [2] lasti
+                 842 to 958 -> 972 [2] lasti
+                 960 to 970 -> 1976 [0]
+                 972 to 1016 -> 1510 [2] lasti
+                 1018 to 1070 -> 1084 [2] lasti
+                 1072 to 1082 -> 1976 [0]
+                 1084 to 1108 -> 1510 [2] lasti
+                 1110 to 1486 -> 1500 [2] lasti
+                 1488 to 1498 -> 1976 [0]
+                 1500 to 1508 -> 1510 [2] lasti
+                 1510 to 1626 -> 1976 [0]
+                 1976 to 2322 -> 2324 [1] lasti
                consts
                   'Converts given text to speech using Google Text-to-Speech API.'
-                  '\x1b[32m Conversion to mp3 sequence initialized startspeed \x1b[36m'
+                  'Get initial net speed..'
+                  ' Conversion to mp3 sequence initialized startspeed '
                   1000000
                   '.2f'
-                  'Mbps\x1b[0m'
+                  'Kbps'
                   0
                   '_'
                   '.ogg'
+                  1
                   'en'
                   False
                   ('text', 'lang', 'slow')
-                  code
-                     argcount  : 1
-                     nlocals   : 2
-                     stacksize : 5
-                     flags     : 51
-                     code
-                        0x4b00010097007c005d267d017401000000000000000000007c016400a6
-                        020000ab020000000000000000a001000000000000000000000000000000
-                        0000000000a6000000ab0000000000000000005600970101008c27640153
-                        00
-                     593           0 RETURN_GENERATOR
-                                   2 POP_TOP
-                                   4 RESUME                   0
-                                   6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                38 (to 86)
-                     
-                     594          10 STORE_FAST               1 (fname)
-                     
-                     593          12 LOAD_GLOBAL              1 (NULL + open)
-                                  24 LOAD_FAST                1 (fname)
-                                  26 LOAD_CONST               0 ('rb')
-                                  28 PRECALL                  2
-                                  32 CALL                     2
-                                  42 LOAD_METHOD              1 (read)
-                                  64 PRECALL                  0
-                                  68 CALL                     0
-                                  78 YIELD_VALUE
-                                  80 RESUME                   1
-                                  82 POP_TOP
-                                  84 JUMP_BACKWARD           39 (to 8)
-                             >>   86 LOAD_CONST               1 (None)
-                                  88 RETURN_VALUE
-                     consts
-                        'rb'
-                        None
-                     names      ('open', 'read')
-                     varnames   ('.0', 'fname')
-                     freevars   ()
-                     cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
-                     name       '<genexpr>'
-                     firstlineno 593
-                     lnotab 0x0a0102ff
-                  'mp3'
-                  ('format',)
-                  'chunk'
-                  '\x1b[32m Conversion successful! Output file: '
-                  '\x1b[0m'
-                  'Sorry boss we are sad to note the followingconnection issue arised: '
+                  'Sorry boss connection problem encountered: '
                   ' in '
-                  1
                   '/'
                   ':'
                   5
                   None
-                  '\x1b[31m Error during conversion attempt '
+                  ' Error during conversion attempt '
                   2
                   '\n'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code 0x970067007c005d077d0164007c019b009d0291028c085300
-                     622           0 RESUME                   0
+                     751           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 7 (to 22)
                      
-                     623           8 STORE_FAST               1 (line)
+                     752           8 STORE_FAST               1 (line)
                      
-                     622          10 LOAD_CONST               0 ('  > ')
+                     751          10 LOAD_CONST               0 ('  > ')
                                   12 LOAD_FAST                1 (line)
                                   14 FORMAT_VALUE             0
                                   16 BUILD_STRING             2
                                   18 LIST_APPEND              2
                                   20 JUMP_BACKWARD            8 (to 6)
                              >>   22 RETURN_VALUE
                      consts
                         '  > '
                      names      ()
                      varnames   ('.0', 'line')
                      freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 622
+                     firstlineno 751
                      lnotab 0x080102ff
                   3
                   'Conversion unsuccessful after '
-                  ' \x07ttempts.'
+                  ' attempts.'
                   'Done'
-                  '\x1b[33m Final Network Speed: '
-                  ' Mbps\x1b[0m'
-               names      ('os', 'path', 'exists', 'mkdir', 'speedtest', 'Speedtest', 'get_best_server', 'download', 'logger', 'info', 'range', 'len', 'CHUNK_SIZE', 'math', 'ceil', 'gTTS', 'save', 'sorted', 'listdir', 'join_audios', 'export', 'reversed', 'list', 'startswith', 'remove', 'join', 'Exception', 'ConnectionError', 'ConnectionAbortedError', 'ConnectionRefusedError', 'ConnectionResetError', 'error', 'time', 'sleep', 'requests', 'exceptions', 'RequestException', 'traceback', 'extract_tb', 'sys', 'exc_info', 'map', 'str')
-               varnames   ('self', 'text', 'output_file', 'ogg_folder', 'retries', 'st', 'download_speed', 'attempt', 'i', 'chunk', 'output_filename', 'tts', 'combined_files', 'combined_audio', 'fname', 'e', 'tb')
+                  'Get final speed ...'
+                  'Final Network Speed: '
+                  ' Kbps'
+               names      ('os', 'path', 'exists', 'mkdir', 'print', 'DYELLOW', 'RESET', 'speedtest', 'Speedtest', 'get_best_server', 'download', 'logger', 'info', 'GREEN', 'CYAN', 'range', 'len', 'gTTS', 'save', 'append', 'Exception', 'ConnectionError', 'ConnectionAbortedError', 'ConnectionRefusedError', 'ConnectionResetError', 'error', 'time', 'sleep', 'requests', 'exceptions', 'RequestException', 'DRED', 'traceback', 'extract_tb', 'sys', 'exc_info', 'join', 'map', 'str', 'exit', 'FileSynthesis', 'join_audios', 'YELLOW')
+               varnames   ('self', 'text', 'output_file', 'CHUNK_SIZE', 'ogg_folder', 'retries', 'out_ls', 'st', 'download_speed', 'attempt', 'counter', 'i', 'chunk', 'output_filename', 'tts', 'e', 'tb')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'Synthesise'
-               firstlineno 566
+               firstlineno 704
                lnotab
-                  0x020202013e0128022601280128012201020108ff08ff10042401020102
-                  024a0124017201120124012c034202100102ff20042e0360012a01660222
-                  01020102ff06ff100308034601240102ff040108ff040102ff16023c0326
-                  014a011201240108ff040102ff040102ff160256013e0128ff2e02280114
-                  f908090c0122010aff100426013401220136ff16fe26013401220136ff
+                  0x0202040102013e0128013c01260128012801220210010cff020108ff06
+                  010cff04fe1005240102010202040140011a0110010a023e01160224012a
+                  012c01080324010c010cfe0a034e013c0326014a011201320108ff040102
+                  ff040102ff02010cff140256013e0128ff2e02280114f908090c0122010a
+                  ff1002280526013602260134011e01220252fe16fa26013602260134011e
+                  01220252fe
             code
                argcount  : 1
                nlocals   : 7
-               stacksize : 6
+               stacksize : 11
                flags     : 3
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007400000000
-                  00000000000000a001000000000000000000000000000000000000000064
-                  02a6010000ab010000000000000000010009007405000000000000000000
-                  007c006403a6020000ab02000000000000000035007d0174070000000000
-                  00000000006a0400000000000000007c01a6010000ab0100000000000000
-                  007d0264047d03740b000000000000000000007c026a0600000000000000
-                  00a6010000ab01000000000000000044005d2e7d047c02a0070000000000
-                  0000000000000000000000000000007c04a6010000ab0100000000000000
-                  007d057c037c05a0080000000000000000000000000000000000000000a6
-                  000000ab0000000000000000007a0d00007d038c2f7c0363026400640064
-                  00a6020000ab020000000000000000010053002300310073047702780359
-                  007701010059000100010064005300230074120000000000000000000024
-                  0072297d06740000000000000000000000a00a0000000000000000000000
-                  00000000000000000064057c069b0064069d03a6010000ab010000000000
-                  0000000100590064007d067e066400530064007d067e0677017700780359
-                  007701
-               638           0 RESUME                   0
+                  00000000000000a001000000000000000000000000000000000000000074
+                  04000000000000000000009b0064027406000000000000000000009b009d
+                  03a6010000ab010000000000000000010009007409000000000000000000
+                  007c006403a6020000ab02000000000000000035007d01740b0000000000
+                  00000000006a0600000000000000007c01a6010000ab0100000000000000
+                  007d0264047d03740f000000000000000000007411000000000000000000
+                  007c026a090000000000000000a6010000ab010000000000000000a60100
+                  00ab01000000000000000044005d267d047c026a0900000000000000007c
+                  04190000000000000000007d057c037c05a00a0000000000000000000000
+                  000000000000000000a6000000ab0000000000000000007a0d00007d038c
+                  277417000000000000000000007418000000000000000000009b00640574
+                  06000000000000000000009b009d03a6010000ab01000000000000000001
+                  007c036302640064006400a6020000ab0200000000000000000100530023
+                  003100730477027803590077010100590001000100640053002300741a00
+                  000000000000000000240072417d06740000000000000000000000a00e00
+                  00000000000000000000000000000000000000741e000000000000000000
+                  009b0064067420000000000000000000009b007c009b0064077406000000
+                  000000000000009b0064087c069b009d08a6010000ab0100000000000000
+                  000100590064007d067e066400530064007d067e06770177007803590077
+                  01
+               774           0 RESUME                   0
                
-               639           2 LOAD_GLOBAL              0 (logger)
+               776           2 LOAD_GLOBAL              0 (logger)
                             14 LOAD_METHOD              1 (info)
                             36 LOAD_CONST               1 ('Processing the file...\n')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               640          54 LOAD_GLOBAL              0 (logger)
+               777          54 LOAD_GLOBAL              0 (logger)
                             66 LOAD_METHOD              1 (info)
                
-               641          88 LOAD_CONST               2 ('\x1b[32m Initializing pdf to text conversion sequence...\x1b[0m')
+               778          88 LOAD_GLOBAL              4 (GREEN)
+                           100 FORMAT_VALUE             0
+                           102 LOAD_CONST               2 (' Initializing pdf to text conversion sequence...')
+                           104 LOAD_GLOBAL              6 (RESET)
+                           116 FORMAT_VALUE             0
+                           118 BUILD_STRING             3
+               
+               777         120 PRECALL                  1
+                           124 CALL                     1
+                           134 POP_TOP
+               
+               779         136 NOP
+               
+               780         138 LOAD_GLOBAL              9 (NULL + open)
+                           150 LOAD_FAST                0 (pdf_path)
+                           152 LOAD_CONST               3 ('rb')
+                           154 PRECALL                  2
+                           158 CALL                     2
+                           168 BEFORE_WITH
+                           170 STORE_FAST               1 (file)
                
-               640          90 PRECALL                  1
-                            94 CALL                     1
-                           104 POP_TOP
-               
-               642         106 NOP
-               
-               643         108 LOAD_GLOBAL              5 (NULL + open)
-                           120 LOAD_FAST                0 (pdf_path)
-                           122 LOAD_CONST               3 ('rb')
-                           124 PRECALL                  2
-                           128 CALL                     2
-                           138 BEFORE_WITH
-                           140 STORE_FAST               1 (file)
-               
-               644         142 LOAD_GLOBAL              7 (NULL + PyPDF2)
-                           154 LOAD_ATTR                4 (PdfReader)
-                           164 LOAD_FAST                1 (file)
-                           166 PRECALL                  1
-                           170 CALL                     1
-                           180 STORE_FAST               2 (pdf_reader)
-               
-               645         182 LOAD_CONST               4 ('')
-                           184 STORE_FAST               3 (text)
-               
-               646         186 LOAD_GLOBAL             11 (NULL + range)
-                           198 LOAD_FAST                2 (pdf_reader)
-                           200 LOAD_ATTR                6 (numPages)
-                           210 PRECALL                  1
-                           214 CALL                     1
-                           224 GET_ITER
-                       >>  226 FOR_ITER                46 (to 320)
-                           228 STORE_FAST               4 (page_num)
-               
-               647         230 LOAD_FAST                2 (pdf_reader)
-                           232 LOAD_METHOD              7 (getPage)
-                           254 LOAD_FAST                4 (page_num)
-                           256 PRECALL                  1
-                           260 CALL                     1
-                           270 STORE_FAST               5 (page)
-               
-               648         272 LOAD_FAST                3 (text)
-                           274 LOAD_FAST                5 (page)
-                           276 LOAD_METHOD              8 (extractText)
-                           298 PRECALL                  0
-                           302 CALL                     0
-                           312 BINARY_OP               13 (+=)
-                           316 STORE_FAST               3 (text)
-                           318 JUMP_BACKWARD           47 (to 226)
-               
-               649     >>  320 LOAD_FAST                3 (text)
-               
-               643         322 SWAP                     2
-                           324 LOAD_CONST               0 (None)
-                           326 LOAD_CONST               0 (None)
-                           328 LOAD_CONST               0 (None)
-                           330 PRECALL                  2
-                           334 CALL                     2
-                           344 POP_TOP
-                           346 RETURN_VALUE
-                       >>  348 PUSH_EXC_INFO
-                           350 WITH_EXCEPT_START
-                           352 POP_JUMP_FORWARD_IF_TRUE     4 (to 362)
-                           354 RERAISE                  2
-                       >>  356 COPY                     3
-                           358 POP_EXCEPT
-                           360 RERAISE                  1
-                       >>  362 POP_TOP
-                           364 POP_EXCEPT
-                           366 POP_TOP
-                           368 POP_TOP
-                           370 LOAD_CONST               0 (None)
-                           372 RETURN_VALUE
-                       >>  374 PUSH_EXC_INFO
-               
-               650         376 LOAD_GLOBAL             18 (Exception)
-                           388 CHECK_EXC_MATCH
-                           390 POP_JUMP_FORWARD_IF_FALSE    41 (to 474)
-                           392 STORE_FAST               6 (e)
-               
-               651         394 LOAD_GLOBAL              0 (logger)
-                           406 LOAD_METHOD             10 (error)
-                           428 LOAD_CONST               5 ('\x1b[31m Something went wrong:')
-                           430 LOAD_FAST                6 (e)
-                           432 FORMAT_VALUE             0
-                           434 LOAD_CONST               6 ('\x1b[0m')
-                           436 BUILD_STRING             3
-                           438 PRECALL                  1
-                           442 CALL                     1
-                           452 POP_TOP
-                           454 POP_EXCEPT
-                           456 LOAD_CONST               0 (None)
-                           458 STORE_FAST               6 (e)
-                           460 DELETE_FAST              6 (e)
-                           462 LOAD_CONST               0 (None)
-                           464 RETURN_VALUE
-                       >>  466 LOAD_CONST               0 (None)
-                           468 STORE_FAST               6 (e)
-                           470 DELETE_FAST              6 (e)
-                           472 RERAISE                  1
-               
-               650     >>  474 RERAISE                  0
-                       >>  476 COPY                     3
-                           478 POP_EXCEPT
-                           480 RERAISE                  1
+               781         172 LOAD_GLOBAL             11 (NULL + PyPDF2)
+                           184 LOAD_ATTR                6 (PdfReader)
+                           194 LOAD_FAST                1 (file)
+                           196 PRECALL                  1
+                           200 CALL                     1
+                           210 STORE_FAST               2 (pdf_reader)
+               
+               782         212 LOAD_CONST               4 ('')
+                           214 STORE_FAST               3 (text)
+               
+               783         216 LOAD_GLOBAL             15 (NULL + range)
+                           228 LOAD_GLOBAL             17 (NULL + len)
+                           240 LOAD_FAST                2 (pdf_reader)
+                           242 LOAD_ATTR                9 (pages)
+                           252 PRECALL                  1
+                           256 CALL                     1
+                           266 PRECALL                  1
+                           270 CALL                     1
+                           280 GET_ITER
+                       >>  282 FOR_ITER                38 (to 360)
+                           284 STORE_FAST               4 (page_num)
+               
+               784         286 LOAD_FAST                2 (pdf_reader)
+                           288 LOAD_ATTR                9 (pages)
+                           298 LOAD_FAST                4 (page_num)
+                           300 BINARY_SUBSCR
+                           310 STORE_FAST               5 (page)
+               
+               785         312 LOAD_FAST                3 (text)
+                           314 LOAD_FAST                5 (page)
+                           316 LOAD_METHOD             10 (extract_text)
+                           338 PRECALL                  0
+                           342 CALL                     0
+                           352 BINARY_OP               13 (+=)
+                           356 STORE_FAST               3 (text)
+                           358 JUMP_BACKWARD           39 (to 282)
+               
+               786     >>  360 LOAD_GLOBAL             23 (NULL + print)
+                           372 LOAD_GLOBAL             24 (DGREEN)
+                           384 FORMAT_VALUE             0
+                           386 LOAD_CONST               5 ('Ok')
+                           388 LOAD_GLOBAL              6 (RESET)
+                           400 FORMAT_VALUE             0
+                           402 BUILD_STRING             3
+                           404 PRECALL                  1
+                           408 CALL                     1
+                           418 POP_TOP
+               
+               787         420 LOAD_FAST                3 (text)
+               
+               780         422 SWAP                     2
+                           424 LOAD_CONST               0 (None)
+                           426 LOAD_CONST               0 (None)
+                           428 LOAD_CONST               0 (None)
+                           430 PRECALL                  2
+                           434 CALL                     2
+                           444 POP_TOP
+                           446 RETURN_VALUE
+                       >>  448 PUSH_EXC_INFO
+                           450 WITH_EXCEPT_START
+                           452 POP_JUMP_FORWARD_IF_TRUE     4 (to 462)
+                           454 RERAISE                  2
+                       >>  456 COPY                     3
+                           458 POP_EXCEPT
+                           460 RERAISE                  1
+                       >>  462 POP_TOP
+                           464 POP_EXCEPT
+                           466 POP_TOP
+                           468 POP_TOP
+                           470 LOAD_CONST               0 (None)
+                           472 RETURN_VALUE
+                       >>  474 PUSH_EXC_INFO
+               
+               788         476 LOAD_GLOBAL             26 (Exception)
+                           488 CHECK_EXC_MATCH
+                           490 POP_JUMP_FORWARD_IF_FALSE    65 (to 622)
+                           492 STORE_FAST               6 (e)
+               
+               789         494 LOAD_GLOBAL              0 (logger)
+                           506 LOAD_METHOD             14 (error)
+               
+               790         528 LOAD_GLOBAL             30 (DRED)
+                           540 FORMAT_VALUE             0
+                           542 LOAD_CONST               6 ("Failed to extract text from '")
+                           544 LOAD_GLOBAL             32 (YELLOW)
+                           556 FORMAT_VALUE             0
+                           558 LOAD_FAST                0 (pdf_path)
+                           560 FORMAT_VALUE             0
+                           562 LOAD_CONST               7 ("'")
+                           564 LOAD_GLOBAL              6 (RESET)
+                           576 FORMAT_VALUE             0
+                           578 LOAD_CONST               8 (':\n ')
+                           580 LOAD_FAST                6 (e)
+                           582 FORMAT_VALUE             0
+                           584 BUILD_STRING             8
+               
+               789         586 PRECALL                  1
+                           590 CALL                     1
+                           600 POP_TOP
+                           602 POP_EXCEPT
+                           604 LOAD_CONST               0 (None)
+                           606 STORE_FAST               6 (e)
+                           608 DELETE_FAST              6 (e)
+                           610 LOAD_CONST               0 (None)
+                           612 RETURN_VALUE
+                       >>  614 LOAD_CONST               0 (None)
+                           616 STORE_FAST               6 (e)
+                           618 DELETE_FAST              6 (e)
+                           620 RERAISE                  1
+               
+               788     >>  622 RERAISE                  0
+                       >>  624 COPY                     3
+                           626 POP_EXCEPT
+                           628 RERAISE                  1
                ExceptionTable:
-                 108 to 138 -> 374 [0]
-                 140 to 320 -> 348 [1] lasti
-                 322 to 344 -> 374 [0]
-                 348 to 354 -> 356 [3] lasti
-                 356 to 360 -> 374 [0]
-                 362 to 362 -> 356 [3] lasti
-                 364 to 368 -> 374 [0]
-                 374 to 392 -> 476 [1] lasti
-                 394 to 452 -> 466 [1] lasti
-                 466 to 474 -> 476 [1] lasti
+                 138 to 168 -> 474 [0]
+                 170 to 420 -> 448 [1] lasti
+                 422 to 444 -> 474 [0]
+                 448 to 454 -> 456 [3] lasti
+                 456 to 460 -> 474 [0]
+                 462 to 462 -> 456 [3] lasti
+                 464 to 468 -> 474 [0]
+                 474 to 492 -> 624 [1] lasti
+                 494 to 600 -> 614 [1] lasti
+                 614 to 622 -> 624 [1] lasti
                consts
                   None
                   'Processing the file...\n'
-                  '\x1b[32m Initializing pdf to text conversion sequence...\x1b[0m'
+                  ' Initializing pdf to text conversion sequence...'
                   'rb'
                   ''
-                  '\x1b[31m Something went wrong:'
-                  '\x1b[0m'
-               names      ('logger', 'info', 'open', 'PyPDF2', 'PdfReader', 'range', 'numPages', 'getPage', 'extractText', 'Exception', 'error')
+                  'Ok'
+                  "Failed to extract text from '"
+                  "'"
+                  ':\n '
+               names      ('logger', 'info', 'GREEN', 'RESET', 'open', 'PyPDF2', 'PdfReader', 'range', 'len', 'pages', 'extract_text', 'print', 'DGREEN', 'Exception', 'error', 'DRED', 'YELLOW')
                varnames   ('pdf_path', 'file', 'pdf_reader', 'text', 'page_num', 'page', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'pdf_to_text'
-               firstlineno 638
+               firstlineno 774
                lnotab
-                  0x02013401220102ff100202012201280104012c012a01300102fa360712
-                  0150ff
+                  0x02023401220120ff1002020122012801040146011a0130013c0102f936
+                  08120122013aff24ff
             code
                argcount  : 1
-               nlocals   : 3
-               stacksize : 6
+               nlocals   : 4
+               stacksize : 10
                flags     : 3
                code
-                  0x97007401000000000000000000007c0064016402ac03a6030000ab0300
-                  0000000000000035007d017c01a001000000000000000000000000000000
-                  0000000000a6000000ab000000000000000000a002000000000000000000
-                  000000000000000000000064046405a6020000ab0200000000000000007d
-                  02640064006400a6020000ab02000000000000000001006e0b2300310073
-                  04770278035900770101005900010001007c025300
-               653           0 RESUME                   0
+                  0x970009007401000000000000000000007c0064016402ac03a6030000ab
+                  03000000000000000035007d017c01a00100000000000000000000000000
+                  00000000000000a6000000ab000000000000000000a00200000000000000
+                  0000000000000000000000000064046405a6020000ab0200000000000000
+                  007d02640064006400a6020000ab02000000000000000001006e0b230031
+                  007304770278035900770101005900010001007c02530023007406000000
+                  00000000000000240072310100740800000000000000000000a005000000
+                  00000000000000000000000000000000006406a006000000000000000000
+                  00000000000000000000007c00a6010000ab010000000000000000a60100
+                  00ab0100000000000000000100590064005300740e000000000000000000
+                  00240072467d03740800000000000000000000a005000000000000000000
+                  00000000000000000000007410000000000000000000009b0064077c009b
+                  0064087413000000000000000000007c03a6010000ab0100000000000000
+                  009b007414000000000000000000009b009d06a6010000ab010000000000
+                  0000000100590064007d037e036400530064007d037e0377017700780359
+                  007701
+               792           0 RESUME                   0
                
-               654           2 LOAD_GLOBAL              1 (NULL + open)
-                            14 LOAD_FAST                0 (input_file)
-                            16 LOAD_CONST               1 ('r')
-                            18 LOAD_CONST               2 ('ignore')
-                            20 KW_NAMES                 3
-                            22 PRECALL                  3
-                            26 CALL                     3
-                            36 BEFORE_WITH
-                            38 STORE_FAST               1 (file)
+               794           2 NOP
                
-               655          40 LOAD_FAST                1 (file)
-                            42 LOAD_METHOD              1 (read)
-                            64 PRECALL                  0
-                            68 CALL                     0
-                            78 LOAD_METHOD              2 (replace)
-                           100 LOAD_CONST               4 ('\n')
-                           102 LOAD_CONST               5 (' ')
-                           104 PRECALL                  2
-                           108 CALL                     2
-                           118 STORE_FAST               2 (text)
+               795           4 LOAD_GLOBAL              1 (NULL + open)
+                            16 LOAD_FAST                0 (input_file)
+                            18 LOAD_CONST               1 ('r')
+                            20 LOAD_CONST               2 ('ignore')
+                            22 KW_NAMES                 3
+                            24 PRECALL                  3
+                            28 CALL                     3
+                            38 BEFORE_WITH
+                            40 STORE_FAST               1 (file)
+               
+               796          42 LOAD_FAST                1 (file)
+                            44 LOAD_METHOD              1 (read)
+                            66 PRECALL                  0
+                            70 CALL                     0
+                            80 LOAD_METHOD              2 (replace)
+                           102 LOAD_CONST               4 ('\n')
+                           104 LOAD_CONST               5 (' ')
+                           106 PRECALL                  2
+                           110 CALL                     2
+                           120 STORE_FAST               2 (text)
                
-               654         120 LOAD_CONST               0 (None)
-                           122 LOAD_CONST               0 (None)
+               795         122 LOAD_CONST               0 (None)
                            124 LOAD_CONST               0 (None)
-                           126 PRECALL                  2
-                           130 CALL                     2
-                           140 POP_TOP
-                           142 JUMP_FORWARD            11 (to 166)
-                       >>  144 PUSH_EXC_INFO
-                           146 WITH_EXCEPT_START
-                           148 POP_JUMP_FORWARD_IF_TRUE     4 (to 158)
-                           150 RERAISE                  2
-                       >>  152 COPY                     3
-                           154 POP_EXCEPT
-                           156 RERAISE                  1
-                       >>  158 POP_TOP
-                           160 POP_EXCEPT
-                           162 POP_TOP
+                           126 LOAD_CONST               0 (None)
+                           128 PRECALL                  2
+                           132 CALL                     2
+                           142 POP_TOP
+                           144 JUMP_FORWARD            11 (to 168)
+                       >>  146 PUSH_EXC_INFO
+                           148 WITH_EXCEPT_START
+                           150 POP_JUMP_FORWARD_IF_TRUE     4 (to 160)
+                           152 RERAISE                  2
+                       >>  154 COPY                     3
+                           156 POP_EXCEPT
+                           158 RERAISE                  1
+                       >>  160 POP_TOP
+                           162 POP_EXCEPT
                            164 POP_TOP
+                           166 POP_TOP
+               
+               797     >>  168 LOAD_FAST                2 (text)
+                           170 RETURN_VALUE
+                       >>  172 PUSH_EXC_INFO
+               
+               798         174 LOAD_GLOBAL              6 (FileNotFoundError)
+                           186 CHECK_EXC_MATCH
+                           188 POP_JUMP_FORWARD_IF_FALSE    49 (to 288)
+                           190 POP_TOP
+               
+               799         192 LOAD_GLOBAL              8 (logger)
+                           204 LOAD_METHOD              5 (error)
+                           226 LOAD_CONST               6 ("File '{}' was not found.")
+                           228 LOAD_METHOD              6 (format)
+                           250 LOAD_FAST                0 (input_file)
+                           252 PRECALL                  1
+                           256 CALL                     1
+                           266 PRECALL                  1
+                           270 CALL                     1
+                           280 POP_TOP
+                           282 POP_EXCEPT
+                           284 LOAD_CONST               0 (None)
+                           286 RETURN_VALUE
+               
+               800     >>  288 LOAD_GLOBAL             14 (Exception)
+                           300 CHECK_EXC_MATCH
+                           302 POP_JUMP_FORWARD_IF_FALSE    70 (to 444)
+                           304 STORE_FAST               3 (e)
+               
+               801         306 LOAD_GLOBAL              8 (logger)
+                           318 LOAD_METHOD              5 (error)
+               
+               802         340 LOAD_GLOBAL             16 (DRED)
+                           352 FORMAT_VALUE             0
+                           354 LOAD_CONST               7 ('Error converting ')
+                           356 LOAD_FAST                0 (input_file)
+                           358 FORMAT_VALUE             0
+                           360 LOAD_CONST               8 (' to text: ')
+                           362 LOAD_GLOBAL             19 (NULL + str)
+                           374 LOAD_FAST                3 (e)
+                           376 PRECALL                  1
+                           380 CALL                     1
+                           390 FORMAT_VALUE             0
+               
+               803         392 LOAD_GLOBAL             20 (RESET)
                
-               656     >>  166 LOAD_FAST                2 (text)
-                           168 RETURN_VALUE
+               802         404 FORMAT_VALUE             0
+                           406 BUILD_STRING             6
+               
+               801         408 PRECALL                  1
+                           412 CALL                     1
+                           422 POP_TOP
+                           424 POP_EXCEPT
+                           426 LOAD_CONST               0 (None)
+                           428 STORE_FAST               3 (e)
+                           430 DELETE_FAST              3 (e)
+                           432 LOAD_CONST               0 (None)
+                           434 RETURN_VALUE
+                       >>  436 LOAD_CONST               0 (None)
+                           438 STORE_FAST               3 (e)
+                           440 DELETE_FAST              3 (e)
+                           442 RERAISE                  1
+               
+               800     >>  444 RERAISE                  0
+                       >>  446 COPY                     3
+                           448 POP_EXCEPT
+                           450 RERAISE                  1
                ExceptionTable:
-                 38 to 118 -> 144 [1] lasti
-                 144 to 150 -> 152 [3] lasti
-                 158 to 158 -> 152 [3] lasti
+                 4 to 38 -> 172 [0]
+                 40 to 120 -> 146 [1] lasti
+                 122 to 144 -> 172 [0]
+                 146 to 152 -> 154 [3] lasti
+                 154 to 158 -> 172 [0]
+                 160 to 160 -> 154 [3] lasti
+                 162 to 168 -> 172 [0]
+                 172 to 280 -> 446 [1] lasti
+                 288 to 304 -> 446 [1] lasti
+                 306 to 422 -> 436 [1] lasti
+                 436 to 444 -> 446 [1] lasti
                consts
                   None
                   'r'
                   'ignore'
                   ('errors',)
                   '\n'
                   ' '
-               names      ('open', 'read', 'replace')
-               varnames   ('input_file', 'file', 'text')
+                  "File '{}' was not found."
+                  'Error converting '
+                  ' to text: '
+               names      ('open', 'read', 'replace', 'FileNotFoundError', 'logger', 'error', 'format', 'Exception', 'DRED', 'str', 'RESET')
+               varnames   ('input_file', 'file', 'text', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'text_file'
-               firstlineno 653
-               lnotab 0x0201260150ff2e02
+               firstlineno 792
+               lnotab 0x02020201260150ff2e020601120160011201220134010cff04ff24ff
             code
                argcount  : 1
                nlocals   : 4
-               stacksize : 6
+               stacksize : 9
                flags     : 3
                code
                   0x97000900740000000000000000000000a0010000000000000000000000
-                  00000000000000000064017c009b0064029d03a6010000ab010000000000
-                  00000001007405000000000000000000007c00a6010000ab010000000000
-                  0000007d01640384007c016a0300000000000000004400a6000000ab0000
-                  000000000000007d026404a0040000000000000000000000000000000000
-                  0000007c02a6010000ab01000000000000000053002300740a0000000000
-                  0000000000240072297d03740000000000000000000000a0060000000000
-                  00000000000000000000000000000064057c039b0064069d03a6010000ab
-                  0100000000000000000100590064007d037e036400530064007d037e0377
-                  017700780359007701
-               658           0 RESUME                   0
+                  0000000000000000007404000000000000000000009b0064017c009b0064
+                  027406000000000000000000009b009d05a6010000ab0100000000000000
+                  0001007409000000000000000000007c00a6010000ab0100000000000000
+                  007d01640384007c016a0500000000000000004400a6000000ab00000000
+                  00000000007d026404a00600000000000000000000000000000000000000
+                  007c02a6010000ab01000000000000000053002300740e00000000000000
+                  000000240072220100740000000000000000000000a00800000000000000
+                  0000000000000000000000000064057c009b0064069d03a6010000ab0100
+                  000000000000000100590064005300741200000000000000000000240072
+                  397d03740000000000000000000000a00800000000000000000000000000
+                  000000000000007414000000000000000000009b0064077c009b0064087c
+                  039b007406000000000000000000009b009d06a6010000ab010000000000
+                  0000000100590064007d037e036400530064007d037e0377017700780359
+                  007701
+               805           0 RESUME                   0
                
-               659           2 NOP
+               807           2 NOP
                
-               660           4 LOAD_GLOBAL              0 (logger)
+               808           4 LOAD_GLOBAL              0 (logger)
                             16 LOAD_METHOD              1 (info)
-                            38 LOAD_CONST               1 ('\x1b[34m Converting ')
-                            40 LOAD_FAST                0 (docx_path)
-                            42 FORMAT_VALUE             0
-                            44 LOAD_CONST               2 (' to text...\x1b[0m')
-                            46 BUILD_STRING             3
-                            48 PRECALL                  1
-                            52 CALL                     1
-                            62 POP_TOP
-               
-               661          64 LOAD_GLOBAL              5 (NULL + Document)
-                            76 LOAD_FAST                0 (docx_path)
-                            78 PRECALL                  1
-                            82 CALL                     1
-                            92 STORE_FAST               1 (doc)
+                            38 LOAD_GLOBAL              4 (BLUE)
+                            50 FORMAT_VALUE             0
+                            52 LOAD_CONST               1 (' Converting ')
+                            54 LOAD_FAST                0 (docx_path)
+                            56 FORMAT_VALUE             0
+                            58 LOAD_CONST               2 (' to text...')
+                            60 LOAD_GLOBAL              6 (RESET)
+                            72 FORMAT_VALUE             0
+                            74 BUILD_STRING             5
+                            76 PRECALL                  1
+                            80 CALL                     1
+                            90 POP_TOP
+               
+               809          92 LOAD_GLOBAL              9 (NULL + Document)
+                           104 LOAD_FAST                0 (docx_path)
+                           106 PRECALL                  1
+                           110 CALL                     1
+                           120 STORE_FAST               1 (doc)
+               
+               810         122 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 810>)
+                           124 MAKE_FUNCTION            0
+                           126 LOAD_FAST                1 (doc)
+                           128 LOAD_ATTR                5 (paragraphs)
+                           138 GET_ITER
+                           140 PRECALL                  0
+                           144 CALL                     0
+                           154 STORE_FAST               2 (paragraphs)
+               
+               811         156 LOAD_CONST               4 ('\n')
+                           158 LOAD_METHOD              6 (join)
+                           180 LOAD_FAST                2 (paragraphs)
+                           182 PRECALL                  1
+                           186 CALL                     1
+                           196 RETURN_VALUE
+                       >>  198 PUSH_EXC_INFO
                
-               662          94 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 662>)
-                            96 MAKE_FUNCTION            0
-                            98 LOAD_FAST                1 (doc)
-                           100 LOAD_ATTR                3 (paragraphs)
-                           110 GET_ITER
-                           112 PRECALL                  0
-                           116 CALL                     0
-                           126 STORE_FAST               2 (paragraphs)
-               
-               663         128 LOAD_CONST               4 ('\n')
-                           130 LOAD_METHOD              4 (join)
-                           152 LOAD_FAST                2 (paragraphs)
-                           154 PRECALL                  1
-                           158 CALL                     1
-                           168 RETURN_VALUE
-                       >>  170 PUSH_EXC_INFO
+               812         200 LOAD_GLOBAL             14 (FileNotFoundError)
+                           212 CHECK_EXC_MATCH
+                           214 POP_JUMP_FORWARD_IF_FALSE    34 (to 284)
+                           216 POP_TOP
+               
+               813         218 LOAD_GLOBAL              0 (logger)
+                           230 LOAD_METHOD              8 (error)
+                           252 LOAD_CONST               5 ("File '")
+                           254 LOAD_FAST                0 (docx_path)
+                           256 FORMAT_VALUE             0
+                           258 LOAD_CONST               6 ("' was not found.")
+                           260 BUILD_STRING             3
+                           262 PRECALL                  1
+                           266 CALL                     1
+                           276 POP_TOP
+                           278 POP_EXCEPT
+                           280 LOAD_CONST               0 (None)
+                           282 RETURN_VALUE
+               
+               814     >>  284 LOAD_GLOBAL             18 (Exception)
+                           296 CHECK_EXC_MATCH
+                           298 POP_JUMP_FORWARD_IF_FALSE    57 (to 414)
+                           300 STORE_FAST               3 (e)
+               
+               815         302 LOAD_GLOBAL              0 (logger)
+                           314 LOAD_METHOD              8 (error)
+               
+               816         336 LOAD_GLOBAL             20 (DRED)
+                           348 FORMAT_VALUE             0
+                           350 LOAD_CONST               7 ('Error converting ')
+                           352 LOAD_FAST                0 (docx_path)
+                           354 FORMAT_VALUE             0
+                           356 LOAD_CONST               8 (' to text: ')
+                           358 LOAD_FAST                3 (e)
+                           360 FORMAT_VALUE             0
                
-               664         172 LOAD_GLOBAL             10 (Exception)
-                           184 CHECK_EXC_MATCH
-                           186 POP_JUMP_FORWARD_IF_FALSE    41 (to 270)
-                           188 STORE_FAST               3 (e)
-               
-               665         190 LOAD_GLOBAL              0 (logger)
-                           202 LOAD_METHOD              6 (error)
-               
-               666         224 LOAD_CONST               5 ('\x1b[31m Something went wrong in docx_to_text():')
-                           226 LOAD_FAST                3 (e)
-                           228 FORMAT_VALUE             0
-                           230 LOAD_CONST               6 ('\x1b[0m')
-                           232 BUILD_STRING             3
-               
-               665         234 PRECALL                  1
-                           238 CALL                     1
-                           248 POP_TOP
-                           250 POP_EXCEPT
-                           252 LOAD_CONST               0 (None)
-                           254 STORE_FAST               3 (e)
-                           256 DELETE_FAST              3 (e)
-                           258 LOAD_CONST               0 (None)
-                           260 RETURN_VALUE
-                       >>  262 LOAD_CONST               0 (None)
-                           264 STORE_FAST               3 (e)
-                           266 DELETE_FAST              3 (e)
-                           268 RERAISE                  1
-               
-               664     >>  270 RERAISE                  0
-                       >>  272 COPY                     3
-                           274 POP_EXCEPT
-                           276 RERAISE                  1
+               817         362 LOAD_GLOBAL              6 (RESET)
+               
+               816         374 FORMAT_VALUE             0
+                           376 BUILD_STRING             6
+               
+               815         378 PRECALL                  1
+                           382 CALL                     1
+                           392 POP_TOP
+                           394 POP_EXCEPT
+                           396 LOAD_CONST               0 (None)
+                           398 STORE_FAST               3 (e)
+                           400 DELETE_FAST              3 (e)
+                           402 LOAD_CONST               0 (None)
+                           404 RETURN_VALUE
+                       >>  406 LOAD_CONST               0 (None)
+                           408 STORE_FAST               3 (e)
+                           410 DELETE_FAST              3 (e)
+                           412 RERAISE                  1
+               
+               814     >>  414 RERAISE                  0
+                       >>  416 COPY                     3
+                           418 POP_EXCEPT
+                           420 RERAISE                  1
                ExceptionTable:
-                 4 to 166 -> 170 [0]
-                 170 to 188 -> 272 [1] lasti
-                 190 to 248 -> 262 [1] lasti
-                 262 to 270 -> 272 [1] lasti
+                 4 to 194 -> 198 [0]
+                 198 to 276 -> 416 [1] lasti
+                 284 to 300 -> 416 [1] lasti
+                 302 to 392 -> 406 [1] lasti
+                 406 to 414 -> 416 [1] lasti
                consts
                   None
-                  '\x1b[34m Converting '
-                  ' to text...\x1b[0m'
+                  ' Converting '
+                  ' to text...'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     662           0 RESUME                   0
+                     810           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (paragraph)
                                   10 LOAD_FAST                1 (paragraph)
                                   12 LOAD_ATTR                0 (text)
                                   22 LIST_APPEND              2
                                   24 JUMP_BACKWARD           10 (to 6)
                              >>   26 RETURN_VALUE
                      consts
                      names      ('text',)
                      varnames   ('.0', 'paragraph')
                      freevars   ()
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 662
+                     firstlineno 810
                      lnotab 0x
                   '\n'
-                  '\x1b[31m Something went wrong in docx_to_text():'
-                  '\x1b[0m'
-               names      ('logger', 'info', 'Document', 'paragraphs', 'join', 'Exception', 'error')
+                  "File '"
+                  "' was not found."
+                  'Error converting '
+                  ' to text: '
+               names      ('logger', 'info', 'BLUE', 'RESET', 'Document', 'paragraphs', 'join', 'FileNotFoundError', 'error', 'Exception', 'DRED')
                varnames   ('docx_path', 'doc', 'paragraphs', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'docx_to_text'
-               firstlineno 658
-               lnotab 0x020102013c011e0122012c01120122010aff24ff
+               firstlineno 805
+               lnotab 0x0202020158011e0122012c0112014201120122011a010cff04ff24ff
             code
                argcount  : 1
                nlocals   : 6
-               stacksize : 10
+               stacksize : 6
                flags     : 3
                code
                   0x870697007c00a0000000000000000000000000000000000000000000a6
-                  000000ab0000000000000000007d0168006401a3018a0688066601640284
-                  087c014400a6000000ab0000000000000000007d017c01440090035d397d
-                  0209007c02a00100000000000000000000000000000000000000006403a6
-                  010000ab010000000000000000728e09007405000000000000000000007c
-                  02a6010000ab0100000000000000007d037c026400640485021900000000
-                  00000000007d0490026e9423007406000000000000000000002400726501
-                  00740800000000000000000000a005000000000000000000000000000000
-                  00000000006405a00600000000000000000000000000000000000000007c
-                  02a6010000ab010000000000000000a6010000ab01000000000000000001
-                  0059000900740f000000000000000000007c037c04a6020000ab02000000
-                  000000000001008c7f230074100000000000000000000024007217010074
-                  13000000000000000000006a0a00000000000000006406a6010000ab0100
-                  00000000000000010059008c9f770078035900770177007803590077017c
-                  02a00b0000000000000000000000000000000000000000a6000000ab0000
-                  00000000000000a001000000000000000000000000000000000000000064
-                  07a6010000ab01000000000000000073277c02a00b000000000000000000
-                  0000000000000000000000a6000000ab000000000000000000a001000000
-                  00000000000000000000000000000000006408a6010000ab010000000000
-                  00000072dd09007419000000000000000000007c02a6010000ab01000000
-                  00000000007d037c02640064098502190000000000000000007d0490016e
-                  b82300740600000000000000000000240072670100740800000000000000
-                  000000a00500000000000000000000000000000000000000006405a00600
-                  000000000000000000000000000000000000007c02a6010000ab01000000
-                  0000000000a6010000ab010000000000000000010059000900740f000000
-                  000000000000007c037c04a6020000ab020000000000000000010090018c
-                  5c2300741000000000000000000000240072180100741300000000000000
-                  0000006a0a00000000000000006406a6010000ab01000000000000000001
-                  00590090018c7d7700780359007701741a00000000000000000000240072
-                  457d05740800000000000000000000a00e00000000000000000000000000
-                  00000000000000640aa00600000000000000000000000000000000000000
-                  007c02741f000000000000000000007c05a6010000ab0100000000000000
-                  00a6020000ab020000000000000000a6010000ab01000000000000000001
-                  00590064007d057e056eff64007d057e05770177007803590077017c02a0
-                  010000000000000000000000000000000000000000640ba6010000ab0100
-                  00000000000000728f09007421000000000000000000007c02a6010000ab
-                  0100000000000000007d037c02640064048502190000000000000000007d
-                  046ec7230074060000000000000000000024007267010074080000000000
-                  0000000000a00500000000000000000000000000000000000000006405a0
-                  0600000000000000000000000000000000000000007c02a6010000ab0100
-                  00000000000000a6010000ab010000000000000000010059000900740f00
-                  0000000000000000007c037c04a6020000ab020000000000000000010090
-                  028c4d230074100000000000000000000024007218010074130000000000
-                  00000000006a0a00000000000000006406a6010000ab0100000000000000
-                  000100590090028c6e770078035900770177007803590077017408000000
-                  00000000000000a005000000000000000000000000000000000000000064
-                  0ca6010000ab010000000000000000010009000900740f00000000000000
-                  0000007c037c04a6020000ab020000000000000000010090028ca4230074
-                  10000000000000000000002400721801007413000000000000000000006a
-                  0a00000000000000006406a6010000ab0100000000000000000100590090
-                  028cc577007803590077010900740f000000000000000000007c037c04a6
-                  020000ab020000000000000000010090028cdc2300741000000000000000
-                  0000002400721801007413000000000000000000006a0a00000000000000
-                  006406a6010000ab0100000000000000000100590090028cfd7700780359
-                  00770123000900740f000000000000000000007c037c04a6020000ab0200
-                  000000000000000100770023007410000000000000000000002400721701
-                  007413000000000000000000006a0a00000000000000006406a6010000ab
-                  010000000000000000010059007700770078035900770178035900770164
-                  005300
+                  000000ab0000000000000000007d016401640267027d0268006403a3018a
+                  0688066601640484087c014400a6000000ab0000000000000000007d017c
+                  01440090015d407d037c03a0010000000000000000000000000000000000
+                  0000006405a6010000ab0100000000000000007225740400000000000000
+                  000000a00300000000000000000000000000000000000000007c03a60100
+                  00ab0100000000000000007d047c03640064068502190000000000000000
+                  007d056ec17c03a0040000000000000000000000000000000000000000a6
+                  000000ab000000000000000000a001000000000000000000000000000000
+                  0000000000740b000000000000000000007c02a6010000ab010000000000
+                  000000a6010000ab01000000000000000072257404000000000000000000
+                  00a00600000000000000000000000000000000000000007c03a6010000ab
+                  0100000000000000007d047c03640064078502190000000000000000007d
+                  056e687c03a00100000000000000000000000000000000000000006408a6
+                  010000ab0100000000000000007225740400000000000000000000a00700
+                  000000000000000000000000000000000000007c03a6010000ab01000000
+                  00000000007d047c03640064068502190000000000000000007d056e2e74
+                  1000000000000000000000a0090000000000000000000000000000000000
+                  0000006409a6010000ab0100000000000000000100741500000000000000
+                  0000006a0b0000000000000000640aa6010000ab01000000000000000001
+                  000900740400000000000000000000a00c00000000000000000000000000
+                  0000000000000064007c047c05a6030000ab030000000000000000010090
+                  018c1d2300741a0000000000000000000024007218010074150000000000
+                  00000000006a0b0000000000000000640aa6010000ab0100000000000000
+                  000100590090018c3e770078035900770164005300
                              0 MAKE_CELL                6 (ls)
                
-               670           2 RESUME                   0
+               821           2 RESUME                   0
                
-               671           4 LOAD_FAST                0 (self)
+               822           4 LOAD_FAST                0 (self)
                              6 LOAD_METHOD              0 (preprocess)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 STORE_FAST               1 (input_list)
                
-               672          44 BUILD_SET                0
-                            46 LOAD_CONST               1 (frozenset({'docx', 'txt', 'doc', 'pdf'}))
-                            48 SET_UPDATE               1
-                            50 STORE_DEREF              6 (ls)
-               
-               673          52 LOAD_CLOSURE             6 (ls)
-                            54 BUILD_TUPLE              1
-                            56 LOAD_CONST               2 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 673>)
-                            58 MAKE_FUNCTION            8 (closure)
-                            60 LOAD_FAST                1 (input_list)
-                            62 GET_ITER
-                            64 PRECALL                  0
-                            68 CALL                     0
-                            78 STORE_FAST               1 (input_list)
-               
-               674          80 LOAD_FAST                1 (input_list)
-                            82 GET_ITER
-                       >>   84 EXTENDED_ARG             3
-                            86 FOR_ITER               825 (to 1738)
-                            88 STORE_FAST               2 (input_file)
-               
-               675          90 NOP
-               
-               676          92 LOAD_FAST                2 (input_file)
-                            94 LOAD_METHOD              1 (endswith)
-                           116 LOAD_CONST               3 ('.pdf')
-                           118 PRECALL                  1
-                           122 CALL                     1
-                           132 POP_JUMP_FORWARD_IF_FALSE   142 (to 418)
-               
-               677         134 NOP
-               
-               678         136 LOAD_GLOBAL              5 (NULL + pdf_to_text)
-                           148 LOAD_FAST                2 (input_file)
-                           150 PRECALL                  1
-                           154 CALL                     1
-                           164 STORE_FAST               3 (text)
-               
-               679         166 LOAD_FAST                2 (input_file)
-                           168 LOAD_CONST               0 (None)
-                           170 LOAD_CONST               4 (-4)
-                           172 BUILD_SLICE              2
-                           174 BINARY_SUBSCR
-                           184 STORE_FAST               4 (output_file)
-                           186 EXTENDED_ARG             2
-                           188 JUMP_FORWARD           660 (to 1510)
-                       >>  190 PUSH_EXC_INFO
-               
-               680         192 LOAD_GLOBAL              6 (FileNotFoundError)
-                           204 CHECK_EXC_MATCH
-                           206 POP_JUMP_FORWARD_IF_FALSE   101 (to 410)
-                           208 POP_TOP
-               
-               681         210 LOAD_GLOBAL              8 (logger)
-                           222 LOAD_METHOD              5 (error)
-               
-               682         244 LOAD_CONST               5 ("File '{}' was not found.")
-                           246 LOAD_METHOD              6 (format)
-                           268 LOAD_FAST                2 (input_file)
-                           270 PRECALL                  1
-                           274 CALL                     1
-               
-               681         284 PRECALL                  1
-                           288 CALL                     1
-                           298 POP_TOP
-               
-               683         300 POP_EXCEPT
-               
-               712         302 NOP
-               
-               713         304 LOAD_GLOBAL             15 (NULL + Synthesise)
-                           316 LOAD_FAST                3 (text)
-                           318 LOAD_FAST                4 (output_file)
-                           320 PRECALL                  2
-                           324 CALL                     2
-                           334 POP_TOP
-                           336 JUMP_BACKWARD          127 (to 84)
-                       >>  338 PUSH_EXC_INFO
-               
-               714         340 LOAD_GLOBAL             16 (KeyboardInterrupt)
-                           352 CHECK_EXC_MATCH
-                           354 POP_JUMP_FORWARD_IF_FALSE    23 (to 402)
-                           356 POP_TOP
-               
-               715         358 LOAD_GLOBAL             19 (NULL + sys)
-                           370 LOAD_ATTR               10 (exit)
-                           380 LOAD_CONST               6 (1)
-                           382 PRECALL                  1
-                           386 CALL                     1
-                           396 POP_TOP
-                           398 POP_EXCEPT
-                           400 JUMP_BACKWARD          159 (to 84)
-               
-               714     >>  402 RERAISE                  0
-                       >>  404 COPY                     3
-                           406 POP_EXCEPT
-                           408 RERAISE                  1
-               
-               680     >>  410 RERAISE                  0
-                       >>  412 COPY                     3
-                           414 POP_EXCEPT
-                           416 RERAISE                  1
-               
-               685     >>  418 LOAD_FAST                2 (input_file)
-                           420 LOAD_METHOD             11 (lower)
-                           442 PRECALL                  0
-                           446 CALL                     0
-                           456 LOAD_METHOD              1 (endswith)
-                           478 LOAD_CONST               7 ('.docx')
-                           480 PRECALL                  1
-                           484 CALL                     1
-                           494 POP_JUMP_FORWARD_IF_TRUE    39 (to 574)
-                           496 LOAD_FAST                2 (input_file)
-                           498 LOAD_METHOD             11 (lower)
-                           520 PRECALL                  0
-                           524 CALL                     0
-                           534 LOAD_METHOD              1 (endswith)
-                           556 LOAD_CONST               8 ('.doc')
-                           558 PRECALL                  1
-                           562 CALL                     1
-                           572 POP_JUMP_FORWARD_IF_FALSE   221 (to 1016)
-               
-               686     >>  574 NOP
-               
-               687         576 LOAD_GLOBAL             25 (NULL + docx_to_text)
-                           588 LOAD_FAST                2 (input_file)
-                           590 PRECALL                  1
-                           594 CALL                     1
-                           604 STORE_FAST               3 (text)
-               
-               688         606 LOAD_FAST                2 (input_file)
-                           608 LOAD_CONST               0 (None)
-                           610 LOAD_CONST               9 (-5)
-                           612 BUILD_SLICE              2
-                           614 BINARY_SUBSCR
-                           624 STORE_FAST               4 (output_file)
-                           626 EXTENDED_ARG             1
-                           628 JUMP_FORWARD           440 (to 1510)
-                       >>  630 PUSH_EXC_INFO
-               
-               689         632 LOAD_GLOBAL              6 (FileNotFoundError)
-                           644 CHECK_EXC_MATCH
-                           646 POP_JUMP_FORWARD_IF_FALSE   103 (to 854)
-                           648 POP_TOP
-               
-               690         650 LOAD_GLOBAL              8 (logger)
-                           662 LOAD_METHOD              5 (error)
-               
-               691         684 LOAD_CONST               5 ("File '{}' was not found.")
-                           686 LOAD_METHOD              6 (format)
-                           708 LOAD_FAST                2 (input_file)
-                           710 PRECALL                  1
-                           714 CALL                     1
-               
-               690         724 PRECALL                  1
-                           728 CALL                     1
-                           738 POP_TOP
-               
-               692         740 POP_EXCEPT
-               
-               712         742 NOP
+               823          44 LOAD_CONST               1 ('docx')
+                            46 LOAD_CONST               2 ('doc')
+                            48 BUILD_LIST               2
+                            50 STORE_FAST               2 (extdoc)
                
-               713         744 LOAD_GLOBAL             15 (NULL + Synthesise)
-                           756 LOAD_FAST                3 (text)
-                           758 LOAD_FAST                4 (output_file)
-                           760 PRECALL                  2
-                           764 CALL                     2
-                           774 POP_TOP
-                           776 EXTENDED_ARG             1
-                           778 JUMP_BACKWARD          348 (to 84)
-                       >>  780 PUSH_EXC_INFO
-               
-               714         782 LOAD_GLOBAL             16 (KeyboardInterrupt)
-                           794 CHECK_EXC_MATCH
-                           796 POP_JUMP_FORWARD_IF_FALSE    24 (to 846)
-                           798 POP_TOP
+               824          52 BUILD_SET                0
+                            54 LOAD_CONST               3 (frozenset({'docx', 'txt', 'doc', 'pdf'}))
+                            56 SET_UPDATE               1
+                            58 STORE_DEREF              6 (ls)
+               
+               825          60 LOAD_CLOSURE             6 (ls)
+                            62 BUILD_TUPLE              1
+                            64 LOAD_CONST               4 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 825>)
+                            66 MAKE_FUNCTION            8 (closure)
+                            68 LOAD_FAST                1 (input_list)
+                            70 GET_ITER
+                            72 PRECALL                  0
+                            76 CALL                     0
+                            86 STORE_FAST               1 (input_list)
+               
+               826          88 LOAD_FAST                1 (input_list)
+                            90 GET_ITER
+                       >>   92 EXTENDED_ARG             1
+                            94 FOR_ITER               320 (to 736)
+                            96 STORE_FAST               3 (input_file)
+               
+               827          98 LOAD_FAST                3 (input_file)
+                           100 LOAD_METHOD              1 (endswith)
+                           122 LOAD_CONST               5 ('.pdf')
+                           124 PRECALL                  1
+                           128 CALL                     1
+                           138 POP_JUMP_FORWARD_IF_FALSE    37 (to 214)
+               
+               828         140 LOAD_GLOBAL              4 (FileSynthesis)
+                           152 LOAD_METHOD              3 (pdf_to_text)
+                           174 LOAD_FAST                3 (input_file)
+                           176 PRECALL                  1
+                           180 CALL                     1
+                           190 STORE_FAST               4 (text)
+               
+               829         192 LOAD_FAST                3 (input_file)
+                           194 LOAD_CONST               0 (None)
+                           196 LOAD_CONST               6 (-4)
+                           198 BUILD_SLICE              2
+                           200 BINARY_SUBSCR
+                           210 STORE_FAST               5 (output_file)
+                           212 JUMP_FORWARD           193 (to 600)
+               
+               831     >>  214 LOAD_FAST                3 (input_file)
+                           216 LOAD_METHOD              4 (lower)
+                           238 PRECALL                  0
+                           242 CALL                     0
+                           252 LOAD_METHOD              1 (endswith)
+                           274 LOAD_GLOBAL             11 (NULL + tuple)
+                           286 LOAD_FAST                2 (extdoc)
+                           288 PRECALL                  1
+                           292 CALL                     1
+                           302 PRECALL                  1
+                           306 CALL                     1
+                           316 POP_JUMP_FORWARD_IF_FALSE    37 (to 392)
                
-               715         800 LOAD_GLOBAL             19 (NULL + sys)
-                           812 LOAD_ATTR               10 (exit)
-                           822 LOAD_CONST               6 (1)
-                           824 PRECALL                  1
-                           828 CALL                     1
-                           838 POP_TOP
-                           840 POP_EXCEPT
-                           842 EXTENDED_ARG             1
-                           844 JUMP_BACKWARD          381 (to 84)
+               833         318 LOAD_GLOBAL              4 (FileSynthesis)
+                           330 LOAD_METHOD              6 (docx_to_text)
+                           352 LOAD_FAST                3 (input_file)
+                           354 PRECALL                  1
+                           358 CALL                     1
+                           368 STORE_FAST               4 (text)
                
-               714     >>  846 RERAISE                  0
-                       >>  848 COPY                     3
-                           850 POP_EXCEPT
-                           852 RERAISE                  1
+               834         370 LOAD_FAST                3 (input_file)
+                           372 LOAD_CONST               0 (None)
+                           374 LOAD_CONST               7 (-5)
+                           376 BUILD_SLICE              2
+                           378 BINARY_SUBSCR
+                           388 STORE_FAST               5 (output_file)
+                           390 JUMP_FORWARD           104 (to 600)
+               
+               836     >>  392 LOAD_FAST                3 (input_file)
+                           394 LOAD_METHOD              1 (endswith)
+                           416 LOAD_CONST               8 ('.txt')
+                           418 PRECALL                  1
+                           422 CALL                     1
+                           432 POP_JUMP_FORWARD_IF_FALSE    37 (to 508)
                
-               694     >>  854 LOAD_GLOBAL             26 (Exception)
-                           866 CHECK_EXC_MATCH
-                           868 POP_JUMP_FORWARD_IF_FALSE    69 (to 1008)
-                           870 STORE_FAST               5 (e)
-               
-               695         872 LOAD_GLOBAL              8 (logger)
-                           884 LOAD_METHOD             14 (exception)
-                           906 LOAD_CONST              10 ('Error converting {} to text: {}')
-               
-               696         908 LOAD_METHOD              6 (format)
-                           930 LOAD_FAST                2 (input_file)
-                           932 LOAD_GLOBAL             31 (NULL + str)
-                           944 LOAD_FAST                5 (e)
-                           946 PRECALL                  1
-                           950 CALL                     1
-                           960 PRECALL                  2
-                           964 CALL                     2
+               837         434 LOAD_GLOBAL              4 (FileSynthesis)
+                           446 LOAD_METHOD              7 (text_file)
+                           468 LOAD_FAST                3 (input_file)
+                           470 PRECALL                  1
+                           474 CALL                     1
+                           484 STORE_FAST               4 (text)
+               
+               838         486 LOAD_FAST                3 (input_file)
+                           488 LOAD_CONST               0 (None)
+                           490 LOAD_CONST               6 (-4)
+                           492 BUILD_SLICE              2
+                           494 BINARY_SUBSCR
+                           504 STORE_FAST               5 (output_file)
+                           506 JUMP_FORWARD            46 (to 600)
+               
+               841     >>  508 LOAD_GLOBAL             16 (logger)
+                           520 LOAD_METHOD              9 (error)
+                           542 LOAD_CONST               9 ('Unsupported file format. Please provide a PDF, txt, or Word document.')
+                           544 PRECALL                  1
+                           548 CALL                     1
+                           558 POP_TOP
+               
+               843         560 LOAD_GLOBAL             21 (NULL + sys)
+                           572 LOAD_ATTR               11 (exit)
+                           582 LOAD_CONST              10 (1)
+                           584 PRECALL                  1
+                           588 CALL                     1
+                           598 POP_TOP
+               
+               844     >>  600 NOP
+               
+               845         602 LOAD_GLOBAL              4 (FileSynthesis)
+                           614 LOAD_METHOD             12 (Synthesise)
+                           636 LOAD_CONST               0 (None)
+                           638 LOAD_FAST                4 (text)
+                           640 LOAD_FAST                5 (output_file)
+                           642 PRECALL                  3
+                           646 CALL                     3
+                           656 POP_TOP
+                           658 EXTENDED_ARG             1
+                           660 JUMP_BACKWARD          285 (to 92)
+                       >>  662 PUSH_EXC_INFO
                
-               695         974 PRECALL                  1
-                           978 CALL                     1
-                           988 POP_TOP
-                           990 POP_EXCEPT
-                           992 LOAD_CONST               0 (None)
-                           994 STORE_FAST               5 (e)
-                           996 DELETE_FAST              5 (e)
-                           998 JUMP_FORWARD           255 (to 1510)
-                       >> 1000 LOAD_CONST               0 (None)
-                          1002 STORE_FAST               5 (e)
-                          1004 DELETE_FAST              5 (e)
-                          1006 RERAISE                  1
-               
-               694     >> 1008 RERAISE                  0
-                       >> 1010 COPY                     3
-                          1012 POP_EXCEPT
-                          1014 RERAISE                  1
-               
-               698     >> 1016 LOAD_FAST                2 (input_file)
-                          1018 LOAD_METHOD              1 (endswith)
-                          1040 LOAD_CONST              11 ('.txt')
-                          1042 PRECALL                  1
-                          1046 CALL                     1
-                          1056 POP_JUMP_FORWARD_IF_FALSE   143 (to 1344)
-               
-               699        1058 NOP
-               
-               700        1060 LOAD_GLOBAL             33 (NULL + text_file)
-                          1072 LOAD_FAST                2 (input_file)
-                          1074 PRECALL                  1
-                          1078 CALL                     1
-                          1088 STORE_FAST               3 (text)
-               
-               701        1090 LOAD_FAST                2 (input_file)
-                          1092 LOAD_CONST               0 (None)
-                          1094 LOAD_CONST               4 (-4)
-                          1096 BUILD_SLICE              2
-                          1098 BINARY_SUBSCR
-                          1108 STORE_FAST               4 (output_file)
-                          1110 JUMP_FORWARD           199 (to 1510)
-                       >> 1112 PUSH_EXC_INFO
-               
-               702        1114 LOAD_GLOBAL              6 (FileNotFoundError)
-                          1126 CHECK_EXC_MATCH
-                          1128 POP_JUMP_FORWARD_IF_FALSE   103 (to 1336)
-                          1130 POP_TOP
-               
-               703        1132 LOAD_GLOBAL              8 (logger)
-                          1144 LOAD_METHOD              5 (error)
-               
-               704        1166 LOAD_CONST               5 ("File '{}' was not found.")
-                          1168 LOAD_METHOD              6 (format)
-                          1190 LOAD_FAST                2 (input_file)
-                          1192 PRECALL                  1
-                          1196 CALL                     1
-               
-               703        1206 PRECALL                  1
-                          1210 CALL                     1
-                          1220 POP_TOP
-               
-               705        1222 POP_EXCEPT
-               
-               712        1224 NOP
-               
-               713        1226 LOAD_GLOBAL             15 (NULL + Synthesise)
-                          1238 LOAD_FAST                3 (text)
-                          1240 LOAD_FAST                4 (output_file)
-                          1242 PRECALL                  2
-                          1246 CALL                     2
-                          1256 POP_TOP
-                          1258 EXTENDED_ARG             2
-                          1260 JUMP_BACKWARD          589 (to 84)
-                       >> 1262 PUSH_EXC_INFO
-               
-               714        1264 LOAD_GLOBAL             16 (KeyboardInterrupt)
-                          1276 CHECK_EXC_MATCH
-                          1278 POP_JUMP_FORWARD_IF_FALSE    24 (to 1328)
-                          1280 POP_TOP
-               
-               715        1282 LOAD_GLOBAL             19 (NULL + sys)
-                          1294 LOAD_ATTR               10 (exit)
-                          1304 LOAD_CONST               6 (1)
-                          1306 PRECALL                  1
-                          1310 CALL                     1
-                          1320 POP_TOP
-                          1322 POP_EXCEPT
-                          1324 EXTENDED_ARG             2
-                          1326 JUMP_BACKWARD          622 (to 84)
-               
-               714     >> 1328 RERAISE                  0
-                       >> 1330 COPY                     3
-                          1332 POP_EXCEPT
-                          1334 RERAISE                  1
-               
-               702     >> 1336 RERAISE                  0
-                       >> 1338 COPY                     3
-                          1340 POP_EXCEPT
-                          1342 RERAISE                  1
-               
-               708     >> 1344 LOAD_GLOBAL              8 (logger)
-                          1356 LOAD_METHOD              5 (error)
-                          1378 LOAD_CONST              12 ('Unsupported file format. Please provide a PDF, txt, or Word document.')
-                          1380 PRECALL                  1
-                          1384 CALL                     1
-                          1394 POP_TOP
-               
-               710        1396 NOP
-               
-               712        1398 NOP
-               
-               713        1400 LOAD_GLOBAL             15 (NULL + Synthesise)
-                          1412 LOAD_FAST                3 (text)
-                          1414 LOAD_FAST                4 (output_file)
-                          1416 PRECALL                  2
-                          1420 CALL                     2
-                          1430 POP_TOP
-                          1432 EXTENDED_ARG             2
-                          1434 JUMP_BACKWARD          676 (to 84)
-                       >> 1436 PUSH_EXC_INFO
-               
-               714        1438 LOAD_GLOBAL             16 (KeyboardInterrupt)
-                          1450 CHECK_EXC_MATCH
-                          1452 POP_JUMP_FORWARD_IF_FALSE    24 (to 1502)
-                          1454 POP_TOP
-               
-               715        1456 LOAD_GLOBAL             19 (NULL + sys)
-                          1468 LOAD_ATTR               10 (exit)
-                          1478 LOAD_CONST               6 (1)
-                          1480 PRECALL                  1
-                          1484 CALL                     1
-                          1494 POP_TOP
-                          1496 POP_EXCEPT
-                          1498 EXTENDED_ARG             2
-                          1500 JUMP_BACKWARD          709 (to 84)
-               
-               714     >> 1502 RERAISE                  0
-                       >> 1504 COPY                     3
-                          1506 POP_EXCEPT
-                          1508 RERAISE                  1
-               
-               712     >> 1510 NOP
-               
-               713        1512 LOAD_GLOBAL             15 (NULL + Synthesise)
-                          1524 LOAD_FAST                3 (text)
-                          1526 LOAD_FAST                4 (output_file)
-                          1528 PRECALL                  2
-                          1532 CALL                     2
-                          1542 POP_TOP
-                          1544 EXTENDED_ARG             2
-                          1546 JUMP_BACKWARD          732 (to 84)
-                       >> 1548 PUSH_EXC_INFO
-               
-               714        1550 LOAD_GLOBAL             16 (KeyboardInterrupt)
-                          1562 CHECK_EXC_MATCH
-                          1564 POP_JUMP_FORWARD_IF_FALSE    24 (to 1614)
-                          1566 POP_TOP
-               
-               715        1568 LOAD_GLOBAL             19 (NULL + sys)
-                          1580 LOAD_ATTR               10 (exit)
-                          1590 LOAD_CONST               6 (1)
-                          1592 PRECALL                  1
-                          1596 CALL                     1
-                          1606 POP_TOP
-                          1608 POP_EXCEPT
-                          1610 EXTENDED_ARG             2
-                          1612 JUMP_BACKWARD          765 (to 84)
-               
-               714     >> 1614 RERAISE                  0
-                       >> 1616 COPY                     3
-                          1618 POP_EXCEPT
-                          1620 RERAISE                  1
-                       >> 1622 PUSH_EXC_INFO
-               
-               712        1624 NOP
-               
-               713        1626 LOAD_GLOBAL             15 (NULL + Synthesise)
-                          1638 LOAD_FAST                3 (text)
-                          1640 LOAD_FAST                4 (output_file)
-                          1642 PRECALL                  2
-                          1646 CALL                     2
-                          1656 POP_TOP
-                          1658 RERAISE                  0
-                       >> 1660 PUSH_EXC_INFO
-               
-               714        1662 LOAD_GLOBAL             16 (KeyboardInterrupt)
-                          1674 CHECK_EXC_MATCH
-                          1676 POP_JUMP_FORWARD_IF_FALSE    23 (to 1724)
-                          1678 POP_TOP
-               
-               715        1680 LOAD_GLOBAL             19 (NULL + sys)
-                          1692 LOAD_ATTR               10 (exit)
-                          1702 LOAD_CONST               6 (1)
-                          1704 PRECALL                  1
-                          1708 CALL                     1
-                          1718 POP_TOP
-                          1720 POP_EXCEPT
-                          1722 RERAISE                  0
+               846         664 LOAD_GLOBAL             26 (KeyboardInterrupt)
+                           676 CHECK_EXC_MATCH
+                           678 POP_JUMP_FORWARD_IF_FALSE    24 (to 728)
+                           680 POP_TOP
                
-               714     >> 1724 RERAISE                  0
-                       >> 1726 COPY                     3
-                          1728 POP_EXCEPT
-                          1730 RERAISE                  1
-                       >> 1732 COPY                     3
-                          1734 POP_EXCEPT
-                          1736 RERAISE                  1
+               847         682 LOAD_GLOBAL             21 (NULL + sys)
+                           694 LOAD_ATTR               11 (exit)
+                           704 LOAD_CONST              10 (1)
+                           706 PRECALL                  1
+                           710 CALL                     1
+                           720 POP_TOP
+                           722 POP_EXCEPT
+                           724 EXTENDED_ARG             1
+                           726 JUMP_BACKWARD          318 (to 92)
+               
+               846     >>  728 RERAISE                  0
+                       >>  730 COPY                     3
+                           732 POP_EXCEPT
+                           734 RERAISE                  1
                
-               674     >> 1738 LOAD_CONST               0 (None)
-                          1740 RETURN_VALUE
+               826     >>  736 LOAD_CONST               0 (None)
+                           738 RETURN_VALUE
                ExceptionTable:
-                 92 to 132 -> 1622 [1]
-                 136 to 184 -> 190 [1]
-                 186 to 188 -> 1622 [1]
-                 190 to 298 -> 412 [2] lasti
-                 300 to 300 -> 1622 [1]
-                 304 to 334 -> 338 [1]
-                 338 to 396 -> 404 [2] lasti
-                 402 to 402 -> 404 [2] lasti
-                 410 to 410 -> 412 [2] lasti
-                 412 to 572 -> 1622 [1]
-                 576 to 624 -> 630 [1]
-                 626 to 628 -> 1622 [1]
-                 630 to 738 -> 1010 [2] lasti
-                 740 to 740 -> 1622 [1]
-                 744 to 774 -> 780 [1]
-                 780 to 838 -> 848 [2] lasti
-                 846 to 846 -> 848 [2] lasti
-                 854 to 870 -> 1010 [2] lasti
-                 872 to 988 -> 1000 [2] lasti
-                 990 to 998 -> 1622 [1]
-                 1000 to 1008 -> 1010 [2] lasti
-                 1010 to 1056 -> 1622 [1]
-                 1060 to 1108 -> 1112 [1]
-                 1110 to 1110 -> 1622 [1]
-                 1112 to 1220 -> 1338 [2] lasti
-                 1222 to 1222 -> 1622 [1]
-                 1226 to 1256 -> 1262 [1]
-                 1262 to 1320 -> 1330 [2] lasti
-                 1328 to 1328 -> 1330 [2] lasti
-                 1336 to 1336 -> 1338 [2] lasti
-                 1338 to 1394 -> 1622 [1]
-                 1400 to 1430 -> 1436 [1]
-                 1436 to 1494 -> 1504 [2] lasti
-                 1502 to 1502 -> 1504 [2] lasti
-                 1512 to 1542 -> 1548 [1]
-                 1548 to 1606 -> 1616 [2] lasti
-                 1614 to 1614 -> 1616 [2] lasti
-                 1622 to 1622 -> 1732 [2] lasti
-                 1626 to 1656 -> 1660 [3]
-                 1658 to 1658 -> 1732 [2] lasti
-                 1660 to 1718 -> 1726 [4] lasti
-                 1720 to 1722 -> 1732 [2] lasti
-                 1724 to 1724 -> 1726 [4] lasti
-                 1726 to 1730 -> 1732 [2] lasti
+                 602 to 656 -> 662 [1]
+                 662 to 720 -> 730 [2] lasti
+                 728 to 728 -> 730 [2] lasti
                consts
                   None
+                  'docx'
+                  'doc'
                   frozenset({'docx', 'txt', 'doc', 'pdf'})
                   code
                      argcount  : 1
                      nlocals   : 2
-                     stacksize : 5
+                     stacksize : 7
                      flags     : 19
                      code
-                        0x9501970067007c005d2b7d017c01a00000000000000000000000000000
+                        0x9501970067007c005d387d017c01a00000000000000000000000000000
                         00000000000000a6000000ab000000000000000000a00100000000000000
-                        000000000000000000000000008902a6010000ab010000000000000000af
-                        297c0191028c2c5300
+                        000000000000000000000000007405000000000000000000008902a60100
+                        00ab010000000000000000a6010000ab010000000000000000af367c0191
+                        028c395300
                                    0 COPY_FREE_VARS           1
                      
-                     673           2 RESUME                   0
+                     825           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                43 (to 96)
+                             >>    8 FOR_ITER                56 (to 122)
                                   10 STORE_FAST               1 (item)
                                   12 LOAD_FAST                1 (item)
                                   14 LOAD_METHOD              0 (lower)
                                   36 PRECALL                  0
                                   40 CALL                     0
                                   50 LOAD_METHOD              1 (endswith)
-                                  72 LOAD_DEREF               2 (ls)
-                                  74 PRECALL                  1
-                                  78 CALL                     1
-                                  88 POP_JUMP_BACKWARD_IF_FALSE    41 (to 8)
-                                  90 LOAD_FAST                1 (item)
-                                  92 LIST_APPEND              2
-                                  94 JUMP_BACKWARD           44 (to 8)
-                             >>   96 RETURN_VALUE
+                                  72 LOAD_GLOBAL              5 (NULL + tuple)
+                                  84 LOAD_DEREF               2 (ls)
+                                  86 PRECALL                  1
+                                  90 CALL                     1
+                                 100 PRECALL                  1
+                                 104 CALL                     1
+                                 114 POP_JUMP_BACKWARD_IF_FALSE    54 (to 8)
+                                 116 LOAD_FAST                1 (item)
+                                 118 LIST_APPEND              2
+                                 120 JUMP_BACKWARD           57 (to 8)
+                             >>  122 RETURN_VALUE
                      consts
-                     names      ('lower', 'endswith')
+                     names      ('lower', 'endswith', 'tuple')
                      varnames   ('.0', 'item')
                      freevars   ('ls',)
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 673
+                     firstlineno 825
                      lnotab 0x
                   '.pdf'
                   -4
-                  "File '{}' was not found."
-                  1
-                  '.docx'
-                  '.doc'
                   -5
-                  'Error converting {} to text: {}'
                   '.txt'
                   'Unsupported file format. Please provide a PDF, txt, or Word document.'
-               names      ('preprocess', 'endswith', 'pdf_to_text', 'FileNotFoundError', 'logger', 'error', 'format', 'Synthesise', 'KeyboardInterrupt', 'sys', 'exit', 'lower', 'docx_to_text', 'Exception', 'exception', 'str', 'text_file')
-               varnames   ('self', 'input_list', 'input_file', 'text', 'output_file', 'e')
+                  1
+               names      ('preprocess', 'endswith', 'FileSynthesis', 'pdf_to_text', 'lower', 'tuple', 'docx_to_text', 'text_file', 'logger', 'error', 'sys', 'exit', 'Synthesise', 'KeyboardInterrupt')
+               varnames   ('self', 'input_list', 'extdoc', 'input_file', 'text', 'output_file')
                freevars   ()
                cellvars   ('ls',)
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'audiofy'
-               firstlineno 670
+               firstlineno 821
                lnotab
-                  0x0401280108011c010a0102012a0102011e011a011201220128ff100202
-                  1d0201240112012cff08de08059c0102011e011a011201220128ff100202
-                  140201260112012eff08ec1201240142ff22ff08042a0102011e01180112
-                  01220128ff100202070201260112012eff08f40806340202020201260112
-                  012eff08fe0201260112012eff0afe0201240112012cff0ed8
-            (16000,)
-            ('tempfile', 3)
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'preprocess', 'Iterable', 'bytes', 'int', 'AudioSegment', 'join_audios', 'str', 'Synthesise', 'pdf_to_text', 'text_file', 'docx_to_text', 'audiofy')
+                  0x04012801080108011c010a012a01340116026802340116022a01340116
+                  033402280102013e0112012eff08ec
+            (20000, 'tempfile', 5)
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'preprocess', 'staticmethod', 'join_audios', 'str', 'int', 'Synthesise', 'pdf_to_text', 'text_file', 'docx_to_text', 'audiofy')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+         filename   '/media/skye/skye/FileMAC/filemac/converter.py'
          name       'FileSynthesis'
-         firstlineno 541
-         lnotab 0x0a020604060d22061e48060f0605060a0202
+         firstlineno 661
+         lnotab
+            0x0a020604060d020104ff0e0102172246020104ff0e010211020104ff0e
+            01020c020104ff0e01020d0202
       'FileSynthesis'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             045300
-         723           0 RESUME                   0
+         855           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('VideoConverter')
                        8 STORE_NAME               2 (__qualname__)
          
-         725          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 725>)
+         857          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/skye/FileMAC/filemac/converter.py", line 857>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-         729          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 729>)
+         861          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/skye/FileMAC/filemac/converter.py", line 861>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (preprocess)
          
-         745          22 LOAD_CONST               3 (<code object CONVERT_VIDEO, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 745>)
+         877          22 LOAD_CONST               3 (<code object CONVERT_VIDEO, file "/media/skye/skye/FileMAC/filemac/converter.py", line 877>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (CONVERT_VIDEO)
                       28 LOAD_CONST               4 (None)
                       30 RETURN_VALUE
          consts
             'VideoConverter'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   0064005300
-               725           0 RESUME                   0
+               857           0 RESUME                   0
                
-               726           2 LOAD_FAST                1 (input_file)
+               858           2 LOAD_FAST                1 (input_file)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (input_file)
                
-               727          16 LOAD_FAST                2 (out_format)
+               859          16 LOAD_FAST                2 (out_format)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (out_format)
                             30 LOAD_CONST               0 (None)
                             32 RETURN_VALUE
                consts
                   None
                names      ('input_file', 'out_format')
                varnames   ('self', 'input_file', 'out_format')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       '__init__'
-               firstlineno 725
+               firstlineno 857
                lnotab 0x02010e01
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
@@ -6976,391 +8179,413 @@
                   010000ab01000000000000000044005d5b7d027400000000000000000000
                   006a010000000000000000a00a0000000000000000000000000000000000
                   0000007c006a0300000000000000007c02a6020000ab0200000000000000
                   007d037400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c03a6010000ab010000000000
                   00000072157c01a00400000000000000000000000000000000000000007c
                   03a6010000ab01000000000000000001008c5c7c015300
-               729           0 RESUME                   0
+               861           0 RESUME                   0
                
-               730           2 BUILD_LIST               0
+               862           2 BUILD_LIST               0
                              4 STORE_FAST               1 (files_to_process)
                
-               732           6 LOAD_GLOBAL              0 (os)
+               864           6 LOAD_GLOBAL              0 (os)
                             18 LOAD_ATTR                1 (path)
                             28 LOAD_METHOD              2 (isfile)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                3 (input_file)
                             62 PRECALL                  1
                             66 CALL                     1
                             76 POP_JUMP_FORWARD_IF_FALSE    27 (to 132)
                
-               733          78 LOAD_FAST                1 (files_to_process)
+               865          78 LOAD_FAST                1 (files_to_process)
                             80 LOAD_METHOD              4 (append)
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                3 (input_file)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                            130 JUMP_FORWARD           213 (to 558)
                
-               734     >>  132 LOAD_GLOBAL              0 (os)
+               866     >>  132 LOAD_GLOBAL              0 (os)
                            144 LOAD_ATTR                1 (path)
                            154 LOAD_METHOD              5 (isdir)
                            176 LOAD_FAST                0 (self)
                            178 LOAD_ATTR                3 (input_file)
                            188 PRECALL                  1
                            192 CALL                     1
                            202 POP_JUMP_FORWARD_IF_FALSE   177 (to 558)
                
-               735         204 LOAD_GLOBAL              1 (NULL + os)
+               867         204 LOAD_GLOBAL              1 (NULL + os)
                            216 LOAD_ATTR                6 (listdir)
                            226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                3 (input_file)
                            238 PRECALL                  1
                            242 CALL                     1
                            252 POP_JUMP_FORWARD_IF_NOT_NONE    35 (to 324)
                
-               736         254 LOAD_GLOBAL             15 (NULL + print)
+               868         254 LOAD_GLOBAL             15 (NULL + print)
                            266 LOAD_CONST               1 ('Cannot work with empty folder')
                            268 PRECALL                  1
                            272 CALL                     1
                            282 POP_TOP
                
-               737         284 LOAD_GLOBAL             17 (NULL + sys)
+               869         284 LOAD_GLOBAL             17 (NULL + sys)
                            296 LOAD_ATTR                9 (exit)
                            306 LOAD_CONST               2 (1)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 POP_TOP
                
-               738     >>  324 LOAD_GLOBAL              1 (NULL + os)
+               870     >>  324 LOAD_GLOBAL              1 (NULL + os)
                            336 LOAD_ATTR                6 (listdir)
                            346 LOAD_FAST                0 (self)
                            348 LOAD_ATTR                3 (input_file)
                            358 PRECALL                  1
                            362 CALL                     1
                            372 GET_ITER
                        >>  374 FOR_ITER                91 (to 558)
                            376 STORE_FAST               2 (file)
                
-               739         378 LOAD_GLOBAL              0 (os)
+               871         378 LOAD_GLOBAL              0 (os)
                            390 LOAD_ATTR                1 (path)
                            400 LOAD_METHOD             10 (join)
                            422 LOAD_FAST                0 (self)
                            424 LOAD_ATTR                3 (input_file)
                            434 LOAD_FAST                2 (file)
                            436 PRECALL                  2
                            440 CALL                     2
                            450 STORE_FAST               3 (file_path)
                
-               740         452 LOAD_GLOBAL              0 (os)
+               872         452 LOAD_GLOBAL              0 (os)
                            464 LOAD_ATTR                1 (path)
                            474 LOAD_METHOD              2 (isfile)
                            496 LOAD_FAST                3 (file_path)
                            498 PRECALL                  1
                            502 CALL                     1
                            512 POP_JUMP_FORWARD_IF_FALSE    21 (to 556)
                
-               741         514 LOAD_FAST                1 (files_to_process)
+               873         514 LOAD_FAST                1 (files_to_process)
                            516 LOAD_METHOD              4 (append)
                            538 LOAD_FAST                3 (file_path)
                            540 PRECALL                  1
                            544 CALL                     1
                            554 POP_TOP
                        >>  556 JUMP_BACKWARD           92 (to 374)
                
-               743     >>  558 LOAD_FAST                1 (files_to_process)
+               875     >>  558 LOAD_FAST                1 (files_to_process)
                            560 RETURN_VALUE
                consts
                   None
                   'Cannot work with empty folder'
                   1
                names      ('os', 'path', 'isfile', 'input_file', 'append', 'isdir', 'listdir', 'print', 'sys', 'exit', 'join')
                varnames   ('self', 'files_to_process', 'file', 'file_path')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'preprocess'
-               firstlineno 729
+               firstlineno 861
                lnotab 0x0201040248013601480132011e01280136014a013e012c02
             code
                argcount  : 1
                nlocals   : 10
                stacksize : 8
                flags     : 3
                code
                   0x970009007c00a0000000000000000000000000000000000000000000a6
                   000000ab0000000000000000007d017c006a010000000000000000a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
                   0000007d02640184007c014400a6000000ab0000000000000000007d0174
-                  07000000000000000000006402a6010000ab01000000000000000001007c
-                  01440090015d0a7d037c02a0020000000000000000000000000000000000
-                  000000a6000000ab00000000000000000074080000000000000000000076
-                  00724c740a000000000000000000006a060000000000000000a007000000
+                  07000000000000000000007408000000000000000000009b006402740a00
+                  0000000000000000009b009d03a6010000ab01000000000000000001007c
+                  01440090015d357d037c02a0020000000000000000000000000000000000
+                  000000a6000000ab000000000000000000740c0000000000000000000076
+                  00724c740e000000000000000000006a080000000000000000a009000000
                   00000000000000000000000000000000007c03a6010000ab010000000000
-                  0000005c0200007d047d057c0464037a0000007c02a00800000000000000
+                  0000005c0200007d047d057c0464037a0000007c02a00a00000000000000
                   00000000000000000000000000a6000000ab0000000000000000007a0000
                   007d067407000000000000000000007c06a6010000ab0100000000000000
                   0001006e237407000000000000000000006404a6010000ab010000000000
-                  00000001007413000000000000000000006a0a00000000000000006405a6
+                  00000001007417000000000000000000006a0c00000000000000006405a6
                   010000ab010000000000000000010064066407640864066409640a640b9c
-                  067d070900740700000000000000000000640ca6010000ab010000000000
-                  00000001007417000000000000000000007c03a6010000ab010000000000
-                  0000007d080900740700000000000000000000640d7c069b00640e9d03a6
-                  010000ab01000000000000000001007c08a00c0000000000000000000000
-                  0000000000000000007c067c077c0219000000000000000000ac0fa60200
-                  00ab020000000000000000010009007407000000000000000000006410a6
-                  010000ab01000000000000000001007c08a00d0000000000000000000000
-                  000000000000000000a6000000ab000000000000000000010090018c0c64
-                  0053002300741c0000000000000000000024007227010074070000000000
-                  00000000006411a6010000ab010000000000000000010074130000000000
-                  00000000006a0a00000000000000006405a6010000ab0100000000000000
-                  000100590064005300741e000000000000000000002400721a7d09740700
-                  0000000000000000007c09a6010000ab0100000000000000000100590064
-                  007d097e096400530064007d097e0977017700780359007701
-               745           0 RESUME                   0
+                  067d070900740700000000000000000000741a000000000000000000009b
+                  00640c740a000000000000000000009b009d03a6010000ab010000000000
+                  0000000100741d000000000000000000007c03a6010000ab010000000000
+                  0000007d080900740700000000000000000000741e000000000000000000
+                  009b00640d7c069b00740a000000000000000000009b009d04a6010000ab
+                  01000000000000000001007c08a010000000000000000000000000000000
+                  00000000007c067c077c0219000000000000000000ac0ea6020000ab0200
+                  000000000000000100090074070000000000000000000074220000000000
+                  00000000009b00640f740a000000000000000000009b009d03a6010000ab
+                  01000000000000000001007c08a012000000000000000000000000000000
+                  0000000000a6000000ab000000000000000000010090018c376400530023
+                  007426000000000000000000002400722701007407000000000000000000
+                  006410a6010000ab01000000000000000001007417000000000000000000
+                  006a0c00000000000000006405a6010000ab010000000000000000010059
+                  00640053007428000000000000000000002400721a7d0974070000000000
+                  00000000007c09a6010000ab0100000000000000000100590064007d097e
+                  096400530064007d097e0977017700780359007701
+               877           0 RESUME                   0
                
-               746           2 NOP
+               878           2 NOP
                
-               747           4 LOAD_FAST                0 (self)
+               879           4 LOAD_FAST                0 (self)
                              6 LOAD_METHOD              0 (preprocess)
                             28 PRECALL                  0
                             32 CALL                     0
                             42 STORE_FAST               1 (input_list)
                
-               748          44 LOAD_FAST                0 (self)
+               880          44 LOAD_FAST                0 (self)
                             46 LOAD_ATTR                1 (out_format)
                             56 LOAD_METHOD              2 (upper)
                             78 PRECALL                  0
                             82 CALL                     0
                             92 STORE_FAST               2 (out_f)
                
-               749          94 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 749>)
+               881          94 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 881>)
                             96 MAKE_FUNCTION            0
                             98 LOAD_FAST                1 (input_list)
                            100 GET_ITER
                            102 PRECALL                  0
                            106 CALL                     0
                            116 STORE_FAST               1 (input_list)
                
-               751         118 LOAD_GLOBAL              7 (NULL + print)
-                           130 LOAD_CONST               2 ('\x1b[1;33mInitializing conversion..\x1b[0m')
-                           132 PRECALL                  1
-                           136 CALL                     1
-                           146 POP_TOP
-               
-               753         148 LOAD_FAST                1 (input_list)
-                           150 GET_ITER
-                       >>  152 EXTENDED_ARG             1
-                           154 FOR_ITER               266 (to 688)
-                           156 STORE_FAST               3 (file)
-               
-               754         158 LOAD_FAST                2 (out_f)
-                           160 LOAD_METHOD              2 (upper)
-                           182 PRECALL                  0
-                           186 CALL                     0
-                           196 LOAD_GLOBAL              8 (SUPPORTED_VIDEO_FORMATS)
-                           208 CONTAINS_OP              0
-                           210 POP_JUMP_FORWARD_IF_FALSE    76 (to 364)
-               
-               755         212 LOAD_GLOBAL             10 (os)
-                           224 LOAD_ATTR                6 (path)
-                           234 LOAD_METHOD              7 (splitext)
-                           256 LOAD_FAST                3 (file)
-                           258 PRECALL                  1
-                           262 CALL                     1
-                           272 UNPACK_SEQUENCE          2
-                           276 STORE_FAST               4 (_)
-                           278 STORE_FAST               5 (ext)
-               
-               756         280 LOAD_FAST                4 (_)
-                           282 LOAD_CONST               3 ('.')
-                           284 BINARY_OP                0 (+)
-                           288 LOAD_FAST                2 (out_f)
-                           290 LOAD_METHOD              8 (lower)
-                           312 PRECALL                  0
-                           316 CALL                     0
-                           326 BINARY_OP                0 (+)
-                           330 STORE_FAST               6 (output_filename)
-               
-               757         332 LOAD_GLOBAL              7 (NULL + print)
-                           344 LOAD_FAST                6 (output_filename)
-                           346 PRECALL                  1
-                           350 CALL                     1
-                           360 POP_TOP
-                           362 JUMP_FORWARD            35 (to 434)
-               
-               759     >>  364 LOAD_GLOBAL              7 (NULL + print)
-                           376 LOAD_CONST               4 ('Unsupported output format')
-                           378 PRECALL                  1
-                           382 CALL                     1
-                           392 POP_TOP
+               883         118 LOAD_GLOBAL              7 (NULL + print)
+                           130 LOAD_GLOBAL              8 (DYELLOW)
+                           142 FORMAT_VALUE             0
+                           144 LOAD_CONST               2 ('Initializing conversion..')
+                           146 LOAD_GLOBAL             10 (RESET)
+                           158 FORMAT_VALUE             0
+                           160 BUILD_STRING             3
+                           162 PRECALL                  1
+                           166 CALL                     1
+                           176 POP_TOP
                
-               760         394 LOAD_GLOBAL             19 (NULL + sys)
-                           406 LOAD_ATTR               10 (exit)
-                           416 LOAD_CONST               5 (1)
-                           418 PRECALL                  1
-                           422 CALL                     1
-                           432 POP_TOP
+               885         178 LOAD_FAST                1 (input_list)
+                           180 GET_ITER
+                       >>  182 EXTENDED_ARG             1
+                           184 FOR_ITER               309 (to 804)
+                           186 STORE_FAST               3 (file)
+               
+               886         188 LOAD_FAST                2 (out_f)
+                           190 LOAD_METHOD              2 (upper)
+                           212 PRECALL                  0
+                           216 CALL                     0
+                           226 LOAD_GLOBAL             12 (SUPPORTED_VIDEO_FORMATS)
+                           238 CONTAINS_OP              0
+                           240 POP_JUMP_FORWARD_IF_FALSE    76 (to 394)
+               
+               887         242 LOAD_GLOBAL             14 (os)
+                           254 LOAD_ATTR                8 (path)
+                           264 LOAD_METHOD              9 (splitext)
+                           286 LOAD_FAST                3 (file)
+                           288 PRECALL                  1
+                           292 CALL                     1
+                           302 UNPACK_SEQUENCE          2
+                           306 STORE_FAST               4 (_)
+                           308 STORE_FAST               5 (ext)
+               
+               888         310 LOAD_FAST                4 (_)
+                           312 LOAD_CONST               3 ('.')
+                           314 BINARY_OP                0 (+)
+                           318 LOAD_FAST                2 (out_f)
+                           320 LOAD_METHOD             10 (lower)
+                           342 PRECALL                  0
+                           346 CALL                     0
+                           356 BINARY_OP                0 (+)
+                           360 STORE_FAST               6 (output_filename)
                
-               762     >>  434 LOAD_CONST               6 ('mpeg4')
+               889         362 LOAD_GLOBAL              7 (NULL + print)
+                           374 LOAD_FAST                6 (output_filename)
+                           376 PRECALL                  1
+                           380 CALL                     1
+                           390 POP_TOP
+                           392 JUMP_FORWARD            35 (to 464)
                
-               763         436 LOAD_CONST               7 ('rawvideo')
+               891     >>  394 LOAD_GLOBAL              7 (NULL + print)
+                           406 LOAD_CONST               4 ('Unsupported output format')
+                           408 PRECALL                  1
+                           412 CALL                     1
+                           422 POP_TOP
+               
+               892         424 LOAD_GLOBAL             23 (NULL + sys)
+                           436 LOAD_ATTR               12 (exit)
+                           446 LOAD_CONST               5 (1)
+                           448 PRECALL                  1
+                           452 CALL                     1
+                           462 POP_TOP
                
-               765         438 LOAD_CONST               8 ('libvpx')
+               894     >>  464 LOAD_CONST               6 ('mpeg4')
                
-               766         440 LOAD_CONST               6 ('mpeg4')
+               895         466 LOAD_CONST               7 ('rawvideo')
                
-               767         442 LOAD_CONST               9 ('MPEG4')
+               897         468 LOAD_CONST               8 ('libvpx')
                
-               768         444 LOAD_CONST              10 ('flv')
+               898         470 LOAD_CONST               6 ('mpeg4')
                
-               761         446 LOAD_CONST              11 (('MP4', 'AVI', 'WEBM', 'MOV', 'MKV', 'FLV'))
-                           448 BUILD_CONST_KEY_MAP      6
-                           450 STORE_FAST               7 (format_codec)
+               899         472 LOAD_CONST               9 ('MPEG4')
                
-               771         452 NOP
+               900         474 LOAD_CONST              10 ('flv')
                
-               772         454 LOAD_GLOBAL              7 (NULL + print)
-                           466 LOAD_CONST              12 ('\x1b[1;34mLoad file\x1b[0m')
-                           468 PRECALL                  1
-                           472 CALL                     1
-                           482 POP_TOP
+               893         476 LOAD_CONST              11 (('MP4', 'AVI', 'WEBM', 'MOV', 'MKV', 'FLV'))
+                           478 BUILD_CONST_KEY_MAP      6
+                           480 STORE_FAST               7 (format_codec)
                
-               773         484 LOAD_GLOBAL             23 (NULL + VideoFileClip)
-                           496 LOAD_FAST                3 (file)
-                           498 PRECALL                  1
-                           502 CALL                     1
-                           512 STORE_FAST               8 (video)
+               903         482 NOP
                
-               774         514 NOP
+               904         484 LOAD_GLOBAL              7 (NULL + print)
+                           496 LOAD_GLOBAL             26 (DBLUE)
+                           508 FORMAT_VALUE             0
+                           510 LOAD_CONST              12 ('oad file')
+                           512 LOAD_GLOBAL             10 (RESET)
+                           524 FORMAT_VALUE             0
+                           526 BUILD_STRING             3
+                           528 PRECALL                  1
+                           532 CALL                     1
+                           542 POP_TOP
                
-               775         516 LOAD_GLOBAL              7 (NULL + print)
-                           528 LOAD_CONST              13 ('\x1b[1;35mConverting file to ')
-                           530 LOAD_FAST                6 (output_filename)
-                           532 FORMAT_VALUE             0
-                           534 LOAD_CONST              14 ('\x1b[0m')
-                           536 BUILD_STRING             3
-                           538 PRECALL                  1
-                           542 CALL                     1
-                           552 POP_TOP
-               
-               776         554 LOAD_FAST                8 (video)
-                           556 LOAD_METHOD             12 (write_videofile)
-               
-               777         578 LOAD_FAST                6 (output_filename)
-                           580 LOAD_FAST                7 (format_codec)
-                           582 LOAD_FAST                2 (out_f)
-                           584 BINARY_SUBSCR
-               
-               776         594 KW_NAMES                15
-                           596 PRECALL                  2
-                           600 CALL                     2
-                           610 POP_TOP
+               905         544 LOAD_GLOBAL             29 (NULL + VideoFileClip)
+                           556 LOAD_FAST                3 (file)
+                           558 PRECALL                  1
+                           562 CALL                     1
+                           572 STORE_FAST               8 (video)
                
-               778         612 NOP
+               906         574 NOP
                
-               779         614 LOAD_GLOBAL              7 (NULL + print)
-                           626 LOAD_CONST              16 ('\x1b[1;32mDone\x1b[0m')
-                           628 PRECALL                  1
-                           632 CALL                     1
-                           642 POP_TOP
+               907         576 LOAD_GLOBAL              7 (NULL + print)
+                           588 LOAD_GLOBAL             30 (DMAGENTA)
+                           600 FORMAT_VALUE             0
+                           602 LOAD_CONST              13 ('Converting file to ')
+                           604 LOAD_FAST                6 (output_filename)
+                           606 FORMAT_VALUE             0
+                           608 LOAD_GLOBAL             10 (RESET)
+                           620 FORMAT_VALUE             0
+                           622 BUILD_STRING             4
+                           624 PRECALL                  1
+                           628 CALL                     1
+                           638 POP_TOP
+               
+               908         640 LOAD_FAST                8 (video)
+                           642 LOAD_METHOD             16 (write_videofile)
+               
+               909         664 LOAD_FAST                6 (output_filename)
+                           666 LOAD_FAST                7 (format_codec)
+                           668 LOAD_FAST                2 (out_f)
+                           670 BINARY_SUBSCR
+               
+               908         680 KW_NAMES                14
+                           682 PRECALL                  2
+                           686 CALL                     2
+                           696 POP_TOP
+               
+               910         698 NOP
+               
+               911         700 LOAD_GLOBAL              7 (NULL + print)
+                           712 LOAD_GLOBAL             34 (DGREEN)
+                           724 FORMAT_VALUE             0
+                           726 LOAD_CONST              15 ('Done')
+                           728 LOAD_GLOBAL             10 (RESET)
+                           740 FORMAT_VALUE             0
+                           742 BUILD_STRING             3
+                           744 PRECALL                  1
+                           748 CALL                     1
+                           758 POP_TOP
+               
+               912         760 LOAD_FAST                8 (video)
+                           762 LOAD_METHOD             18 (close)
+                           784 PRECALL                  0
+                           788 CALL                     0
+                           798 POP_TOP
+                           800 EXTENDED_ARG             1
+                           802 JUMP_BACKWARD          311 (to 182)
                
-               780         644 LOAD_FAST                8 (video)
-                           646 LOAD_METHOD             13 (close)
-                           668 PRECALL                  0
-                           672 CALL                     0
-                           682 POP_TOP
-                           684 EXTENDED_ARG             1
-                           686 JUMP_BACKWARD          268 (to 152)
-               
-               753     >>  688 LOAD_CONST               0 (None)
-                           690 RETURN_VALUE
-                       >>  692 PUSH_EXC_INFO
-               
-               781         694 LOAD_GLOBAL             28 (KeyboardInterrupt)
-                           706 CHECK_EXC_MATCH
-                           708 POP_JUMP_FORWARD_IF_FALSE    39 (to 788)
-                           710 POP_TOP
-               
-               782         712 LOAD_GLOBAL              7 (NULL + print)
-                           724 LOAD_CONST              17 ('\nExiting..')
-                           726 PRECALL                  1
-                           730 CALL                     1
-                           740 POP_TOP
-               
-               783         742 LOAD_GLOBAL             19 (NULL + sys)
-                           754 LOAD_ATTR               10 (exit)
-                           764 LOAD_CONST               5 (1)
-                           766 PRECALL                  1
-                           770 CALL                     1
-                           780 POP_TOP
-                           782 POP_EXCEPT
-                           784 LOAD_CONST               0 (None)
-                           786 RETURN_VALUE
+               885     >>  804 LOAD_CONST               0 (None)
+                           806 RETURN_VALUE
+                       >>  808 PUSH_EXC_INFO
+               
+               913         810 LOAD_GLOBAL             38 (KeyboardInterrupt)
+                           822 CHECK_EXC_MATCH
+                           824 POP_JUMP_FORWARD_IF_FALSE    39 (to 904)
+                           826 POP_TOP
+               
+               914         828 LOAD_GLOBAL              7 (NULL + print)
+                           840 LOAD_CONST              16 ('\nExiting..')
+                           842 PRECALL                  1
+                           846 CALL                     1
+                           856 POP_TOP
                
-               784     >>  788 LOAD_GLOBAL             30 (Exception)
-                           800 CHECK_EXC_MATCH
-                           802 POP_JUMP_FORWARD_IF_FALSE    26 (to 856)
-                           804 STORE_FAST               9 (e)
-               
-               785         806 LOAD_GLOBAL              7 (NULL + print)
-                           818 LOAD_FAST                9 (e)
-                           820 PRECALL                  1
-                           824 CALL                     1
-                           834 POP_TOP
-                           836 POP_EXCEPT
-                           838 LOAD_CONST               0 (None)
-                           840 STORE_FAST               9 (e)
-                           842 DELETE_FAST              9 (e)
-                           844 LOAD_CONST               0 (None)
-                           846 RETURN_VALUE
-                       >>  848 LOAD_CONST               0 (None)
-                           850 STORE_FAST               9 (e)
-                           852 DELETE_FAST              9 (e)
-                           854 RERAISE                  1
+               915         858 LOAD_GLOBAL             23 (NULL + sys)
+                           870 LOAD_ATTR               12 (exit)
+                           880 LOAD_CONST               5 (1)
+                           882 PRECALL                  1
+                           886 CALL                     1
+                           896 POP_TOP
+                           898 POP_EXCEPT
+                           900 LOAD_CONST               0 (None)
+                           902 RETURN_VALUE
                
-               784     >>  856 RERAISE                  0
-                       >>  858 COPY                     3
-                           860 POP_EXCEPT
-                           862 RERAISE                  1
+               916     >>  904 LOAD_GLOBAL             40 (Exception)
+                           916 CHECK_EXC_MATCH
+                           918 POP_JUMP_FORWARD_IF_FALSE    26 (to 972)
+                           920 STORE_FAST               9 (e)
+               
+               917         922 LOAD_GLOBAL              7 (NULL + print)
+                           934 LOAD_FAST                9 (e)
+                           936 PRECALL                  1
+                           940 CALL                     1
+                           950 POP_TOP
+                           952 POP_EXCEPT
+                           954 LOAD_CONST               0 (None)
+                           956 STORE_FAST               9 (e)
+                           958 DELETE_FAST              9 (e)
+                           960 LOAD_CONST               0 (None)
+                           962 RETURN_VALUE
+                       >>  964 LOAD_CONST               0 (None)
+                           966 STORE_FAST               9 (e)
+                           968 DELETE_FAST              9 (e)
+                           970 RERAISE                  1
+               
+               916     >>  972 RERAISE                  0
+                       >>  974 COPY                     3
+                           976 POP_EXCEPT
+                           978 RERAISE                  1
                ExceptionTable:
-                 4 to 686 -> 692 [0]
-                 692 to 780 -> 858 [1] lasti
-                 788 to 804 -> 858 [1] lasti
-                 806 to 834 -> 848 [1] lasti
-                 848 to 856 -> 858 [1] lasti
+                 4 to 802 -> 808 [0]
+                 808 to 896 -> 974 [1] lasti
+                 904 to 920 -> 974 [1] lasti
+                 922 to 950 -> 964 [1] lasti
+                 964 to 972 -> 974 [1] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 6
                      flags     : 19
                      code
                         0x8701970067007c005d248a017401000000000000000000008801660164
                         0084087402000000000000000000004400a6000000ab0000000000000000
                         00a6010000ab010000000000000000af22890191028c255300
                                    0 MAKE_CELL                1 (item)
                      
-                     749           2 RESUME                   0
+                     881           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                36 (to 82)
                                   10 STORE_DEREF              1 (item)
                                   12 LOAD_GLOBAL              1 (NULL + any)
                                   24 LOAD_CLOSURE             1 (item)
                                   26 BUILD_TUPLE              1
-                                  28 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 749>)
+                                  28 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 881>)
                                   30 MAKE_FUNCTION            8 (closure)
                      
-                     750          32 LOAD_GLOBAL              2 (SUPPORTED_VIDEO_FORMATS)
+                     882          32 LOAD_GLOBAL              2 (SUPPORTED_VIDEO_FORMATS)
                      
-                     749          44 GET_ITER
+                     881          44 GET_ITER
                                   46 PRECALL                  0
                                   50 CALL                     0
                                   60 PRECALL                  1
                                   64 CALL                     1
                                   74 POP_JUMP_BACKWARD_IF_FALSE    34 (to 8)
                                   76 LOAD_DEREF               1 (item)
                                   78 LIST_APPEND              2
@@ -7375,148 +8600,147 @@
                            code
                               0x95014b00010097007c005d2b7d018902a0000000000000000000000000
                               000000000000000000a6000000ab000000000000000000a0010000000000
                               0000000000000000000000000000007c01a6010000ab0100000000000000
                               005600970101008c2c64005300
                                          0 COPY_FREE_VARS           1
                            
-                           749           2 RETURN_GENERATOR
+                           881           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                43 (to 98)
                            
-                           750          12 STORE_FAST               1 (ext)
+                           882          12 STORE_FAST               1 (ext)
                                         14 LOAD_DEREF               2 (item)
                                         16 LOAD_METHOD              0 (upper)
                                         38 PRECALL                  0
                                         42 CALL                     0
                                         52 LOAD_METHOD              1 (endswith)
                                         74 LOAD_FAST                1 (ext)
                                         76 PRECALL                  1
                                         80 CALL                     1
                            
-                           749          90 YIELD_VALUE
+                           881          90 YIELD_VALUE
                                         92 RESUME                   1
                                         94 POP_TOP
                                         96 JUMP_BACKWARD           44 (to 10)
                                    >>   98 LOAD_CONST               0 (None)
                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('upper', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                            name       '<genexpr>'
-                           firstlineno 749
+                           firstlineno 881
                            lnotab 0x0c014eff
                      names      ('any', 'SUPPORTED_VIDEO_FORMATS')
                      varnames   ('.0',)
                      freevars   ()
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 749
+                     firstlineno 881
                      lnotab 0x20010cff
-                  '\x1b[1;33mInitializing conversion..\x1b[0m'
+                  'Initializing conversion..'
                   '.'
                   'Unsupported output format'
                   1
                   'mpeg4'
                   'rawvideo'
                   'libvpx'
                   'MPEG4'
                   'flv'
                   ('MP4', 'AVI', 'WEBM', 'MOV', 'MKV', 'FLV')
-                  '\x1b[1;34mLoad file\x1b[0m'
-                  '\x1b[1;35mConverting file to '
-                  '\x1b[0m'
+                  'oad file'
+                  'Converting file to '
                   ('codec',)
-                  '\x1b[1;32mDone\x1b[0m'
+                  'Done'
                   '\nExiting..'
-               names      ('preprocess', 'out_format', 'upper', 'print', 'SUPPORTED_VIDEO_FORMATS', 'os', 'path', 'splitext', 'lower', 'sys', 'exit', 'VideoFileClip', 'write_videofile', 'close', 'KeyboardInterrupt', 'Exception')
+               names      ('preprocess', 'out_format', 'upper', 'print', 'DYELLOW', 'RESET', 'SUPPORTED_VIDEO_FORMATS', 'os', 'path', 'splitext', 'lower', 'sys', 'exit', 'DBLUE', 'VideoFileClip', 'DMAGENTA', 'write_videofile', 'DGREEN', 'close', 'KeyboardInterrupt', 'Exception')
                varnames   ('self', 'input_list', 'out_f', 'file', '_', 'ext', 'output_filename', 'format_codec', 'video', 'e')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'CONVERT_VIDEO'
-               firstlineno 745
+               firstlineno 877
                lnotab
-                  0x020102012801320118021e020a0136014401340120021e012802020102
-                  0202010201020102f9060a02011e011e0102012601180110ff120202011e
+                  0x020102012801320118023c020a0136014401340120021e012802020102
+                  0202010201020102f9060a02013c011e0102014001180110ff120202013c
                   012ce5061c12011e012e01120132ff
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'preprocess', 'CONVERT_VIDEO')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+         filename   '/media/skye/skye/FileMAC/filemac/converter.py'
          name       'VideoConverter'
-         firstlineno 723
+         firstlineno 855
          lnotab 0x0a0206040610
       'VideoConverter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             045300
-         793           0 RESUME                   0
+         925           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AudioConverter')
                        8 STORE_NAME               2 (__qualname__)
          
-         795          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 795>)
+         927          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/skye/FileMAC/filemac/converter.py", line 927>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-         799          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 799>)
+         931          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/skye/FileMAC/filemac/converter.py", line 931>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (preprocess)
          
-         815          22 LOAD_CONST               3 (<code object pydub_conv, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 815>)
+         947          22 LOAD_CONST               3 (<code object pydub_conv, file "/media/skye/skye/FileMAC/filemac/converter.py", line 947>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (pydub_conv)
                       28 LOAD_CONST               4 (None)
                       30 RETURN_VALUE
          consts
             'AudioConverter'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   0064005300
-               795           0 RESUME                   0
+               927           0 RESUME                   0
                
-               796           2 LOAD_FAST                1 (input_file)
+               928           2 LOAD_FAST                1 (input_file)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (input_file)
                
-               797          16 LOAD_FAST                2 (out_format)
+               929          16 LOAD_FAST                2 (out_format)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (out_format)
                             30 LOAD_CONST               0 (None)
                             32 RETURN_VALUE
                consts
                   None
                names      ('input_file', 'out_format')
                varnames   ('self', 'input_file', 'out_format')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       '__init__'
-               firstlineno 795
+               firstlineno 927
                lnotab 0x02010e01
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
@@ -7535,274 +8759,306 @@
                   010000ab01000000000000000044005d5b7d027400000000000000000000
                   006a010000000000000000a00a0000000000000000000000000000000000
                   0000007c006a0300000000000000007c02a6020000ab0200000000000000
                   007d037400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c03a6010000ab010000000000
                   00000072157c01a00400000000000000000000000000000000000000007c
                   03a6010000ab01000000000000000001008c5c7c015300
-               799           0 RESUME                   0
+               931           0 RESUME                   0
                
-               800           2 BUILD_LIST               0
+               932           2 BUILD_LIST               0
                              4 STORE_FAST               1 (files_to_process)
                
-               802           6 LOAD_GLOBAL              0 (os)
+               934           6 LOAD_GLOBAL              0 (os)
                             18 LOAD_ATTR                1 (path)
                             28 LOAD_METHOD              2 (isfile)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                3 (input_file)
                             62 PRECALL                  1
                             66 CALL                     1
                             76 POP_JUMP_FORWARD_IF_FALSE    27 (to 132)
                
-               803          78 LOAD_FAST                1 (files_to_process)
+               935          78 LOAD_FAST                1 (files_to_process)
                             80 LOAD_METHOD              4 (append)
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                3 (input_file)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                            130 JUMP_FORWARD           213 (to 558)
                
-               804     >>  132 LOAD_GLOBAL              0 (os)
+               936     >>  132 LOAD_GLOBAL              0 (os)
                            144 LOAD_ATTR                1 (path)
                            154 LOAD_METHOD              5 (isdir)
                            176 LOAD_FAST                0 (self)
                            178 LOAD_ATTR                3 (input_file)
                            188 PRECALL                  1
                            192 CALL                     1
                            202 POP_JUMP_FORWARD_IF_FALSE   177 (to 558)
                
-               805         204 LOAD_GLOBAL              1 (NULL + os)
+               937         204 LOAD_GLOBAL              1 (NULL + os)
                            216 LOAD_ATTR                6 (listdir)
                            226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                3 (input_file)
                            238 PRECALL                  1
                            242 CALL                     1
                            252 POP_JUMP_FORWARD_IF_NOT_NONE    35 (to 324)
                
-               806         254 LOAD_GLOBAL             15 (NULL + print)
+               938         254 LOAD_GLOBAL             15 (NULL + print)
                            266 LOAD_CONST               1 ('Cannot work with empty folder')
                            268 PRECALL                  1
                            272 CALL                     1
                            282 POP_TOP
                
-               807         284 LOAD_GLOBAL             17 (NULL + sys)
+               939         284 LOAD_GLOBAL             17 (NULL + sys)
                            296 LOAD_ATTR                9 (exit)
                            306 LOAD_CONST               2 (1)
                            308 PRECALL                  1
                            312 CALL                     1
                            322 POP_TOP
                
-               808     >>  324 LOAD_GLOBAL              1 (NULL + os)
+               940     >>  324 LOAD_GLOBAL              1 (NULL + os)
                            336 LOAD_ATTR                6 (listdir)
                            346 LOAD_FAST                0 (self)
                            348 LOAD_ATTR                3 (input_file)
                            358 PRECALL                  1
                            362 CALL                     1
                            372 GET_ITER
                        >>  374 FOR_ITER                91 (to 558)
                            376 STORE_FAST               2 (file)
                
-               809         378 LOAD_GLOBAL              0 (os)
+               941         378 LOAD_GLOBAL              0 (os)
                            390 LOAD_ATTR                1 (path)
                            400 LOAD_METHOD             10 (join)
                            422 LOAD_FAST                0 (self)
                            424 LOAD_ATTR                3 (input_file)
                            434 LOAD_FAST                2 (file)
                            436 PRECALL                  2
                            440 CALL                     2
                            450 STORE_FAST               3 (file_path)
                
-               810         452 LOAD_GLOBAL              0 (os)
+               942         452 LOAD_GLOBAL              0 (os)
                            464 LOAD_ATTR                1 (path)
                            474 LOAD_METHOD              2 (isfile)
                            496 LOAD_FAST                3 (file_path)
                            498 PRECALL                  1
                            502 CALL                     1
                            512 POP_JUMP_FORWARD_IF_FALSE    21 (to 556)
                
-               811         514 LOAD_FAST                1 (files_to_process)
+               943         514 LOAD_FAST                1 (files_to_process)
                            516 LOAD_METHOD              4 (append)
                            538 LOAD_FAST                3 (file_path)
                            540 PRECALL                  1
                            544 CALL                     1
                            554 POP_TOP
                        >>  556 JUMP_BACKWARD           92 (to 374)
                
-               813     >>  558 LOAD_FAST                1 (files_to_process)
+               945     >>  558 LOAD_FAST                1 (files_to_process)
                            560 RETURN_VALUE
                consts
                   None
                   'Cannot work with empty folder'
                   1
                names      ('os', 'path', 'isfile', 'input_file', 'append', 'isdir', 'listdir', 'print', 'sys', 'exit', 'join')
                varnames   ('self', 'files_to_process', 'file', 'file_path')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'preprocess'
-               firstlineno 799
+               firstlineno 931
                lnotab 0x0201040248013601480132011e01280136014a013e012c02
             code
                argcount  : 1
-               nlocals   : 8
-               stacksize : 6
+               nlocals   : 9
+               stacksize : 7
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d017c006a0100000000000000007d02640184
                   007c014400a6000000ab0000000000000000007d01740500000000000000
-                  0000006402a6010000ab01000000000000000001007c0144005dc37d037c
-                  02a0030000000000000000000000000000000000000000a6000000ab0000
-                  000000000000007408000000000000000000007600722b740a0000000000
-                  00000000006a060000000000000000a00700000000000000000000000000
+                  0000007406000000000000000000009b0064027408000000000000000000
+                  009b009d03a6010000ab01000000000000000001007c0144005dfa7d037c
+                  02a0050000000000000000000000000000000000000000a6000000ab0000
+                  00000000000000740c000000000000000000007600722b740e0000000000
+                  00000000006a080000000000000000a00900000000000000000000000000
                   000000000000007c03a6010000ab0100000000000000005c0200007d047d
                   057c0464037a0000007c027a0000007d066e237405000000000000000000
-                  006404a6010000ab01000000000000000001007411000000000000000000
-                  006a0900000000000000006405a6010000ab010000000000000000010074
-                  14000000000000000000006a0b0000000000000000a00c00000000000000
-                  000000000000000000000000007c03a6010000ab0100000000000000007d
-                  0774050000000000000000000064067c069b0064079d03a6010000ab0100
-                  0000000000000001007c07a00d0000000000000000000000000000000000
-                  0000007c067c02ac08a6020000ab02000000000000000001007405000000
-                  000000000000006409a6010000ab01000000000000000001008cc4640053
-                  00
-               815           0 RESUME                   0
+                  006404a6010000ab01000000000000000001007415000000000000000000
+                  006a0b00000000000000006405a6010000ab01000000000000000001007c
+                  05640564008502190000000000000000007d077405000000000000000000
+                  007c077c02a6020000ab0200000000000000000100741800000000000000
+                  0000006a0d0000000000000000a00e000000000000000000000000000000
+                  00000000007c037c07a6020000ab0200000000000000007d087405000000
+                  00000000000000741e000000000000000000009b0064067c069b00740800
+                  0000000000000000009b009d04a6010000ab01000000000000000001007c
+                  08a01000000000000000000000000000000000000000007c067c02ac07a6
+                  020000ab0200000000000000000100740500000000000000000000742200
+                  0000000000000000009b0064087408000000000000000000009b009d03a6
+                  010000ab01000000000000000001008cfb64005300
+               947           0 RESUME                   0
                
-               816           2 LOAD_FAST                0 (self)
+               948           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (preprocess)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (input_list)
                
-               817          42 LOAD_FAST                0 (self)
+               949          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                1 (out_format)
                             54 STORE_FAST               2 (out_f)
                
-               818          56 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 818>)
+               950          56 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 950>)
                             58 MAKE_FUNCTION            0
                             60 LOAD_FAST                1 (input_list)
                             62 GET_ITER
                             64 PRECALL                  0
                             68 CALL                     0
                             78 STORE_FAST               1 (input_list)
                
-               820          80 LOAD_GLOBAL              5 (NULL + print)
-                            92 LOAD_CONST               2 ('\x1b[1;33mInitializing conversion..\x1b[0m')
-                            94 PRECALL                  1
-                            98 CALL                     1
-                           108 POP_TOP
+               952          80 LOAD_GLOBAL              5 (NULL + print)
+                            92 LOAD_GLOBAL              6 (DYELLOW)
+                           104 FORMAT_VALUE             0
+                           106 LOAD_CONST               2 ('Initializing conversion..')
+                           108 LOAD_GLOBAL              8 (RESET)
+                           120 FORMAT_VALUE             0
+                           122 BUILD_STRING             3
+                           124 PRECALL                  1
+                           128 CALL                     1
+                           138 POP_TOP
+               
+               953         140 LOAD_FAST                1 (input_list)
+                           142 GET_ITER
+                       >>  144 FOR_ITER               250 (to 646)
+                           146 STORE_FAST               3 (file)
+               
+               954         148 LOAD_FAST                2 (out_f)
+                           150 LOAD_METHOD              5 (lower)
+                           172 PRECALL                  0
+                           176 CALL                     0
+                           186 LOAD_GLOBAL             12 (SUPPORTED_AUDIO_FORMATS)
+                           198 CONTAINS_OP              0
+                           200 POP_JUMP_FORWARD_IF_FALSE    43 (to 288)
+               
+               955         202 LOAD_GLOBAL             14 (os)
+                           214 LOAD_ATTR                8 (path)
+                           224 LOAD_METHOD              9 (splitext)
+                           246 LOAD_FAST                3 (file)
+                           248 PRECALL                  1
+                           252 CALL                     1
+                           262 UNPACK_SEQUENCE          2
+                           266 STORE_FAST               4 (_)
+                           268 STORE_FAST               5 (ext)
+               
+               956         270 LOAD_FAST                4 (_)
+                           272 LOAD_CONST               3 ('.')
+                           274 BINARY_OP                0 (+)
+                           278 LOAD_FAST                2 (out_f)
+                           280 BINARY_OP                0 (+)
+                           284 STORE_FAST               6 (output_filename)
+                           286 JUMP_FORWARD            35 (to 358)
                
-               821         110 LOAD_FAST                1 (input_list)
-                           112 GET_ITER
-                       >>  114 FOR_ITER               195 (to 506)
-                           116 STORE_FAST               3 (file)
-               
-               822         118 LOAD_FAST                2 (out_f)
-                           120 LOAD_METHOD              3 (lower)
-                           142 PRECALL                  0
-                           146 CALL                     0
-                           156 LOAD_GLOBAL              8 (SUPPORTED_AUDIO_FORMATS)
-                           168 CONTAINS_OP              0
-                           170 POP_JUMP_FORWARD_IF_FALSE    43 (to 258)
-               
-               823         172 LOAD_GLOBAL             10 (os)
-                           184 LOAD_ATTR                6 (path)
-                           194 LOAD_METHOD              7 (splitext)
-                           216 LOAD_FAST                3 (file)
-                           218 PRECALL                  1
-                           222 CALL                     1
-                           232 UNPACK_SEQUENCE          2
-                           236 STORE_FAST               4 (_)
-                           238 STORE_FAST               5 (ext)
-               
-               824         240 LOAD_FAST                4 (_)
-                           242 LOAD_CONST               3 ('.')
-                           244 BINARY_OP                0 (+)
-                           248 LOAD_FAST                2 (out_f)
-                           250 BINARY_OP                0 (+)
-                           254 STORE_FAST               6 (output_filename)
-                           256 JUMP_FORWARD            35 (to 328)
-               
-               826     >>  258 LOAD_GLOBAL              5 (NULL + print)
-                           270 LOAD_CONST               4 ('Unsupported output format')
-                           272 PRECALL                  1
-                           276 CALL                     1
-                           286 POP_TOP
-               
-               827         288 LOAD_GLOBAL             17 (NULL + sys)
-                           300 LOAD_ATTR                9 (exit)
-                           310 LOAD_CONST               5 (1)
-                           312 PRECALL                  1
-                           316 CALL                     1
-                           326 POP_TOP
-               
-               828     >>  328 LOAD_GLOBAL             20 (pydub)
-                           340 LOAD_ATTR               11 (AudioSegment)
-                           350 LOAD_METHOD             12 (from_file)
-                           372 LOAD_FAST                3 (file)
-                           374 PRECALL                  1
-                           378 CALL                     1
-                           388 STORE_FAST               7 (audio)
-               
-               829         390 LOAD_GLOBAL              5 (NULL + print)
-                           402 LOAD_CONST               6 ('\x1b[1;35mConverting to ')
-                           404 LOAD_FAST                6 (output_filename)
-                           406 FORMAT_VALUE             0
-                           408 LOAD_CONST               7 ('\x1b[0m')
-                           410 BUILD_STRING             3
-                           412 PRECALL                  1
-                           416 CALL                     1
-                           426 POP_TOP
+               958     >>  288 LOAD_GLOBAL              5 (NULL + print)
+                           300 LOAD_CONST               4 ('Unsupported output format')
+                           302 PRECALL                  1
+                           306 CALL                     1
+                           316 POP_TOP
+               
+               959         318 LOAD_GLOBAL             21 (NULL + sys)
+                           330 LOAD_ATTR               11 (exit)
+                           340 LOAD_CONST               5 (1)
+                           342 PRECALL                  1
+                           346 CALL                     1
+                           356 POP_TOP
+               
+               960     >>  358 LOAD_FAST                5 (ext)
+                           360 LOAD_CONST               5 (1)
+                           362 LOAD_CONST               0 (None)
+                           364 BUILD_SLICE              2
+                           366 BINARY_SUBSCR
+                           376 STORE_FAST               7 (fmt)
+               
+               961         378 LOAD_GLOBAL              5 (NULL + print)
+                           390 LOAD_FAST                7 (fmt)
+                           392 LOAD_FAST                2 (out_f)
+                           394 PRECALL                  2
+                           398 CALL                     2
+                           408 POP_TOP
                
-               830         428 LOAD_FAST                7 (audio)
-                           430 LOAD_METHOD             13 (export)
-                           452 LOAD_FAST                6 (output_filename)
-                           454 LOAD_FAST                2 (out_f)
-                           456 KW_NAMES                 8
+               962         410 LOAD_GLOBAL             24 (pydub)
+                           422 LOAD_ATTR               13 (AudioSegment)
+                           432 LOAD_METHOD             14 (from_file)
+                           454 LOAD_FAST                3 (file)
+                           456 LOAD_FAST                7 (fmt)
                            458 PRECALL                  2
                            462 CALL                     2
-                           472 POP_TOP
+                           472 STORE_FAST               8 (audio)
                
-               832         474 LOAD_GLOBAL              5 (NULL + print)
-                           486 LOAD_CONST               9 ('\x1b[1;32mDone\x1b[0m')
-                           488 PRECALL                  1
-                           492 CALL                     1
-                           502 POP_TOP
-                           504 JUMP_BACKWARD          196 (to 114)
+               963         474 LOAD_GLOBAL              5 (NULL + print)
+                           486 LOAD_GLOBAL             30 (DMAGENTA)
+                           498 FORMAT_VALUE             0
+                           500 LOAD_CONST               6 ('Converting to ')
+                           502 LOAD_FAST                6 (output_filename)
+                           504 FORMAT_VALUE             0
+                           506 LOAD_GLOBAL              8 (RESET)
+                           518 FORMAT_VALUE             0
+                           520 BUILD_STRING             4
+                           522 PRECALL                  1
+                           526 CALL                     1
+                           536 POP_TOP
+               
+               964         538 LOAD_FAST                8 (audio)
+                           540 LOAD_METHOD             16 (export)
+                           562 LOAD_FAST                6 (output_filename)
+                           564 LOAD_FAST                2 (out_f)
+                           566 KW_NAMES                 7
+                           568 PRECALL                  2
+                           572 CALL                     2
+                           582 POP_TOP
+               
+               966         584 LOAD_GLOBAL              5 (NULL + print)
+                           596 LOAD_GLOBAL             34 (DGREEN)
+                           608 FORMAT_VALUE             0
+                           610 LOAD_CONST               8 ('Done')
+                           612 LOAD_GLOBAL              8 (RESET)
+                           624 FORMAT_VALUE             0
+                           626 BUILD_STRING             3
+                           628 PRECALL                  1
+                           632 CALL                     1
+                           642 POP_TOP
+                           644 JUMP_BACKWARD          251 (to 144)
                
-               821     >>  506 LOAD_CONST               0 (None)
-                           508 RETURN_VALUE
+               953     >>  646 LOAD_CONST               0 (None)
+                           648 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 6
                      flags     : 19
                      code
                         0x8701970067007c005d248a017401000000000000000000008801660164
                         0084087402000000000000000000004400a6000000ab0000000000000000
                         00a6010000ab010000000000000000af22890191028c255300
                                    0 MAKE_CELL                1 (item)
                      
-                     818           2 RESUME                   0
+                     950           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                36 (to 82)
                                   10 STORE_DEREF              1 (item)
                                   12 LOAD_GLOBAL              1 (NULL + any)
                                   24 LOAD_CLOSURE             1 (item)
                                   26 BUILD_TUPLE              1
-                                  28 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 818>)
+                                  28 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 950>)
                                   30 MAKE_FUNCTION            8 (closure)
                      
-                     819          32 LOAD_GLOBAL              2 (SUPPORTED_AUDIO_FORMATS)
+                     951          32 LOAD_GLOBAL              2 (SUPPORTED_AUDIO_FORMATS)
                      
-                     818          44 GET_ITER
+                     950          44 GET_ITER
                                   46 PRECALL                  0
                                   50 CALL                     0
                                   60 PRECALL                  1
                                   64 CALL                     1
                                   74 POP_JUMP_BACKWARD_IF_FALSE    34 (to 8)
                                   76 LOAD_DEREF               1 (item)
                                   78 LIST_APPEND              2
@@ -7817,139 +9073,138 @@
                            code
                               0x95014b00010097007c005d2b7d018902a0000000000000000000000000
                               000000000000000000a6000000ab000000000000000000a0010000000000
                               0000000000000000000000000000007c01a6010000ab0100000000000000
                               005600970101008c2c64005300
                                          0 COPY_FREE_VARS           1
                            
-                           818           2 RETURN_GENERATOR
+                           950           2 RETURN_GENERATOR
                                          4 POP_TOP
                                          6 RESUME                   0
                                          8 LOAD_FAST                0 (.0)
                                    >>   10 FOR_ITER                43 (to 98)
                            
-                           819          12 STORE_FAST               1 (ext)
+                           951          12 STORE_FAST               1 (ext)
                                         14 LOAD_DEREF               2 (item)
                                         16 LOAD_METHOD              0 (lower)
                                         38 PRECALL                  0
                                         42 CALL                     0
                                         52 LOAD_METHOD              1 (endswith)
                                         74 LOAD_FAST                1 (ext)
                                         76 PRECALL                  1
                                         80 CALL                     1
                            
-                           818          90 YIELD_VALUE
+                           950          90 YIELD_VALUE
                                         92 RESUME                   1
                                         94 POP_TOP
                                         96 JUMP_BACKWARD           44 (to 10)
                                    >>   98 LOAD_CONST               0 (None)
                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('lower', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                            name       '<genexpr>'
-                           firstlineno 818
+                           firstlineno 950
                            lnotab 0x0c014eff
                      names      ('any', 'SUPPORTED_AUDIO_FORMATS')
                      varnames   ('.0',)
                      freevars   ()
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 818
+                     firstlineno 950
                      lnotab 0x20010cff
-                  '\x1b[1;33mInitializing conversion..\x1b[0m'
+                  'Initializing conversion..'
                   '.'
                   'Unsupported output format'
                   1
-                  '\x1b[1;35mConverting to '
-                  '\x1b[0m'
+                  'Converting to '
                   ('format',)
-                  '\x1b[1;32mDone\x1b[0m'
-               names      ('preprocess', 'out_format', 'print', 'lower', 'SUPPORTED_AUDIO_FORMATS', 'os', 'path', 'splitext', 'sys', 'exit', 'pydub', 'AudioSegment', 'from_file', 'export')
-               varnames   ('self', 'input_list', 'out_f', 'file', '_', 'ext', 'output_filename', 'audio')
+                  'Done'
+               names      ('preprocess', 'out_format', 'print', 'DYELLOW', 'RESET', 'lower', 'SUPPORTED_AUDIO_FORMATS', 'os', 'path', 'splitext', 'sys', 'exit', 'pydub', 'AudioSegment', 'from_file', 'DMAGENTA', 'export', 'DGREEN')
+               varnames   ('self', 'input_list', 'out_f', 'file', '_', 'ext', 'output_filename', 'fmt', 'audio')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'pydub_conv'
-               firstlineno 815
+               firstlineno 947
                lnotab
-                  0x020128010e0118021e0108013601440112021e0128013e0126012e0220
-                  f5
+                  0x020128010e0118023c0108013601440112021e01280114012001400140
+                  012e023ef3
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'preprocess', 'pydub_conv')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+         filename   '/media/skye/skye/FileMAC/filemac/converter.py'
          name       'AudioConverter'
-         firstlineno 793
+         firstlineno 925
          lnotab 0x0a0206040610
       'AudioConverter'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             045300
-         842           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('ImageConverter')
-                       8 STORE_NAME               2 (__qualname__)
+          976           0 RESUME                   0
+                        2 LOAD_NAME                0 (__name__)
+                        4 STORE_NAME               1 (__module__)
+                        6 LOAD_CONST               0 ('ImageConverter')
+                        8 STORE_NAME               2 (__qualname__)
          
-         844          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 844>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (__init__)
+          978          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/skye/FileMAC/filemac/converter.py", line 978>)
+                       12 MAKE_FUNCTION            0
+                       14 STORE_NAME               3 (__init__)
          
-         848          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 848>)
-                      18 MAKE_FUNCTION            0
-                      20 STORE_NAME               4 (preprocess)
+          982          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/skye/FileMAC/filemac/converter.py", line 982>)
+                       18 MAKE_FUNCTION            0
+                       20 STORE_NAME               4 (preprocess)
          
-         868          22 LOAD_CONST               3 (<code object convert_image, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 868>)
-                      24 MAKE_FUNCTION            0
-                      26 STORE_NAME               5 (convert_image)
-                      28 LOAD_CONST               4 (None)
-                      30 RETURN_VALUE
+         1002          22 LOAD_CONST               3 (<code object convert_image, file "/media/skye/skye/FileMAC/filemac/converter.py", line 1002>)
+                       24 MAKE_FUNCTION            0
+                       26 STORE_NAME               5 (convert_image)
+                       28 LOAD_CONST               4 (None)
+                       30 RETURN_VALUE
          consts
             'ImageConverter'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code
                   0x97007c017c005f0000000000000000007c027c005f0100000000000000
                   0064005300
-               844           0 RESUME                   0
+               978           0 RESUME                   0
                
-               845           2 LOAD_FAST                1 (input_file)
+               979           2 LOAD_FAST                1 (input_file)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (input_file)
                
-               846          16 LOAD_FAST                2 (out_format)
+               980          16 LOAD_FAST                2 (out_format)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (out_format)
                             30 LOAD_CONST               0 (None)
                             32 RETURN_VALUE
                consts
                   None
                names      ('input_file', 'out_format')
                varnames   ('self', 'input_file', 'out_format')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       '__init__'
-               firstlineno 844
+               firstlineno 978
                lnotab 0x02010e01
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
@@ -7972,546 +9227,570 @@
                   000000000000000000000000000000000000007c03a6010000ab01000000
                   000000000072157c01a00400000000000000000000000000000000000000
                   007c03a6010000ab01000000000000000001008c5c7c0153002300741600
                   000000000000000000240072270100740f000000000000000000006403a6
                   010000ab01000000000000000001007411000000000000000000006a0900
                   000000000000006402a6010000ab01000000000000000001005900640053
                   007700780359007701
-               848           0 RESUME                   0
-               
-               849           2 NOP
-               
-               850           4 BUILD_LIST               0
-                             6 STORE_FAST               1 (files_to_process)
-               
-               852           8 LOAD_GLOBAL              0 (os)
-                            20 LOAD_ATTR                1 (path)
-                            30 LOAD_METHOD              2 (isfile)
-                            52 LOAD_FAST                0 (self)
-                            54 LOAD_ATTR                3 (input_file)
-                            64 PRECALL                  1
-                            68 CALL                     1
-                            78 POP_JUMP_FORWARD_IF_FALSE    27 (to 134)
-               
-               853          80 LOAD_FAST                1 (files_to_process)
-                            82 LOAD_METHOD              4 (append)
-                           104 LOAD_FAST                0 (self)
-                           106 LOAD_ATTR                3 (input_file)
-                           116 PRECALL                  1
-                           120 CALL                     1
-                           130 POP_TOP
-                           132 JUMP_FORWARD           213 (to 560)
-               
-               854     >>  134 LOAD_GLOBAL              0 (os)
-                           146 LOAD_ATTR                1 (path)
-                           156 LOAD_METHOD              5 (isdir)
-                           178 LOAD_FAST                0 (self)
-                           180 LOAD_ATTR                3 (input_file)
-                           190 PRECALL                  1
-                           194 CALL                     1
-                           204 POP_JUMP_FORWARD_IF_FALSE   177 (to 560)
-               
-               855         206 LOAD_GLOBAL              1 (NULL + os)
-                           218 LOAD_ATTR                6 (listdir)
-                           228 LOAD_FAST                0 (self)
-                           230 LOAD_ATTR                3 (input_file)
-                           240 PRECALL                  1
-                           244 CALL                     1
-                           254 POP_JUMP_FORWARD_IF_NOT_NONE    35 (to 326)
-               
-               856         256 LOAD_GLOBAL             15 (NULL + print)
-                           268 LOAD_CONST               1 ('Cannot work with empty folder')
-                           270 PRECALL                  1
-                           274 CALL                     1
-                           284 POP_TOP
-               
-               857         286 LOAD_GLOBAL             17 (NULL + sys)
-                           298 LOAD_ATTR                9 (exit)
-                           308 LOAD_CONST               2 (1)
-                           310 PRECALL                  1
-                           314 CALL                     1
-                           324 POP_TOP
-               
-               858     >>  326 LOAD_GLOBAL              1 (NULL + os)
-                           338 LOAD_ATTR                6 (listdir)
-                           348 LOAD_FAST                0 (self)
-                           350 LOAD_ATTR                3 (input_file)
-                           360 PRECALL                  1
-                           364 CALL                     1
-                           374 GET_ITER
-                       >>  376 FOR_ITER                91 (to 560)
-                           378 STORE_FAST               2 (file)
-               
-               859         380 LOAD_GLOBAL              0 (os)
-                           392 LOAD_ATTR                1 (path)
-                           402 LOAD_METHOD             10 (join)
-                           424 LOAD_FAST                0 (self)
-                           426 LOAD_ATTR                3 (input_file)
-                           436 LOAD_FAST                2 (file)
-                           438 PRECALL                  2
-                           442 CALL                     2
-                           452 STORE_FAST               3 (file_path)
-               
-               860         454 LOAD_GLOBAL              0 (os)
-                           466 LOAD_ATTR                1 (path)
-                           476 LOAD_METHOD              2 (isfile)
-                           498 LOAD_FAST                3 (file_path)
-                           500 PRECALL                  1
-                           504 CALL                     1
-                           514 POP_JUMP_FORWARD_IF_FALSE    21 (to 558)
-               
-               861         516 LOAD_FAST                1 (files_to_process)
-                           518 LOAD_METHOD              4 (append)
-                           540 LOAD_FAST                3 (file_path)
-                           542 PRECALL                  1
-                           546 CALL                     1
-                           556 POP_TOP
-                       >>  558 JUMP_BACKWARD           92 (to 376)
+                982           0 RESUME                   0
                
-               863     >>  560 LOAD_FAST                1 (files_to_process)
-                           562 RETURN_VALUE
-                       >>  564 PUSH_EXC_INFO
+                983           2 NOP
                
-               864         566 LOAD_GLOBAL             22 (FileNotFoundError)
-                           578 CHECK_EXC_MATCH
-                           580 POP_JUMP_FORWARD_IF_FALSE    39 (to 660)
-                           582 POP_TOP
-               
-               865         584 LOAD_GLOBAL             15 (NULL + print)
-                           596 LOAD_CONST               3 ('File not found')
-                           598 PRECALL                  1
-                           602 CALL                     1
-                           612 POP_TOP
+                984           4 BUILD_LIST               0
+                              6 STORE_FAST               1 (files_to_process)
                
-               866         614 LOAD_GLOBAL             17 (NULL + sys)
-                           626 LOAD_ATTR                9 (exit)
-                           636 LOAD_CONST               2 (1)
-                           638 PRECALL                  1
-                           642 CALL                     1
-                           652 POP_TOP
-                           654 POP_EXCEPT
-                           656 LOAD_CONST               0 (None)
-                           658 RETURN_VALUE
-               
-               864     >>  660 RERAISE                  0
-                       >>  662 COPY                     3
-                           664 POP_EXCEPT
-                           666 RERAISE                  1
+                986           8 LOAD_GLOBAL              0 (os)
+                             20 LOAD_ATTR                1 (path)
+                             30 LOAD_METHOD              2 (isfile)
+                             52 LOAD_FAST                0 (self)
+                             54 LOAD_ATTR                3 (input_file)
+                             64 PRECALL                  1
+                             68 CALL                     1
+                             78 POP_JUMP_FORWARD_IF_FALSE    27 (to 134)
+               
+                987          80 LOAD_FAST                1 (files_to_process)
+                             82 LOAD_METHOD              4 (append)
+                            104 LOAD_FAST                0 (self)
+                            106 LOAD_ATTR                3 (input_file)
+                            116 PRECALL                  1
+                            120 CALL                     1
+                            130 POP_TOP
+                            132 JUMP_FORWARD           213 (to 560)
+               
+                988     >>  134 LOAD_GLOBAL              0 (os)
+                            146 LOAD_ATTR                1 (path)
+                            156 LOAD_METHOD              5 (isdir)
+                            178 LOAD_FAST                0 (self)
+                            180 LOAD_ATTR                3 (input_file)
+                            190 PRECALL                  1
+                            194 CALL                     1
+                            204 POP_JUMP_FORWARD_IF_FALSE   177 (to 560)
+               
+                989         206 LOAD_GLOBAL              1 (NULL + os)
+                            218 LOAD_ATTR                6 (listdir)
+                            228 LOAD_FAST                0 (self)
+                            230 LOAD_ATTR                3 (input_file)
+                            240 PRECALL                  1
+                            244 CALL                     1
+                            254 POP_JUMP_FORWARD_IF_NOT_NONE    35 (to 326)
+               
+                990         256 LOAD_GLOBAL             15 (NULL + print)
+                            268 LOAD_CONST               1 ('Cannot work with empty folder')
+                            270 PRECALL                  1
+                            274 CALL                     1
+                            284 POP_TOP
+               
+                991         286 LOAD_GLOBAL             17 (NULL + sys)
+                            298 LOAD_ATTR                9 (exit)
+                            308 LOAD_CONST               2 (1)
+                            310 PRECALL                  1
+                            314 CALL                     1
+                            324 POP_TOP
+               
+                992     >>  326 LOAD_GLOBAL              1 (NULL + os)
+                            338 LOAD_ATTR                6 (listdir)
+                            348 LOAD_FAST                0 (self)
+                            350 LOAD_ATTR                3 (input_file)
+                            360 PRECALL                  1
+                            364 CALL                     1
+                            374 GET_ITER
+                        >>  376 FOR_ITER                91 (to 560)
+                            378 STORE_FAST               2 (file)
+               
+                993         380 LOAD_GLOBAL              0 (os)
+                            392 LOAD_ATTR                1 (path)
+                            402 LOAD_METHOD             10 (join)
+                            424 LOAD_FAST                0 (self)
+                            426 LOAD_ATTR                3 (input_file)
+                            436 LOAD_FAST                2 (file)
+                            438 PRECALL                  2
+                            442 CALL                     2
+                            452 STORE_FAST               3 (file_path)
+               
+                994         454 LOAD_GLOBAL              0 (os)
+                            466 LOAD_ATTR                1 (path)
+                            476 LOAD_METHOD              2 (isfile)
+                            498 LOAD_FAST                3 (file_path)
+                            500 PRECALL                  1
+                            504 CALL                     1
+                            514 POP_JUMP_FORWARD_IF_FALSE    21 (to 558)
+               
+                995         516 LOAD_FAST                1 (files_to_process)
+                            518 LOAD_METHOD              4 (append)
+                            540 LOAD_FAST                3 (file_path)
+                            542 PRECALL                  1
+                            546 CALL                     1
+                            556 POP_TOP
+                        >>  558 JUMP_BACKWARD           92 (to 376)
+               
+                997     >>  560 LOAD_FAST                1 (files_to_process)
+                            562 RETURN_VALUE
+                        >>  564 PUSH_EXC_INFO
+               
+                998         566 LOAD_GLOBAL             22 (FileNotFoundError)
+                            578 CHECK_EXC_MATCH
+                            580 POP_JUMP_FORWARD_IF_FALSE    39 (to 660)
+                            582 POP_TOP
+               
+                999         584 LOAD_GLOBAL             15 (NULL + print)
+                            596 LOAD_CONST               3 ('File not found')
+                            598 PRECALL                  1
+                            602 CALL                     1
+                            612 POP_TOP
+               
+               1000         614 LOAD_GLOBAL             17 (NULL + sys)
+                            626 LOAD_ATTR                9 (exit)
+                            636 LOAD_CONST               2 (1)
+                            638 PRECALL                  1
+                            642 CALL                     1
+                            652 POP_TOP
+                            654 POP_EXCEPT
+                            656 LOAD_CONST               0 (None)
+                            658 RETURN_VALUE
+               
+                998     >>  660 RERAISE                  0
+                        >>  662 COPY                     3
+                            664 POP_EXCEPT
+                            666 RERAISE                  1
                ExceptionTable:
                  4 to 560 -> 564 [0]
                  564 to 652 -> 662 [1] lasti
                  660 to 660 -> 662 [1] lasti
                consts
                   None
                   'Cannot work with empty folder'
                   1
                   'File not found'
                names      ('os', 'path', 'isfile', 'input_file', 'append', 'isdir', 'listdir', 'print', 'sys', 'exit', 'join', 'FileNotFoundError')
                varnames   ('self', 'files_to_process', 'file', 'file_path')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'preprocess'
-               firstlineno 848
+               firstlineno 982
                lnotab
                   0x02010201040248013601480132011e01280136014a013e012c02060112
                   011e012efe
             code
                argcount  : 1
                nlocals   : 9
                stacksize : 7
                flags     : 3
                code
                   0x8709970009007c00a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007d017c006a010000000000000000a0
                   020000000000000000000000000000000000000000a6000000ab00000000
                   00000000008a0988096601640184087c014400a6000000ab000000000000
-                  0000007d017c01440090015d957d027407000000000000000000007c02a6
+                  0000007d017c01440090015dd77d027407000000000000000000007c02a6
                   010000ab01000000000000000001008909a0020000000000000000000000
                   000000000000000000a6000000ab00000000000000000074080000000000
                   000000000076007245740a000000000000000000006a0600000000000000
                   00a00700000000000000000000000000000000000000007c02a6010000ab
                   0100000000000000005c0200007d037d047c037408000000000000000000
                   00890919000000000000000000a008000000000000000000000000000000
                   0000000000a6000000ab0000000000000000007a0000007d056e23740700
                   0000000000000000006402a6010000ab0100000000000000000100741300
                   0000000000000000006a0a00000000000000006403a6010000ab01000000
-                  0000000000010009007407000000000000000000006404a6010000ab0100
-                  0000000000000001007417000000000000000000006a0c00000000000000
+                  000000000001000900740700000000000000000000741600000000000000
+                  0000009b0064047418000000000000000000009b009d03a6010000ab0100
+                  000000000000000100741b000000000000000000006a0e00000000000000
                   007c02a6010000ab0100000000000000007d060900740700000000000000
-                  0000006405a6010000ab0100000000000000000100741b00000000000000
-                  0000006a0e00000000000000007417000000000000000000006a0f000000
-                  00000000007c067416000000000000000000006a100000000000000000a6
+                  000000741e000000000000000000009b0064057418000000000000000000
+                  009b009d03a6010000ab0100000000000000000100742100000000000000
+                  0000006a110000000000000000741b000000000000000000006a12000000
+                  00000000007c06741a000000000000000000006a130000000000000000a6
                   020000ab020000000000000000a6010000ab0100000000000000007d0709
-                  0074070000000000000000000064067c059b0064079d03a6010000ab0100
-                  0000000000000001007c07a0110000000000000000000000000000000000
-                  0000007c058909a6020000ab020000000000000000010074070000000000
-                  00000000006408a6010000ab010000000000000000010009007407000000
-                  000000000000006409a6010000ab01000000000000000001007417000000
-                  000000000000006a0c00000000000000007c05a6010000ab010000000000
-                  0000007d0809007417000000000000000000006a12000000000000000064
-                  0a7c08a6020000ab02000000000000000001000900741700000000000000
-                  0000006a130000000000000000640ba6010000ab01000000000000000001
-                  007417000000000000000000006a140000000000000000a6000000ab0000
-                  00000000000000010090018c97640053002300742a000000000000000000
-                  00240072270100740700000000000000000000640ca6010000ab01000000
-                  000000000001007413000000000000000000006a0a000000000000000064
-                  03a6010000ab010000000000000000010059006400530077007803590077
-                  01
-                             0 MAKE_CELL                9 (out_f)
-               
-               868           2 RESUME                   0
-               
-               869           4 NOP
-               
-               870           6 LOAD_FAST                0 (self)
-                             8 LOAD_METHOD              0 (preprocess)
-                            30 PRECALL                  0
-                            34 CALL                     0
-                            44 STORE_FAST               1 (input_list)
-               
-               871          46 LOAD_FAST                0 (self)
-                            48 LOAD_ATTR                1 (out_format)
-                            58 LOAD_METHOD              2 (upper)
-                            80 PRECALL                  0
-                            84 CALL                     0
-                            94 STORE_DEREF              9 (out_f)
-               
-               873          96 LOAD_CLOSURE             9 (out_f)
-                            98 BUILD_TUPLE              1
-                           100 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 873>)
-                           102 MAKE_FUNCTION            8 (closure)
-                           104 LOAD_FAST                1 (input_list)
-                           106 GET_ITER
-                           108 PRECALL                  0
-                           112 CALL                     0
-                           122 STORE_FAST               1 (input_list)
-               
-               875         124 LOAD_FAST                1 (input_list)
-                           126 GET_ITER
-                       >>  128 EXTENDED_ARG             1
-                           130 FOR_ITER               405 (to 942)
-                           132 STORE_FAST               2 (file)
-               
-               876         134 LOAD_GLOBAL              7 (NULL + print)
-                           146 LOAD_FAST                2 (file)
-                           148 PRECALL                  1
-                           152 CALL                     1
-                           162 POP_TOP
-               
-               877         164 LOAD_DEREF               9 (out_f)
-                           166 LOAD_METHOD              2 (upper)
-                           188 PRECALL                  0
-                           192 CALL                     0
-                           202 LOAD_GLOBAL              8 (SUPPORTED_IMAGE_FORMATS)
-                           214 CONTAINS_OP              0
-                           216 POP_JUMP_FORWARD_IF_FALSE    69 (to 356)
-               
-               878         218 LOAD_GLOBAL             10 (os)
-                           230 LOAD_ATTR                6 (path)
-                           240 LOAD_METHOD              7 (splitext)
-                           262 LOAD_FAST                2 (file)
-                           264 PRECALL                  1
-                           268 CALL                     1
-                           278 UNPACK_SEQUENCE          2
-                           282 STORE_FAST               3 (_)
-                           284 STORE_FAST               4 (ext)
-               
-               879         286 LOAD_FAST                3 (_)
-               
-               880         288 LOAD_GLOBAL              8 (SUPPORTED_IMAGE_FORMATS)
-                           300 LOAD_DEREF               9 (out_f)
-                           302 BINARY_SUBSCR
-                           312 LOAD_METHOD              8 (lower)
-                           334 PRECALL                  0
-                           338 CALL                     0
-               
-               879         348 BINARY_OP                0 (+)
-                           352 STORE_FAST               5 (output_filename)
-                           354 JUMP_FORWARD            35 (to 426)
-               
-               882     >>  356 LOAD_GLOBAL              7 (NULL + print)
-                           368 LOAD_CONST               2 ('Unsupported output format')
-                           370 PRECALL                  1
-                           374 CALL                     1
-                           384 POP_TOP
-               
-               883         386 LOAD_GLOBAL             19 (NULL + sys)
-                           398 LOAD_ATTR               10 (exit)
-                           408 LOAD_CONST               3 (1)
-                           410 PRECALL                  1
-                           414 CALL                     1
-                           424 POP_TOP
-               
-               884     >>  426 NOP
-               
-               885         428 LOAD_GLOBAL              7 (NULL + print)
-                           440 LOAD_CONST               4 ('\x1b[1;33mReading input image..\x1b[0m')
-                           442 PRECALL                  1
-                           446 CALL                     1
-                           456 POP_TOP
-               
-               886         458 LOAD_GLOBAL             23 (NULL + cv2)
-                           470 LOAD_ATTR               12 (imread)
-                           480 LOAD_FAST                2 (file)
-                           482 PRECALL                  1
-                           486 CALL                     1
-                           496 STORE_FAST               6 (img)
-               
-               887         498 NOP
-               
-               888         500 LOAD_GLOBAL              7 (NULL + print)
-                           512 LOAD_CONST               5 ('\x1b[1;35mConverting to PIL image\x1b[0m')
-                           514 PRECALL                  1
-                           518 CALL                     1
-                           528 POP_TOP
-               
-               889         530 LOAD_GLOBAL             27 (NULL + Image)
-                           542 LOAD_ATTR               14 (fromarray)
-                           552 LOAD_GLOBAL             23 (NULL + cv2)
-                           564 LOAD_ATTR               15 (cvtColor)
-                           574 LOAD_FAST                6 (img)
-                           576 LOAD_GLOBAL             22 (cv2)
-                           588 LOAD_ATTR               16 (COLOR_BGR2RGB)
-                           598 PRECALL                  2
-                           602 CALL                     2
-                           612 PRECALL                  1
-                           616 CALL                     1
-                           626 STORE_FAST               7 (pil_img)
-               
-               890         628 NOP
-               
-               891         630 LOAD_GLOBAL              7 (NULL + print)
-                           642 LOAD_CONST               6 ('\x1b[1;36mSaving image as ')
-                           644 LOAD_FAST                5 (output_filename)
-                           646 FORMAT_VALUE             0
-                           648 LOAD_CONST               7 ('\x1b[0m')
-                           650 BUILD_STRING             3
-                           652 PRECALL                  1
-                           656 CALL                     1
-                           666 POP_TOP
-               
-               892         668 LOAD_FAST                7 (pil_img)
-                           670 LOAD_METHOD             17 (save)
-                           692 LOAD_FAST                5 (output_filename)
-                           694 LOAD_DEREF               9 (out_f)
-                           696 PRECALL                  2
-                           700 CALL                     2
-                           710 POP_TOP
-               
-               893         712 LOAD_GLOBAL              7 (NULL + print)
-                           724 LOAD_CONST               8 ('\x1b[1;32mDone\x1b[0m')
-                           726 PRECALL                  1
-                           730 CALL                     1
-                           740 POP_TOP
-               
-               894         742 NOP
-               
-               895         744 LOAD_GLOBAL              7 (NULL + print)
-                           756 LOAD_CONST               9 ('\x1b[1;35mLoad and display image\x1b[0m')
-                           758 PRECALL                  1
-                           762 CALL                     1
-                           772 POP_TOP
-               
-               896         774 LOAD_GLOBAL             23 (NULL + cv2)
-                           786 LOAD_ATTR               12 (imread)
-                           796 LOAD_FAST                5 (output_filename)
-                           798 PRECALL                  1
-                           802 CALL                     1
-                           812 STORE_FAST               8 (opencv_img)
-               
-               897         814 NOP
-               
-               898         816 LOAD_GLOBAL             23 (NULL + cv2)
-                           828 LOAD_ATTR               18 (imshow)
-                           838 LOAD_CONST              10 ('OpenCV Image')
-                           840 LOAD_FAST                8 (opencv_img)
-                           842 PRECALL                  2
-                           846 CALL                     2
-                           856 POP_TOP
-               
-               900         858 NOP
-               
-               901         860 LOAD_GLOBAL             23 (NULL + cv2)
-                           872 LOAD_ATTR               19 (waitKey)
-                           882 LOAD_CONST              11 (0)
-                           884 PRECALL                  1
-                           888 CALL                     1
-                           898 POP_TOP
-               
-               902         900 LOAD_GLOBAL             23 (NULL + cv2)
-                           912 LOAD_ATTR               20 (destroyAllWindows)
-                           922 PRECALL                  0
-                           926 CALL                     0
-                           936 POP_TOP
-                           938 EXTENDED_ARG             1
-                           940 JUMP_BACKWARD          407 (to 128)
-               
-               875     >>  942 LOAD_CONST               0 (None)
-                           944 RETURN_VALUE
-                       >>  946 PUSH_EXC_INFO
-               
-               903         948 LOAD_GLOBAL             42 (KeyboardInterrupt)
-                           960 CHECK_EXC_MATCH
-                           962 POP_JUMP_FORWARD_IF_FALSE    39 (to 1042)
-                           964 POP_TOP
-               
-               904         966 LOAD_GLOBAL              7 (NULL + print)
-                           978 LOAD_CONST              12 ('\nExiting..')
-                           980 PRECALL                  1
-                           984 CALL                     1
-                           994 POP_TOP
-               
-               905         996 LOAD_GLOBAL             19 (NULL + sys)
-                          1008 LOAD_ATTR               10 (exit)
-                          1018 LOAD_CONST               3 (1)
-                          1020 PRECALL                  1
-                          1024 CALL                     1
-                          1034 POP_TOP
-                          1036 POP_EXCEPT
-                          1038 LOAD_CONST               0 (None)
-                          1040 RETURN_VALUE
-               
-               903     >> 1042 RERAISE                  0
-                       >> 1044 COPY                     3
-                          1046 POP_EXCEPT
-                          1048 RERAISE                  1
+                  0074070000000000000000000064067c059b007418000000000000000000
+                  009b009d03a6010000ab01000000000000000001007c07a0140000000000
+                  0000000000000000000000000000007c058909a6020000ab020000000000
+                  0000000100740700000000000000000000742a000000000000000000009b
+                  0064077418000000000000000000009b009d03a6010000ab010000000000
+                  00000001000900740700000000000000000000741e000000000000000000
+                  009b0064087418000000000000000000009b009d03a6010000ab01000000
+                  00000000000100741b000000000000000000006a0e00000000000000007c
+                  05a6010000ab0100000000000000007d080900741b000000000000000000
+                  006a16000000000000000064097c08a6020000ab02000000000000000001
+                  000900741b000000000000000000006a170000000000000000640aa60100
+                  00ab0100000000000000000100741b000000000000000000006a18000000
+                  0000000000a6000000ab000000000000000000010090018cd96400530023
+                  007432000000000000000000002400722701007407000000000000000000
+                  00640ba6010000ab01000000000000000001007413000000000000000000
+                  006a0a00000000000000006403a6010000ab010000000000000000010059
+                  00640053007700780359007701
+                              0 MAKE_CELL                9 (out_f)
+               
+               1002           2 RESUME                   0
+               
+               1003           4 NOP
+               
+               1004           6 LOAD_FAST                0 (self)
+                              8 LOAD_METHOD              0 (preprocess)
+                             30 PRECALL                  0
+                             34 CALL                     0
+                             44 STORE_FAST               1 (input_list)
+               
+               1005          46 LOAD_FAST                0 (self)
+                             48 LOAD_ATTR                1 (out_format)
+                             58 LOAD_METHOD              2 (upper)
+                             80 PRECALL                  0
+                             84 CALL                     0
+                             94 STORE_DEREF              9 (out_f)
+               
+               1007          96 LOAD_CLOSURE             9 (out_f)
+                             98 BUILD_TUPLE              1
+                            100 LOAD_CONST               1 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 1007>)
+                            102 MAKE_FUNCTION            8 (closure)
+                            104 LOAD_FAST                1 (input_list)
+                            106 GET_ITER
+                            108 PRECALL                  0
+                            112 CALL                     0
+                            122 STORE_FAST               1 (input_list)
+               
+               1009         124 LOAD_FAST                1 (input_list)
+                            126 GET_ITER
+                        >>  128 EXTENDED_ARG             1
+                            130 FOR_ITER               471 (to 1074)
+                            132 STORE_FAST               2 (file)
+               
+               1010         134 LOAD_GLOBAL              7 (NULL + print)
+                            146 LOAD_FAST                2 (file)
+                            148 PRECALL                  1
+                            152 CALL                     1
+                            162 POP_TOP
+               
+               1011         164 LOAD_DEREF               9 (out_f)
+                            166 LOAD_METHOD              2 (upper)
+                            188 PRECALL                  0
+                            192 CALL                     0
+                            202 LOAD_GLOBAL              8 (SUPPORTED_IMAGE_FORMATS)
+                            214 CONTAINS_OP              0
+                            216 POP_JUMP_FORWARD_IF_FALSE    69 (to 356)
+               
+               1012         218 LOAD_GLOBAL             10 (os)
+                            230 LOAD_ATTR                6 (path)
+                            240 LOAD_METHOD              7 (splitext)
+                            262 LOAD_FAST                2 (file)
+                            264 PRECALL                  1
+                            268 CALL                     1
+                            278 UNPACK_SEQUENCE          2
+                            282 STORE_FAST               3 (_)
+                            284 STORE_FAST               4 (ext)
+               
+               1013         286 LOAD_FAST                3 (_)
+               
+               1014         288 LOAD_GLOBAL              8 (SUPPORTED_IMAGE_FORMATS)
+                            300 LOAD_DEREF               9 (out_f)
+                            302 BINARY_SUBSCR
+                            312 LOAD_METHOD              8 (lower)
+                            334 PRECALL                  0
+                            338 CALL                     0
+               
+               1013         348 BINARY_OP                0 (+)
+                            352 STORE_FAST               5 (output_filename)
+                            354 JUMP_FORWARD            35 (to 426)
+               
+               1016     >>  356 LOAD_GLOBAL              7 (NULL + print)
+                            368 LOAD_CONST               2 ('Unsupported output format')
+                            370 PRECALL                  1
+                            374 CALL                     1
+                            384 POP_TOP
+               
+               1017         386 LOAD_GLOBAL             19 (NULL + sys)
+                            398 LOAD_ATTR               10 (exit)
+                            408 LOAD_CONST               3 (1)
+                            410 PRECALL                  1
+                            414 CALL                     1
+                            424 POP_TOP
+               
+               1018     >>  426 NOP
+               
+               1019         428 LOAD_GLOBAL              7 (NULL + print)
+                            440 LOAD_GLOBAL             22 (DYELLOW)
+                            452 FORMAT_VALUE             0
+                            454 LOAD_CONST               4 ('Reading input image..')
+                            456 LOAD_GLOBAL             24 (RESET)
+                            468 FORMAT_VALUE             0
+                            470 BUILD_STRING             3
+                            472 PRECALL                  1
+                            476 CALL                     1
+                            486 POP_TOP
+               
+               1020         488 LOAD_GLOBAL             27 (NULL + cv2)
+                            500 LOAD_ATTR               14 (imread)
+                            510 LOAD_FAST                2 (file)
+                            512 PRECALL                  1
+                            516 CALL                     1
+                            526 STORE_FAST               6 (img)
+               
+               1021         528 NOP
+               
+               1022         530 LOAD_GLOBAL              7 (NULL + print)
+                            542 LOAD_GLOBAL             30 (DMAGENTA)
+                            554 FORMAT_VALUE             0
+                            556 LOAD_CONST               5 ('Converting to PIL image')
+                            558 LOAD_GLOBAL             24 (RESET)
+                            570 FORMAT_VALUE             0
+                            572 BUILD_STRING             3
+                            574 PRECALL                  1
+                            578 CALL                     1
+                            588 POP_TOP
+               
+               1023         590 LOAD_GLOBAL             33 (NULL + Image)
+                            602 LOAD_ATTR               17 (fromarray)
+                            612 LOAD_GLOBAL             27 (NULL + cv2)
+                            624 LOAD_ATTR               18 (cvtColor)
+                            634 LOAD_FAST                6 (img)
+                            636 LOAD_GLOBAL             26 (cv2)
+                            648 LOAD_ATTR               19 (COLOR_BGR2RGB)
+                            658 PRECALL                  2
+                            662 CALL                     2
+                            672 PRECALL                  1
+                            676 CALL                     1
+                            686 STORE_FAST               7 (pil_img)
+               
+               1024         688 NOP
+               
+               1025         690 LOAD_GLOBAL              7 (NULL + print)
+                            702 LOAD_CONST               6 ('\x1b[1;36mSaving image as ')
+                            704 LOAD_FAST                5 (output_filename)
+                            706 FORMAT_VALUE             0
+                            708 LOAD_GLOBAL             24 (RESET)
+                            720 FORMAT_VALUE             0
+                            722 BUILD_STRING             3
+                            724 PRECALL                  1
+                            728 CALL                     1
+                            738 POP_TOP
+               
+               1026         740 LOAD_FAST                7 (pil_img)
+                            742 LOAD_METHOD             20 (save)
+                            764 LOAD_FAST                5 (output_filename)
+                            766 LOAD_DEREF               9 (out_f)
+                            768 PRECALL                  2
+                            772 CALL                     2
+                            782 POP_TOP
+               
+               1027         784 LOAD_GLOBAL              7 (NULL + print)
+                            796 LOAD_GLOBAL             42 (DGREEN)
+                            808 FORMAT_VALUE             0
+                            810 LOAD_CONST               7 ('Done')
+                            812 LOAD_GLOBAL             24 (RESET)
+                            824 FORMAT_VALUE             0
+                            826 BUILD_STRING             3
+                            828 PRECALL                  1
+                            832 CALL                     1
+                            842 POP_TOP
+               
+               1028         844 NOP
+               
+               1029         846 LOAD_GLOBAL              7 (NULL + print)
+                            858 LOAD_GLOBAL             30 (DMAGENTA)
+                            870 FORMAT_VALUE             0
+                            872 LOAD_CONST               8 ('Load and display image')
+                            874 LOAD_GLOBAL             24 (RESET)
+                            886 FORMAT_VALUE             0
+                            888 BUILD_STRING             3
+                            890 PRECALL                  1
+                            894 CALL                     1
+                            904 POP_TOP
+               
+               1030         906 LOAD_GLOBAL             27 (NULL + cv2)
+                            918 LOAD_ATTR               14 (imread)
+                            928 LOAD_FAST                5 (output_filename)
+                            930 PRECALL                  1
+                            934 CALL                     1
+                            944 STORE_FAST               8 (opencv_img)
+               
+               1031         946 NOP
+               
+               1032         948 LOAD_GLOBAL             27 (NULL + cv2)
+                            960 LOAD_ATTR               22 (imshow)
+                            970 LOAD_CONST               9 ('OpenCV Image')
+                            972 LOAD_FAST                8 (opencv_img)
+                            974 PRECALL                  2
+                            978 CALL                     2
+                            988 POP_TOP
+               
+               1034         990 NOP
+               
+               1035         992 LOAD_GLOBAL             27 (NULL + cv2)
+                           1004 LOAD_ATTR               23 (waitKey)
+                           1014 LOAD_CONST              10 (0)
+                           1016 PRECALL                  1
+                           1020 CALL                     1
+                           1030 POP_TOP
+               
+               1036        1032 LOAD_GLOBAL             27 (NULL + cv2)
+                           1044 LOAD_ATTR               24 (destroyAllWindows)
+                           1054 PRECALL                  0
+                           1058 CALL                     0
+                           1068 POP_TOP
+                           1070 EXTENDED_ARG             1
+                           1072 JUMP_BACKWARD          473 (to 128)
+               
+               1009     >> 1074 LOAD_CONST               0 (None)
+                           1076 RETURN_VALUE
+                        >> 1078 PUSH_EXC_INFO
+               
+               1037        1080 LOAD_GLOBAL             50 (KeyboardInterrupt)
+                           1092 CHECK_EXC_MATCH
+                           1094 POP_JUMP_FORWARD_IF_FALSE    39 (to 1174)
+                           1096 POP_TOP
+               
+               1038        1098 LOAD_GLOBAL              7 (NULL + print)
+                           1110 LOAD_CONST              11 ('\nExiting..')
+                           1112 PRECALL                  1
+                           1116 CALL                     1
+                           1126 POP_TOP
+               
+               1039        1128 LOAD_GLOBAL             19 (NULL + sys)
+                           1140 LOAD_ATTR               10 (exit)
+                           1150 LOAD_CONST               3 (1)
+                           1152 PRECALL                  1
+                           1156 CALL                     1
+                           1166 POP_TOP
+                           1168 POP_EXCEPT
+                           1170 LOAD_CONST               0 (None)
+                           1172 RETURN_VALUE
+               
+               1037     >> 1174 RERAISE                  0
+                        >> 1176 COPY                     3
+                           1178 POP_EXCEPT
+                           1180 RERAISE                  1
                ExceptionTable:
-                 6 to 940 -> 946 [0]
-                 946 to 1034 -> 1044 [1] lasti
-                 1042 to 1042 -> 1044 [1] lasti
+                 6 to 1072 -> 1078 [0]
+                 1078 to 1166 -> 1176 [1] lasti
+                 1174 to 1174 -> 1176 [1] lasti
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 7
                      flags     : 19
                      code
                         0x95018701970067007c005d2a8a01740100000000000000000000880166
                         016400840874020000000000000000000089021900000000000000000044
                         00a6000000ab000000000000000000a6010000ab010000000000000000af
                         28890191028c2b5300
-                                   0 COPY_FREE_VARS           1
-                                   2 MAKE_CELL                1 (item)
+                                    0 COPY_FREE_VARS           1
+                                    2 MAKE_CELL                1 (item)
                      
-                     873           4 RESUME                   0
-                                   6 BUILD_LIST               0
-                                   8 LOAD_FAST                0 (.0)
-                             >>   10 FOR_ITER                42 (to 96)
-                                  12 STORE_DEREF              1 (item)
-                                  14 LOAD_GLOBAL              1 (NULL + any)
-                                  26 LOAD_CLOSURE             1 (item)
-                                  28 BUILD_TUPLE              1
-                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/converter.py", line 873>)
-                                  32 MAKE_FUNCTION            8 (closure)
-                     
-                     874          34 LOAD_GLOBAL              2 (SUPPORTED_IMAGE_FORMATS)
-                                  46 LOAD_DEREF               2 (out_f)
-                                  48 BINARY_SUBSCR
-                     
-                     873          58 GET_ITER
-                                  60 PRECALL                  0
-                                  64 CALL                     0
-                                  74 PRECALL                  1
-                                  78 CALL                     1
-                                  88 POP_JUMP_BACKWARD_IF_FALSE    40 (to 10)
-                                  90 LOAD_DEREF               1 (item)
-                                  92 LIST_APPEND              2
-                                  94 JUMP_BACKWARD           43 (to 10)
-                             >>   96 RETURN_VALUE
+                     1007           4 RESUME                   0
+                                    6 BUILD_LIST               0
+                                    8 LOAD_FAST                0 (.0)
+                              >>   10 FOR_ITER                42 (to 96)
+                                   12 STORE_DEREF              1 (item)
+                                   14 LOAD_GLOBAL              1 (NULL + any)
+                                   26 LOAD_CLOSURE             1 (item)
+                                   28 BUILD_TUPLE              1
+                                   30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/converter.py", line 1007>)
+                                   32 MAKE_FUNCTION            8 (closure)
+                     
+                     1008          34 LOAD_GLOBAL              2 (SUPPORTED_IMAGE_FORMATS)
+                                   46 LOAD_DEREF               2 (out_f)
+                                   48 BINARY_SUBSCR
+                     
+                     1007          58 GET_ITER
+                                   60 PRECALL                  0
+                                   64 CALL                     0
+                                   74 PRECALL                  1
+                                   78 CALL                     1
+                                   88 POP_JUMP_BACKWARD_IF_FALSE    40 (to 10)
+                                   90 LOAD_DEREF               1 (item)
+                                   92 LIST_APPEND              2
+                                   94 JUMP_BACKWARD           43 (to 10)
+                              >>   96 RETURN_VALUE
                      consts
                         code
                            argcount  : 1
                            nlocals   : 2
                            stacksize : 4
                            flags     : 51
                            code
                               0x95014b00010097007c005d2b7d018902a0000000000000000000000000
                               000000000000000000a6000000ab000000000000000000a0010000000000
                               0000000000000000000000000000007c01a6010000ab0100000000000000
                               005600970101008c2c64005300
-                                         0 COPY_FREE_VARS           1
+                                          0 COPY_FREE_VARS           1
                            
-                           873           2 RETURN_GENERATOR
-                                         4 POP_TOP
-                                         6 RESUME                   0
-                                         8 LOAD_FAST                0 (.0)
-                                   >>   10 FOR_ITER                43 (to 98)
+                           1007           2 RETURN_GENERATOR
+                                          4 POP_TOP
+                                          6 RESUME                   0
+                                          8 LOAD_FAST                0 (.0)
+                                    >>   10 FOR_ITER                43 (to 98)
                            
-                           874          12 STORE_FAST               1 (ext)
-                                        14 LOAD_DEREF               2 (item)
-                                        16 LOAD_METHOD              0 (lower)
-                                        38 PRECALL                  0
-                                        42 CALL                     0
-                                        52 LOAD_METHOD              1 (endswith)
-                                        74 LOAD_FAST                1 (ext)
-                                        76 PRECALL                  1
-                                        80 CALL                     1
+                           1008          12 STORE_FAST               1 (ext)
+                                         14 LOAD_DEREF               2 (item)
+                                         16 LOAD_METHOD              0 (lower)
+                                         38 PRECALL                  0
+                                         42 CALL                     0
+                                         52 LOAD_METHOD              1 (endswith)
+                                         74 LOAD_FAST                1 (ext)
+                                         76 PRECALL                  1
+                                         80 CALL                     1
                            
-                           873          90 YIELD_VALUE
-                                        92 RESUME                   1
-                                        94 POP_TOP
-                                        96 JUMP_BACKWARD           44 (to 10)
-                                   >>   98 LOAD_CONST               0 (None)
-                                       100 RETURN_VALUE
+                           1007          90 YIELD_VALUE
+                                         92 RESUME                   1
+                                         94 POP_TOP
+                                         96 JUMP_BACKWARD           44 (to 10)
+                                    >>   98 LOAD_CONST               0 (None)
+                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('lower', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                            name       '<genexpr>'
-                           firstlineno 873
+                           firstlineno 1007
                            lnotab 0x0c014eff
                      names      ('any', 'SUPPORTED_IMAGE_FORMATS')
                      varnames   ('.0',)
                      freevars   ('out_f',)
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                      name       '<listcomp>'
-                     firstlineno 873
+                     firstlineno 1007
                      lnotab 0x220118ff
                   'Unsupported output format'
                   1
-                  '\x1b[1;33mReading input image..\x1b[0m'
-                  '\x1b[1;35mConverting to PIL image\x1b[0m'
+                  'Reading input image..'
+                  'Converting to PIL image'
                   '\x1b[1;36mSaving image as '
-                  '\x1b[0m'
-                  '\x1b[1;32mDone\x1b[0m'
-                  '\x1b[1;35mLoad and display image\x1b[0m'
+                  'Done'
+                  'Load and display image'
                   'OpenCV Image'
                   0
                   '\nExiting..'
-               names      ('preprocess', 'out_format', 'upper', 'print', 'SUPPORTED_IMAGE_FORMATS', 'os', 'path', 'splitext', 'lower', 'sys', 'exit', 'cv2', 'imread', 'Image', 'fromarray', 'cvtColor', 'COLOR_BGR2RGB', 'save', 'imshow', 'waitKey', 'destroyAllWindows', 'KeyboardInterrupt')
+               names      ('preprocess', 'out_format', 'upper', 'print', 'SUPPORTED_IMAGE_FORMATS', 'os', 'path', 'splitext', 'lower', 'sys', 'exit', 'DYELLOW', 'RESET', 'cv2', 'imread', 'DMAGENTA', 'Image', 'fromarray', 'cvtColor', 'COLOR_BGR2RGB', 'save', 'DGREEN', 'imshow', 'waitKey', 'destroyAllWindows', 'KeyboardInterrupt')
                varnames   ('self', 'input_list', 'file', '_', 'ext', 'output_filename', 'img', 'pil_img', 'opencv_img')
                freevars   ()
                cellvars   ('out_f',)
-               filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+               filename   '/media/skye/skye/FileMAC/filemac/converter.py'
                name       'convert_image'
-               firstlineno 868
+               firstlineno 1002
                lnotab
                   0x04010201280132021c020a011e013601440102013cff08031e01280102
-                  011e01280102011e016201020126012c011e0102011e01280102012a0202
+                  013c01280102013c016201020132012c013c0102013c01280102012a0202
                   0128012ae5061c12011e012efe
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'preprocess', 'convert_image')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+         filename   '/media/skye/skye/FileMAC/filemac/converter.py'
          name       'ImageConverter'
-         firstlineno 842
+         firstlineno 976
          lnotab 0x0a0206040614
       'ImageConverter'
-   names      ('logging', 'logging.handlers', 'math', 'os', 're', 'sqlite3', 'sys', 'time', 'pdf2docx', 'parse', 'traceback', 'typing', 'Iterable', 'cv2', 'pandas', 'pd', 'pydub', 'PyPDF2', 'subprocess', 'requests', 'speedtest', 'PIL', 'Image', 'docx', 'Document', 'gtts', 'gTTS', 'pptx', 'Presentation', 'AudioSegment', 'moviepy.editor', 'VideoFileClip', 'formats', 'SUPPORTED_VIDEO_FORMATS', 'reportlab.lib.pagesizes', 'letter', 'reportlab.platypus', 'Paragraph', 'SimpleDocTemplate', 'SUPPORTED_AUDIO_FORMATS', 'SUPPORTED_IMAGE_FORMATS', 'PYGAME_DETECT_AVX2', 'basicConfig', 'INFO', 'getLogger', '__name__', 'logger', 'MakeConversion', 'FileSynthesis', 'VideoConverter', 'AudioConverter', 'ImageConverter')
+   names      ('logging', 'logging.handlers', 'os', 're', 'sqlite3', 'subprocess', 'sys', 'time', 'traceback', 'pdf2image', 'convert_from_path', 'cv2', 'pandas', 'pd', 'pydub', 'PyPDF2', 'requests', 'speedtest', 'docx', 'Document', 'gtts', 'gTTS', 'moviepy.editor', 'VideoFileClip', 'pdf2docx', 'parse', 'PIL', 'Image', 'pptx', 'Presentation', 'AudioSegment', 'colors', 'RESET', 'GREEN', 'DGREEN', 'YELLOW', 'DYELLOW', 'CYAN', 'BLUE', 'DBLUE', 'DMAGENTA', 'DRED', 'ICYAN', 'reportlab.lib.pagesizes', 'letter', 'reportlab.platypus', 'Paragraph', 'SimpleDocTemplate', 'formats', 'SUPPORTED_AUDIO_FORMATS', 'SUPPORTED_IMAGE_FORMATS', 'SUPPORTED_VIDEO_FORMATS', 'PYGAME_DETECT_AVX2', 'basicConfig', 'INFO', 'getLogger', '__name__', 'logger', 'MakeConversion', 'Scanner', 'FileSynthesis', 'VideoConverter', 'AudioConverter', 'ImageConverter')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/media/skye/Skye/FileMAC/fmac/converter.py'
+   filename   '/media/skye/skye/FileMAC/filemac/converter.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0202080108010801080108010801080108010c0108020c01080108
-      01080108010802080108010c010c020c030c010c020c010c010c0110010c
-      010c0804012e0120031a7f007f007f006f1a7f00371a461a31
+      0x00ff02020801080208010801080108010801080108030c010801080108
+      010802080108010c020c020c010c010c010c010c0134020c011002140a04
+      012e0120031a7f007f007f007f001d1a491a7f00431a461a33
```

### Comparing `filemac-1.0.2/filemac/__pycache__/formats.cpython-311.pyc` & `filemac-1.0.3/filemac/__pycache__/formats.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/filemac/colors.py` & `filemac-1.0.3/filemac/colors.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,39 +2,71 @@
 
 from colorama import Fore, Style, init
 
 init(autoreset=True)
 
 if os.name == "posix":
     RESET = '\033[0m'
+
     RED = '\033[91m'
     DRED = '\033[1;91m'
+    FRED = '\033[2;91m'
+
     GREEN = '\033[92m'
     DGREEN = '\033[1;92m'
+    FGREEN = '\033[2;92m'
+
     YELLOW = '\033[93m'
     DYELLOW = '\033[1;93m'
+    FYELLOW = '\033[2;93m'
+
     BLUE = '\033[94m'
     DBLUE = '\033[1;94m'
+    FBLUE = '\033[2;94m'
+
     MAGENTA = '\033[95m'
     DMAGENTA = '\033[1;95m'
+    FMAGENTA = '\033[2;95m'
+    IMAGENTA = '\033[3;95m'
+
     CYAN = '\033[96m'
     DCYAN = '\033[1;96m'
+    FCYAN = '\033[2;96m'
     ICYAN = '\033[3;96m'
 
+    BWHITE = '\033[1m'
+    BBWHITE = '\033[5;97;1m'
+
 elif os.name == "nt":
     RESET = Style.RESET_ALL
+
     RED = Fore.LIGHTRED_EX
     DRED = Fore.RED
+    FRED = Fore.RED
+
     GREEN = Fore.LIGHTGREEN_EX
     DGREEN = Fore.GREEN
+    FGREEN = Fore.GREEN
+
     YELLOW = Fore.LIGHTYELLOW_EX
+    FYELLOW = Fore.YELLOW
     DYELLOW = Fore.YELLOW
+
     BLUE = Fore.LIGHTBLUE_EX
     DBLUE = Fore.BLUE
+    FBLUE = Fore.BLUE
+
     MAGENTA = Fore.LIGHTMAGENTA_EX
     DMAGENTA = Fore.MAGENTA
+    IMAGENTA = Fore.LIGHTMAGENTA_EX
+    FMAGENTA = Fore.MAGENTA
+
     CYAN = Fore.LIGHTCYAN_EX
     DCYAN = Fore.CYAN
     ICYAN = Fore.WHITE
+    FCYAN = Fore.CYAN
+
+    BWHITE = Fore.WHITE
+    BWHITE = Fore.WHITE
 
-#return RESET, RED, DRED, GREEN, DGREEN, YELLOW, DYELLOW, BLUE, DBLUE,
-#MAGENTA, DMAGENTA, CYAN, DCYAN
+# return RESET, RED, DRED, GREEN, DGREEN, YELLOW, DYELLOW, BLUE, DBLUE,
+# MAGENTA, DMAGENTA, CYAN, DCYAN
```

### Comparing `filemac-1.0.2/filemac/converter.py` & `filemac-1.0.3/filemac/converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,50 +3,55 @@
 import logging.handlers
 # import math
 import os
 import re
 import sqlite3
 import subprocess
 import sys
-import time
+# import time
 import traceback
-# import pdfminer.high_level
-# from typing import Iterable
-from pdf2image import convert_from_path
+import math
 import cv2
 import pandas as pd
 import pydub
 import PyPDF2
 # import pytesseract
 import requests
-import speedtest
+# import speedtest
 from docx import Document
 # from pydub.playback import play
 from gtts import gTTS
 # from PyPDF2 import PdfFileReader
 from moviepy.editor import VideoFileClip
 from pdf2docx import parse
+# import pdfminer.high_level
+# from typing import Iterable
+from pdf2image import convert_from_path
 from PIL import Image
 from pptx import Presentation
 from pydub import AudioSegment
-from .colors import (RESET, GREEN, DGREEN, YELLOW, DYELLOW, CYAN, BLUE, DBLUE,
-                     MAGENTA, DMAGENTA, RED, DRED, ICYAN)
 from reportlab.lib.pagesizes import letter
 from reportlab.platypus import Paragraph, SimpleDocTemplate
 
+from .colors import (BLUE, CYAN, DBLUE, DCYAN, DGREEN, DMAGENTA, DRED, DYELLOW,
+                     GREEN, ICYAN, MAGENTA, RED, RESET, YELLOW, BWHITE)
 from .formats import (SUPPORTED_AUDIO_FORMATS, SUPPORTED_IMAGE_FORMATS,
                       SUPPORTED_VIDEO_FORMATS)
 
 # import pygame
 # from aspose.words import Document as aspose_document
 # from aspose.slides import Presentation as aspose_presentation
 # from show_progress import progress_show
 # from PIL import ImageDraw, ImageFont
 ###############################################################################
 
+_ext_word = ["doc", "docx"]
+_ext_ppt_ = ["ppt", "pptx"]
+_ext_xls = ["xls", "xlsx"]
+
 PYGAME_DETECT_AVX2 = 1
 logging.basicConfig(level=logging.INFO, format='%(levelname)-8s %(message)s')
 logger = logging.getLogger(__name__)
 
 
 class MakeConversion:
 
@@ -84,115 +89,141 @@
             print(e)
 
 ###############################################################################
 # Convert word file to pdf document (docx)
 ###############################################################################
     def word_to_pdf(self):
         word_list = self.preprocess()
-        ls = ["doc", "docx"]
+
         word_list = [
-            item for item in word_list if any(item.lower().endswith(ext) for ext in ls)]
+            item for item in word_list if any(item.lower().endswith(ext) for ext in _ext_word)]
         for word_file in word_list:
-            if word_file.lower().endswith("doc"):
-                pdf_file = word_file[:-3] + "pdf"
-            elif word_file.lower().endswith("docx"):
-                pdf_file = word_file[:-4] + "pdf"
+
+            pdf_file_dir = os.path.dirname(word_file)
+            pdf_file = os.path.splitext(word_file)[0] + '.pdf'
 
             try:
                 print(
                     f'{BLUE}Converting: {RESET}{word_file} {BLUE}to {RESET}{pdf_file}')
                 if os.name == 'posix':  # Check if running on Linux
                     # Use subprocess to run the dpkg and grep commands
                     result = subprocess.run(
                         ['dpkg', '-l', 'libreoffice'], stdout=subprocess.PIPE, text=True)
                     if result.returncode != 0:
                         print(
                             "Please install libreoffice to use this functionality !")
                         sys.exit(1)
-                    subprocess.run(['soffice', '--convert-to',
-                                   'pdf', word_file, pdf_file])
-                    # print(f"{DMAGENTA} Successfully converted {word_file} to {pdf_file}{RESET}")
+                    subprocess.run(
+                        ['soffice', '--convert-to', 'pdf', word_file, '--outdir', pdf_file_dir])
+
+                    print(
+                        f"{DMAGENTA} Successfully converted {word_file} to {pdf_file}{RESET}")
+                    return pdf_file
+
                 elif os.name == "nt":
                     try:
                         from docx2pdf import convert
                     except ImportError:
                         print("Run pip install docx2pdf for this function to work")
                         sys.exit(1)
                     convert(word_file, pdf_file)
                     print(
                         f"{DMAGENTA} Successfully converted {word_file} to {pdf_file}{RESET}")
+                    return pdf_file
 
             except Exception as e:
                 print(f"Error converting {word_file} to {pdf_file}: {e}")
 
 ###############################################################################
 # Convert pdf file to word document (docx)
 ###############################################################################
     def pdf_to_word(self):
         pdf_list = self.preprocess()
         pdf_list = [item for item in pdf_list if item.lower().endswith("pdf")]
         for pdf_file in pdf_list:
-            if pdf_file.lower().endswith("pdf"):
-                word_file = pdf_file[:-3] + "docx"
+            word_file = pdf_file[:-3] + \
+                "docx" if pdf_file.lower().endswith("pdf") else None
 
             try:
-
+                print(F"{DYELLOW}Parse the pdf document..{RESET}")
                 parse(pdf_file, word_file, start=0, end=None)
 
-                print(f'{GREEN}Converting to word..{RESET}', end='\r')
-
-                logger.info(f"{DMAGENTA} Successfully converted{pdf_file} \
-to {word_file}{RESET}")
+                logger.info(f"{MAGENTA}New file is {CYAN}{word_file}{RESET}")
+                logger.info(f"{DGREEN}Success👨‍💻✅{RESET}")
             except KeyboardInterrupt:
-                print("\nExiting..")
+                print("\nQuit❕")
                 sys.exit(1)
             except Exception as e:
                 logger.info(f'{DRED}All conversion attempts have failed: \
 {e}{RESET}')
 
 ###############################################################################
 # Convert text file(s) to pdf document (docx)
 ###############################################################################
-    def txt_to_pdf(input_file, output_file):
+    def txt_to_pdf(self):
         """Convert a .txt file to a PDF."""
+        txt_list = self.preprocess()
+        _list_ = [item for item in txt_list if item.lower().endswith("txt")]
+        for _file_ in _list_:
+            _pdf_ = _file_[:-3] + \
+                "pdf" if _file_.lower().endswith("txt") else None
+            # Read the contents of the input .txt file
+            with open(_file_, 'r', encoding='utf-8') as file:
+                text_contents = file.readlines()
+
+            # Initialize the PDF document
+            logger.info(F"{DYELLOW}Initialize the PDF document{RESET}")
+            doc = SimpleDocTemplate(_pdf_, pagesize=letter)
 
-        # Read the contents of the input .txt file
-        with open(input_file, 'r', encoding='utf-8') as file:
-            text_contents = file.readlines()
-
-        # Initialize the PDF document
-        doc = SimpleDocTemplate(output_file, pagesize=letter)
-
-        # Create a story to hold the elements of the PDF
-        story = []
-
-        # Iterate through each line in the input .txt file and add it to the PDF
-        for line in text_contents:
-            story.append(Paragraph(line.strip(), style="normalText"))
+            # Create a story to hold the elements of the PDF
+            logger.info(
+                F"{DYELLOW}Create a story to hold the elements of the PDF{RESET}")
+            story = []
 
-        # Build and write the PDF document
-        doc.build(story)
+            # Iterate through each line in the input .txt file and add it to the PDF
+            logger.info(
+                F"{DYELLOW}Iterate through each line in the input .txt file and add it to the PDF{RESET}")
+            _line_count_ = 0
+            try:
+                for line in text_contents:
+                    _line_count_ += 1
+                    logger.info(
+                        f"Lines {DBLUE}{_line_count_}{RESET}/{len(text_contents)}")
+                    story.append(Paragraph(line.strip(), style="normalText"))
+
+            except KeyboardInterrupt:
+                print("\nQuit❕⌨️")
+                sys.exit(1)
+            except Exception as e:
+                logger.error(e)
+                pass
+            # Build and write the PDF document
+            logger.info(f"{DYELLOW}Build and write the PDF document{RESET}")
+            doc.build(story)
+            logger.info(f"{MAGENTA}New file is {CYAN}{_pdf_}{RESET}")
+            print(f"\n{DGREEN}Success👨‍💻✅{RESET}")
 
 ###############################################################################
 # Convert word file(s) to pptx document (pptx/ppt)
 ###############################################################################
     def word_to_pptx(self):
         word_list = self.preprocess()
         word_list = [item for item in word_list if item.lower().endswith(
             "docx") or item.lower().endswith("doc")]
 
         for word_file in word_list:
 
             if word_list is None:
                 print("Please provide appropriate file type")
                 sys.exit(1)
-            if word_file.lower().endswith("docx"):
-                pptx_file = word_file[:-4] + "pptx"
-            elif word_file.lower().endswith("doc"):
-                pptx_file = word_file[:-3] + "pptx"
+            ext = os.path.splitext(word_file)[-1][1:]
+
+            pptx_file = (os.path.splitext(word_file)[
+                         0] + ".pptx") if ext in list(_ext_word) else None
+
             try:
                 # Load the Word document
                 print(F"{DYELLOW}Load the Word document..{RESET}")
                 doc = Document(word_file)
 
                 # Create a new PowerPoint presentation
                 print(F"{DYELLOW}Create a new PowerPoint presentation..{RESET}")
@@ -202,61 +233,62 @@
                 print(
                     f"{DGREEN}Populating pptx slides with {DYELLOW}{len(doc.paragraphs)}{DGREEN} entries..{RESET}")
                 count = 0
                 for paragraph in doc.paragraphs:
                     count += 1
                     perc = (count/len(doc.paragraphs))*100
                     print(
-                        f"{DMAGENTA}Progress:: \033[1;36m{perc:.2f}%{RESET}", end="\r")
+                        f"{DMAGENTA}Progress:: {DCYAN}{perc:.2f}%{RESET}", end="\r")
                     # Create a new slide in the PowerPoint presentation
                     slide = prs.slides.add_slide(prs.slide_layouts[1])
 
                     # Add the paragraph text to the slide
                     slide.shapes.title.text = paragraph.text
 
                 # Save the PowerPoint presentation
                 prs.save(pptx_file)
-                print(f"\n{DGREEN}Done{RESET}")
-            except KeyboardInterrupt:
-                print("\nExiting")
-                sys.exit(1)
+                logger.info(f"{MAGENTA}New file is {CYAN}{pptx_file}{RESET}")
+                print(f"\n{DGREEN}Success👨‍💻✅{RESET}")
             except KeyboardInterrupt:
-                print("\nExiting..")
+                print("\nQuit❕⌨️")
                 sys.exit(1)
             except Exception as e:
                 logger.error(e)
 
 ###############################################################################
 # Convert word file to txt file'''
 ###############################################################################
 
     def word_to_txt(self):
         word_list = self.preprocess()
-        word_list = [item for item in word_list if item.lower().endswith(
-            "docx") or item.lower().endswith("doc")]
+        word_list = [item for item in word_list if os.path.splitext(
+            item)[-1][1:].lower() in list(_ext_word)]
+
         for file_path in word_list:
-            if file_path.lower().endswith("docx"):
-                txt_file = file_path[:-4] + "txt"
-            elif file_path.lower().endswith("doc"):
-                txt_file = file_path[:-3] + "txt"
+            ext = os.path.splitext(file_path)[-1][1:]
+            txt_file = (os.path.splitext(file_path)[
+                        0] + ".txt") if ext in list(_ext_word) else "output.txt"
+
             try:
+                logger.info(f"{DYELLOW}Create Doument Tablet{RESET}")
                 doc = Document(file_path)
-                print("INFO Processing...")
 
                 with open(txt_file, 'w', encoding='utf-8') as f:
                     Par = 0
                     for paragraph in doc.paragraphs:
                         f.write(paragraph.text + '\n')
                         Par += 1
 
-                        print(f"Par:{BLUE}{Par}/{len(doc.paragraphs)}{RESET}", end='\r')
-                    logger.info(f"{DMAGENTA}Conversion of file to txt success{RESET}")
+                        print(
+                            f"Par:{BLUE}{Par}/{len(doc.paragraphs)}{RESET}", end='\r')
+                    logger.info(
+                        f"{DMAGENTA}Conversion of file to txt success{RESET}")
 
             except KeyboardInterrupt:
-                print("\nExit")
+                print("\nQuit❕⌨️")
                 sys.exit()
             except Exception as e:
                 logger.error(
                     f"Dear user something went amiss while attempting the conversion:\n {e}")
                 with open("conversion.log", "a") as log_file:
                     log_file.write(f"Couldn't convert {file_path} to {txt_file}:\
 REASON->{e}")
@@ -266,24 +298,30 @@
 ###############################################################################
     def pdf_to_txt(self):
         pdf_list = self.preprocess()
         pdf_list = [item for item in pdf_list if item.lower().endswith("pdf")]
         for file_path in pdf_list:
             txt_file = file_path[:-3] + "txt"
             try:
+                print(F"{DYELLOW}Open and read the pdf document..{RESET}")
                 with open(file_path, 'rb') as file:
                     pdf_reader = PyPDF2.PdfReader(file)
                     text = ''
+                    _pg_ = 0
+                    print(F"{YELLOW}Convert pages..{RESET}")
                     for page_num in range(len(pdf_reader.pages)):
+                        _pg_ += 1
+                        logger.info(
+                            f"Page {DBLUE}{_pg_}{RESET}/{len(pdf_reader.pages)}")
                         page = pdf_reader.pages[page_num]
                         text += page.extract_text()
                 with open(txt_file, 'w', encoding='utf-8') as f:
                     f.write(text)
-                    logger.info(f"{DMAGENTA}Successfully converted {file_path} to \
-{txt_file}{RESET}")
+                logger.info(f"{MAGENTA}New file is {CYAN}{txt_file}{RESET}")
+                logger.info(f"{DGREEN}Success👨‍💻✅{RESET}")
             except Exception as e:
                 logger.error(
                     f"Oops somethin went astray while converting {file_path} \
 to {txt_file}: {e}")
                 with open("conversion.log", "a") as log_file:
                     log_file.write(
                         f"Error converting {file_path} to {txt_file}: {e}\n")
@@ -292,23 +330,29 @@
 # Convert ppt file to word document
 ###############################################################################
     def ppt_to_word(self):
         ppt_list = self.preprocess()
         ppt_list = [item for item in ppt_list if item.lower().endswith(
             "pptx") or item.lower().endswith("ppt")]
         for file_path in ppt_list:
-            if file_path.lower().endswith("pptx"):
-                word_file = file_path[:-4] + "docx"
-            elif file_path.lower().endswith("ppt"):
-                word_file = file_path[:-3] + "docx"
+            ext = os.path.splitext(file_path)[-1][1:]
+            word_file = (os.path.splitext(file_path)[
+                         0] + ".docx") if ext in list(_ext_ppt_) else None
             try:
+                logger.info(f"{DYELLOW}Create Doument Tablet{RESET}")
                 presentation = Presentation(file_path)
                 document = Document()
 
+                logger.info(
+                    F"Slide count ={DMAGENTA} {len(presentation.slides)}{RESET}")
+                _slide_count_ = 0
                 for slide in presentation.slides:
+                    _slide_count_ += 1
+                    print(
+                        F"INFO\tSlide {DBLUE}{_slide_count_}{RESET}/{len(presentation.slides)}{RESET}", end='\r')
                     for shape in slide.shapes:
                         if shape.has_text_frame:
                             text_frame = shape.text_frame
                             for paragraph in text_frame.paragraphs:
                                 new_paragraph = document.add_paragraph()
                                 for run in paragraph.runs:
                                     new_run = new_paragraph.add_run(run.text)
@@ -328,77 +372,77 @@
                                     except AttributeError:
                                         # Ignore error and continue without
                                         # setting the font color
                                         pass
                             # Add a new paragraph after each slide
                             document.add_paragraph()
                 document.save(word_file)
-                logger.info(f"{DMAGENTA}Successfully converted {file_path} to \
-        {word_file}{RESET}")
+                logger.info(f"\n{MAGENTA}New file is {CYAN}{word_file}{RESET}")
+                logger.info(f"{DGREEN}Success👨‍💻✅{RESET}")
             except Exception as e:
                 logger.error(
-                    f"Oops somethin gwent awry while attempting to convert \
-        {file_path} to {word_file}:\n>>>{e}")
+                    f"\n❌Oops something went awry {RED}{e}{RESET}")
                 with open("conversion.log", "a") as log_file:
                     log_file.write(
-                        f"Oops something went astray while attempting \
-        convert {file_path} to {word_file}:{e}\n")
+                        f"\n❌Oops something went astray{RED}{e}{RESET}")
 
 ###############################################################################
 # Convert text file to word
 ###############################################################################
     def text_to_word(self):
         flist = self.preprocess()
         flist = [item for item in flist if item.lower().endswith("txt")]
         for file_path in flist:
             if file_path.lower().endswith("txt"):
                 word_file = file_path[:-3] + "docx"
 
             try:
                 # Read the text file
+                logger.info(f"{DCYAN}Open and read the text file{RESET}")
                 with open(file_path, 'r', encoding='utf-8', errors='ignore') as file:
                     text_content = file.read()
 
                 # Filter out non-XML characters
                 filtered_content = re.sub(
                     r'[^\x09\x0A\x0D\x20-\uD7FF\uE000-\uFFFD]+', '', text_content)
 
                 # Create a new Word document
+                logger.info(f"{DYELLOW}Create Doument Tablet{RESET}")
                 doc = Document()
                 # Add the filtered text content to the document
                 doc.add_paragraph(filtered_content)
 
                 # Save the document as a Word file
                 doc.save(word_file)
-                logger.info(f"{DMAGENTA}Successfully converted {file_path} to \
-        {word_file}{RESET}")
+                logger.info(f"{MAGENTA}New file is {DCYAN}{word_file}{RESET}")
+                logger.info(f"{DGREEN}Success👨‍💻✅{RESET}")
             except FileExistsError as e:
-                logger.error(f"{str(e)}")
+                logger.error(f"{str(e)}📁")
             except Exception as e:
                 logger.error(
-                    f"Oops Unable to perfom requested conversion: {e}\n")
+                    f"\n❌Oops something went awry {RED}{e}{RESET}")
                 with open("conversion.log", "a") as log_file:
                     log_file.write(
-                        f"Error converting {file_path} to {word_file}: \
-{e}\n")
+                        f"\n❌Oops something went astray{RED}{e}{RESET}")
 
 ###############################################################################
 # Convert xlsx file(s) to word file(s)
 ###############################################################################
     def convert_xls_to_word(self):
         xls_list = self.preprocess()
-        ls = ["xlsx", "xls"]
+
         xls_list = [item for item in xls_list if any(
-            item.lower().endswith(ext) for ext in ls)]
+            item.lower().endswith(ext) for ext in _ext_xls)]
+
         print(F"{DGREEN}Initializing conversion sequence{RESET}")
+
         for xls_file in xls_list:
-            if xls_file.lower().endswith("xlsx"):
-                word_file = xls_file[:-4] + "docx"
-            elif xls_file.lower().endswith("xls"):
-                word_file = xls_file[:-3] + "docx"
+            ext = os.path.splitext(xls_file)[-1][1:]
+            word_file = (os.path.splitext(xls_file)[
+                         0] + ".docx") if ext in list(_ext_xls) else None
             try:
                 '''Read the XLS file using pandas'''
 
                 df = pd.read_excel(xls_file)
 
                 '''Create a new Word document'''
                 doc = Document()
@@ -417,35 +461,34 @@
 {DBLUE}{percentage:.1f}%{RESET}", end="\r")
                     # print(f"\033[1;36m{row}{RESET}")
 
                 # Save the Word document
                 doc.save(word_file)
                 print(F"{DGREEN}Conversion successful!{RESET}", end="\n")
             except KeyboardInterrupt:
-                print("\nExiting")
+                print("\nQuit⌨️")
                 sys.exit(1)
             except Exception as e:
-                print("Oops Conversion failed:", str(e))
+                print(f"{RED}Oops Conversion failed:❕{RESET}", str(e))
 
 ###############################################################################
     '''Convert xlsx/xls file/files to text file format'''
 ###############################################################################
 
     def convert_xls_to_text(self):
         xls_list = self.preprocess()
-        ls = ["xlsx", "xls"]
+
         xls_list = [
             item for item in xls_list if any(item.lower().endswith(ext)
-                                             for ext in ls)]
+                                             for ext in _ext_xls)]
         print(F"{DGREEN}Initializing conversion sequence{RESET}")
         for xls_file in xls_list:
-            if xls_file .lower().endswith("xlsx"):
-                txt_file = xls_file[:-4] + "txt"
-            elif xls_file .lower().endswith("xls"):
-                txt_file = xls_file[:-3] + "txt"
+            ext = os.path.splitext(xls_file)[-1][1:]
+            txt_file = (os.path.splitext(xls_file)[
+                        0] + ".txt") if ext in list(_ext_xls) else None
             try:
                 # Read the XLS file using pandas
                 logger.info(f"Converting {xls_file}..")
                 df = pd.read_excel(xls_file)
 
                 # Convert the dataframe to plain text
                 text = df.to_string(index=False)
@@ -459,78 +502,76 @@
 lines {RESET}", end="\n")
                 # Write the plain text to the output file
                 with open(txt_file, 'w') as file:
                     file.write(text)
 
                 print(F"{DGREEN}Conversion successful!{RESET}", end="\n")
             except KeyboardInterrupt:
-                print("\nExiting")
+                print("\nQuit❕")
                 sys.exit(1)
             except Exception as e:
                 print("Oops Conversion failed:", str(e))
 
 ###############################################################################
     '''Convert xlsx/xls file to csv(comma seperated values) format'''
 ###############################################################################
 
     def convert_xlsx_to_csv(self):
         xls_list = self.preprocess()
-        ls = ["xlsx", "xls"]
+
         xls_list = [
             item for item in xls_list if any(item.lower().endswith(ext)
-                                             for ext in ls)]
+                                             for ext in _ext_xls)]
         for xls_file in xls_list:
-            if xls_file.lower().endswith("xlsx"):
-                csv_file = xls_file[:-4] + "csv"
-            elif xls_file.lower().endswith("xls"):
-                csv_file = xls_file[:-3] + "csv"
+            ext = os.path.splitext(xls_file)[-1][1:]
+            csv_file = (os.path.splitext(xls_file)[
+                        0] + ".csv") if ext in list(_ext_xls) else None
             try:
                 '''Load the Excel file'''
                 print(F"{DGREEN}Initializing conversion sequence{RESET}")
                 df = pd.read_excel(xls_file)
                 logger.info(f"Converting {xls_file}..")
                 total_rows = df.shape[0]
                 print(f"Writing {DYELLOW}{total_rows} rows {RESET}", end="\n")
                 for i in range(101):
                     print(f"Progress: {i}%", end="\r")
                 '''Save the DataFrame to CSV'''
                 df.to_csv(csv_file, index=False)
                 print(F"{DMAGENTA} Conversion successful{RESET}")
+
             except KeyboardInterrupt:
-                print("Exiting")
+                print("\nQuit❕")
                 sys.exit(1)
             except Exception as e:
                 print(e)
 
 ###############################################################################
 # Convert xlsx file(s) to sqlite
 ###############################################################################
 
     def convert_xlsx_to_database(self):
         xlsx_list = self.preprocess()
-        ls = ["xlsx", "xls"]
         xlsx_list = [
             item for item in xlsx_list if any(item.lower().endswith(ext)
-                                              for ext in ls)]
+                                              for ext in _ext_xls)]
         for xlsx_file in xlsx_list:
-            if xlsx_file.lower().endswith("xlsx"):
-                sqlfile = xlsx_file[:-4]
-            elif xlsx_file.lower().endswith("xls"):
-                sqlfile = xlsx_file[:-3]
+            ext = os.path.splitext(xlsx_file)[-1][1:]
+            sqlfile = (os.path.splitext(xlsx_file)[
+                       0] + ".sql") if ext in list(_ext_xls) else None
             try:
                 db_file = input(
                     F"{DBLUE}Please enter desired sql filename: {RESET}")
                 table_name = input(
                     "Please enter desired table name: ")
                 # res = ["db_file", "table_name"]
                 if any(db_file) == "":
-                    db_file = sqlfile + "sql"
-                    table_name = sqlfile
+                    db_file = sqlfile
+                    table_name = sqlfile[:-4]
                 if not db_file.endswith(".sql"):
-                    db_file = db_file + ".sql"
+                    db_file = sqlfile
                 column = 0
                 for i in range(20):
                     column += 0
                 # Read the Excel file into a pandas DataFrame
                 print(f"Reading {xlsx_file}...")
                 df = pd.read_excel(xlsx_file)
                 print(f"{DGREEN}Initializing conversion sequence{RESET}")
@@ -542,15 +583,15 @@
                 df.to_sql(table_name, column, conn,
                           if_exists='replace', index=False)
                 print(
                     f"Operation successful{RESET} file saved as \033[32{db_file}{RESET}")
                 # Close the database connection
                 conn.close()
             except KeyboardInterrupt:
-                print("\nExiting")
+                print("\nQuit❕")
                 sys.exit(1)
             except Exception as e:
                 logger.error(f"{e}")
 
 ###############################################################################
 # Create image objects from given files
 ###############################################################################
@@ -563,15 +604,15 @@
         file_list = [
             item for item in path_list if any(item.lower().endswith(ext)
                                               for ext in ls)]
         imgs = []
         for file in file_list:
             if file.lower().endswith("pdf"):
                 # Convert the PDF to a list of PIL image objects
-                print("Generate image objects ..")
+                print(f"{DBLUE}Generate image objects ..{RESET}")
                 images = convert_from_path(file)
 
                 # Save each image to a file
                 fname = file[:-4]
                 print(f"{YELLOW}Target images{BLUE} {len(images)}{RESET}")
                 for i, image in enumerate(images):
                     print(f"{DBLUE}{i}{RESET}", end="\r")
@@ -641,14 +682,28 @@
             tx = extract.OCR()
             if tx is not None:
                 text += tx
         print(text)
         print(f"{GREEN}Ok{RESET}")
         return text
 
+    def scanAsLongImg(self):
+        file = self.input_file
+        from .longImg import LImage
+        LI = LImage(file)
+        fl = LI.preprocess()
+        from .OCRTextExtractor import ExtractText
+
+        # fpath = file.split('.')[0] + '.png'
+        tx = ExtractText(fl)
+        text = tx.OCR()
+        print(text)
+        print(f"{GREEN}Ok{RESET}")
+        return text
+
 
 class FileSynthesis:
 
     def __init__(self, input_file):
         self.input_file = input_file
         # self.CHUNK_SIZE = 20_000
 
@@ -685,94 +740,147 @@
         for i in range(1, len(files)):
             combined_ogg += ogg_files[i]
 
         # Export the combined ogg to new mp3 file or ogg file
         combined_ogg.export(output_file + "_master.ogg", format='ogg')
         print(F"{DGREEN}Master file:Ok                                                                             {RESET}")
 
-    def Synthesise(self, text: str, output_file: str, CHUNK_SIZE: int = 20_000, ogg_folder: str = 'tempfile', retries: int = 5) -> None:
+    def Synthesise(self, text: str, output_file: str, CHUNK_SIZE: int = 10_000, _tmp_folder_: str = 'tmp_dir', max_retries: int = 10) -> None:
         """Converts given text to speech using Google Text-to-Speech API."""
         out_ls = []
+        # Define directories and other useful variables for genrating output_file and checkpoint_file
+        out_dir = os.path.split(output_file)[0]
+        _file_ = os.path.split(output_file)[1]
+        _full_output_path_ = os.path.join(out_dir, _tmp_folder_, _file_)
+        # Create a checkpoint_file for conversion resumption if need be
+        _check_file = os.path.splitext(_file_)[0] + '.ch'
+        _check_dir_path_ = os.path.join(out_dir, _tmp_folder_, _check_file)
+        checkpoint_file = _check_dir_path_
+
+        # Initialize start chank
+        start_chunk = 0
+        # Check if there is any checkpoint record in chekpoint file for resumption
+        if os.path.exists(checkpoint_file):
+            logger.info(f"{DYELLOW}Checkpoint file found{RESET}")
+            with open(checkpoint_file, 'r') as f:
+                start_chunk = int(f.read())
+            logger.info(f"{DYELLOW}Resuming from chunk{DBLUE} {start_chunk}{RESET}")
         try:
-            if not os.path.exists(ogg_folder):
-                os.mkdir(ogg_folder)
-            print(f"{DYELLOW}Get initial net speed..{RESET}")
-            st = speedtest.Speedtest()  # get initial network speed
-            st.get_best_server()
-            download_speed: float = st.download()  # Keep units as bytes
-            logger.info(
-
-                f"{GREEN} Conversion to mp3 sequence initialized start\
-speed {CYAN}{download_speed/1_000_000:.2f}Kbps{RESET}")
-
-            for attempt in range(retries):
+            if not os.path.exists(_tmp_folder_):
+                logger.info(f"{DYELLOW}Create temporary directory = {DBLUE}{_tmp_folder_}{RESET}")
+                os.mkdir(_tmp_folder_)
+
+            # print(f"{DYELLOW}Get initial net speed..{RESET}")# st = speedtest.Speedtest()  # get initial network speed# st.get_best_server()# download_speed: float = st.download()  # Keep units as bytes# logger.info( f"{GREEN} Conversion to mp3 sequence initialized start\speed {CYAN}{download_speed/1_000_000:.2f}Kbps{RESET}")
+
+            logger.info(f"{DYELLOW}Start conversion{RESET}")
+            attempt = 0
+            while attempt <= max_retries:
                 try:
                     '''Split input text into smaller parts and generate
                     individual gTTS objects'''
-                    counter = 0
-                    for i in range(0, len(text), CHUNK_SIZE):
+
+                    counter = start_chunk
+                    for ch, i in enumerate(range(start_chunk, len(text), CHUNK_SIZE)):
+                        logger.info(
+                            f"{BWHITE}Chunk {DBLUE}{i}{RESET}/{math.ceil(len(text)/CHUNK_SIZE)}")
                         chunk = text[i:i+CHUNK_SIZE]
-                        output_filename = f"{output_file}_{counter}.ogg"
+
+                        if os.path.exists(f"{_full_output_path_}_{counter}.ogg"):
+                            output_filename = f"{_full_output_path_}_{counter+1}.ogg"
+                        else:
+                            output_filename = f"{_full_output_path_}_{counter}.ogg"
                         counter += 1
-                        # print(output_filename)
-                        if os.path.exists(output_filename):
-                            output_filename = f"{output_file}_{counter+1}.ogg"
-                        # print(output_filename)
+
                         tts = gTTS(text=chunk, lang='en', slow=False)
                         tts.save(output_filename)
-                        out_ls.append(output_filename)
-                    break
-                    # print(out_ls)
+                        # Update checkpoint file
+                        with open(checkpoint_file, 'w') as f:
+                            f.write(str(counter))
+
+                    # Remove checkpoint file as processing is complete
+                    if os.path.exists(checkpoint_file):
+                        os.remove(checkpoint_file)
                     '''Handle any network related issue gracefully'''
-                except Exception in (ConnectionError, ConnectionAbortedError,
-                                     ConnectionRefusedError,
-                                     ConnectionResetError) as e:
-                    logger.error(f"Sorry boss connection problem encountered: {e} in {attempt+1}/{retries}:")
-                    time.sleep(5)  # Wait 5 seconds before retrying
 
                 # Handle connectivity/network error
+                except requests.exceptions.ConnectionError as e:
+                    logger.error(f"Connection error: {e}")
+                    # Exponential backoff for retries
+                    for _sec_ in range(2 ** attempt, 0, -1):
+                        print(f"{BWHITE}Resume in {DBLUE}{_sec_}{RESET}", end='\r')
+                    # Increament the attempts
+                    attempt += 1
+                # Exponential backoff for retries
+                except requests.exceptions.HTTPError as e:
+                    logger.error(f"HTTP error: {e.status_code} - {e.reason}")
+                    for _sec_ in range(2 ** attempt, 0, -1):
+                        print(f"{BWHITE}Resume in {DBLUE}{_sec_}{RESET}", end='\r')
+                    # Increament the attempts
+                    attempt += 1
                 except requests.exceptions.RequestException as e:
                     logger.error(f"{e}")
+
+                    # Exponential backoff for retries
+                    for _sec_ in range(2 ** attempt, 0, -1):
+                        print(f"{BWHITE}Resume in {DBLUE}{_sec_}{RESET}", end='\r')
+                    # Increament the attempts
+                    attempt += 1
+
+                except (ConnectionError, ConnectionAbortedError, ConnectionRefusedError, ConnectionResetError) as e:
+                    logger.error(f'Error during conversion attempt {attempt+1}/{max_retries}: {e}')
+                    # Exponential backoff for retries
+                    for _sec_ in range(2 ** attempt, 0, -1):
+                        print(f"{BWHITE}Resume in {DBLUE}{_sec_}{RESET}", end='\r')
+                        # Increament the attempts
+                        attempt += 1
+
+                # Handle all other types of exceptions
                 except Exception as e:
-                    logger.error(f'{DRED} Error during conversion attempt \
-{attempt+1}/{retries}:{e}{RESET}')
+                    logger.error(f'{DRED} Error during conversion attempt {attempt+1}/{max_retries}:{e}{RESET}')
+
                     tb = traceback.extract_tb(sys.exc_info()[2])
-                    logger.info("\n".join([f"  > {line}"
-                                           for line in map(str, tb)]))
-                    time.sleep(3)  # Wait 5 seconds before retrying
-                    pass
+                    logger.info("\n".join([f"  > {line}" for line in map(str, tb)]))
+                    # Exponential backoff for retries
+                    for _sec_ in range(2 ** attempt, 0, -1):
+                        print(f"{BWHITE}Resume in {DBLUE}{_sec_}{RESET}", end='\r')
+                    # Increament the attempts
+                    attempt += 1
 
-            if attempt >= retries:
-                logger.error(
-                    f"Conversion unsuccessful after {retries} attempts.")
+                else:
+                    print(f"{RED}Maximum retries reached. Unable to complete the operation.{RESET}")
+                    break  # Exit the retry loop if successful
+
+            else:
+                print(f"{RED}Maximum retries reached. Unable to complete the operation after {DMAGENTA} {max_retries} attempts.{RESET}")
                 sys.exit(2)
 
         finally:
-            # print(out_ls)
             # Combine generated gTTS objects
             if len(out_ls) >= 1:
                 FileSynthesis.join_audios(out_ls, output_file)
 
-            st = speedtest.Speedtest()
-            logger.info("Done")
-            print("Get final speed ...")
-            logger.info(
-
-                f"{YELLOW}Final Network Speed: {st.download()/(10**6):.2f} Kbps{RESET}")
+            # st = speedtest.Speedtest()
+            logger.info(f"{DGREEN}Success✅{DGREEN}")
+            # print("Get final speed ...")
+            # logger.info(f"{YELLOW}Final Network Speed: {st.download()/(10**6):.2f} Kbps{RESET}")
 
     @staticmethod
     def pdf_to_text(pdf_path):
-        logger.info('''Processing the file...\n''')
         logger.info(
-            F'{GREEN} Initializing pdf to text conversion sequence...{RESET}')
+            F'{GREEN} Initializing pdf to text conversion{RESET}')
         try:
             with open(pdf_path, 'rb') as file:
                 pdf_reader = PyPDF2.PdfReader(file)
                 text = ''
+                _pg_ = 0
+                print(F"{YELLOW}Convert pages..{RESET}")
                 for page_num in range(len(pdf_reader.pages)):
+                    _pg_ += 1
+                    logger.info(
+                        f"Page {DBLUE}{_pg_}{RESET}/{len(pdf_reader.pages)}")
                     page = pdf_reader.pages[page_num]
                     text += page.extract_text()
                 print(F"{DGREEN}Ok{RESET}")
                 return text
         except Exception as e:
             logger.error(
                 f"{DRED}Failed to extract text from '{YELLOW}{pdf_path}'{RESET}:\n {e}")
@@ -780,47 +888,46 @@
     @staticmethod
     def text_file(input_file):
         try:
             with open(input_file, 'r', errors='ignore') as file:
                 text = file.read().replace('\n', ' ')
             return text
         except FileNotFoundError:
-            logger.error("File '{}' was not found.".format(input_file))
+            logger.error("File '{}' was not found.📁".format(input_file))
         except Exception as e:
             logger.error(
-                F"{DRED}Error converting {input_file} to text: {str(e)}\
-{RESET}")
+                F"{DRED}{str(e)}{RESET}")
 
     @staticmethod
     def docx_to_text(docx_path):
         try:
-            logger.info(f"{BLUE} Converting {docx_path} to text...{RESET}")
+            logger.info(f"{BLUE} Converting {docx_path} to text{RESET}")
             doc = Document(docx_path)
             paragraphs = [paragraph.text for paragraph in doc.paragraphs]
             return '\n'.join(paragraphs)
         except FileNotFoundError:
-            logger.error(f"File '{docx_path}' was not found.")
+            logger.error(f"File '{docx_path}' was not found.📁")
         except Exception as e:
             logger.error(
                 F"{DRED}Error converting {docx_path} to text: {e}\
 {RESET}")
 
     '''Handle input files based on type to initialize conversion sequence'''
 
     def audiofy(self):
         input_list = self.preprocess()
-        extdoc = ["docx", "doc"]
         ls = {"pdf", "docx", "doc", "txt"}
-        input_list = [item for item in input_list if item.lower().endswith(tuple(ls))]
+        input_list = [
+            item for item in input_list if item.lower().endswith(tuple(ls))]
         for input_file in input_list:
             if input_file.endswith('.pdf'):
                 text = FileSynthesis.pdf_to_text(input_file)
                 output_file = input_file[:-4]
 
-            elif input_file.lower().endswith(tuple(extdoc)):
+            elif input_file.lower().endswith(tuple(_ext_word)):
 
                 text = FileSynthesis.docx_to_text(input_file)
                 output_file = input_file[:-5]
 
             elif input_file.endswith('.txt'):
                 text = FileSynthesis.text_file(input_file)
                 output_file = input_file[:-4]
@@ -828,14 +935,15 @@
             else:
                 logger.error('Unsupported file format. Please provide \
 a PDF, txt, or Word document.')
                 sys.exit(1)
             try:
                 FileSynthesis.Synthesise(None, text, output_file)
             except KeyboardInterrupt:
+                print("\nQuit❕")
                 sys.exit(1)
 
 
 ###############################################################################
 # Convert video file to from one format to another'''
 ###############################################################################
 
@@ -849,15 +957,15 @@
     def preprocess(self):
         files_to_process = []
 
         if os.path.isfile(self.input_file):
             files_to_process.append(self.input_file)
         elif os.path.isdir(self.input_file):
             if os.listdir(self.input_file) is None:
-                print("Cannot work with empty folder")
+                print(f"{RED}Cannot work with empty folder{RESET}")
                 sys.exit(1)
             for file in os.listdir(self.input_file):
                 file_path = os.path.join(self.input_file, file)
                 if os.path.isfile(file_path):
                     files_to_process.append(file_path)
 
         return files_to_process
@@ -872,15 +980,15 @@
 
             for file in input_list:
                 if out_f.upper() in SUPPORTED_VIDEO_FORMATS:
                     _, ext = os.path.splitext(file)
                     output_filename = _ + '.' + out_f.lower()
                     print(output_filename)
                 else:
-                    print("Unsupported output format")
+                    print(f"{RED}Unsupported output format{RESET}")
                     sys.exit(1)
                 format_codec = {
                     "MP4": "mpeg4",
                     "AVI": "rawvideo",
                     # "OGV": "avc",
                     "WEBM": "libvpx",
                     "MOV": "mpeg4",
@@ -895,15 +1003,15 @@
                 print(f"{DMAGENTA}Converting file to {output_filename}{RESET}")
                 video.write_videofile(
                     output_filename, codec=format_codec[out_f])
                 '''Close the video file'''
                 print(f"{DGREEN}Done{RESET}")
                 video.close()
         except KeyboardInterrupt:
-            print("\nExiting..")
+            print("\nQuit❕")
             sys.exit(1)
         except Exception as e:
             print(e)
 
 
 ###############################################################################
 # Convert Audio file to from one format to another'''
@@ -919,45 +1027,51 @@
     def preprocess(self):
         files_to_process = []
 
         if os.path.isfile(self.input_file):
             files_to_process.append(self.input_file)
         elif os.path.isdir(self.input_file):
             if os.listdir(self.input_file) is None:
-                print("Cannot work with empty folder")
+                print(f"{RED}Cannot work with empty folder{RESET}")
                 sys.exit(1)
             for file in os.listdir(self.input_file):
                 file_path = os.path.join(self.input_file, file)
                 if os.path.isfile(file_path):
                     files_to_process.append(file_path)
 
         return files_to_process
 
     def pydub_conv(self):
-        input_list = self.preprocess()
-        out_f = self.out_format
-        input_list = [item for item in input_list if any(
-            item.lower().endswith(ext) for ext in SUPPORTED_AUDIO_FORMATS)]
-        print(F"{DYELLOW}Initializing conversion..{RESET}")
-        for file in input_list:
-            if out_f.lower() in SUPPORTED_AUDIO_FORMATS:
-                _, ext = os.path.splitext(file)
-                output_filename = _ + '.' + out_f
-            else:
-                print("Unsupported output format")
-                sys.exit(1)
-            fmt = ext[1:]
-            print(fmt, out_f)
-            audio = pydub.AudioSegment.from_file(file, fmt)
-            print(f"{DMAGENTA}Converting to {output_filename}{RESET}")
-            audio.export(output_filename, format=out_f)
-            # new_audio = pydub.AudioSegment.from_file('output_audio.')
-            print(f"{DGREEN}Done{RESET}")
-            # play(new_audio)
-            # new_audio.close()
+        try:
+            input_list = self.preprocess()
+            out_f = self.out_format
+            input_list = [item for item in input_list if any(
+                item.lower().endswith(ext) for ext in SUPPORTED_AUDIO_FORMATS)]
+            print(F"{DYELLOW}Initializing conversion..{RESET}")
+            for file in input_list:
+                if out_f.lower() in SUPPORTED_AUDIO_FORMATS:
+                    _, ext = os.path.splitext(file)
+                    output_filename = _ + '.' + out_f
+                else:
+                    print(F"{RED}Unsupported output format{RESET}")
+                    sys.exit(1)
+                fmt = ext[1:]
+                print(fmt, out_f)
+                audio = pydub.AudioSegment.from_file(file, fmt)
+                print(f"{DMAGENTA}Converting to {output_filename}{RESET}")
+                audio.export(output_filename, format=out_f)
+                # new_audio = pydub.AudioSegment.from_file('output_audio.')
+                print(f"{DGREEN}Done{RESET}")
+                # play(new_audio)
+                # new_audio.close()
+        except KeyboardInterrupt:
+            print("\nQuit❕")
+            sys.exit(1)
+        except Exception as e:
+            print(f"{RED}{e}{RED}")
 
 
 ###############################################################################
 # Convert images file to from one format to another
 ###############################################################################
 
 
@@ -980,15 +1094,15 @@
                 for file in os.listdir(self.input_file):
                     file_path = os.path.join(self.input_file, file)
                     if os.path.isfile(file_path):
                         files_to_process.append(file_path)
 
             return files_to_process
         except FileNotFoundError:
-            print("File not found")
+            print("File not found❕")
             sys.exit(1)
 
     def convert_image(self):
         try:
             input_list = self.preprocess()
             out_f = self.out_format.upper()
 
@@ -1019,9 +1133,9 @@
                 '''Display the images: '''
                 cv2.imshow('OpenCV Image', opencv_img)
                 # pil_img.show()
                 '''Wait for the user to press a key and close the windows: '''
                 cv2.waitKey(0)
                 cv2.destroyAllWindows()
         except KeyboardInterrupt:
-            print("\nExiting..")
+            print("\nQuit❕")
             sys.exit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `filemac-1.0.2/filemac/fmac.py` & `filemac-1.0.3/filemac/fmac.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import logging
 import logging.handlers
 import sys
 
 from . import handle_warnings
 from .AudioExtractor import ExtractAudio
-from .colors import (RESET, DYELLOW)
+from .colors import CYAN, DYELLOW, RESET
 from .converter import (AudioConverter, FileSynthesis, ImageConverter,
                         MakeConversion, Scanner, VideoConverter)
 from .formats import (SUPPORTED_AUDIO_FORMATS_SHOW, SUPPORTED_DOC_FORMATS,
                       SUPPORTED_IMAGE_FORMATS_SHOW,
                       SUPPORTED_VIDEO_FORMATS_SHOW)
 from .image_op import Compress_Size
 from .OCRTextExtractor import ExtractText
@@ -117,27 +117,37 @@
         example {DYELLOW}filemac --analyze_video example.mp4 {RESET}")
 
     parser.add_argument("-t", "--target_format",
                         help="Target format for conversion (optional)")
 
     parser.add_argument(
         "--resize_image", help=f"change size of an image compress/decompress \
-        example {DYELLOW}filemac --resize_image example.png -t png {RESET}")
+        example {DYELLOW}filemac --resize_image example.png -t_size 2mb -t png {RESET}")
 
     parser.add_argument("-t_size", help="used in combination with resize_image \
                         to specify target image size")
 
     parser.add_argument(
         "-S", "--scan", help=f"Scan pdf file and extract text\
                         example {DYELLOW}filemac --scan example.pdf {RESET}")
 
     parser.add_argument(
+
+        "-doc2L", "--doc_long_image", help=f"Convert pdf file to long image\
+                        example {DYELLOW}filemac --doc_long_image example.pdf {RESET}")
+
+    parser.add_argument(
         "-SA", "--scanAsImg", help=f"Scan pdf file and extract text\
                         example {DYELLOW}filemac --scanAsImg example.pdf {RESET}")
 
+    parser.add_argument(
+        "-SALI", "--scanAsLong_Image", help=f"Scan {CYAN}[doc, docx, pdf]\
+        {RESET} file and extract text,-> very effective\
+                    example {DYELLOW}filemac --scanAsImg example.pdf {RESET}")
+
     parser.add_argument("--OCR", help=f"Extract text from an image.\
         example {DYELLOW}filemac --OCR image.png{RESET}")
 
     args = parser.parse_args()
 
 
 # Call function to handle document conversion inputs before begining conversion
@@ -147,23 +157,23 @@
     if args.convert_doc:
         ev = Eval(args.convert_doc, args.target_format)
         ev.document_eval()
 
 
 # Call function to handle video conversion inputs before begining conversion
     elif args.convert_video:
-        if args.convert_video == 'help' or args.convert_video is None:
+        if args.convert_video == 'help':
             print(SUPPORTED_VIDEO_FORMATS_SHOW)
             sys.exit(1)
         ev = VideoConverter(args.convert_video, args.target_format)
         ev.CONVERT_VIDEO()
 # Call function to handle image conversion inputs before begining conversion
 
     elif args.convert_image:
-        if args.convert_image == 'help' or args.convert_image is None:
+        if args.convert_image == 'help':
             print(SUPPORTED_IMAGE_FORMATS_SHOW)
             sys.exit(1)
         conv = ImageConverter(args.convert_image, args.target_format)
         conv.convert_image()
 
 # Handle image resizing
     elif args.resize_image:
@@ -173,15 +183,15 @@
 # Handle documents to images conversion
     elif args.convert_doc2image:
         conv = MakeConversion(args.convert_doc2image)
         conv.doc2image(args.target_format)
 
 # Call function to handle audio conversion inputs before begining conversion
     elif args.convert_audio:
-        if args.convert_audio == 'help' or args.convert_audio is None:
+        if args.convert_audio == 'help':
             print(SUPPORTED_AUDIO_FORMATS_SHOW)
             sys.exit(1)
         ev = AudioConverter(args.convert_audio, args.target_format)
         ev.pydub_conv()
 
 
 # Call module to evaluate audio files before making audio extraction from input video files conversion
@@ -193,15 +203,27 @@
     elif args.scan:
         sc = Scanner(args.scan)
         sc.scanPDF()
 
 # Call module to scan the input FILE as image object and extract text
     elif args.scanAsImg:
         sc = Scanner(args.scanAsImg)
-        tx = sc.scanAsImgs()
+        sc.scanAsImgs()
+
+# Call module to scan the input FILE as long image object and extract text
+# effective for text intengration(combining)
+    elif args.scanAsLong_Image:
+        sc = Scanner(args.scanAsLong_Image)
+        sc.scanAsLongImg()
+
+# convert document to long image
+    elif args.doc_long_image:
+        from .longImg import LImage
+        conv = LImage(args.doc_long_image)
+        conv.preprocess()
 # Call module to handle Candidate images for text extraction inputs before begining conversion
     elif args.OCR:
         conv = ExtractText(args.OCR)
         conv.OCR()
 
     elif args.Analyze_video:
         analyzer = SA(args.Analyze_video)
```

### Comparing `filemac-1.0.2/filemac/formats.py` & `filemac-1.0.3/filemac/formats.py`

 * *Files identical despite different names*

### Comparing `filemac-1.0.2/filemac/image_op.py` & `filemac-1.0.3/filemac/image_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from PIL import Image
 import os
 import logging
 import logging.handlers
+from .colors import DYELLOW, RESET, YELLOW, DGREEN, DMAGENTA, BLUE
 
 logging.basicConfig(level=logging.INFO, format='%(levelname)-8s %(message)s')
 logger = logging.getLogger(__name__)
 
 
 class Compress_Size:
 
     def __init__(self, input_image_path):
         self.input_image_path = input_image_path
 
     def resize_image(self, target_size):
+        input_image_path = self.input_image_path
         ext = input_image_path[-3:]
         output_image_path = os.path.splitext(input_image_path)[0] + f"_resized.{ext}"
 
         original_image = Image.open(input_image_path)
         original_size = original_image.size
         size = os.path.getsize(input_image_path)
-        print(f"Original image size \033[93m{size/1000_000:.2f}MiB")
+        print(f"Original image size {YELLOW}{size/1000_000:.2f}MiB{RESET}")
 
         # Calculate the aspect ratio of the original image
         aspect_ratio = original_size[0] / original_size[1]
 
         # Convert the target sixze to bytes
         tz = int(target_size[:-2])
         if target_size[-2:].lower() == 'mb':
             target_size_bytes = tz * 1024 * 1024
         elif target_size[-2:].lower() == 'kb':
             target_size_bytes = tz * 1024
         else:
-            logger.warning("Invalid units. Please use either \033[1;95m'MB'\033[0m\
-    or \033[1;95m'KB'\033[0m")
+            logger.warning(f"Invalid units. Please use either {DMAGENTA}'MB'{RESET}\
+    or {DMAGENTA}'KB'{RESET}")
 
         # Calculate the new dimensions based on the target size
         new_width, new_height = Compress_Size.calculate_new_dimensions(original_size, aspect_ratio, target_size_bytes)
-        print("\033[94mProcessing ..\033[0m")
+        print(F"{BLUE}Processing ..{RESET}")
         resized_image = original_image.resize((new_width, new_height))
-        resized_image.save(output_image_path)
+        resized_image.save(output_image_path, optimize=True, format='png')
         t_size = os.path.getsize(output_image_path)/1000_000
-        print("\033[1;92mOk\033[0m")
-        print(f"Image resized to \033[1;93m{t_size:.2f}\033[0m and saved to \033[1;93m{output_image_path}")
+        print(F"{DGREEN}Ok{RESET}")
+        print(f"Image resized to {DYELLOW}{t_size:.2f}{RESET} and saved to {DYELLOW}{output_image_path}")
 
     def calculate_new_dimensions(original_size, aspect_ratio, target_size_bytes):
         # Calculate the new dimensions based on the target size in bytes
         original_size_bytes = original_size[0] * original_size[1] * 3  # Assuming 24-bit color depth
         scale_factor = (target_size_bytes / original_size_bytes) ** 0.5
 
         new_width = int(original_size[0] * scale_factor)
```

### Comparing `filemac-1.0.2/filemac.egg-info/PKG-INFO` & `filemac-1.0.3/filemac.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filemac
-Version: 1.0.2
+Version: 1.0.3
 Summary: Open source Python CLI toolkit for conversion, manipulation, Analysis
 Author: wambua
 Author-email: wambuamwiky2001@gmail.com
 License: GPL v3
 Keywords: file-conversion,file-analysis,file-manipulation,ocr,image-conversion
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
@@ -22,14 +22,20 @@
 License-File: LICENSE
 
 # fconverter
 A python file `conversion`, `manipulation`, `Analysis` toolkit
 `This is a Linux command-line interface (CLI) utility that coverts documents from one format to another,
 analyzes files, manipulates files.
 Your can also convert text file to mp3 formart using google Text to speech library (gTTS).
+## Name variations
+```shell
+   filemac -h
+   Filemac -h
+   FILEMAC -h
+   ```
 
 ## Installation
 1. using pip
 
    ```shell
 	pip install filemac
    ```
```

### Comparing `filemac-1.0.2/filemac.egg-info/SOURCES.txt` & `filemac-1.0.3/filemac.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 LICENSE
 MANIFEST.ini
 README.md
+README.md~
 setup.py
+setup.py~
 version.txt
+version.txt~
 .github/workflows/python-publish.yml
 __pycache__/Analyzer.cpython-311.pyc
 __pycache__/AudioExtractor.cpython-311.pyc
 __pycache__/OCRTextExtractor.cpython-311.pyc
 __pycache__/Simple_v_Analyzer.cpython-311.pyc
 __pycache__/converter.cpython-311.pyc
 __pycache__/formarts.cpython-311.pyc
 __pycache__/formats.cpython-311.pyc
+__pycache__/setup.cpython-311.pyc
 __pycache__/show_progress.cpython-311.pyc
 filemac/AudioExtractor.py
 filemac/OCRTextExtractor.py
 filemac/Simple_v_Analyzer.py
 filemac/__init__.py
 filemac/colors.py
 filemac/converter.py
 filemac/dd.py
 filemac/fmac.py
 filemac/formats.py
 filemac/handle_warnings.py
 filemac/image_op.py
+filemac/longImg.py
+filemac/pdfaudio.py
 filemac.egg-info/PKG-INFO
 filemac.egg-info/SOURCES.txt
 filemac.egg-info/dependency_links.txt
 filemac.egg-info/entry_points.txt
 filemac.egg-info/not-zip-safe
 filemac.egg-info/requires.txt
 filemac.egg-info/top_level.txt
 filemac/__pycache__/AudioExtractor.cpython-311.pyc
 filemac/__pycache__/OCRTextExtractor.cpython-311.pyc
 filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc
 filemac/__pycache__/colors.cpython-311.pyc
 filemac/__pycache__/converter.cpython-311.pyc
-filemac/__pycache__/formats.cpython-311.pyc
+filemac/__pycache__/formats.cpython-311.pyc
+tets/dd.py
+tets/test.py
+tets/__pycache__/dd.cpython-311.pyc
```

### Comparing `filemac-1.0.2/setup.py` & `filemac-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,19 @@
     packages=find_namespace_packages(exclude=EXCLUDE_FROM_PACKAGES),
     description=DESCRIPTION,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
 
     entry_points={
         "console_scripts": [
-            "filemac=filemac:main"
-        ]},
+            "filemac=filemac:main",
+            "Filemac=filemac:main",
+            "FILEMAC=filemac:main",
+        ],
+    },
 
 
     python_requires=">=3.6",
     install_requires=[
         'argparse',
         'pdfminer.six',
         'python-docx',
@@ -77,10 +80,8 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-
-
 )
```

