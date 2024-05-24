# Comparing `tmp/labjack_pic-0.0.5.tar.gz` & `tmp/labjack_pic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labjack_pic-0.0.5.tar", last modified: Mon Jun  5 16:05:54 2023, max compression
+gzip compressed data, was "labjack_pic-0.0.6.tar", last modified: Fri May 24 21:20:46 2024, max compression
```

## Comparing `labjack_pic-0.0.5.tar` & `labjack_pic-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/
--rw-rw-r--   0 markrages  (1001) markrages  (1000)    11357 2022-11-20 02:22:29.000000 labjack_pic-0.0.5/LICENSE
--rw-rw-r--   0 markrages  (1001) markrages  (1000)     3182 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/PKG-INFO
--rw-rw-r--   0 markrages  (1001) markrages  (1000)     2642 2022-12-14 01:50:19.000000 labjack_pic-0.0.5/README.md
--rw-rw-r--   0 markrages  (1001) markrages  (1000)      726 2023-06-05 16:04:43.000000 labjack_pic-0.0.5/pyproject.toml
--rw-rw-r--   0 markrages  (1001) markrages  (1000)       38 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/setup.cfg
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.298288 labjack_pic-0.0.5/src/
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/src/labjack_pic/
--rw-rw-r--   0 markrages  (1001) markrages  (1000)        1 2022-12-01 04:10:46.000000 labjack_pic-0.0.5/src/labjack_pic/__init__.py
--rwxrwxr-x   0 markrages  (1001) markrages  (1000)    15613 2023-06-05 16:00:08.000000 labjack_pic-0.0.5/src/labjack_pic/lj_pic.py
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/src/labjack_pic/u3_manager/
--rw-rw-r--   0 markrages  (1001) markrages  (1000)        0 2022-12-01 04:10:38.000000 labjack_pic-0.0.5/src/labjack_pic/u3_manager/__init__.py
--rwxr--r--   0 markrages  (1001) markrages  (1000)    13637 2023-06-05 16:00:37.000000 labjack_pic-0.0.5/src/labjack_pic/u3_manager/u3_manager.py
-drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2023-06-05 16:05:54.302288 labjack_pic-0.0.5/src/labjack_pic.egg-info/
--rw-rw-r--   0 markrages  (1001) markrages  (1000)     3182 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/PKG-INFO
--rw-rw-r--   0 markrages  (1001) markrages  (1000)      402 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/SOURCES.txt
--rw-rw-r--   0 markrages  (1001) markrages  (1000)        1 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/dependency_links.txt
--rw-rw-r--   0 markrages  (1001) markrages  (1000)       56 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/entry_points.txt
--rw-rw-r--   0 markrages  (1001) markrages  (1000)       23 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/requires.txt
--rw-rw-r--   0 markrages  (1001) markrages  (1000)       12 2023-06-05 16:05:54.000000 labjack_pic-0.0.5/src/labjack_pic.egg-info/top_level.txt
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2024-05-24 21:20:46.960547 labjack_pic-0.0.6/
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)    11357 2022-11-20 02:22:29.000000 labjack_pic-0.0.6/LICENSE
+-rw-r--r--   0 markrages  (1001) markrages  (1000)     3500 2024-05-24 21:20:46.960547 labjack_pic-0.0.6/PKG-INFO
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)     2907 2024-05-17 15:09:30.000000 labjack_pic-0.0.6/README.md
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)      726 2024-05-24 21:17:46.000000 labjack_pic-0.0.6/pyproject.toml
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)       38 2024-05-24 21:20:46.960547 labjack_pic-0.0.6/setup.cfg
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2024-05-24 21:20:46.956547 labjack_pic-0.0.6/src/
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2024-05-24 21:20:46.960547 labjack_pic-0.0.6/src/labjack_pic/
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)        1 2022-12-01 04:10:46.000000 labjack_pic-0.0.6/src/labjack_pic/__init__.py
+-rwxrwxr-x   0 markrages  (1001) markrages  (1000)    24127 2024-05-24 20:43:17.000000 labjack_pic-0.0.6/src/labjack_pic/lj_pic.py
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2024-05-24 21:20:46.960547 labjack_pic-0.0.6/src/labjack_pic/u3_manager/
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)        0 2022-12-01 04:10:38.000000 labjack_pic-0.0.6/src/labjack_pic/u3_manager/__init__.py
+-rwxr--r--   0 markrages  (1001) markrages  (1000)    13637 2023-06-05 16:00:37.000000 labjack_pic-0.0.6/src/labjack_pic/u3_manager/u3_manager.py
+drwxrwxr-x   0 markrages  (1001) markrages  (1000)        0 2024-05-24 21:20:46.960547 labjack_pic-0.0.6/src/labjack_pic.egg-info/
+-rw-r--r--   0 markrages  (1001) markrages  (1000)     3500 2024-05-24 21:20:46.000000 labjack_pic-0.0.6/src/labjack_pic.egg-info/PKG-INFO
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)      402 2024-05-24 21:20:46.000000 labjack_pic-0.0.6/src/labjack_pic.egg-info/SOURCES.txt
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)        1 2024-05-24 21:20:46.000000 labjack_pic-0.0.6/src/labjack_pic.egg-info/dependency_links.txt
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)       56 2024-05-24 21:20:46.000000 labjack_pic-0.0.6/src/labjack_pic.egg-info/entry_points.txt
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)       23 2024-05-24 21:20:46.000000 labjack_pic-0.0.6/src/labjack_pic.egg-info/requires.txt
+-rw-rw-r--   0 markrages  (1001) markrages  (1000)       12 2024-05-24 21:20:46.000000 labjack_pic-0.0.6/src/labjack_pic.egg-info/top_level.txt
```

### Comparing `labjack_pic-0.0.5/LICENSE` & `labjack_pic-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `labjack_pic-0.0.5/PKG-INFO` & `labjack_pic-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: labjack_pic
-Version: 0.0.5
+Version: 0.0.6
 Summary: Program PIC microcontrollers using LabJack U3
 Author-email: Mark Rages <markrages@gmail.com>
 Project-URL: Homepage, https://github.com/markrages/labjack_pic/
 Project-URL: Bug Tracker, https://github.com/markrages/labjack_pic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: intelhex
+Requires-Dist: LabJackPython
 
 # labjack_pic
 
 Program PIC microcontrollers using LabJack U3
 
 I have multiple PICkits 1, 2, and 3, but none of them can program the
 part I selected for my latest project. Rather than shell out for yet
@@ -56,18 +58,30 @@
 ## Devices supported
 
 This script only supports low-voltage programming. This means MCLR is
 not available as a general-purpose input in the circuit.  This also
 means that this programmer cannot recover a part that has been
 programmed to MCLR-as-input.
 
-Currently supports devices covered by [Programming Specification 40002317](https://ww1.microchip.com/downloads/aemDocuments/documents/MCU08/ProductDocuments/ProgrammingSpecifications/PIC16F180XX-Family-Programming-Specification-40002317.pdf) and [Programming Specification 40002266](https://ww1.microchip.com/downloads/aemtest/MCU08/ProductDocuments/ProgrammingSpecifications/PIC16F171XX-Family-Programming-Specification-40002266.pdf).
+Currently supports devices covered by [Programming Specification 40002317](https://ww1.microchip.com/downloads/aemDocuments/documents/MCU08/ProductDocuments/ProgrammingSpecifications/PIC16F180XX-Family-Programming-Specification-40002317.pdf), [Programming Specification 40002266](https://ww1.microchip.com/downloads/aemtest/MCU08/ProductDocuments/ProgrammingSpecifications/PIC16F171XX-Family-Programming-Specification-40002266.pdf), and [Programming Specification 40001683B](https://ww1.microchip.com/downloads/en/DeviceDoc/40001683B.pdf)
 
 These are:
 
+- PIC16F1703
+- PIC16LF1703
+- PIC16F1704
+- PIC16LF1704
+- PIC16F1705
+- PIC16LF1705
+- PIC16F1707
+- PIC16LF1707
+- PIC16F1708
+- PIC16LF1708
+- PIC16F1709
+- PIC16LF1709
 - PIC16F17114
 - PIC16F17115
 - PIC16F17124
 - PIC16F17125
 - PIC16F17126
 - PIC16F17144
 - PIC16F17145
```

