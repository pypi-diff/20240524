# Comparing `tmp/zahner_potentiostat-1.1.0.tar.gz` & `tmp/zahner_potentiostat-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zahner_potentiostat-1.1.0.tar", last modified: Mon Jan 16 07:13:43 2023, max compression
+gzip compressed data, was "zahner_potentiostat-1.1.1.tar", last modified: Fri May 24 05:49:40 2024, max compression
```

## Comparing `zahner_potentiostat-1.1.0.tar` & `zahner_potentiostat-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:43.409923 zahner_potentiostat-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1085 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     6583 2023-01-16 07:13:43.409923 zahner_potentiostat-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5240 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-16 07:13:43.409923 zahner_potentiostat-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1706 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:43.405923 zahner_potentiostat-1.1.0/zahner_potentiostat/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:43.409923 zahner_potentiostat-1.1.0/zahner_potentiostat/display/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10270 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/display/dcplot.py
--rw-r--r--   0 runner    (1001) docker     (116)    15970 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/display/onlinedisplay.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:43.409923 zahner_potentiostat-1.1.0/zahner_potentiostat/drivecycle/
--rw-r--r--   0 runner    (1001) docker     (116)     8054 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/drivecycle/HUDDSCOL.py
--rw-r--r--   0 runner    (1001) docker     (116)     4419 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/drivecycle/NYCCCOL.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/drivecycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5042 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/drivecycle/cycle_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:43.409923 zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/
--rw-r--r--   0 runner    (1001) docker     (116)       52 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    98082 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/control.py
--rw-r--r--   0 runner    (1001) docker     (116)     5201 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/datahandler.py
--rw-r--r--   0 runner    (1001) docker     (116)    21428 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/datareceiver.py
--rw-r--r--   0 runner    (1001) docker     (116)     4239 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/error.py
--rw-r--r--   0 runner    (1001) docker     (116)    12788 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/searcher.py
--rw-r--r--   0 runner    (1001) docker     (116)    15549 2023-01-16 07:13:33.000000 zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/serial_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-16 07:13:43.405923 zahner_potentiostat-1.1.0/zahner_potentiostat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6583 2023-01-16 07:13:43.000000 zahner_potentiostat-1.1.0/zahner_potentiostat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      898 2023-01-16 07:13:43.000000 zahner_potentiostat-1.1.0/zahner_potentiostat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-16 07:13:43.000000 zahner_potentiostat-1.1.0/zahner_potentiostat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       26 2023-01-16 07:13:43.000000 zahner_potentiostat-1.1.0/zahner_potentiostat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2023-01-16 07:13:43.000000 zahner_potentiostat-1.1.0/zahner_potentiostat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.915853 zahner_potentiostat-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.907853 zahner_potentiostat-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.907853 zahner_potentiostat-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.911853 zahner_potentiostat-1.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/LICENSES/matplotlib
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/LICENSES/numpy
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/LICENSES/pyserial
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/LICENSES/scipy
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-24 05:49:40.915853 zahner_potentiostat-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 05:49:40.915853 zahner_potentiostat-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.911853 zahner_potentiostat-1.1.1/zahner_potentiostat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.911853 zahner_potentiostat-1.1.1/zahner_potentiostat/display/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/display/dcplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15970 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/display/onlinedisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.911853 zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/HUDDSCOL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/NYCCCOL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/cycle_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/sources.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.911853 zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98082 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/datahandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21428 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/datareceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12788 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15549 2024-05-24 05:49:34.000000 zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/serial_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 05:49:40.915853 zahner_potentiostat-1.1.1/zahner_potentiostat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-24 05:49:40.000000 zahner_potentiostat-1.1.1/zahner_potentiostat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-24 05:49:40.000000 zahner_potentiostat-1.1.1/zahner_potentiostat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 05:49:40.000000 zahner_potentiostat-1.1.1/zahner_potentiostat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 05:49:40.000000 zahner_potentiostat-1.1.1/zahner_potentiostat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 05:49:40.000000 zahner_potentiostat-1.1.1/zahner_potentiostat.egg-info/top_level.txt
```

### Comparing `zahner_potentiostat-1.1.0/LICENSE` & `zahner_potentiostat-1.1.1/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Zahner-Elektrik GmbH & Co. KG
+Copyright (c) 2024 Zahner-Elektrik
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `zahner_potentiostat-1.1.0/PKG-INFO` & `zahner_potentiostat-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,73 @@
 Metadata-Version: 2.1
 Name: zahner_potentiostat
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library to control Zahner Potentiostats.
-Home-page: https://zahner.de/
-Author: Maximilian Krapp
-Author-email: maximilian.krapp@zahner.de
-License: MIT
-Project-URL: Documentation, https://doc.zahner.de/zahner_potentiostat/index.html
+Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
+License: MIT License
+        
+        Copyright (c) 2024 Zahner-Elektrik
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Documentation, https://doc.zahner.de/zahner_potentiostat
 Project-URL: Examples, https://github.com/Zahner-elektrik/Zahner-Remote-Python
 Project-URL: Source Code, https://github.com/Zahner-elektrik/zahner_potentiostat
 Project-URL: Bug Tracker, https://github.com/Zahner-elektrik/zahner_potentiostat/issues
-Keywords: potentiostat, electrochemistry, chemistry, eis, cyclic voltammetry, fuel-cell, battery
-Platform: any
+Project-URL: Homepage, https://zahner.de/
+Keywords: potentiostat,electrochemistry,chemistry,eis,cyclic voltammetry,fuel-cell,battery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: pyserial
+Requires-Dist: numpy
 
 # zahner_potentiostat
 
 zahner_potentiostat is a library to control external [Zahner Potentiostats](https://zahner.de/products#external-potentiostats) like **PP212, PP222, PP242, XPOT2 or EL1002**.
 
 It was developed to **easily integrate** external Zahner Potentiostats into Python scripts for more **complex measurement** tasks and for **automation purposes**.
 
 The control concept is that there are different primitives which can be combined for different electrochemical measurement methods.  
 These primitives can all be configured differently to match the application. In the documentation in the respective function all possible configuration setter methods are listed. The complete documentation of the functions can be found on the [API documentation website](https://doc.zahner.de/zahner_potentiostat/).  
 
+> [!NOTE]  
+> **Only with this library and a PP212, PP222, PP242, EL1002 or XPOT2 device you can not use AC methods. For AC methods like EIS a [Zennium](https://zahner.de/products#potentiostats) with [EPC](https://zahner.de/products-details/addon-cards/epc42) and the [thales_remote](https://github.com/Zahner-elektrik/Thales-Remote-Python) library is necessary.**
+
 **The following [primitives](https://en.wikipedia.org/wiki/Language_primitive) are available to compose methods with:**  
 
 * Potentiostatic or galvanostatic polarization  
   * [measurePolarization()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measurePolarization)  
 * Open circuit voltage/potential scan  
   * [measureOCV()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measureOCV)  
   * [measureOCVScan()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measureOCVScan)  
@@ -103,15 +130,15 @@
 ZahnerPP2x2.measurePolarization()
 ```
 
 # 📖 Examples
 
 The application of the library is shown in the example repository [Zahner-Remote-Python](https://github.com/Zahner-elektrik/Zahner-Remote-Python).
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send an <a href="mailto:support@zahner.de?subject=Zahner-Remote-Python Question&body=Your Message">e-mail</a> to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Remote-Python](https://github.com/Zahner-elektrik/Zahner-Remote-Python/issues) repository. If you already found a solution to your problem, **we would love to review your pull request**!
```

### Comparing `zahner_potentiostat-1.1.0/README.md` & `zahner_potentiostat-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 zahner_potentiostat is a library to control external [Zahner Potentiostats](https://zahner.de/products#external-potentiostats) like **PP212, PP222, PP242, XPOT2 or EL1002**.
 
 It was developed to **easily integrate** external Zahner Potentiostats into Python scripts for more **complex measurement** tasks and for **automation purposes**.
 
 The control concept is that there are different primitives which can be combined for different electrochemical measurement methods.  
 These primitives can all be configured differently to match the application. In the documentation in the respective function all possible configuration setter methods are listed. The complete documentation of the functions can be found on the [API documentation website](https://doc.zahner.de/zahner_potentiostat/).  
 
+> [!NOTE]  
+> **Only with this library and a PP212, PP222, PP242, EL1002 or XPOT2 device you can not use AC methods. For AC methods like EIS a [Zennium](https://zahner.de/products#potentiostats) with [EPC](https://zahner.de/products-details/addon-cards/epc42) and the [thales_remote](https://github.com/Zahner-elektrik/Thales-Remote-Python) library is necessary.**
+
 **The following [primitives](https://en.wikipedia.org/wiki/Language_primitive) are available to compose methods with:**  
 
 * Potentiostatic or galvanostatic polarization  
   * [measurePolarization()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measurePolarization)  
 * Open circuit voltage/potential scan  
   * [measureOCV()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measureOCV)  
   * [measureOCVScan()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measureOCVScan)  
@@ -73,15 +76,15 @@
 ZahnerPP2x2.measurePolarization()
 ```
 
 # 📖 Examples
 
 The application of the library is shown in the example repository [Zahner-Remote-Python](https://github.com/Zahner-elektrik/Zahner-Remote-Python).
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send an <a href="mailto:support@zahner.de?subject=Zahner-Remote-Python Question&body=Your Message">e-mail</a> to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Remote-Python](https://github.com/Zahner-elektrik/Zahner-Remote-Python/issues) repository. If you already found a solution to your problem, **we would love to review your pull request**!
```

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/display/dcplot.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/display/dcplot.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/display/onlinedisplay.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/display/onlinedisplay.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/drivecycle/HUDDSCOL.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/HUDDSCOL.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/drivecycle/NYCCCOL.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/NYCCCOL.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/drivecycle/cycle_importer.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/drivecycle/cycle_importer.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/control.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/control.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/datahandler.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/datahandler.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/datareceiver.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/datareceiver.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/error.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/error.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/searcher.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/searcher.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat/scpi_control/serial_interface.py` & `zahner_potentiostat-1.1.1/zahner_potentiostat/scpi_control/serial_interface.py`

 * *Files identical despite different names*

### Comparing `zahner_potentiostat-1.1.0/zahner_potentiostat.egg-info/PKG-INFO` & `zahner_potentiostat-1.1.1/zahner_potentiostat.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,73 @@
 Metadata-Version: 2.1
-Name: zahner-potentiostat
-Version: 1.1.0
+Name: zahner_potentiostat
+Version: 1.1.1
 Summary: Library to control Zahner Potentiostats.
-Home-page: https://zahner.de/
-Author: Maximilian Krapp
-Author-email: maximilian.krapp@zahner.de
-License: MIT
-Project-URL: Documentation, https://doc.zahner.de/zahner_potentiostat/index.html
+Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
+License: MIT License
+        
+        Copyright (c) 2024 Zahner-Elektrik
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Documentation, https://doc.zahner.de/zahner_potentiostat
 Project-URL: Examples, https://github.com/Zahner-elektrik/Zahner-Remote-Python
 Project-URL: Source Code, https://github.com/Zahner-elektrik/zahner_potentiostat
 Project-URL: Bug Tracker, https://github.com/Zahner-elektrik/zahner_potentiostat/issues
-Keywords: potentiostat, electrochemistry, chemistry, eis, cyclic voltammetry, fuel-cell, battery
-Platform: any
+Project-URL: Homepage, https://zahner.de/
+Keywords: potentiostat,electrochemistry,chemistry,eis,cyclic voltammetry,fuel-cell,battery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: pyserial
+Requires-Dist: numpy
 
 # zahner_potentiostat
 
 zahner_potentiostat is a library to control external [Zahner Potentiostats](https://zahner.de/products#external-potentiostats) like **PP212, PP222, PP242, XPOT2 or EL1002**.
 
 It was developed to **easily integrate** external Zahner Potentiostats into Python scripts for more **complex measurement** tasks and for **automation purposes**.
 
 The control concept is that there are different primitives which can be combined for different electrochemical measurement methods.  
 These primitives can all be configured differently to match the application. In the documentation in the respective function all possible configuration setter methods are listed. The complete documentation of the functions can be found on the [API documentation website](https://doc.zahner.de/zahner_potentiostat/).  
 
+> [!NOTE]  
+> **Only with this library and a PP212, PP222, PP242, EL1002 or XPOT2 device you can not use AC methods. For AC methods like EIS a [Zennium](https://zahner.de/products#potentiostats) with [EPC](https://zahner.de/products-details/addon-cards/epc42) and the [thales_remote](https://github.com/Zahner-elektrik/Thales-Remote-Python) library is necessary.**
+
 **The following [primitives](https://en.wikipedia.org/wiki/Language_primitive) are available to compose methods with:**  
 
 * Potentiostatic or galvanostatic polarization  
   * [measurePolarization()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measurePolarization)  
 * Open circuit voltage/potential scan  
   * [measureOCV()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measureOCV)  
   * [measureOCVScan()](https://doc.zahner.de/zahner_potentiostat/scpi_control/control.html#zahner_potentiostat.scpi_control.control.SCPIDevice.measureOCVScan)  
@@ -103,15 +130,15 @@
 ZahnerPP2x2.measurePolarization()
 ```
 
 # 📖 Examples
 
 The application of the library is shown in the example repository [Zahner-Remote-Python](https://github.com/Zahner-elektrik/Zahner-Remote-Python).
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send an <a href="mailto:support@zahner.de?subject=Zahner-Remote-Python Question&body=Your Message">e-mail</a> to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with a respective title and description on the the [Zahner-Remote-Python](https://github.com/Zahner-elektrik/Zahner-Remote-Python/issues) repository. If you already found a solution to your problem, **we would love to review your pull request**!
```