### Comparing `labjack_pic-0.0.5/README.md` & `labjack_pic-0.0.6/src/labjack_pic.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: labjack_pic
+Version: 0.0.6
+Summary: Program PIC microcontrollers using LabJack U3
+Author-email: Mark Rages <markrages@gmail.com>
+Project-URL: Homepage, https://github.com/markrages/labjack_pic/
+Project-URL: Bug Tracker, https://github.com/markrages/labjack_pic/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: intelhex
+Requires-Dist: LabJackPython
+
 # labjack_pic
 
 Program PIC microcontrollers using LabJack U3
 
 I have multiple PICkits 1, 2, and 3, but none of them can program the
 part I selected for my latest project. Rather than shell out for yet
 another PICkit, I wrote this script to program the part using a
@@ -42,18 +58,30 @@
 ## Devices supported
 
 This script only supports low-voltage programming. This means MCLR is
 not available as a general-purpose input in the circuit.  This also
 means that this programmer cannot recover a part that has been
 programmed to MCLR-as-input.
 
-Currently supports devices covered by [Programming Specification 40002317](https://ww1.microchip.com/downloads/aemDocuments/documents/MCU08/ProductDocuments/ProgrammingSpecifications/PIC16F180XX-Family-Programming-Specification-40002317.pdf) and [Programming Specification 40002266](https://ww1.microchip.com/downloads/aemtest/MCU08/ProductDocuments/ProgrammingSpecifications/PIC16F171XX-Family-Programming-Specification-40002266.pdf).
+Currently supports devices covered by [Programming Specification 40002317](https://ww1.microchip.com/downloads/aemDocuments/documents/MCU08/ProductDocuments/ProgrammingSpecifications/PIC16F180XX-Family-Programming-Specification-40002317.pdf), [Programming Specification 40002266](https://ww1.microchip.com/downloads/aemtest/MCU08/ProductDocuments/ProgrammingSpecifications/PIC16F171XX-Family-Programming-Specification-40002266.pdf), and [Programming Specification 40001683B](https://ww1.microchip.com/downloads/en/DeviceDoc/40001683B.pdf)
 
 These are:
 
+- PIC16F1703
+- PIC16LF1703
+- PIC16F1704
+- PIC16LF1704
+- PIC16F1705
+- PIC16LF1705
+- PIC16F1707
+- PIC16LF1707
+- PIC16F1708
+- PIC16LF1708
+- PIC16F1709
+- PIC16LF1709
 - PIC16F17114
 - PIC16F17115
 - PIC16F17124
 - PIC16F17125
 - PIC16F17126
 - PIC16F17144
 - PIC16F17145
```

### Comparing `labjack_pic-0.0.5/pyproject.toml` & `labjack_pic-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "labjack_pic"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Mark Rages", email="markrages@gmail.com" },
 ]
 description = "Program PIC microcontrollers using LabJack U3"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `labjack_pic-0.0.5/src/labjack_pic/u3_manager/u3_manager.py` & `labjack_pic-0.0.6/src/labjack_pic/u3_manager/u3_manager.py`

 * *Files identical despite different names*

