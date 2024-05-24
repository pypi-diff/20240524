# Comparing `tmp/propylean-0.2.5.tar.gz` & `tmp/propylean-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propylean-0.2.5.tar", last modified: Sat Mar 18 07:08:00 2023, max compression
+gzip compressed data, was "propylean-0.2.6.tar", last modified: Fri May 24 12:42:24 2024, max compression
```

## Comparing `propylean-0.2.5.tar` & `propylean-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 07:08:00.661945 propylean-0.2.5/
--rw-rw-rw-   0        0        0     1096 2023-03-18 07:00:39.000000 propylean-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     4159 2023-03-18 07:08:00.662946 propylean-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3391 2023-01-07 07:53:18.000000 propylean-0.2.5/README.md
--rw-rw-rw-   0        0        0      108 2023-01-07 07:53:20.000000 propylean-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0      911 2023-03-18 07:08:00.664982 propylean-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-18 07:08:00.513323 propylean-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-18 07:08:00.564800 propylean-0.2.5/src/propylean/
--rw-rw-rw-   0        0        0     1153 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/__init__.py
--rw-rw-rw-   0        0        0     4909 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-18 07:08:00.632352 propylean-0.2.5/src/propylean/equipments/
--rw-rw-rw-   0        0        0      317 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/equipments/__init__.py
--rw-rw-rw-   0        0        0    49113 2023-02-24 12:37:16.000000 propylean-0.2.5/src/propylean/equipments/abstract_equipment_classes.py
--rw-rw-rw-   0        0        0     7983 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/equipments/exchangers.py
--rw-rw-rw-   0        0        0    47279 2023-02-24 12:37:16.000000 propylean-0.2.5/src/propylean/equipments/generic_equipment_classes.py
--rw-rw-rw-   0        0        0    24767 2023-02-24 12:37:16.000000 propylean-0.2.5/src/propylean/equipments/rotary.py
--rw-rw-rw-   0        0        0     1961 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/equipments/separators.py
--rw-rw-rw-   0        0        0    20217 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/equipments/static.py
--rw-rw-rw-   0        0        0     3477 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/equipments/storages.py
-drwxrwxrwx   0        0        0        0 2023-03-18 07:08:00.657281 propylean-0.2.5/src/propylean/instruments/
--rw-rw-rw-   0        0        0      173 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/instruments/__init__.py
--rw-rw-rw-   0        0        0     5170 2023-03-18 07:00:39.000000 propylean-0.2.5/src/propylean/instruments/control.py
--rw-rw-rw-   0        0        0      633 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/instruments/measurement.py
--rw-rw-rw-   0        0        0      628 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/instruments/safety.py
--rw-rw-rw-   0        0        0    26590 2023-03-18 07:00:39.000000 propylean-0.2.5/src/propylean/properties.py
--rw-rw-rw-   0        0        0      173 2023-01-07 07:53:20.000000 propylean-0.2.5/src/propylean/settings.py
--rw-rw-rw-   0        0        0    30165 2023-03-18 07:00:39.000000 propylean-0.2.5/src/propylean/streams.py
--rw-rw-rw-   0        0        0     5696 2023-03-18 07:00:39.000000 propylean-0.2.5/src/propylean/validators.py
-drwxrwxrwx   0        0        0        0 2023-03-18 07:08:00.585240 propylean-0.2.5/src/propylean.egg-info/
--rw-rw-rw-   0        0        0     4159 2023-03-18 07:08:00.000000 propylean-0.2.5/src/propylean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2023-03-18 07:08:00.000000 propylean-0.2.5/src/propylean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 07:08:00.000000 propylean-0.2.5/src/propylean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-03-18 07:08:00.000000 propylean-0.2.5/src/propylean.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-18 07:08:00.000000 propylean-0.2.5/src/propylean.egg-info/top_level.txt
+drwxrwxr-x   0 abhishekr  (1000) abhishekr  (1000)        0 2024-05-24 12:42:24.066613 propylean-0.2.6/
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     1083 2024-05-24 12:40:02.000000 propylean-0.2.6/LICENSE
+-rw-r--r--   0 abhishekr  (1000) abhishekr  (1000)     4128 2024-05-24 12:42:24.066613 propylean-0.2.6/PKG-INFO
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     3313 2023-07-15 17:36:36.000000 propylean-0.2.6/README.md
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)      103 2023-07-15 17:36:37.000000 propylean-0.2.6/pyproject.toml
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)      874 2024-05-24 12:42:24.066613 propylean-0.2.6/setup.cfg
+drwxrwxr-x   0 abhishekr  (1000) abhishekr  (1000)        0 2024-05-24 12:42:24.038613 propylean-0.2.6/src/
+drwxrwxr-x   0 abhishekr  (1000) abhishekr  (1000)        0 2024-05-24 12:42:24.046613 propylean-0.2.6/src/propylean/
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     1128 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/__init__.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     4774 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/constants.py
+drwxrwxr-x   0 abhishekr  (1000) abhishekr  (1000)        0 2024-05-24 12:42:24.058613 propylean-0.2.6/src/propylean/equipments/
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)      312 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/equipments/__init__.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)    47393 2024-05-24 12:40:02.000000 propylean-0.2.6/src/propylean/equipments/abstract_equipment_classes.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     7797 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/equipments/exchangers.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)    46213 2023-08-06 14:02:47.000000 propylean-0.2.6/src/propylean/equipments/generic_equipment_classes.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)    24178 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/equipments/rotary.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     1900 2023-07-29 11:56:04.000000 propylean-0.2.6/src/propylean/equipments/separators.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)    19762 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/equipments/static.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     3377 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/equipments/storages.py
+drwxrwxr-x   0 abhishekr  (1000) abhishekr  (1000)        0 2024-05-24 12:42:24.062613 propylean-0.2.6/src/propylean/instruments/
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)      171 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/instruments/__init__.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     5067 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/instruments/control.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     9745 2024-05-24 12:40:02.000000 propylean-0.2.6/src/propylean/instruments/measurement.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)      610 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/instruments/safety.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)    23389 2024-05-24 12:40:02.000000 propylean-0.2.6/src/propylean/properties.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     2405 2024-05-24 12:40:02.000000 propylean-0.2.6/src/propylean/series.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)      169 2023-07-15 17:36:37.000000 propylean-0.2.6/src/propylean/settings.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)    29379 2024-05-24 12:40:02.000000 propylean-0.2.6/src/propylean/streams.py
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)     8021 2024-05-24 12:40:02.000000 propylean-0.2.6/src/propylean/validators.py
+drwxrwxr-x   0 abhishekr  (1000) abhishekr  (1000)        0 2024-05-24 12:42:24.062613 propylean-0.2.6/src/propylean.egg-info/
+-rw-r--r--   0 abhishekr  (1000) abhishekr  (1000)     4128 2024-05-24 12:42:24.000000 propylean-0.2.6/src/propylean.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)      893 2024-05-24 12:42:24.000000 propylean-0.2.6/src/propylean.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)        1 2024-05-24 12:42:24.000000 propylean-0.2.6/src/propylean.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)       21 2024-05-24 12:42:24.000000 propylean-0.2.6/src/propylean.egg-info/requires.txt
+-rw-rw-r--   0 abhishekr  (1000) abhishekr  (1000)       10 2024-05-24 12:42:24.000000 propylean-0.2.6/src/propylean.egg-info/top_level.txt
```

### Comparing `propylean-0.2.5/LICENSE` & `propylean-0.2.6/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2023, 2022, 2021 Abhishek Venkitta Raman
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c)2024, 2023, 2022, 2021 Abhishek Venkitta Raman
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `propylean-0.2.5/PKG-INFO` & `propylean-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,100 @@
-Metadata-Version: 2.1
-Name: propylean
-Version: 0.2.5
-Summary: The open-source calculations and analytics package for chemical process industries.
-Home-page: https://github.com/abhishekvraman/Propylean
-Author: Abhishek V Raman
-Author-email: 
-Project-URL: Bug Tracker, https://github.com/abhishekvraman/Propylean/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Manufacturing
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Windows](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml)
-[![macOS](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml)
-[![Ubuntu](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml)
-[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/abhishekvraman/Propylean/blob/main/LICENSE)
-[![PythonVersions](https://img.shields.io/pypi/pyversions/propylean.svg?style=flat)](https://pypi.python.org/pypi/propylean)
-# Propylean
-#### The open-source analytics and calculation package for chemical process industries.
-
-## What is Propylean
-Propylean name is derived from words Process/Production + Python + lean programming/manufacturing.
-Propylean is a Python library which will help engineers analyse production plants focusing on chemical and related process industries using only Python environments.
-Supports for general calculations like hydraulics, vessel sizing and other process engineering calculations is provided and constantly updated.
-By coupling this library with available data analysis/machine learning frameworks, engineers will be able to enhance operations of their plants. Ultimate aspiration of this project is to enable process industries transit to zero carbon operation.
-
-## Objective
-To increase the utilization of open-source software and analytics tools in the chemical and related industries.
-
-## Vision
-Vision of Propylean is to:
-- Enable chemical and related industries to use analytics and ML frameworks
-- Improve operational agility and efficiency of the plant
-- Be a cheap simulation-software alternative for small manufacturers
-- One-stop shop for all process engineering calculations
-- Help the industry transition to Net-Zero emissions
-- Inculcate coding/programing skills in manufacturing engineers
-
-## Installation and Requirements
-To download use below command or download the wheel file from PyPi page.
-
-Pip command:
-`pip install propylean`
-
-PyPi page:
-https://pypi.org/project/propylean/
-
-## Getting Started and Documentation
-To get started with Propylean, have a look at the getting started documenation.
-https://github.com/abhishekvraman/Propylean/wiki/Getting-started-with-Propylean
-
-## Supported objects that can be imported:
-
-* equipments.rotary
-    1. CentrifugalPump
-    2. PositiveDisplacementPump
-    3. CentrifugalCompressor
-    4. TurboExpander
-* equipments.static
-    1. PipeSegment
-* equipments.storage
-    1. VerticalStorage
-    2. Bullet
-    3. Tank
-    4. Sphere
-* equipments.exchangers
-    1. AirCooler
-    2. ElectricHeater
-* instruments
-    1. ControlValve
-    2. FlowMeter
-* streams
-    1. MaterialStream
-    2. EnergyStream
-* properties
-    1. Pressure
-    2. Temperature
-    3. MassFlowRate
-    4. Components (Molecular components)
-    5. Length
-    6. Time
-    7. Mass
-    8. MolecularWeigth
-    9. MolarFlowRate
-    10. VolumetricFlowRate
-    11. Volume
-    12. Density
-    13. DViscosity
-    14. Power
-    15. Frequency
+Metadata-Version: 2.1
+Name: propylean
+Version: 0.2.6
+Summary: The open-source calculations and analytics package for chemical process industries.
+Home-page: https://github.com/abhishekvraman/Propylean
+Author: Abhishek V Raman
+Author-email: 
+Project-URL: Bug Tracker, https://github.com/abhishekvraman/Propylean/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Manufacturing
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: fluids
+Requires-Dist: thermo
+
+[![Windows](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml)
+[![macOS](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml)
+[![Ubuntu](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml)
+[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/abhishekvraman/Propylean/blob/main/LICENSE)
+[![PythonVersions](https://img.shields.io/pypi/pyversions/propylean.svg?style=flat)](https://pypi.python.org/pypi/propylean)
+# Propylean
+#### The open-source analytics and calculation package for chemical process industries.
+
+## What is Propylean
+Propylean name is derived from words Process/Production + Python + lean programming/manufacturing.
+Propylean is a Python library which will help engineers analyse production plants focusing on chemical and related process industries using only Python environments.
+Supports for general calculations like hydraulics, vessel sizing and other process engineering calculations is provided and constantly updated.
+By coupling this library with available data analysis/machine learning frameworks, engineers will be able to enhance operations of their plants. Ultimate aspiration of this project is to enable process industries transit to zero carbon operation.
+
+## Objective
+To increase the utilization of open-source software and analytics tools in the chemical and related industries.
+
+## Vision
+Vision of Propylean is to:
+- Enable chemical and related industries to use analytics and ML frameworks
+- Improve operational agility and efficiency of the plant
+- Be a cheap simulation-software alternative for small manufacturers
+- One-stop shop for all process engineering calculations
+- Help the industry transition to Net-Zero emissions
+- Inculcate coding/programing skills in manufacturing engineers
+
+## Installation and Requirements
+To download use below command or download the wheel file from PyPi page.
+
+Pip command:
+`pip install propylean`
+
+PyPi page:
+https://pypi.org/project/propylean/
+
+## Getting Started and Documentation
+To get started with Propylean, have a look at the getting started documenation.
+https://github.com/abhishekvraman/Propylean/wiki/Getting-started-with-Propylean
+
+## Supported objects that can be imported:
+
+* equipments.rotary
+    1. CentrifugalPump
+    2. PositiveDisplacementPump
+    3. CentrifugalCompressor
+    4. TurboExpander
+* equipments.static
+    1. PipeSegment
+* equipments.storage
+    1. VerticalStorage
+    2. Bullet
+    3. Tank
+    4. Sphere
+* equipments.exchangers
+    1. AirCooler
+    2. ElectricHeater
+* instruments
+    1. ControlValve
+    2. FlowMeter
+* streams
+    1. MaterialStream
+    2. EnergyStream
+* properties
+    1. Pressure
+    2. Temperature
+    3. MassFlowRate
+    4. Components (Molecular components)
+    5. Length
+    6. Time
+    7. Mass
+    8. MolecularWeigth
+    9. MolarFlowRate
+    10. VolumetricFlowRate
+    11. Volume
+    12. Density
+    13. DViscosity
+    14. Power
+    15. Frequency
```

### Comparing `propylean-0.2.5/README.md` & `propylean-0.2.6/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-[![Windows](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml)
-[![macOS](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml)
-[![Ubuntu](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml)
-[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/abhishekvraman/Propylean/blob/main/LICENSE)
-[![PythonVersions](https://img.shields.io/pypi/pyversions/propylean.svg?style=flat)](https://pypi.python.org/pypi/propylean)
-# Propylean
-#### The open-source analytics and calculation package for chemical process industries.
-
-## What is Propylean
-Propylean name is derived from words Process/Production + Python + lean programming/manufacturing.
-Propylean is a Python library which will help engineers analyse production plants focusing on chemical and related process industries using only Python environments.
-Supports for general calculations like hydraulics, vessel sizing and other process engineering calculations is provided and constantly updated.
-By coupling this library with available data analysis/machine learning frameworks, engineers will be able to enhance operations of their plants. Ultimate aspiration of this project is to enable process industries transit to zero carbon operation.
-
-## Objective
-To increase the utilization of open-source software and analytics tools in the chemical and related industries.
-
-## Vision
-Vision of Propylean is to:
-- Enable chemical and related industries to use analytics and ML frameworks
-- Improve operational agility and efficiency of the plant
-- Be a cheap simulation-software alternative for small manufacturers
-- One-stop shop for all process engineering calculations
-- Help the industry transition to Net-Zero emissions
-- Inculcate coding/programing skills in manufacturing engineers
-
-## Installation and Requirements
-To download use below command or download the wheel file from PyPi page.
-
-Pip command:
-`pip install propylean`
-
-PyPi page:
-https://pypi.org/project/propylean/
-
-## Getting Started and Documentation
-To get started with Propylean, have a look at the getting started documenation.
-https://github.com/abhishekvraman/Propylean/wiki/Getting-started-with-Propylean
-
-## Supported objects that can be imported:
-
-* equipments.rotary
-    1. CentrifugalPump
-    2. PositiveDisplacementPump
-    3. CentrifugalCompressor
-    4. TurboExpander
-* equipments.static
-    1. PipeSegment
-* equipments.storage
-    1. VerticalStorage
-    2. Bullet
-    3. Tank
-    4. Sphere
-* equipments.exchangers
-    1. AirCooler
-    2. ElectricHeater
-* instruments
-    1. ControlValve
-    2. FlowMeter
-* streams
-    1. MaterialStream
-    2. EnergyStream
-* properties
-    1. Pressure
-    2. Temperature
-    3. MassFlowRate
-    4. Components (Molecular components)
-    5. Length
-    6. Time
-    7. Mass
-    8. MolecularWeigth
-    9. MolarFlowRate
-    10. VolumetricFlowRate
-    11. Volume
-    12. Density
-    13. DViscosity
-    14. Power
-    15. Frequency
+[![Windows](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml)
+[![macOS](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml)
+[![Ubuntu](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml)
+[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/abhishekvraman/Propylean/blob/main/LICENSE)
+[![PythonVersions](https://img.shields.io/pypi/pyversions/propylean.svg?style=flat)](https://pypi.python.org/pypi/propylean)
+# Propylean
+#### The open-source analytics and calculation package for chemical process industries.
+
+## What is Propylean
+Propylean name is derived from words Process/Production + Python + lean programming/manufacturing.
+Propylean is a Python library which will help engineers analyse production plants focusing on chemical and related process industries using only Python environments.
+Supports for general calculations like hydraulics, vessel sizing and other process engineering calculations is provided and constantly updated.
+By coupling this library with available data analysis/machine learning frameworks, engineers will be able to enhance operations of their plants. Ultimate aspiration of this project is to enable process industries transit to zero carbon operation.
+
+## Objective
+To increase the utilization of open-source software and analytics tools in the chemical and related industries.
+
+## Vision
+Vision of Propylean is to:
+- Enable chemical and related industries to use analytics and ML frameworks
+- Improve operational agility and efficiency of the plant
+- Be a cheap simulation-software alternative for small manufacturers
+- One-stop shop for all process engineering calculations
+- Help the industry transition to Net-Zero emissions
+- Inculcate coding/programing skills in manufacturing engineers
+
+## Installation and Requirements
+To download use below command or download the wheel file from PyPi page.
+
+Pip command:
+`pip install propylean`
+
+PyPi page:
+https://pypi.org/project/propylean/
+
+## Getting Started and Documentation
+To get started with Propylean, have a look at the getting started documenation.
+https://github.com/abhishekvraman/Propylean/wiki/Getting-started-with-Propylean
+
+## Supported objects that can be imported:
+
+* equipments.rotary
+    1. CentrifugalPump
+    2. PositiveDisplacementPump
+    3. CentrifugalCompressor
+    4. TurboExpander
+* equipments.static
+    1. PipeSegment
+* equipments.storage
+    1. VerticalStorage
+    2. Bullet
+    3. Tank
+    4. Sphere
+* equipments.exchangers
+    1. AirCooler
+    2. ElectricHeater
+* instruments
+    1. ControlValve
+    2. FlowMeter
+* streams
+    1. MaterialStream
+    2. EnergyStream
+* properties
+    1. Pressure
+    2. Temperature
+    3. MassFlowRate
+    4. Components (Molecular components)
+    5. Length
+    6. Time
+    7. Mass
+    8. MolecularWeigth
+    9. MolarFlowRate
+    10. VolumetricFlowRate
+    11. Volume
+    12. Density
+    13. DViscosity
+    14. Power
+    15. Frequency
```

### Comparing `propylean-0.2.5/src/propylean/__init__.py` & `propylean-0.2.6/src/propylean/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from propylean import equipments
-from propylean import properties 
-from propylean import streams
-from propylean import settings
-from propylean import constants
-from propylean import instruments
-
-# Import individual equipments. Copy paste from equipment.__init__.
-from propylean.equipments.exchangers import AirCooler, ElectricHeater
-from propylean.equipments.rotary import CentrifugalPump, PositiveDisplacementPump,\
-    CentrifugalCompressor
-from propylean.equipments.static import PipeSegment
-from propylean.equipments.storages import VerticalStorage, Bullet, Tank, Sphere
-
-# Import individual instruments. Copy paste from instruments.__init__.
-from propylean.instruments.control import ControlValve
-from propylean.instruments.measurement import FlowMeter
-from propylean.instruments.safety import PressureSafetyValve
-
-# Import streams.
-from propylean.streams import EnergyStream, MaterialStream
-
-# Import properties.
-from propylean.properties import Length, Time, Pressure, Temperature, MassFlowRate,\
-    Mass, MolecularWeigth, MolarFlowRate, VolumetricFlowRate, Volume, Density,\
+from propylean import equipments
+from propylean import properties 
+from propylean import streams
+from propylean import settings
+from propylean import constants
+from propylean import instruments
+
+# Import individual equipments. Copy paste from equipment.__init__.
+from propylean.equipments.exchangers import AirCooler, ElectricHeater
+from propylean.equipments.rotary import CentrifugalPump, PositiveDisplacementPump,\
+    CentrifugalCompressor
+from propylean.equipments.static import PipeSegment
+from propylean.equipments.storages import VerticalStorage, Bullet, Tank, Sphere
+
+# Import individual instruments. Copy paste from instruments.__init__.
+from propylean.instruments.control import ControlValve
+from propylean.instruments.measurement import FlowMeter
+from propylean.instruments.safety import PressureSafetyValve
+
+# Import streams.
+from propylean.streams import EnergyStream, MaterialStream
+
+# Import properties.
+from propylean.properties import Length, Time, Pressure, Temperature, MassFlowRate,\
+    Mass, MolecularWeigth, MolarFlowRate, VolumetricFlowRate, Volume, Density,\
     DViscosity, Power, Frequency, Components
```

### Comparing `propylean-0.2.5/src/propylean/constants.py` & `propylean-0.2.6/src/propylean/constants.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-class Constants(object):
-    g = 9.8 # m/s^2
-    R = 8.3144 # J/K/mol
-    ROUGHNESS = (4.57e-5, 4.5e-5, 0.000259, 1.5e-5, 1.5e-6) #in m
-    Le_BY_D = {"plastic": [17, 13, 72, 46, 3.3, 9, 400, 120, 530, 700],
-               "steel": [13, 10, 57, 37, 2.6, 7.5, 320, 95, 420, 560]}
-    REDUCER_Le_BY_D_PLASTIC = {9: 10, 8: 30, 7: 75, 6: 175, 5: 420, 4: 1150}
-    REDUCER_Le_BY_D_STEEL = {9: 3, 8: 8, 7: 18, 6: 38, 5: 85, 4: 220}
-    HEAD_TYPES = ["hemispherical", "elliptical", "torispherical", "flat"]
-
-class ConversionFactors(object):
-    """
-    Class to store all conversion factors for a specific property.
-    """
-    LENGTH = {
-            'foot': 1/3.28083,
-            'yard': 1/1.09361,
-            'mile': 1/0.000621371,
-            'cm': 1/100,
-            'inch': 1/39.3701,
-            'km':10^3,
-            'mm': 1/1000,
-            'm': 1
-            }
-    TIME = {
-            'year': (3600*24*30*12),
-            'month': (3600*24*30),
-            'week': (3600*24*7),
-            'day': (3600*24),
-            'hour':3600,
-            'min': 60,
-            'sec': 1
-            }
-    PRESSURE = {'atm': 101320,
-                'bar': 100000,
-                'psi': 6893,
-                'kPa': 1000,
-                'MPa': 1000000,
-                'kg/cm^2': 98070,
-                'ata': 98070,
-                'Torr': 133.3,
-                'mm Hg': 133.3,
-                'in water':2490,
-                'm water': 0.00981,
-                'Pa': 1
-                }
-    MASSFLOWRATE = {'g/s': 1000,
-                    'kg/min': 1/(1/60),
-                    'kg/d': 1*(24*60*60),
-                    'kg/h': 1*(60*60),
-                    'lb/s': 2.204,
-                    'lb/min': 2.204*60,
-                    'lb/h': 2.204*(60*60),
-                    'lb/d': 2.204*(60*60*24),
-                    'ton/h': 0.001*(60*60),
-                    'ton/d': 0.001*(60*60*24),
-                    'kg/s': 1
-                    }
-    MASS = {'g': 1000,
-            'lb': 2.204,
-            'ton': 0.001,
-            'kg': 1
-            }
-    MOLECULARWEIGTH = {
-                        'kg/mol': 0.001,
-                        'g/mol': 1
-                    }
-    MOLARFLOWRATE = {'lbmol/h': 7.93664,
-                                'mol/min': 1*60,
-                                'mol/d': 1*(24*60*60),
-                                'mol/h': 1*(60*60),
-                                'lbmol/s': 7.93664*3600,
-                                'lbmol/min': 7.93664*60,
-                                'lbmol/d': 7.93664*24,
-                                'kmol/h': 1/1000*(60*24),
-                                'kmol/d': 1000*(60*60*24),
-                                'mol/s': 1
-                                }
-    VOLUMETRICFLOWRATE = {'ft^3/s': 35.3146,
-                            'cm^3/s': 1000000,
-                            'm^3/min': 60,
-                            'm^3/h': 3600,
-                            'm^3/d': 3600*24,
-                            'ft^3/min': 35.3146*60,
-                            'ft^3/h': 35.3146*60*60,
-                            'ft^3/d': 35.3146*60*60*24,
-                            'gal/s': 264.172,
-                            'gal/min': 264.172*60,
-                            'gal/h': 264.172*60*60,
-                            'gal/d': 264.172*60*60*24,
-                            'lit/s': 1000,
-                            'lit/min': 60000,
-                            'lit/h': 3600000,
-                            'lit/d': 3600000*24,
-                            'm^3/s': 1
-                            }
-    VOLUME = {'ft^3': 35.3146,
-            'cm^3': 1000000,
-            'gal': 264.172,
-            'lit': 1000,
-            'm^3': 1
-            }
-    DENSITY = {'g/cm^3': 0.001,
-                'lbm/ft^3': 0.062479,
-                'kg/m^3': 1
-                }
-    DVISCOSITY = {'lb/(ft-s)': 1.4881,
-                    'cP': 1000,
-                    'Pa-s': 1
-                    }
-    POWER = {'BTU/h': 0.293071070172222,
-            'BTU/min': 17.5842642103333,
-            'BTU/s': 1055.05585262,
-            'cal/h': 0.001163,
-            'cal/s': 4.1868,
-            'erg/h': 2.777778E-11,
-            'erg/min': 1.666667E-9,
-            'erg/s': 1E-7,
-            'hp': 735.49875,
-            'MMBTU/h': 293071.070172222,
-            'MMBTU/min': 17584264.2103333,
-            'MMBTU/s': 1055055852.62,
-            'kW': 1000,
-            'MW': 1000000,
-            'GW': 1000000000,
-            'TW': 1000000000000,
-            'kWh/d': 41.667,
-            'MWh/d': 41666.67,
-            'GWh/d': 41666666.67,
-            'TWh/d': 41666666666.67,
-            'W': 1
-            }
-    FREQUENCY = {'/hour': 3600,
-                '/min': 60,
-                'Hz': 1
+class Constants(object):
+    g = 9.8 # m/s^2
+    R = 8.3144 # J/K/mol
+    ROUGHNESS = (4.57e-5, 4.5e-5, 0.000259, 1.5e-5, 1.5e-6) #in m
+    Le_BY_D = {"plastic": [17, 13, 72, 46, 3.3, 9, 400, 120, 530, 700],
+               "steel": [13, 10, 57, 37, 2.6, 7.5, 320, 95, 420, 560]}
+    REDUCER_Le_BY_D_PLASTIC = {9: 10, 8: 30, 7: 75, 6: 175, 5: 420, 4: 1150}
+    REDUCER_Le_BY_D_STEEL = {9: 3, 8: 8, 7: 18, 6: 38, 5: 85, 4: 220}
+    HEAD_TYPES = ["hemispherical", "elliptical", "torispherical", "flat"]
+
+class ConversionFactors(object):
+    """
+    Class to store all conversion factors for a specific property.
+    """
+    LENGTH = {
+            'foot': 1/3.28083,
+            'yard': 1/1.09361,
+            'mile': 1/0.000621371,
+            'cm': 1/100,
+            'inch': 1/39.3701,
+            'km':10^3,
+            'mm': 1/1000,
+            'm': 1
+            }
+    TIME = {
+            'year': (3600*24*30*12),
+            'month': (3600*24*30),
+            'week': (3600*24*7),
+            'day': (3600*24),
+            'hour':3600,
+            'min': 60,
+            'sec': 1
+            }
+    PRESSURE = {'atm': 101320,
+                'bar': 100000,
+                'psi': 6893,
+                'kPa': 1000,
+                'MPa': 1000000,
+                'kg/cm^2': 98070,
+                'ata': 98070,
+                'Torr': 133.3,
+                'mm Hg': 133.3,
+                'in water':2490,
+                'm water': 0.00981,
+                'Pa': 1
+                }
+    MASSFLOWRATE = {'g/s': 1000,
+                    'kg/min': 1/(1/60),
+                    'kg/d': 1*(24*60*60),
+                    'kg/h': 1*(60*60),
+                    'lb/s': 2.204,
+                    'lb/min': 2.204*60,
+                    'lb/h': 2.204*(60*60),
+                    'lb/d': 2.204*(60*60*24),
+                    'ton/h': 0.001*(60*60),
+                    'ton/d': 0.001*(60*60*24),
+                    'kg/s': 1
+                    }
+    MASS = {'g': 1000,
+            'lb': 2.204,
+            'ton': 0.001,
+            'kg': 1
+            }
+    MOLECULARWEIGTH = {
+                        'kg/mol': 0.001,
+                        'g/mol': 1
+                    }
+    MOLARFLOWRATE = {'lbmol/h': 7.93664,
+                                'mol/min': 1*60,
+                                'mol/d': 1*(24*60*60),
+                                'mol/h': 1*(60*60),
+                                'lbmol/s': 7.93664*3600,
+                                'lbmol/min': 7.93664*60,
+                                'lbmol/d': 7.93664*24,
+                                'kmol/h': 1/1000*(60*24),
+                                'kmol/d': 1000*(60*60*24),
+                                'mol/s': 1
+                                }
+    VOLUMETRICFLOWRATE = {'ft^3/s': 35.3146,
+                            'cm^3/s': 1000000,
+                            'm^3/min': 60,
+                            'm^3/h': 3600,
+                            'm^3/d': 3600*24,
+                            'ft^3/min': 35.3146*60,
+                            'ft^3/h': 35.3146*60*60,
+                            'ft^3/d': 35.3146*60*60*24,
+                            'gal/s': 264.172,
+                            'gal/min': 264.172*60,
+                            'gal/h': 264.172*60*60,
+                            'gal/d': 264.172*60*60*24,
+                            'lit/s': 1000,
+                            'lit/min': 60000,
+                            'lit/h': 3600000,
+                            'lit/d': 3600000*24,
+                            'm^3/s': 1
+                            }
+    VOLUME = {'ft^3': 35.3146,
+            'cm^3': 1000000,
+            'gal': 264.172,
+            'lit': 1000,
+            'm^3': 1
+            }
+    DENSITY = {'g/cm^3': 0.001,
+                'lbm/ft^3': 0.062479,
+                'kg/m^3': 1
+                }
+    DVISCOSITY = {'lb/(ft-s)': 1.4881,
+                    'cP': 1000,
+                    'Pa-s': 1
+                    }
+    POWER = {'BTU/h': 0.293071070172222,
+            'BTU/min': 17.5842642103333,
+            'BTU/s': 1055.05585262,
+            'cal/h': 0.001163,
+            'cal/s': 4.1868,
+            'erg/h': 2.777778E-11,
+            'erg/min': 1.666667E-9,
+            'erg/s': 1E-7,
+            'hp': 735.49875,
+            'MMBTU/h': 293071.070172222,
+            'MMBTU/min': 17584264.2103333,
+            'MMBTU/s': 1055055852.62,
+            'kW': 1000,
+            'MW': 1000000,
+            'GW': 1000000000,
+            'TW': 1000000000000,
+            'kWh/d': 41.667,
+            'MWh/d': 41666.67,
+            'GWh/d': 41666666.67,
+            'TWh/d': 41666666666.67,
+            'W': 1
+            }
+    FREQUENCY = {'/hour': 3600,
+                '/min': 60,
+                'Hz': 1
                 }
```

### Comparing `propylean-0.2.5/src/propylean/equipments/abstract_equipment_classes.py` & `propylean-0.2.6/src/propylean/equipments/abstract_equipment_classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,1058 +1,1044 @@
-import propylean.properties as prop
-from propylean import streams
-from propylean.validators import _Validators
-import warnings
-
-global _material_stream_equipment_map
-_material_stream_equipment_map = dict()
-global _energy_stream_equipment_map
-_energy_stream_equipment_map = dict()
-
-# Defining generic base class for all equipments with one inlet and outlet.
-class _EquipmentOneInletOutlet(object):
-    items = []
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Internal base class to define an equipment with one inlet and outlet.
-            All final classes inherits from this base class.
-            Read individual final classed for further description.
-    
-        PARAMETERS:
-            tag:
-                Required: No
-                Type: str
-                Acceptable values: Any string type
-                Default value: None
-                Description: Equipment tag the user wants to provide. If not provided, then tag is automatically generated
-            
-            dynamic_state:
-                Required: No
-                Type: bool
-                Acceptable values: True or False
-                Default value: False
-                Description: If equipment is in dynamic state and inventory is changing.
-                             TODO: Provide dynamic simulation capabilities.
-            
-            pressure_drop:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Any
-                Default value: None
-                Description: Represents pressure drop the equipment. Negative value implies pressure increase.
-            
-
-        RETURN VALUE:
-            Type: _EquipmentOneInletOutlet
-            Description: Object of type _EquipmentOneInletOutlet
-        
-        ERROR RAISED:
-            Type: Various
-            Description: 
-        
-        SAMPLE USE CASES:
-            >>> class NewEquipment(_EquipmentOneInletOutlet):
-                ......
-        """
-        if 'tag' not in inputs:
-            self.tag = self._create_equipment_tag()  
-        else:
-            self.tag = inputs['tag']
-        self.dynamic_state = False if 'dynamic_state' not in inputs else False
-
-        #Flow properties
-        self._inlet_mass_flowrate = prop.MassFlowRate() 
-        self._outlet_mass_flowrate = prop.MassFlowRate()
-        self.design_flowrate = prop.MassFlowRate()
-
-        #Pressure properties
-        self._pressure_drop = prop.Pressure(0)
-        self._inlet_pressure = prop.Pressure()
-        self._outlet_pressure = prop.Pressure()
-        self._design_pressure = prop.Pressure()
-        
-        #Temperature properties
-        self._temperature_increase = prop.Temperature(0, 'K')
-        self._inlet_temperature = prop.Temperature()
-        self._outlet_temperature = prop.Temperature()
-        self._design_temperature = prop.Temperature()
-
-        #Inlet and outlet material and energy streams
-        self._inlet_material_stream_tag = None
-        self._outlet_material_stream_tag = None
-        self._inlet_energy_stream_tag = None
-        self._outlet_energy_stream_tag = None
-        self._inlet_material_stream_index = None
-        self._outlet_material_stream_index = None
-        self._inlet_energy_stream_index = None
-        self._outlet_energy_stream_index = None
-        
-        #Energy properties
-        self._energy_in = prop.Power()
-        self._energy_out = prop.Power()
-
-        #Other Porperties
-        self.main_fluid = "liquid" if "main_fluid" not in inputs else inputs["main_fluid"]
-        self._is_disconnection = False
-
-        if 'pressure_drop' in inputs:
-            self.pressure_drop = inputs['pressure_drop']
-    
-    @property
-    def index(self):
-      return self._index
-
-    @property
-    def tag(self):
-        return self._tag
-    @tag.setter
-    def tag(self, value):
-        _Validators.validate_arg_prop_value_type("tag", value, (str))
-        if self._check_tag_assigned(value):
-            msg = "Tag '{}' already assigned!".format(value)
-            raise Exception(msg)
-        else:
-            self._tag = value
-
-    @property
-    def inlet_pressure(self):
-        self = self._get_equipment_object(self)
-        return self._inlet_pressure
-    @inlet_pressure.setter
-    def inlet_pressure(self, value):
-        _Validators.validate_arg_prop_value_type("inlet_pressure", value, (prop.Pressure, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
-        if unit is None:
-            unit = self._inlet_pressure.unit
-        self._inlet_pressure = prop.Pressure(value, unit)
-        self._outlet_pressure = self._inlet_pressure - self.pressure_drop
-        self._update_equipment_object(self)
-    
-    @property
-    def outlet_pressure(self):
-        self = self._get_equipment_object(self)
-        return self._outlet_pressure
-    @outlet_pressure.setter
-    def outlet_pressure(self, value):
-        _Validators.validate_arg_prop_value_type("outlet_pressure", value, (prop.Pressure, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
-        if unit is None:
-            unit = self._outlet_pressure.unit
-        self._outlet_pressure = prop.Pressure(value, unit)
-        self._inlet_pressure = self._outlet_pressure + self.pressure_drop
-        self._update_equipment_object(self)
-    
-    @property
-    def pressure_drop(self):
-        self = self._get_equipment_object(self)
-        return self._pressure_drop
-    @pressure_drop.setter
-    def pressure_drop(self, value):
-        _Validators.validate_arg_prop_value_type("pressure_drop", value, (prop.Pressure, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
-        if unit is None:
-            unit = self._pressure_drop.unit
-        self._pressure_drop = prop.Pressure(value, unit)
-        self._outlet_pressure =  self._inlet_pressure - self._pressure_drop
-        self._update_equipment_object(self)
-    
-    @property
-    def design_pressure(self):
-        self = self._get_equipment_object(self)
-        return self._design_pressure
-    @design_pressure.setter
-    def design_pressure(self, value):
-        _Validators.validate_arg_prop_value_type("design_pressure", value, (prop.Pressure, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
-        if unit is None:
-            unit = self._design_pressure.unit
-        self._design_pressure = prop.Pressure(value, unit)
-        self._update_equipment_object(self)
-
-    @property
-    def inlet_temperature(self):
-        self = self._get_equipment_object(self)
-        return self._inlet_temperature
-    @inlet_temperature.setter
-    def inlet_temperature(self, value):
-        _Validators.validate_arg_prop_value_type("inlet_temperature", value, (prop.Temperature, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
-        if unit is None:
-            unit = self._inlet_temperature.unit
-        self._inlet_temperature = prop.Temperature(value, unit)
-        self._outlet_temperature = self._inlet_temperature + self.temperature_increase
-        self._update_equipment_object(self)
-
-    @property
-    def outlet_temperature(self):
-        self = self._get_equipment_object(self)
-        return self._outlet_temperature
-    @outlet_temperature.setter
-    def outlet_temperature(self,value):
-        _Validators.validate_arg_prop_value_type("outlet_temperature", value, (prop.Temperature, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
-        if unit is None:
-            unit = self._outlet_temperature.unit
-        self._outlet_temperature = prop.Temperature(value, unit)
-        self._inlet_temperature = self._outlet_temperature - self.temperature_increase
-        self._update_equipment_object(self)
-
-    @property
-    def temperature_increase(self):
-        self = self._get_equipment_object(self)
-        return self._temperature_increase
-    @temperature_increase.setter
-    def temperature_increase(self, value):
-        _Validators.validate_arg_prop_value_type("temperature_increase", value, (prop.Temperature, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
-        if unit is None:
-            unit = self._temperature_increase.unit
-        self._temperature_increase = prop.Temperature(value, unit)
-        self._outlet_temperature =  self._inlet_temperature + self._temperature_increase
-        self._update_equipment_object(self)
-    @property
-    def temperature_decrease(self):
-        self = self._get_equipment_object(self)
-        decrease = -1 * self._temperature_increase.value
-        return prop.Temperature(decrease, self._temperature_increase.unit)
-    @temperature_decrease.setter
-    def temperature_decrease(self, value):
-        _Validators.validate_arg_prop_value_type("temperature_decrease", value, (prop.Temperature, int, float, tuple))
-        if isinstance(value, prop.Temperature):
-            value = prop.Temperature(-1 * value.value, value.unit)
-        elif isinstance(value, tuple):
-            value = prop.Temperature(-1 * value[0], value[1])
-        elif isinstance(value, (int, float)):
-            value = prop.Temperature(-1 * value, self._temperature_increase.unit)
-        self.temperature_increase = value
-    
-    @property
-    def design_temperature(self):
-        self = self._get_equipment_object(self)
-        return self._design_pressure
-    @design_temperature.setter
-    def design_temperature(self, value):
-        _Validators.validate_arg_prop_value_type("design_temperature", value, (prop.Temperature, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
-        if unit is None:
-            unit = self._design_temperature.unit
-        self._design_temperature = prop.Temperature(value, unit)
-        self._update_equipment_object(self)
-
-    @property
-    def inlet_mass_flowrate(self):
-        self = self._get_equipment_object(self)
-        return self._inlet_mass_flowrate
-    @inlet_mass_flowrate.setter
-    def inlet_mass_flowrate(self, value):
-        _Validators.validate_arg_prop_value_type("inlet_mass_flowrate", value, (prop.MassFlowRate, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.MassFlowRate)
-        if unit is None:
-            unit = self._inlet_mass_flowrate.unit
-        self._inlet_mass_flowrate = prop.MassFlowRate(value, unit)
-        self._outlet_mass_flowrate = self._inlet_mass_flowrate + self.inventory_change_rate
-        self._update_equipment_object(self)
-    
-    @property
-    def outlet_mass_flowrate(self):
-        self = self._get_equipment_object(self)
-        return self._outlet_mass_flowrate
-    @outlet_mass_flowrate.setter
-    def outlet_mass_flowrate(self, value):
-        _Validators.validate_arg_prop_value_type("outlet_mass_flowrate", value, (prop.MassFlowRate, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.MassFlowRate)
-        if unit is None:
-            unit = self._outlet_mass_flowrate.unit
-        self._outlet_mass_flowrate = prop.MassFlowRate(value, unit)
-        self._inlet_mass_flowrate = self._outlet_mass_flowrate - self.inventory_change_rate
-        self._update_equipment_object(self)
-    
-    @property
-    def inventory_change_rate(self):
-        self = self._get_equipment_object(self)
-        if not self.dynamic_state:
-            return prop.MassFlowRate(0, self.inlet_mass_flowrate.unit)            
-        return self._inlet_mass_flowrate - self._outlet_mass_flowrate                             
-    @inventory_change_rate.setter
-    def inventory_change_rate(self, value):
-        raise Exception("Dynamic process is not yet supported.")
-        _Validators.validate_arg_prop_value_type("inventory_change_rate", value, (int))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.MassFlowRate)
-        if unit is None:
-            unit = self.inventory_change_rate.unit
-        self._update_equipment_object(self)
-    
-    @property
-    def energy_in(self):
-        self = self._get_equipment_object(self)
-        return self._energy_in
-    @energy_in.setter
-    def energy_in(self, value):
-        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self.energy_in.unit
-        self._energy_in = prop.Power(value, unit)
-        self._update_equipment_object(self)
-    @energy_in.deleter
-    def energy_in(self):
-        self = self._get_equipment_object(self)
-        del self._energy_in
-        self._update_equipment_object(self)
-
-    @property
-    def energy_out(self):
-        self = self._get_equipment_object(self)
-        return self._energy_out
-    @energy_out.setter
-    def energy_out(self, value):
-        _Validators.validate_arg_prop_value_type("energy_out", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self.energy_out.unit
-        self._energy_in = prop.Power(value, unit)
-        self._update_equipment_object(self)
-    @energy_out.deleter
-    def energy_out(self):
-        self = self._get_equipment_object(self)
-        del self._energy_out
-        self._update_equipment_object(self) 
-    
-    def _get_equipment_index(cls, tag):
-        for index, equipment in enumerate(cls.items):
-            if equipment.tag == tag:
-                return index
-        return None
-    
-    @classmethod
-    def _get_equipment_object(cls, obj):
-        try:
-            return cls.items[obj.index]
-        except IndexError:
-            raise Exception("Equipment does not exist!")
-        except AttributeError:
-            return obj
-    
-    @classmethod
-    def _update_equipment_object(cls, obj):
-        _Validators.validate_arg_prop_value_type("obj", obj, cls)
-        try:
-            cls.items[obj.index] = obj
-        except:
-            pass
-    
-    def __eq__(self, other):
-        if isinstance(other, type(self)):
-            return self.tag == other.tag
-        else:
-            return False
-
-    def get_stream_tag(self, stream_type, direction):
-        """ 
-        DESCRIPTION:
-            Method to tsg ogf stream connected to the equipment using steam 
-            type and the direction.
-        
-        PARAMETERS:
-            stream_type:
-                Required: Yes
-                Type: str
-                Acceptable values: 'm', 'mass', 'e', 'energy'
-                Description: Type of stream user wants to get tag of.
-            direction:
-                Required: Yes
-                Type: str
-                Acceptable values: 'in', 'out', 'inlet' or 'outlet'
-                Description: Direction of stream with respect to equipment user wants to get tag of.
-       
-        RETURN VALUE:
-            Type: str
-            Description: Tag value of stream user has assigned to the stream
-        
-        ERROR RAISED:
-            Type: General TODO
-            Description: Raises error if arguments are incorrect
-        
-        SAMPLE USE CASES:
-            >>> eq1.get_stream_tag('m', 'out')
-            >>> eq1.get_stream_tag('energy', 'in')
-        """
-        _Validators.validate_arg_prop_value_type("stream_type", stream_type, (str))
-        _Validators.validate_arg_prop_value_list("stream_type", stream_type, ['m', 'mass', 'e', 'energy', 'material'])
-        _Validators.validate_arg_prop_value_type("direction", direction, (str))
-        _Validators.validate_arg_prop_value_list("direction", direction, ['in', 'out', 'inlet', 'outlet'])
-
-        if stream_type.lower() in ['material', 'mass', 'm']:
-            stream_tag = [self._inlet_material_stream_tag, self._outlet_material_stream_tag]
-        elif stream_type.lower() in ['energy', 'power', 'e', 'p']:
-            stream_tag = [self._inlet_energy_stream_tag, self._outlet_energy_stream_tag]
-        else:
-            raise Exception('Incorrect stream_type specified! Provided \"'+stream_type+'\". Can only be "material/mass/m" or "energy/e/power/p"]')
-        
-        if direction.lower() in ['in', 'inlet']:
-                return stream_tag[0]
-        elif direction.lower() in ['out', 'outlet']:
-            return stream_tag[1]
-        else:
-            raise Exception('Incorrect direction specified! Provided \"'+direction+'\". Can only be ["in", "out", "inlet", "outlet"]')
-
-    def connect_stream(self,
-                       stream_object=None,
-                       direction=None, 
-                       stream_tag=None,
-                       stream_type=None,
-                       stream_governed=True):
-        """ 
-        DESCRIPTION:
-            Method to connect a stream object with equiment.
-        
-        PARAMETERS:
-            stream_object:
-                Required: No if stream_tag is provided else Yes
-                Type: EnergyStream or MaterialStream
-                Acceptable values: object of specified stream types
-                Default value: None
-                Description: Stream object user wants to connect the equipment with.
-            
-            direction:
-                Required: Yes for material stream. For energy stream not needed
-                Type: str
-                Acceptable values: 'in', 'out', 'inlet' or 'outlet'
-                Default value: None
-                Description: Direction in which stream should be with respect to equipment.
-            
-            stream_tag:
-                Required: No if stream_object is provided else Yes
-                Type: str
-                Acceptable values: stream tag provided by user
-                Default value: None
-                Description: Stream object with known stream_tag user wants to connect the equipment with.
-
-            stream_type:
-                Required: No if stream_object provided
-                Type: str
-                Acceptable values: 'm', 'mass', 'e', 'energy'
-                Description: Type of stream user wants to connect.
-
-            stream_governed:
-                Required: No 
-                Type: bool
-                Default values: True
-                Description: Determines if stream will govern the property. Fluid property will be passed.    
-
-        RETURN VALUE:
-            Type: bool
-            Description: True is returned if connection is successful else False
-        
-        ERROR RAISED:
-            Type: General
-            Description: Error raised if arguments are wrong
-        
-        SAMPLE USE CASES:
-            >>> eq1.connect_stream(en1)
-            >>> eq1.connect_stream(direction='out', stream_tag='Pump-outlet', stream_type='m')
-        """
-        if stream_object is not None:
-            _Validators.validate_arg_prop_value_type("stream_object", stream_object, (streams.MaterialStream, streams.EnergyStream))
-            _Validators.validate_arg_prop_value_type("direction", direction, str)
-            _Validators.validate_arg_prop_value_type("stream_governed", stream_governed, bool)
-            _Validators.validate_arg_prop_value_list("direction", direction, ['in', 'out', 'inlet', 'outlet'])
-            if not (isinstance(stream_object, streams.EnergyStream) or
-                    isinstance(stream_object, streams.MaterialStream)):
-                    raise Exception("Stream object should be of type EnergyStream or Material Stream not " +
-                                    type(stream_object))
-            stream_tag = stream_object.tag
-            if isinstance(stream_object, streams.MaterialStream):
-                stream_type = 'm'
-            elif isinstance(stream_object, streams.EnergyStream):
-                stream_type = 'e'
-        elif not self._is_disconnection and stream_tag is None:
-            raise Exception("Either of Stream Object or Stream Tag is required for connection!")
-        else:
-            _Validators.validate_arg_prop_value_type("stream_tag", stream_tag, str)
-            _Validators.validate_arg_prop_value_type("direction", direction, str)
-            _Validators.validate_arg_prop_value_list("direction", direction, ['in', 'out', 'inlet', 'outlet'])
-            _Validators.validate_arg_prop_value_type("stream_type", stream_type, str)
-            _Validators.validate_arg_prop_value_list("stream_type", stream_type, ['m', 'mass', 'e', 'energy', 'material'])
-            _Validators.validate_arg_prop_value_type("stream_governed", stream_governed, bool)
-        
-        stream_index = streams.get_stream_index(stream_tag, stream_type)
-        is_inlet = True if direction.lower() in ['in', 'inlet'] else False
-
-        mapping_result = self._stream_equipment_mapper(stream_index, stream_type, is_inlet)
-        if self._is_disconnection:
-            stream_tag = stream_index = None
-            
-        if stream_type.lower() in ['material', 'mass', 'm']:
-            if direction.lower() in ['in', 'inlet']:
-                self._inlet_material_stream_tag = stream_tag
-                self._inlet_material_stream_index = stream_index
-            else:
-                self._outlet_material_stream_tag = stream_tag
-                self._outlet_material_stream_index = stream_index
-        else:
-            if direction.lower() in ['in', 'inlet']:
-                self._inlet_energy_stream_tag = stream_tag
-                self._inlet_energy_stream_index = stream_index
-            else:
-                self._outlet_energy_stream_tag = stream_tag
-                self._outlet_energy_stream_index = stream_index
-        
-        if mapping_result and not self._is_disconnection:
-            self._stream_equipment_properties_matcher(stream_index, 
-                                                      stream_type,
-                                                      is_inlet,
-                                                      stream_governed)
-        return mapping_result
-
-    def disconnect_stream(self, 
-                          stream_object=None,
-                          direction=None, 
-                          stream_tag=None,
-                          stream_type=None):
-        """ 
-        DESCRIPTION:
-            Class method to disconnect a stream object from equiment.
-        
-        PARAMETERS:
-            stream_object:
-                Required: No if stream_tag is provided else Yes
-                Type: EnergyStream or MaterialStream
-                Acceptable values: object of specified stream types
-                Default value: None
-                Description: Stream object user wants to disconnect the equipment with.
-            
-            direction:
-                Required: Yes if stream_object or stream_tag not provided
-                Type: str
-                Acceptable values: 'in', 'out', 'inlet' or 'outlet'
-                Default value: None
-                Description: Direction in which stream should be with respect to equipment.
-            
-            stream_tag:
-                Required: No if stream_object is provided else Yes
-                Type: str
-                Acceptable values: stream tag provided by user
-                Default value: None
-                Description: Stream object with known stream_tag user wants to disconnect the equipment from.
-
-            stream_type:
-                Required: No if stream_object provided
-                Type: str
-                Acceptable values: 'm', 'mass', 'e', 'energy'
-                Description: Type of stream user wants to disconnect.
-
-        RETURN VALUE:
-            Type: bool
-            Description: True is returned if disconnection is successful else False
-        
-        ERROR RAISED:
-            Type: General
-            Description: Error raised if arguments are wrong
-        
-        SAMPLE USE CASES:
-            >>> eq1.disconnect_stream(s1)
-            >>> eq1.disconnect_stream(stream_tag='Pump-outlet')
-            >>> eq1.disconnect_stream(direction='in', stream_type="energy")
-        """
-               
-        def define_index_direction(tag):
-            " This function is internal function. Not to be used elsewhere."
-            stream_type = None
-            direction = None
-            if tag == self._inlet_material_stream_tag:
-                stream_type = "m"
-                direction = "in"
-            elif tag == self._outlet_material_stream_tag:
-                stream_type = "m"
-                direction = "out"
-            elif tag == self._inlet_energy_stream_tag:
-                stream_type = "e"
-                direction = "in"
-            elif tag == self._outlet_energy_stream_tag:
-                stream_type = "e"
-                direction = "out"
-            return stream_type, direction
-
-        if stream_object is not None:
-            _Validators.validate_arg_prop_value_type("stream_object", stream_object, (streams.MaterialStream, streams.EnergyStream))
-            stream_type, direction = define_index_direction(stream_object.tag)
-        elif stream_tag is not None:
-            _Validators.validate_arg_prop_value_type("stream_tag", stream_tag, (str))
-            stream_type, direction = define_index_direction(stream_tag)
-        elif (direction is not None and 
-              stream_type is not None):
-              _Validators.validate_arg_prop_value_type("direction", direction, (str))
-              _Validators.validate_arg_prop_value_type("stream_type", stream_type, (str))
-              _Validators.validate_arg_prop_value_list("direction", direction, ['in', 'out', 'inlet', 'outlet'])
-              _Validators.validate_arg_prop_value_list("stream_type", stream_type, ['m', 'mass', 'e', 'energy', 'material'])
-              stream_tag = self.get_stream_tag(stream_type, direction)
-              stream_type, direction = define_index_direction(stream_tag)
-        else:
-            raise Exception("To disconnect stream from equipment, provide either just connected stream object or\
-                             just stream tag or just direction & stream type") 
-
-        # Validate if connection is there.
-        if stream_type is None and direction is None:
-            warnings.warn("Already there is no connection.")
-            return
-
-        if stream_type.lower() in ['material', 'mass', 'm']:
-            if direction.lower() in ['in', 'inlet']:
-                if (self._inlet_material_stream_tag is None or 
-                   self._inlet_material_stream_index is None):
-                   warnings.warn("Material Inlet already has no connection.")
-                   return 
-            else:
-                if (self._outlet_material_stream_tag is None or 
-                   self._outlet_material_stream_index is None):
-                   warnings.warn("Material Outlet already has no connection.")
-                   return 
-                  
-        else:
-            if direction.lower() in ['in', 'inlet']:
-                if (self._inlet_energy_stream_tag is None or 
-                   self._inlet_energy_stream_index is None):
-                   warnings.warn("Energy Inlet already has no connection.")
-                   return 
-            else:
-                if (self._outlet_energy_stream_tag is None or 
-                   self._outlet_energy_stream_index is None):
-                   warnings.warn("Energy Outlet already has no connection.")
-                   return       
-
-        self._is_disconnection = True
-        return self.connect_stream(stream_object,
-                                   direction, 
-                                   stream_tag,
-                                   stream_type)
-      
-    def _stream_equipment_mapper(self, stream_index, stream_type, is_inlet):
-        """ 
-            DESCRIPTION:
-                Internal function to map stream with equipment object.
-                _material_stream_equipment_map and _energy_stream_equipment_map 
-                are dictionary of list which store index of coming from and going 
-                to equipment and type of equipment. Structured like 
-                {12: [10, CentrifugalPump, 21, PipeSegment], 
-                 23: [21, PipeSegment, 36, FlowMeter]]} 
-                where 12th index stream will have data in key no. 12. 
-                Stream is coming from equipment with index 10 and is of type CentrifugalPump.  
-                Stream is going into equipment with index 21 of type PipeSegment.
-            
-            PARAMETERS:
-                stream_index:
-                    Required: Yes
-                    Type: int
-                    Acceptable values: Non-negative integer
-                    Default value: Not Applicable
-                    Description: Index of the stream in the stream list it belongs to.
-                
-                stream_type:
-                    Required: Yes
-                    Type: string
-                    Acceptable values: 'material' or 'energy'
-                    Default value: Not Applicable
-                    Description: Index of the stream in the stream list it belongs to.
-                
-                is_inlet:
-                    Required: Yes
-                    Type: bool
-                    Acceptable values: True or False
-                    Default value: Not Applicable
-                    Description: True or False if stream is inlet to equipment.
-            
-            RETURN VALUE:
-                Type: bool
-                Description: If mapping was successful True is returned else False
-            
-            ERROR RAISED:
-                Type:
-                Description: 
-            
-            SAMPLE USE CASES:
-                >>>  _stream_equipment_mapper(10, 'm', False)
-                >>> stream_index = get_stream_index("Compressor1_power", "energy")
-                >>>  _stream_equipment_mapper(stream_index, 'e', True)
-                
-        """
-
-        if stream_index is None or isinstance(stream_index, list):
-            return False
-        e_type, e_index = (3, 2) if is_inlet else (1, 0)
-        global _material_stream_equipment_map
-        global _energy_stream_equipment_map
-        if stream_type in ['m', 'material']:
-            stream_equipment_map = _material_stream_equipment_map
-        elif stream_type in ['e', 'energy']:
-            stream_equipment_map =_energy_stream_equipment_map
-        else:
-            raise Exception('Incorrect stream type {}'.format(stream_type)+\
-                            " Can only be 'm' or 'e' ")
-        equipment_type = type(self)
-        equipment_index = self._get_equipment_index(self.tag)
-        def set_type_index():
-            old_equipment_type = stream_equipment_map[stream_index][e_type]
-            old_equipment_index = stream_equipment_map[stream_index][e_index]
-            stream_equipment_map[stream_index][e_type] = equipment_type if not self._is_disconnection else None
-            stream_equipment_map[stream_index][e_index] = equipment_index if not self._is_disconnection else None
-            if (not self._is_disconnection and
-                old_equipment_index is not None
-                and old_equipment_type is not None):
-                old_equipment_obj = old_equipment_type.list_objects()[old_equipment_index]
-                old_equipment_obj.disconnect_stream(stream_type=stream_type, direction='in' if is_inlet else 'out')
-                warnings.warn("Equipment type " + str(old_equipment_type) +
-                              " with tag " + old_equipment_obj.tag + 
-                              " was disconnected from stream type " + str(stream_type) +
-                              " with tag " + str(self.get_stream_tag(stream_type,
-                                                                'in' if is_inlet else 'out')))
-        try:
-            set_type_index()   
-        except:
-            try:
-                stream_equipment_map[stream_index] = [None, None, None, None]
-                set_type_index()
-            except Exception as e:
-                raise Exception("Error occured in equipment-stream mapping:", e)
-
-        if stream_type in ['material', 'm']:
-            _material_stream_equipment_map = stream_equipment_map
-        elif stream_type in ['energy', 'e']:
-            _energy_stream_equipment_map = stream_equipment_map
-        return True
-
-    def _stream_equipment_properties_matcher(self, stream_index, 
-                                             stream_type, 
-                                             is_inlet, 
-                                             stream_governed=True):
-        """ 
-            DESCRIPTION:
-                Internal function to match properties of stream with that of equipment object's.
-            
-            PARAMETERS:
-                stream_index:
-                    Required: Yes
-                    Type: int
-                    Acceptable values: Non-negative integer
-                    Default value: Not Applicable
-                    Description: Index of the stream in the stream list it belongs to.
-                
-                stream_type:
-                    Required: Yes
-                    Type: string
-                    Acceptable values: 'material' or 'energy'
-                    Default value: Not Applicable
-                    Description: Index of the stream in the stream list it belongs to.
-                
-                is_inlet:
-                    Required: Yes
-                    Type: bool
-                    Acceptable values: True or False
-                    Default value: Not Applicable
-                    Description: True or False if stream is inlet to equipment or not.
-                
-                stream_governed:
-                    Required: False
-                    Type: bool
-                    Acceptable values: True or False
-                    Default value: Not Applicable
-                    Description: Determines if stream to govern the property or equipment.
-                                 If True, stream property are assigned to equipment.
-                                 If False, equipment property are assigned to stream.
-            
-            RETURN VALUE:
-                Type: bool
-                Description: If matching was successful, True is returned else False.
-            
-            ERROR RAISED:
-                Type:
-                Description: 
-            
-            SAMPLE USE CASES:
-                >>>  _stream_equipment_properties_matcher(10, 'm', False)
-                >>> stream_index = get_stream_index("Compressor1_power", "energy")
-                >>>  _stream_equipment_properties_matcher(stream_index, 'e', True)
-                
-        """
-        def property_matcher(stream_property, equipment_property, stream_governed):
-            if stream_governed:
-                return stream_property, stream_property
-            return equipment_property, equipment_property
-
-        if stream_type.lower() in ['m', 'material', 'mass']:
-            stream_object = streams.MaterialStream.list_objects()[stream_index]
-            if is_inlet:
-                stream_object.mass_flowrate, \
-                self.inlet_mass_flowrate = property_matcher(stream_object.mass_flowrate,
-                                                            self._inlet_mass_flowrate,
-                                                            stream_governed)
-                stream_object.pressure, \
-                self.inlet_pressure = property_matcher(stream_object.pressure,
-                                                       self._inlet_pressure,
-                                                       stream_governed)
-                stream_object.temperature, \
-                self.inlet_temperature = property_matcher(stream_object.temperature,
-                                                          self._inlet_temperature,
-                                                          stream_governed)
-            else:
-                stream_object.mass_flowrate, \
-                self.outlet_mass_flowrate = property_matcher(stream_object.mass_flowrate,
-                                                             self._outlet_mass_flowrate,
-                                                             stream_governed)
-                stream_object.pressure, \
-                self.outlet_pressure = property_matcher(stream_object.pressure,
-                                                        self._outlet_pressure,
-                                                        stream_governed)
-                stream_object.temperature, \
-                self.outlet_temperature = property_matcher(stream_object.temperature,
-                                                           self._outlet_temperature,
-                                                           stream_governed)
-            if not stream_governed:
-                streams.MaterialStream._update_stream_object(stream_object)
-            else:
-                self._update_equipment_object(self)
-        else:
-            stream_object = streams.EnergyStream.list_objects()[stream_index]
-            if is_inlet:
-                stream_object.amount, \
-                self.energy_in = property_matcher(stream_object.amount,
-                                                  self.energy_in,
-                                                  stream_governed)     
-            else:
-                stream_object.amount, \
-                self.energy_out = property_matcher(stream_object.amount,
-                                                    self.energy_out,
-                                                    stream_governed)
-            if not stream_governed:
-                streams.EnergyStream._update_stream_object(stream_object)
-        self._physical_chemical_reaction()
-
-    def _connected_stream_property_getter(self, is_inlet, stream_type, property=None):
-        """ 
-            DESCRIPTION:
-                Internal function to get object of stream.
-            
-            PARAMETERS:
-                is_inlet:
-                    Required: Yes
-                    Type: bool
-                    Default value: Not Applicable
-                    Description: True if stream is inlet to equipment. False if stream is outlet.
-                
-                stream_type:
-                    Required: Yes
-                    Type: string
-                    Acceptable values: 'material' or 'energy'
-                    Default value: Not Applicable
-                    Description: Index of the stream in the stream list it belongs to.
-                
-                property:
-                    Required: Yes if stream_type is material
-                    Type: String
-                    Description: Type of property. See the if else ladder.
-
-            
-            RETURN VALUE:
-                Type: Any supported property
-            
-            ERROR RAISED:
-                Type:
-                Description: 
-            
-            SAMPLE USE CASES:
-                >>> Psat = self._connected_stream_property_getter(True, "material", "Psat")
-                
-        """
-        
-        if stream_type.lower() in ['m', 'material', 'mass']:
-            stream_index = self._inlet_material_stream_index if is_inlet else self._outlet_material_stream_index
-            if stream_index is None:
-                raise Exception("Equipment not connected to MaterialStream!")
-            stream_object = streams.MaterialStream.list_objects()[stream_index]  
-        else:
-            stream_index = self._inlet_energy_stream_index if is_inlet else self._outlet_energy_stream_index
-            if stream_index is None:
-                raise Exception("Equipment not connected to EnergyStream!")
-            stream_object = streams.EnergyStream.list_objects()[stream_index]
-            return stream_object.amount
-        
-        if property=="tag":
-            return stream_object.tag
-        elif property=="pressure":
-            return stream_object.pressure
-        elif property=="temperature":
-            return stream_object.temperature
-        elif property=="mass_flowrate":
-            return stream_object.mass_flowrate
-        elif property=="vol_flowrate":
-            return stream_object.vol_flowrate
-        elif property=="molecular_weight":
-            return stream_object.molecular_weight
-        elif property=="mol_flowrate":
-            return stream_object.mol_flowrate
-        elif property=="components":
-            return stream_object.components
-        elif property=="density":
-            return stream_object.density
-        elif property=="density_l":
-            return stream_object.density_l
-        elif property=="density_g":
-            return stream_object.density_g
-        elif property=="d_viscosity":
-            return stream_object.d_viscosity
-        elif property=="d_viscosity_l":
-            return stream_object.d_viscosity_l
-        elif property=="d_viscosity_g":
-            return stream_object.d_viscosity_g
-        elif property=="isentropic_exponent":
-            return stream_object.isentropic_exponent
-        elif property=="phase":
-            return stream_object.phase
-        elif property=="Z_g":
-            return stream_object.Z_g
-        elif property=="Psat":
-            return stream_object.Psat
-        elif property=="Pc":
-            return stream_object.Pc
-            
-    def _create_equipment_tag(cls):
-        i = 1
-        class_name = type(cls).__name__
-        tag = class_name+ "_" + str(i)
-        while cls._check_tag_assigned(tag):
-            tag = class_name+ "_" + str(i)
-            i += 1
-        return tag
-    
-    def _check_tag_assigned(cls, tag):
-        for equipment in cls.items:
-            if tag == equipment.tag:
-                return True
-        return False
-    
-    def _tuple_property_value_unit_returner(self, value, property_type):
-        """ 
-            DESCRIPTION:
-                Internal function to get value and unit from either tuple,
-                property, float or int based on how user has provided.
-            
-            PARAMETERS:
-                value:
-                    Required: Yes
-                    Type: tuple or property or int or float
-                    Default value: Not Applicable
-                    Description: Value provided by the user
-                
-                property_type:
-                    Required: Yes
-                    Type: Propylean property
-                    Description: Type of property.
-
-            
-            RETURN VALUE:
-                Type: Tuple
-            
-            ERROR RAISED:
-                Type:
-                Description: 
-            
-            SAMPLE USE CASES:
-                self._tuple_property_value_unit_returner(prop.Length(10, "cm"), prop.Length)  
-        """
-        if isinstance(value, tuple):
-            return value[0], value[1]
-        elif isinstance(value, property_type):
-            return value.value, value.unit
-        elif any([isinstance(value, float), isinstance(value, int)]):
-            return value, None
-
-    def _physical_chemical_reaction(self):
-        # If both inlet and outlet streams are not conneted to the equipment
-        # no need to exchange properties between streams.
-        
-        if (self._outlet_material_stream_index is not None and
-            self._inlet_material_stream_index is not None):
-            inlet_m_stream_object = streams.MaterialStream.list_objects()[self._inlet_material_stream_index]
-            outlet_m_stream_object = streams.MaterialStream.list_objects()[self._outlet_material_stream_index]
-
-            # Inlet streams will always be governing.
-            outlet_m_stream_object.molecular_weight = inlet_m_stream_object.molecular_weight
-            outlet_m_stream_object.components = inlet_m_stream_object.components
-            outlet_m_stream_object.density = inlet_m_stream_object.density
-            outlet_m_stream_object.density_l = inlet_m_stream_object.density_l
-            outlet_m_stream_object.density_g = inlet_m_stream_object.density_g
-            outlet_m_stream_object.density_s = inlet_m_stream_object.density_s
-            outlet_m_stream_object.d_viscosity = inlet_m_stream_object.d_viscosity
-            outlet_m_stream_object.d_viscosity_l = inlet_m_stream_object.d_viscosity_l
-            outlet_m_stream_object.d_viscosity_g = inlet_m_stream_object.d_viscosity_g
-            outlet_m_stream_object.isentropic_exponent = inlet_m_stream_object.isentropic_exponent
-            outlet_m_stream_object.phase = inlet_m_stream_object.phase
-            outlet_m_stream_object.Psat = inlet_m_stream_object.Psat
-            outlet_m_stream_object.Pc = inlet_m_stream_object.Pc
-            outlet_m_stream_object.Z_g = inlet_m_stream_object.Z_g
-            outlet_m_stream_object.Z_l = inlet_m_stream_object.Z_l
-
-        if (self._outlet_energy_stream_index is not None and
-            self._inlet_energy_stream_index is not None):
-            inlet_e_stream_object = streams.EnergyStream.list_objects()[self._inlet_energy_stream_index]
-            outlet_e_stream_object = streams.EnergyStream.list_objects()[self._outlet_energy_stream_index]
-            outlet_e_stream_object.amount = inlet_e_stream_object.amount
-
-    def delete(self):
-        """ 
-        DESCRIPTION:
-            Method to delete an equipment object.
-        
-        PARAMETERS:
-            None
-
-        RETURN VALUE:
-            Type: bool
-            Description: True is returned if deletion is successful else False
-        
-        ERROR RAISED:
-            Type: General
-            Description: 
-        
-        SAMPLE USE CASES:
-            >>> eq1 = CentrifugalPump()
-            >>> eq1.delete()
-        """
-        result = True
-        if self._inlet_material_stream_index is not None:
-            result = result & self.disconnect_stream(direction='in',
-                                                     stream_tag=self._inlet_material_stream_tag,
-                                                     stream_type='material')
-        if self._outlet_material_stream_index is not None:
-            result = result & self.disconnect_stream(direction='out',
-                                                     stream_tag=self._outlet_material_stream_tag,
-                                                     stream_type='material')
-        if self._inlet_energy_stream_index is not None:
-            result = result & self.disconnect_stream(direction='in',
-                                                     stream_tag=self._inlet_energy_stream_tag,
-                                                     stream_type='energy')
-        if self._outlet_energy_stream_index is not None:
-            result = result & self.disconnect_stream(direction='out',
-                                                     stream_tag=self._outlet_energy_stream_tag,
-                                                     stream_type='energy')
-        del self.items[self.index]
-        del self
-        return result
-
-#Defining generic base class for all equipments with multiple inlet and outlet. TODO !!!!!!       
-class _EquipmentMultipleInletOutlet:
-    def __init__(self) -> None:
-        pass
+import propylean.properties as prop
+from propylean import streams
+from propylean.validators import _Validators
+import warnings
+
+global _material_stream_equipment_map
+_material_stream_equipment_map = dict()
+global _energy_stream_equipment_map
+_energy_stream_equipment_map = dict()
+
+# Defining generic base class for all equipments with one inlet and outlet.
+class _EquipmentOneInletOutlet(object):
+    items = []
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Internal base class to define an equipment with one inlet and outlet.
+            All final classes inherits from this base class.
+            Read individual final classed for further description.
+    
+        PARAMETERS:
+            tag:
+                Required: No
+                Type: str
+                Acceptable values: Any string type
+                Default value: None
+                Description: Equipment tag the user wants to provide. If not provided, then tag is automatically generated.
+
+            pressure_drop:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Any
+                Default value: None
+                Description: Represents pressure drop the equipment. Negative value implies pressure increase.
+            
+
+        RETURN VALUE:
+            Type: _EquipmentOneInletOutlet
+            Description: Object of type _EquipmentOneInletOutlet
+        
+        ERROR RAISED:
+            Type: Various
+            Description: 
+        
+        SAMPLE USE CASES:
+            >>> class NewEquipment(_EquipmentOneInletOutlet):
+                ......
+        """
+        self.tag = inputs.pop('tag', self._create_equipment_tag())
+
+        #Flow properties
+        self._inlet_mass_flowrate = prop.MassFlowRate() 
+        self._outlet_mass_flowrate = prop.MassFlowRate()
+        self._inventory_change_rate = prop.MassFlowRate()
+        self.design_flowrate = prop.MassFlowRate()
+
+        #Pressure properties
+        self._pressure_drop = prop.Pressure(0)
+        self._inlet_pressure = prop.Pressure()
+        self._outlet_pressure = prop.Pressure()
+        self._design_pressure = prop.Pressure()
+        
+        #Temperature properties
+        self._temperature_increase = prop.Temperature(0, 'K')
+        self._inlet_temperature = prop.Temperature()
+        self._outlet_temperature = prop.Temperature()
+        self._design_temperature = prop.Temperature()
+
+        #Inlet and outlet material and energy streams
+        self._inlet_material_stream_tag = None
+        self._outlet_material_stream_tag = None
+        self._inlet_energy_stream_tag = None
+        self._outlet_energy_stream_tag = None
+        self._inlet_material_stream_index = None
+        self._outlet_material_stream_index = None
+        self._inlet_energy_stream_index = None
+        self._outlet_energy_stream_index = None
+        
+        #Energy properties
+        self._energy_in = prop.Power()
+        self._energy_out = prop.Power()
+
+        #Other Porperties
+        self.main_fluid = "liquid" if "main_fluid" not in inputs else inputs["main_fluid"]
+        self._is_disconnection = False
+
+        if 'pressure_drop' in inputs:
+            self.pressure_drop = inputs['pressure_drop']
+    
+    @property
+    def index(self):
+      return self._index
+
+    @property
+    def tag(self):
+        return self._tag
+    @tag.setter
+    def tag(self, value):
+        _Validators.validate_arg_prop_value_type("tag", value, (str))
+        if self._check_tag_assigned(value):
+            msg = "Tag '{}' already assigned!".format(value)
+            raise Exception(msg)
+        else:
+            self._tag = value
+
+    @property
+    def inlet_pressure(self):
+        self = self._get_equipment_object(self)
+        return self._inlet_pressure
+    @inlet_pressure.setter
+    def inlet_pressure(self, value):
+        _Validators.validate_arg_prop_value_type("inlet_pressure", value, (prop.Pressure, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
+        if unit is None:
+            unit = self._inlet_pressure.unit
+        self._inlet_pressure = prop.Pressure(value, unit)
+        self._outlet_pressure = self._inlet_pressure - self.pressure_drop
+        self._update_equipment_object(self)
+    
+    @property
+    def outlet_pressure(self):
+        self = self._get_equipment_object(self)
+        return self._outlet_pressure
+    @outlet_pressure.setter
+    def outlet_pressure(self, value):
+        _Validators.validate_arg_prop_value_type("outlet_pressure", value, (prop.Pressure, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
+        if unit is None:
+            unit = self._outlet_pressure.unit
+        self._outlet_pressure = prop.Pressure(value, unit)
+        self._inlet_pressure = self._outlet_pressure + self.pressure_drop
+        self._update_equipment_object(self)
+    
+    @property
+    def pressure_drop(self):
+        self = self._get_equipment_object(self)
+        return self._pressure_drop
+    @pressure_drop.setter
+    def pressure_drop(self, value):
+        _Validators.validate_arg_prop_value_type("pressure_drop", value, (prop.Pressure, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
+        if unit is None:
+            unit = self._pressure_drop.unit
+        self._pressure_drop = prop.Pressure(value, unit)
+        self._outlet_pressure =  self._inlet_pressure - self._pressure_drop
+        self._update_equipment_object(self)
+    
+    @property
+    def design_pressure(self):
+        self = self._get_equipment_object(self)
+        return self._design_pressure
+    @design_pressure.setter
+    def design_pressure(self, value):
+        _Validators.validate_arg_prop_value_type("design_pressure", value, (prop.Pressure, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
+        if unit is None:
+            unit = self._design_pressure.unit
+        self._design_pressure = prop.Pressure(value, unit)
+        self._update_equipment_object(self)
+
+    @property
+    def inlet_temperature(self):
+        self = self._get_equipment_object(self)
+        return self._inlet_temperature
+    @inlet_temperature.setter
+    def inlet_temperature(self, value):
+        _Validators.validate_arg_prop_value_type("inlet_temperature", value, (prop.Temperature, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
+        if unit is None:
+            unit = self._inlet_temperature.unit
+        self._inlet_temperature = prop.Temperature(value, unit)
+        self._outlet_temperature = self._inlet_temperature + self.temperature_increase
+        self._update_equipment_object(self)
+
+    @property
+    def outlet_temperature(self):
+        self = self._get_equipment_object(self)
+        return self._outlet_temperature
+    @outlet_temperature.setter
+    def outlet_temperature(self,value):
+        _Validators.validate_arg_prop_value_type("outlet_temperature", value, (prop.Temperature, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
+        if unit is None:
+            unit = self._outlet_temperature.unit
+        self._outlet_temperature = prop.Temperature(value, unit)
+        self._inlet_temperature = self._outlet_temperature - self.temperature_increase
+        self._update_equipment_object(self)
+
+    @property
+    def temperature_increase(self):
+        self = self._get_equipment_object(self)
+        return self._temperature_increase
+    @temperature_increase.setter
+    def temperature_increase(self, value):
+        _Validators.validate_arg_prop_value_type("temperature_increase", value, (prop.Temperature, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
+        if unit is None:
+            unit = self._temperature_increase.unit
+        self._temperature_increase = prop.Temperature(value, unit)
+        self._outlet_temperature =  self._inlet_temperature + self._temperature_increase
+        self._update_equipment_object(self)
+    @property
+    def temperature_decrease(self):
+        self = self._get_equipment_object(self)
+        decrease = -1 * self._temperature_increase.value
+        return prop.Temperature(decrease, self._temperature_increase.unit)
+    @temperature_decrease.setter
+    def temperature_decrease(self, value):
+        _Validators.validate_arg_prop_value_type("temperature_decrease", value, (prop.Temperature, int, float, tuple))
+        if isinstance(value, prop.Temperature):
+            value = prop.Temperature(-1 * value.value, value.unit)
+        elif isinstance(value, tuple):
+            value = prop.Temperature(-1 * value[0], value[1])
+        elif isinstance(value, (int, float)):
+            value = prop.Temperature(-1 * value, self._temperature_increase.unit)
+        self.temperature_increase = value
+    
+    @property
+    def design_temperature(self):
+        self = self._get_equipment_object(self)
+        return self._design_pressure
+    @design_temperature.setter
+    def design_temperature(self, value):
+        _Validators.validate_arg_prop_value_type("design_temperature", value, (prop.Temperature, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
+        if unit is None:
+            unit = self._design_temperature.unit
+        self._design_temperature = prop.Temperature(value, unit)
+        self._update_equipment_object(self)
+
+    @property
+    def inlet_mass_flowrate(self):
+        self = self._get_equipment_object(self)
+        return self._inlet_mass_flowrate
+    @inlet_mass_flowrate.setter
+    def inlet_mass_flowrate(self, value):
+        _Validators.validate_arg_prop_value_type("inlet_mass_flowrate", value, (prop.MassFlowRate, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.MassFlowRate)
+        if unit is None:
+            unit = self._inlet_mass_flowrate.unit
+        self._inlet_mass_flowrate = prop.MassFlowRate(value, unit)
+        self._outlet_mass_flowrate = self._inlet_mass_flowrate + self.inventory_change_rate
+        self._update_equipment_object(self)
+    
+    @property
+    def outlet_mass_flowrate(self):
+        self = self._get_equipment_object(self)
+        return self._outlet_mass_flowrate
+    @outlet_mass_flowrate.setter
+    def outlet_mass_flowrate(self, value):
+        _Validators.validate_arg_prop_value_type("outlet_mass_flowrate", value, (prop.MassFlowRate, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.MassFlowRate)
+        if unit is None:
+            unit = self._outlet_mass_flowrate.unit
+        self._outlet_mass_flowrate = prop.MassFlowRate(value, unit)
+        self._inlet_mass_flowrate = self._outlet_mass_flowrate - self.inventory_change_rate
+        self._update_equipment_object(self)
+    
+    @property
+    def inventory_change_rate(self):
+        self = self._get_equipment_object(self)
+        return self._inventory_change_rate
+    @inventory_change_rate.setter
+    def inventory_change_rate(self, value):
+        _Validators.validate_arg_prop_value_type("inventory_change_rate", value, (int, float, prop.MassFlowRate))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.MassFlowRate)
+        if unit is None:
+            unit = self.inventory_change_rate.unit
+        self._update_equipment_object(self)
+    
+    @property
+    def energy_in(self):
+        self = self._get_equipment_object(self)
+        return self._energy_in
+    @energy_in.setter
+    def energy_in(self, value):
+        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self.energy_in.unit
+        self._energy_in = prop.Power(value, unit)
+        self._update_equipment_object(self)
+    @energy_in.deleter
+    def energy_in(self):
+        self = self._get_equipment_object(self)
+        del self._energy_in
+        self._update_equipment_object(self)
+
+    @property
+    def energy_out(self):
+        self = self._get_equipment_object(self)
+        return self._energy_out
+    @energy_out.setter
+    def energy_out(self, value):
+        _Validators.validate_arg_prop_value_type("energy_out", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self.energy_out.unit
+        self._energy_in = prop.Power(value, unit)
+        self._update_equipment_object(self)
+    @energy_out.deleter
+    def energy_out(self):
+        self = self._get_equipment_object(self)
+        del self._energy_out
+        self._update_equipment_object(self) 
+    
+    def _get_equipment_index(cls, tag):
+        for index, equipment in enumerate(cls.items):
+            if equipment.tag == tag:
+                return index
+        return None
+    
+    @classmethod
+    def _get_equipment_object(cls, obj):
+        try:
+            return cls.items[obj.index]
+        except IndexError:
+            raise Exception("Equipment does not exist!")
+        except AttributeError:
+            return obj
+    
+    @classmethod
+    def _update_equipment_object(cls, obj):
+        _Validators.validate_arg_prop_value_type("obj", obj, cls)
+        try:
+            cls.items[obj.index] = obj
+        except:
+            pass
+    
+    def __eq__(self, other):
+        if isinstance(other, type(self)):
+            return self.tag == other.tag
+        else:
+            return False
+
+    def get_stream_tag(self, stream_type, direction):
+        """ 
+        DESCRIPTION:
+            Method to tsg ogf stream connected to the equipment using steam 
+            type and the direction.
+        
+        PARAMETERS:
+            stream_type:
+                Required: Yes
+                Type: str
+                Acceptable values: 'm', 'mass', 'e', 'energy'
+                Description: Type of stream user wants to get tag of.
+            direction:
+                Required: Yes
+                Type: str
+                Acceptable values: 'in', 'out', 'inlet' or 'outlet'
+                Description: Direction of stream with respect to equipment user wants to get tag of.
+       
+        RETURN VALUE:
+            Type: str
+            Description: Tag value of stream user has assigned to the stream
+        
+        ERROR RAISED:
+            Type: General TODO
+            Description: Raises error if arguments are incorrect
+        
+        SAMPLE USE CASES:
+            >>> eq1.get_stream_tag('m', 'out')
+            >>> eq1.get_stream_tag('energy', 'in')
+        """
+        _Validators.validate_arg_prop_value_type("stream_type", stream_type, (str))
+        _Validators.validate_arg_prop_value_list("stream_type", stream_type, ['m', 'mass', 'e', 'energy', 'material'])
+        _Validators.validate_arg_prop_value_type("direction", direction, (str))
+        _Validators.validate_arg_prop_value_list("direction", direction, ['in', 'out', 'inlet', 'outlet'])
+
+        if stream_type.lower() in ['material', 'mass', 'm']:
+            stream_tag = [self._inlet_material_stream_tag, self._outlet_material_stream_tag]
+        elif stream_type.lower() in ['energy', 'power', 'e', 'p']:
+            stream_tag = [self._inlet_energy_stream_tag, self._outlet_energy_stream_tag]
+        else:
+            raise Exception('Incorrect stream_type specified! Provided \"'+stream_type+'\". Can only be "material/mass/m" or "energy/e/power/p"]')
+        
+        if direction.lower() in ['in', 'inlet']:
+                return stream_tag[0]
+        elif direction.lower() in ['out', 'outlet']:
+            return stream_tag[1]
+        else:
+            raise Exception('Incorrect direction specified! Provided \"'+direction+'\". Can only be ["in", "out", "inlet", "outlet"]')
+
+    def connect_stream(self,
+                       stream_object=None,
+                       direction=None, 
+                       stream_tag=None,
+                       stream_type=None,
+                       stream_governed=True):
+        """ 
+        DESCRIPTION:
+            Method to connect a stream object with equiment.
+        
+        PARAMETERS:
+            stream_object:
+                Required: No if stream_tag is provided else Yes
+                Type: EnergyStream or MaterialStream
+                Acceptable values: object of specified stream types
+                Default value: None
+                Description: Stream object user wants to connect the equipment with.
+            
+            direction:
+                Required: Yes for material stream. For energy stream not needed
+                Type: str
+                Acceptable values: 'in', 'out', 'inlet' or 'outlet'
+                Default value: None
+                Description: Direction in which stream should be with respect to equipment.
+            
+            stream_tag:
+                Required: No if stream_object is provided else Yes
+                Type: str
+                Acceptable values: stream tag provided by user
+                Default value: None
+                Description: Stream object with known stream_tag user wants to connect the equipment with.
+
+            stream_type:
+                Required: No if stream_object provided
+                Type: str
+                Acceptable values: 'm', 'mass', 'e', 'energy'
+                Description: Type of stream user wants to connect.
+
+            stream_governed:
+                Required: No 
+                Type: bool
+                Default values: True
+                Description: Determines if stream will govern the property. Fluid property will be passed.    
+
+        RETURN VALUE:
+            Type: bool
+            Description: True is returned if connection is successful else False
+        
+        ERROR RAISED:
+            Type: General
+            Description: Error raised if arguments are wrong
+        
+        SAMPLE USE CASES:
+            >>> eq1.connect_stream(en1)
+            >>> eq1.connect_stream(direction='out', stream_tag='Pump-outlet', stream_type='m')
+        """
+        if stream_object is not None:
+            _Validators.validate_arg_prop_value_type("stream_object", stream_object, (streams.MaterialStream, streams.EnergyStream))
+            _Validators.validate_arg_prop_value_type("direction", direction, str)
+            _Validators.validate_arg_prop_value_type("stream_governed", stream_governed, bool)
+            _Validators.validate_arg_prop_value_list("direction", direction, ['in', 'out', 'inlet', 'outlet'])
+            if not (isinstance(stream_object, streams.EnergyStream) or
+                    isinstance(stream_object, streams.MaterialStream)):
+                    raise Exception("Stream object should be of type EnergyStream or Material Stream not " +
+                                    type(stream_object))
+            stream_tag = stream_object.tag
+            if isinstance(stream_object, streams.MaterialStream):
+                stream_type = 'm'
+            elif isinstance(stream_object, streams.EnergyStream):
+                stream_type = 'e'
+        elif not self._is_disconnection and stream_tag is None:
+            raise Exception("Either of Stream Object or Stream Tag is required for connection!")
+        else:
+            _Validators.validate_arg_prop_value_type("stream_tag", stream_tag, str)
+            _Validators.validate_arg_prop_value_type("direction", direction, str)
+            _Validators.validate_arg_prop_value_list("direction", direction, ['in', 'out', 'inlet', 'outlet'])
+            _Validators.validate_arg_prop_value_type("stream_type", stream_type, str)
+            _Validators.validate_arg_prop_value_list("stream_type", stream_type, ['m', 'mass', 'e', 'energy', 'material'])
+            _Validators.validate_arg_prop_value_type("stream_governed", stream_governed, bool)
+        
+        stream_index = streams.get_stream_index(stream_tag, stream_type)
+        is_inlet = True if direction.lower() in ['in', 'inlet'] else False
+
+        mapping_result = self._stream_equipment_mapper(stream_index, stream_type, is_inlet)
+        if self._is_disconnection:
+            stream_tag = stream_index = None
+            
+        if stream_type.lower() in ['material', 'mass', 'm']:
+            if direction.lower() in ['in', 'inlet']:
+                self._inlet_material_stream_tag = stream_tag
+                self._inlet_material_stream_index = stream_index
+            else:
+                self._outlet_material_stream_tag = stream_tag
+                self._outlet_material_stream_index = stream_index
+        else:
+            if direction.lower() in ['in', 'inlet']:
+                self._inlet_energy_stream_tag = stream_tag
+                self._inlet_energy_stream_index = stream_index
+            else:
+                self._outlet_energy_stream_tag = stream_tag
+                self._outlet_energy_stream_index = stream_index
+        
+        if mapping_result and not self._is_disconnection:
+            self._stream_equipment_properties_matcher(stream_index, 
+                                                      stream_type,
+                                                      is_inlet,
+                                                      stream_governed)
+        return mapping_result
+
+    def disconnect_stream(self, 
+                          stream_object=None,
+                          direction=None, 
+                          stream_tag=None,
+                          stream_type=None):
+        """ 
+        DESCRIPTION:
+            Class method to disconnect a stream object from equiment.
+        
+        PARAMETERS:
+            stream_object:
+                Required: No if stream_tag is provided else Yes
+                Type: EnergyStream or MaterialStream
+                Acceptable values: object of specified stream types
+                Default value: None
+                Description: Stream object user wants to disconnect the equipment with.
+            
+            direction:
+                Required: Yes if stream_object or stream_tag not provided
+                Type: str
+                Acceptable values: 'in', 'out', 'inlet' or 'outlet'
+                Default value: None
+                Description: Direction in which stream should be with respect to equipment.
+            
+            stream_tag:
+                Required: No if stream_object is provided else Yes
+                Type: str
+                Acceptable values: stream tag provided by user
+                Default value: None
+                Description: Stream object with known stream_tag user wants to disconnect the equipment from.
+
+            stream_type:
+                Required: No if stream_object provided
+                Type: str
+                Acceptable values: 'm', 'mass', 'e', 'energy'
+                Description: Type of stream user wants to disconnect.
+
+        RETURN VALUE:
+            Type: bool
+            Description: True is returned if disconnection is successful else False
+        
+        ERROR RAISED:
+            Type: General
+            Description: Error raised if arguments are wrong
+        
+        SAMPLE USE CASES:
+            >>> eq1.disconnect_stream(s1)
+            >>> eq1.disconnect_stream(stream_tag='Pump-outlet')
+            >>> eq1.disconnect_stream(direction='in', stream_type="energy")
+        """
+               
+        def define_index_direction(tag):
+            " This function is internal function. Not to be used elsewhere."
+            stream_type = None
+            direction = None
+            if tag == self._inlet_material_stream_tag:
+                stream_type = "m"
+                direction = "in"
+            elif tag == self._outlet_material_stream_tag:
+                stream_type = "m"
+                direction = "out"
+            elif tag == self._inlet_energy_stream_tag:
+                stream_type = "e"
+                direction = "in"
+            elif tag == self._outlet_energy_stream_tag:
+                stream_type = "e"
+                direction = "out"
+            return stream_type, direction
+
+        if stream_object is not None:
+            _Validators.validate_arg_prop_value_type("stream_object", stream_object, (streams.MaterialStream, streams.EnergyStream))
+            stream_type, direction = define_index_direction(stream_object.tag)
+        elif stream_tag is not None:
+            _Validators.validate_arg_prop_value_type("stream_tag", stream_tag, (str))
+            stream_type, direction = define_index_direction(stream_tag)
+        elif (direction is not None and 
+              stream_type is not None):
+              _Validators.validate_arg_prop_value_type("direction", direction, (str))
+              _Validators.validate_arg_prop_value_type("stream_type", stream_type, (str))
+              _Validators.validate_arg_prop_value_list("direction", direction, ['in', 'out', 'inlet', 'outlet'])
+              _Validators.validate_arg_prop_value_list("stream_type", stream_type, ['m', 'mass', 'e', 'energy', 'material'])
+              stream_tag = self.get_stream_tag(stream_type, direction)
+              stream_type, direction = define_index_direction(stream_tag)
+        else:
+            raise Exception("To disconnect stream from equipment, provide either just connected stream object or\
+                             just stream tag or just direction & stream type") 
+
+        # Validate if connection is there.
+        if stream_type is None and direction is None:
+            warnings.warn("Already there is no connection.")
+            return
+
+        if stream_type.lower() in ['material', 'mass', 'm']:
+            if direction.lower() in ['in', 'inlet']:
+                if (self._inlet_material_stream_tag is None or 
+                   self._inlet_material_stream_index is None):
+                   warnings.warn("Material Inlet already has no connection.")
+                   return 
+            else:
+                if (self._outlet_material_stream_tag is None or 
+                   self._outlet_material_stream_index is None):
+                   warnings.warn("Material Outlet already has no connection.")
+                   return 
+                  
+        else:
+            if direction.lower() in ['in', 'inlet']:
+                if (self._inlet_energy_stream_tag is None or 
+                   self._inlet_energy_stream_index is None):
+                   warnings.warn("Energy Inlet already has no connection.")
+                   return 
+            else:
+                if (self._outlet_energy_stream_tag is None or 
+                   self._outlet_energy_stream_index is None):
+                   warnings.warn("Energy Outlet already has no connection.")
+                   return       
+
+        self._is_disconnection = True
+        return self.connect_stream(stream_object,
+                                   direction, 
+                                   stream_tag,
+                                   stream_type)
+      
+    def _stream_equipment_mapper(self, stream_index, stream_type, is_inlet):
+        """ 
+            DESCRIPTION:
+                Internal function to map stream with equipment object.
+                _material_stream_equipment_map and _energy_stream_equipment_map 
+                are dictionary of list which store index of coming from and going 
+                to equipment and type of equipment. Structured like 
+                {12: [10, CentrifugalPump, 21, PipeSegment], 
+                 23: [21, PipeSegment, 36, FlowMeter]]} 
+                where 12th index stream will have data in key no. 12. 
+                Stream is coming from equipment with index 10 and is of type CentrifugalPump.  
+                Stream is going into equipment with index 21 of type PipeSegment.
+            
+            PARAMETERS:
+                stream_index:
+                    Required: Yes
+                    Type: int
+                    Acceptable values: Non-negative integer
+                    Default value: Not Applicable
+                    Description: Index of the stream in the stream list it belongs to.
+                
+                stream_type:
+                    Required: Yes
+                    Type: string
+                    Acceptable values: 'material' or 'energy'
+                    Default value: Not Applicable
+                    Description: Index of the stream in the stream list it belongs to.
+                
+                is_inlet:
+                    Required: Yes
+                    Type: bool
+                    Acceptable values: True or False
+                    Default value: Not Applicable
+                    Description: True or False if stream is inlet to equipment.
+            
+            RETURN VALUE:
+                Type: bool
+                Description: If mapping was successful True is returned else False
+            
+            ERROR RAISED:
+                Type:
+                Description: 
+            
+            SAMPLE USE CASES:
+                >>>  _stream_equipment_mapper(10, 'm', False)
+                >>> stream_index = get_stream_index("Compressor1_power", "energy")
+                >>>  _stream_equipment_mapper(stream_index, 'e', True)
+                
+        """
+
+        if stream_index is None or isinstance(stream_index, list):
+            return False
+        e_type, e_index = (3, 2) if is_inlet else (1, 0)
+        global _material_stream_equipment_map
+        global _energy_stream_equipment_map
+        if stream_type in ['m', 'material']:
+            stream_equipment_map = _material_stream_equipment_map
+        elif stream_type in ['e', 'energy']:
+            stream_equipment_map =_energy_stream_equipment_map
+        else:
+            raise Exception('Incorrect stream type {}'.format(stream_type)+\
+                            " Can only be 'm' or 'e' ")
+        equipment_type = type(self)
+        equipment_index = self._get_equipment_index(self.tag)
+        def set_type_index():
+            old_equipment_type = stream_equipment_map[stream_index][e_type]
+            old_equipment_index = stream_equipment_map[stream_index][e_index]
+            stream_equipment_map[stream_index][e_type] = equipment_type if not self._is_disconnection else None
+            stream_equipment_map[stream_index][e_index] = equipment_index if not self._is_disconnection else None
+            if (not self._is_disconnection and
+                old_equipment_index is not None
+                and old_equipment_type is not None):
+                old_equipment_obj = old_equipment_type.list_objects()[old_equipment_index]
+                old_equipment_obj.disconnect_stream(stream_type=stream_type, direction='in' if is_inlet else 'out')
+                warnings.warn("Equipment type " + str(old_equipment_type) +
+                              " with tag " + old_equipment_obj.tag + 
+                              " was disconnected from stream type " + str(stream_type) +
+                              " with tag " + str(self.get_stream_tag(stream_type,
+                                                                'in' if is_inlet else 'out')))
+        try:
+            set_type_index()   
+        except:
+            try:
+                stream_equipment_map[stream_index] = [None, None, None, None]
+                set_type_index()
+            except Exception as e:
+                raise Exception("Error occured in equipment-stream mapping:", e)
+
+        if stream_type in ['material', 'm']:
+            _material_stream_equipment_map = stream_equipment_map
+        elif stream_type in ['energy', 'e']:
+            _energy_stream_equipment_map = stream_equipment_map
+        return True
+
+    def _stream_equipment_properties_matcher(self, stream_index, 
+                                             stream_type, 
+                                             is_inlet, 
+                                             stream_governed=True):
+        """ 
+            DESCRIPTION:
+                Internal function to match properties of stream with that of equipment object's.
+            
+            PARAMETERS:
+                stream_index:
+                    Required: Yes
+                    Type: int
+                    Acceptable values: Non-negative integer
+                    Default value: Not Applicable
+                    Description: Index of the stream in the stream list it belongs to.
+                
+                stream_type:
+                    Required: Yes
+                    Type: string
+                    Acceptable values: 'material' or 'energy'
+                    Default value: Not Applicable
+                    Description: Index of the stream in the stream list it belongs to.
+                
+                is_inlet:
+                    Required: Yes
+                    Type: bool
+                    Acceptable values: True or False
+                    Default value: Not Applicable
+                    Description: True or False if stream is inlet to equipment or not.
+                
+                stream_governed:
+                    Required: False
+                    Type: bool
+                    Acceptable values: True or False
+                    Default value: Not Applicable
+                    Description: Determines if stream to govern the property or equipment.
+                                 If True, stream property are assigned to equipment.
+                                 If False, equipment property are assigned to stream.
+            
+            RETURN VALUE:
+                Type: bool
+                Description: If matching was successful, True is returned else False.
+            
+            ERROR RAISED:
+                Type:
+                Description: 
+            
+            SAMPLE USE CASES:
+                >>>  _stream_equipment_properties_matcher(10, 'm', False)
+                >>> stream_index = get_stream_index("Compressor1_power", "energy")
+                >>>  _stream_equipment_properties_matcher(stream_index, 'e', True)
+                
+        """
+        def property_matcher(stream_property, equipment_property, stream_governed):
+            if stream_governed:
+                return stream_property, stream_property
+            return equipment_property, equipment_property
+
+        if stream_type.lower() in ['m', 'material', 'mass']:
+            stream_object = streams.MaterialStream.list_objects()[stream_index]
+            if is_inlet:
+                stream_object.mass_flowrate, \
+                self.inlet_mass_flowrate = property_matcher(stream_object.mass_flowrate,
+                                                            self._inlet_mass_flowrate,
+                                                            stream_governed)
+                stream_object.pressure, \
+                self.inlet_pressure = property_matcher(stream_object.pressure,
+                                                       self._inlet_pressure,
+                                                       stream_governed)
+                stream_object.temperature, \
+                self.inlet_temperature = property_matcher(stream_object.temperature,
+                                                          self._inlet_temperature,
+                                                          stream_governed)
+            else:
+                stream_object.mass_flowrate, \
+                self.outlet_mass_flowrate = property_matcher(stream_object.mass_flowrate,
+                                                             self._outlet_mass_flowrate,
+                                                             stream_governed)
+                stream_object.pressure, \
+                self.outlet_pressure = property_matcher(stream_object.pressure,
+                                                        self._outlet_pressure,
+                                                        stream_governed)
+                stream_object.temperature, \
+                self.outlet_temperature = property_matcher(stream_object.temperature,
+                                                           self._outlet_temperature,
+                                                           stream_governed)
+            if not stream_governed:
+                streams.MaterialStream._update_stream_object(stream_object)
+            else:
+                self._update_equipment_object(self)
+        else:
+            stream_object = streams.EnergyStream.list_objects()[stream_index]
+            if is_inlet:
+                stream_object.amount, \
+                self.energy_in = property_matcher(stream_object.amount,
+                                                  self.energy_in,
+                                                  stream_governed)     
+            else:
+                stream_object.amount, \
+                self.energy_out = property_matcher(stream_object.amount,
+                                                    self.energy_out,
+                                                    stream_governed)
+            if not stream_governed:
+                streams.EnergyStream._update_stream_object(stream_object)
+        self._physical_chemical_reaction()
+
+    def _connected_stream_property_getter(self, is_inlet, stream_type, property=None):
+        """ 
+            DESCRIPTION:
+                Internal function to get object of stream.
+            
+            PARAMETERS:
+                is_inlet:
+                    Required: Yes
+                    Type: bool
+                    Default value: Not Applicable
+                    Description: True if stream is inlet to equipment. False if stream is outlet.
+                
+                stream_type:
+                    Required: Yes
+                    Type: string
+                    Acceptable values: 'material' or 'energy'
+                    Default value: Not Applicable
+                    Description: Index of the stream in the stream list it belongs to.
+                
+                property:
+                    Required: Yes if stream_type is material
+                    Type: String
+                    Description: Type of property. See the if else ladder.
+
+            
+            RETURN VALUE:
+                Type: Any supported property
+            
+            ERROR RAISED:
+                Type:
+                Description: 
+            
+            SAMPLE USE CASES:
+                >>> Psat = self._connected_stream_property_getter(True, "material", "Psat")
+                
+        """
+        
+        if stream_type.lower() in ['m', 'material', 'mass']:
+            stream_index = self._inlet_material_stream_index if is_inlet else self._outlet_material_stream_index
+            if stream_index is None:
+                raise Exception("Equipment not connected to MaterialStream!")
+            stream_object = streams.MaterialStream.list_objects()[stream_index]  
+        else:
+            stream_index = self._inlet_energy_stream_index if is_inlet else self._outlet_energy_stream_index
+            if stream_index is None:
+                raise Exception("Equipment not connected to EnergyStream!")
+            stream_object = streams.EnergyStream.list_objects()[stream_index]
+            return stream_object.amount
+        
+        if property=="tag":
+            return stream_object.tag
+        elif property=="pressure":
+            return stream_object.pressure
+        elif property=="temperature":
+            return stream_object.temperature
+        elif property=="mass_flowrate":
+            return stream_object.mass_flowrate
+        elif property=="vol_flowrate":
+            return stream_object.vol_flowrate
+        elif property=="molecular_weight":
+            return stream_object.molecular_weight
+        elif property=="mol_flowrate":
+            return stream_object.mol_flowrate
+        elif property=="components":
+            return stream_object.components
+        elif property=="density":
+            return stream_object.density
+        elif property=="density_l":
+            return stream_object.density_l
+        elif property=="density_g":
+            return stream_object.density_g
+        elif property=="d_viscosity":
+            return stream_object.d_viscosity
+        elif property=="d_viscosity_l":
+            return stream_object.d_viscosity_l
+        elif property=="d_viscosity_g":
+            return stream_object.d_viscosity_g
+        elif property=="isentropic_exponent":
+            return stream_object.isentropic_exponent
+        elif property=="phase":
+            return stream_object.phase
+        elif property=="Z_g":
+            return stream_object.Z_g
+        elif property=="Psat":
+            return stream_object.Psat
+        elif property=="Pc":
+            return stream_object.Pc
+            
+    def _create_equipment_tag(cls):
+        i = 1
+        class_name = type(cls).__name__
+        tag = class_name+ "_" + str(i)
+        while cls._check_tag_assigned(tag):
+            tag = class_name+ "_" + str(i)
+            i += 1
+        return tag
+    
+    def _check_tag_assigned(cls, tag):
+        for equipment in cls.items:
+            if tag == equipment.tag:
+                return True
+        return False
+    
+    def _tuple_property_value_unit_returner(self, value, property_type):
+        """ 
+            DESCRIPTION:
+                Internal function to get value and unit from either tuple,
+                property, float or int based on how user has provided.
+            
+            PARAMETERS:
+                value:
+                    Required: Yes
+                    Type: tuple or property or int or float
+                    Default value: Not Applicable
+                    Description: Value provided by the user
+                
+                property_type:
+                    Required: Yes
+                    Type: Propylean property
+                    Description: Type of property.
+
+            
+            RETURN VALUE:
+                Type: Tuple
+            
+            ERROR RAISED:
+                Type:
+                Description: 
+            
+            SAMPLE USE CASES:
+                self._tuple_property_value_unit_returner(prop.Length(10, "cm"), prop.Length)  
+        """
+        if isinstance(value, tuple):
+            return value[0], value[1]
+        elif isinstance(value, property_type):
+            return value.value, value.unit
+        elif any([isinstance(value, float), isinstance(value, int)]):
+            return value, None
+
+    def _physical_chemical_reaction(self):
+        # If both inlet and outlet streams are not conneted to the equipment
+        # no need to exchange properties between streams.
+        
+        if (self._outlet_material_stream_index is not None and
+            self._inlet_material_stream_index is not None):
+            inlet_m_stream_object = streams.MaterialStream.list_objects()[self._inlet_material_stream_index]
+            outlet_m_stream_object = streams.MaterialStream.list_objects()[self._outlet_material_stream_index]
+
+            # Inlet streams will always be governing.
+            outlet_m_stream_object.molecular_weight = inlet_m_stream_object.molecular_weight
+            outlet_m_stream_object.components = inlet_m_stream_object.components
+            outlet_m_stream_object.density = inlet_m_stream_object.density
+            outlet_m_stream_object.density_l = inlet_m_stream_object.density_l
+            outlet_m_stream_object.density_g = inlet_m_stream_object.density_g
+            outlet_m_stream_object.density_s = inlet_m_stream_object.density_s
+            outlet_m_stream_object.d_viscosity = inlet_m_stream_object.d_viscosity
+            outlet_m_stream_object.d_viscosity_l = inlet_m_stream_object.d_viscosity_l
+            outlet_m_stream_object.d_viscosity_g = inlet_m_stream_object.d_viscosity_g
+            outlet_m_stream_object.isentropic_exponent = inlet_m_stream_object.isentropic_exponent
+            outlet_m_stream_object.phase = inlet_m_stream_object.phase
+            outlet_m_stream_object.Psat = inlet_m_stream_object.Psat
+            outlet_m_stream_object.Pc = inlet_m_stream_object.Pc
+            outlet_m_stream_object.Z_g = inlet_m_stream_object.Z_g
+            outlet_m_stream_object.Z_l = inlet_m_stream_object.Z_l
+
+        if (self._outlet_energy_stream_index is not None and
+            self._inlet_energy_stream_index is not None):
+            inlet_e_stream_object = streams.EnergyStream.list_objects()[self._inlet_energy_stream_index]
+            outlet_e_stream_object = streams.EnergyStream.list_objects()[self._outlet_energy_stream_index]
+            outlet_e_stream_object.amount = inlet_e_stream_object.amount
+
+    def delete(self):
+        """ 
+        DESCRIPTION:
+            Method to delete an equipment object.
+        
+        PARAMETERS:
+            None
+
+        RETURN VALUE:
+            Type: bool
+            Description: True is returned if deletion is successful else False
+        
+        ERROR RAISED:
+            Type: General
+            Description: 
+        
+        SAMPLE USE CASES:
+            >>> eq1 = CentrifugalPump()
+            >>> eq1.delete()
+        """
+        result = True
+        if self._inlet_material_stream_index is not None:
+            result = result & self.disconnect_stream(direction='in',
+                                                     stream_tag=self._inlet_material_stream_tag,
+                                                     stream_type='material')
+        if self._outlet_material_stream_index is not None:
+            result = result & self.disconnect_stream(direction='out',
+                                                     stream_tag=self._outlet_material_stream_tag,
+                                                     stream_type='material')
+        if self._inlet_energy_stream_index is not None:
+            result = result & self.disconnect_stream(direction='in',
+                                                     stream_tag=self._inlet_energy_stream_tag,
+                                                     stream_type='energy')
+        if self._outlet_energy_stream_index is not None:
+            result = result & self.disconnect_stream(direction='out',
+                                                     stream_tag=self._outlet_energy_stream_tag,
+                                                     stream_type='energy')
+        del self.items[self.index]
+        del self
+        return result
+
+#Defining generic base class for all equipments with multiple inlet and outlet. TODO !!!!!!       
+class _EquipmentMultipleInletOutlet:
+    def __init__(self) -> None:
+        pass
```

### Comparing `propylean-0.2.5/src/propylean/equipments/exchangers.py` & `propylean-0.2.6/src/propylean/equipments/exchangers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-from propylean.equipments.generic_equipment_classes import _Exchangers
-from propylean import streams
-from propylean import properties as prop
-from propylean.validators import _Validators
-
-# Start of final classes of heat exchangers
-class ShellnTubeExchanger(_Exchangers):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__( **inputs)
-        self._index = len(ShellnTubeExchanger.items)
-        ShellnTubeExchanger.items.append(self)
-    
-    def __repr__(self):
-        return "Shell & Tube Exchanger with tag: " + self.tag   
-    def __hash__(self):
-        return hash(self.__repr__())
-    
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-
-class AirCooler(_Exchangers):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__( **inputs)
-        self.fan_power = prop.Power() if "fan_power" not in inputs else inputs["fan_power"]
-        del self.energy_out
-        self._index = len(AirCooler.items)
-        AirCooler.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Air Cooler with tag: " + self.tag   
-    def __hash__(self):
-        return hash(self.__repr__())
-    
-    @property
-    def temperature_change(self):
-        self = self._get_equipment_object(self)
-        value = -1 * self._temperature_change.value
-        return prop.Temperature(value, self._temperature_change.unit)
-    @temperature_change.setter
-    def temperature_change(self, value):
-        _Validators.validate_arg_prop_value_type("temperature_change", value, (prop.Temperature, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
-        if unit is None:
-            unit = self._temperature_change.unit
-        self._temperature_change = prop.Temperature(-1 * value, unit)
-        self._outlet_temperature =  self._inlet_temperature + self._temperature_change
-        self._update_equipment_object(self)
-
-    @property
-    def fan_power(self):
-        self = self._get_equipment_object(self)
-        return self._fan_power
-    @fan_power.setter
-    def fan_power(self, value):
-        _Validators.validate_arg_prop_value_type("fan_power", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self._fan_power.unit         
-        self._fan_power = prop.Power(value, unit)
-        self._update_equipment_object(self) 
-
-    @property
-    def energy_in(self):
-        return self.fan_power
-    @energy_in.setter
-    def energy_in(self, value):
-        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self.energy_in.unit
-        self._energy_in = prop.Power(value, unit)
-        self._update_equipment_object(self)
-
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-    
-    def connect_stream(self, 
-                       stream_object=None, 
-                       direction=None, 
-                       stream_tag=None, 
-                       stream_type=None,
-                       stream_governed=True):
-        
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'e']):
-            if direction is not None and 'out' in direction:
-                raise Exception('AirCooler only supports fan energy inlet.')
-            direction = 'in'
-            stream_governed = False
-        return super().connect_stream(direction=direction, 
-                                      stream_object=stream_object, 
-                                      stream_tag=stream_tag, 
-                                      stream_type=stream_type,
-                                      stream_governed=stream_governed)
-    
-    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'e']):
-            if direction is not None and 'out' in direction:
-                raise Exception('AirCooler only supports fan energy inlet.')
-            direction = 'in'
-        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
-
-class ElectricHeater(_Exchangers):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__( **inputs)
-        self.power = prop.Power() if "power" not in inputs else inputs["power"]
-        del self.energy_out
-        self._index = len(ElectricHeater.items)
-        ElectricHeater.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Electric Heater with tag: " + self.tag   
-    def __hash__(self):
-        return hash(self.__repr__())
-    
-    def connect_stream(self, 
-                       stream_object=None, 
-                       direction=None, 
-                       stream_tag=None, 
-                       stream_type=None,
-                       stream_governed=True):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'e']):
-            if direction is not None and 'out' in direction:
-                raise Exception('ElectricHeater only supports energy inlet.')
-            direction = 'in'
-            stream_governed = False
-        return super().connect_stream(direction=direction, 
-                                      stream_object=stream_object, 
-                                      stream_tag=stream_tag, 
-                                      stream_type=stream_type,
-                                      stream_governed=stream_governed)
-    
-    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'e']):
-            if direction is not None and 'out' in direction:
-                raise Exception('ElectricHeater only supports energy inlet.')
-            direction = 'in'
-        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
-
-    @property
-    def power(self):
-        self = self._get_equipment_object(self)
-        return self._power
-    @power.setter
-    def power(self, value):
-        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self._power.unit         
-        self._power = prop.Power(value, unit)
-        self._update_equipment_object(self) 
-
-    @property
-    def energy_in(self):
-        return self.power
-    @energy_in.setter
-    def energy_in(self, value):
-        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self.energy_in.unit
-        self._energy_in = prop.Power(value, unit)
-        self._update_equipment_object(self)
-
-    @classmethod
-    def list_objects(cls):
-        return cls.items
+from propylean.equipments.generic_equipment_classes import _Exchangers
+from propylean import streams
+from propylean import properties as prop
+from propylean.validators import _Validators
+
+# Start of final classes of heat exchangers
+class ShellnTubeExchanger(_Exchangers):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__( **inputs)
+        self._index = len(ShellnTubeExchanger.items)
+        ShellnTubeExchanger.items.append(self)
+    
+    def __repr__(self):
+        return "Shell & Tube Exchanger with tag: " + self.tag   
+    def __hash__(self):
+        return hash(self.__repr__())
+    
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+
+class AirCooler(_Exchangers):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__( **inputs)
+        self.fan_power = prop.Power() if "fan_power" not in inputs else inputs["fan_power"]
+        del self.energy_out
+        self._index = len(AirCooler.items)
+        AirCooler.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Air Cooler with tag: " + self.tag   
+    def __hash__(self):
+        return hash(self.__repr__())
+    
+    @property
+    def temperature_change(self):
+        self = self._get_equipment_object(self)
+        value = -1 * self._temperature_change.value
+        return prop.Temperature(value, self._temperature_change.unit)
+    @temperature_change.setter
+    def temperature_change(self, value):
+        _Validators.validate_arg_prop_value_type("temperature_change", value, (prop.Temperature, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Temperature)
+        if unit is None:
+            unit = self._temperature_change.unit
+        self._temperature_change = prop.Temperature(-1 * value, unit)
+        self._outlet_temperature =  self._inlet_temperature + self._temperature_change
+        self._update_equipment_object(self)
+
+    @property
+    def fan_power(self):
+        self = self._get_equipment_object(self)
+        return self._fan_power
+    @fan_power.setter
+    def fan_power(self, value):
+        _Validators.validate_arg_prop_value_type("fan_power", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self._fan_power.unit         
+        self._fan_power = prop.Power(value, unit)
+        self._update_equipment_object(self) 
+
+    @property
+    def energy_in(self):
+        return self.fan_power
+    @energy_in.setter
+    def energy_in(self, value):
+        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self.energy_in.unit
+        self._energy_in = prop.Power(value, unit)
+        self._update_equipment_object(self)
+
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+    
+    def connect_stream(self, 
+                       stream_object=None, 
+                       direction=None, 
+                       stream_tag=None, 
+                       stream_type=None,
+                       stream_governed=True):
+        
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'e']):
+            if direction is not None and 'out' in direction:
+                raise Exception('AirCooler only supports fan energy inlet.')
+            direction = 'in'
+            stream_governed = False
+        return super().connect_stream(direction=direction, 
+                                      stream_object=stream_object, 
+                                      stream_tag=stream_tag, 
+                                      stream_type=stream_type,
+                                      stream_governed=stream_governed)
+    
+    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'e']):
+            if direction is not None and 'out' in direction:
+                raise Exception('AirCooler only supports fan energy inlet.')
+            direction = 'in'
+        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
+
+class ElectricHeater(_Exchangers):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__( **inputs)
+        self.power = prop.Power() if "power" not in inputs else inputs["power"]
+        del self.energy_out
+        self._index = len(ElectricHeater.items)
+        ElectricHeater.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Electric Heater with tag: " + self.tag   
+    def __hash__(self):
+        return hash(self.__repr__())
+    
+    def connect_stream(self, 
+                       stream_object=None, 
+                       direction=None, 
+                       stream_tag=None, 
+                       stream_type=None,
+                       stream_governed=True):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'e']):
+            if direction is not None and 'out' in direction:
+                raise Exception('ElectricHeater only supports energy inlet.')
+            direction = 'in'
+            stream_governed = False
+        return super().connect_stream(direction=direction, 
+                                      stream_object=stream_object, 
+                                      stream_tag=stream_tag, 
+                                      stream_type=stream_type,
+                                      stream_governed=stream_governed)
+    
+    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'e']):
+            if direction is not None and 'out' in direction:
+                raise Exception('ElectricHeater only supports energy inlet.')
+            direction = 'in'
+        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
+
+    @property
+    def power(self):
+        self = self._get_equipment_object(self)
+        return self._power
+    @power.setter
+    def power(self, value):
+        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self._power.unit         
+        self._power = prop.Power(value, unit)
+        self._update_equipment_object(self) 
+
+    @property
+    def energy_in(self):
+        return self.power
+    @energy_in.setter
+    def energy_in(self, value):
+        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self.energy_in.unit
+        self._energy_in = prop.Power(value, unit)
+        self._update_equipment_object(self)
+
+    @classmethod
+    def list_objects(cls):
+        return cls.items
 # End of final classes of heat exchangers
```

### Comparing `propylean-0.2.5/src/propylean/equipments/generic_equipment_classes.py` & `propylean-0.2.6/src/propylean/equipments/generic_equipment_classes.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1067 +1,1067 @@
-from propylean.equipments.abstract_equipment_classes import _EquipmentOneInletOutlet, _EquipmentMultipleInletOutlet
-import propylean.properties as prop
-from propylean.constants import Constants
-from propylean.settings import Settings
-from pandas import DataFrame
-from propylean.validators import _Validators
-from math import pi, sqrt, acos
-import fluids.compressible as compressible_fluid
-from warnings import warn
-
-# Defining generic class for all types of pressure changers like Pumps, Compressors and Expanders.
-class _PressureChangers(_EquipmentOneInletOutlet):
-    def __init__(self,**inputs) -> None:
-        """ 
-            DESCRIPTION:
-                Parent class for all equipment which has primary task to change
-                pressure of a stream. For e.g. Pumps and compressors.
-            
-            PARAMETERS:                
-                pressure_drop or differential_pressure:
-                    Required: No
-                    Type: int/float or Pressure(recommended)
-                    Acceptable values: Non-negative integer
-                    Default value: based on unit    
-                    Description: Pressure drop or differential pressure of the equipment.
-                
-                efficiency:
-                    Required: No
-                    Type: int or float or Efficiency (recommended)
-                    Acceptable values: Non-negative integer
-                    Default value: 1    
-                    Description: Efficiency of the equipment.
-
-                performance_curve:
-                    Required: No
-                    Type: pandas DataFrame
-                    Acceptable values: Non-negative integer in dataframe with flow and head values.
-                    Default value: pandas.DataFrame()    
-                    Description: Performance curve of the pump. 
-                                 E.g. pd.DataFrame([{'flow':[2, 10, 30, 67], 'head':[45, 20, 10, 2]}]) 
-
-            RETURN VALUE:
-                Type: _PressureChangers
-                Description: object with all _EquipmentOneInletOutlet and other pressure changer properties.
-            
-            ERROR RAISED:
-                Type:
-                Description: 
-            
-            SAMPLE USE CASES:
-                >>>  class AwesomeCompressor(_PressureChangers):
-                >>>     def __init__(**kwargs):
-                >>>         some_property = 20
-                
-        """
-        
-        if 'pressure_drop' in inputs:
-            inputs['differential_pressure'] = -1 * inputs['pressure_drop']
-            del inputs['pressure_drop']
-        
-        super().__init__(**inputs)
-        
-        if 'differential_pressure' in inputs:
-            if ((self._inlet_pressure != None or self._outlet_pressure != None) and
-                 'performance_curve' in inputs):
-                 raise Exception('Input only one of differential pressure or performance_curve.')
-            diff_presure = inputs['differential_pressure'] 
-            if isinstance(diff_presure, prop.Pressure):
-                self._pressure_drop = prop.Pressure(-1 * diff_presure.value,
-                                                    diff_presure.unit)
-            elif isinstance(diff_presure, tuple):
-                self._pressure_drop = prop.Pressure(-1 * diff_presure[0],
-                                                     diff_presure[1])
-                 
-        self._performance_curve = DataFrame()
-        if 'performance_curve' in inputs:
-            self.performace_curve = inputs['performance_curve']
-        
-        self.efficiency = 1 if 'efficiency' not in inputs else inputs['efficiency']
-        
-    @property
-    def suction_pressure(self):
-        return super(_PressureChangers, self).inlet_pressure
-    @suction_pressure.setter
-    def suction_pressure(self, value):
-        super(_PressureChangers, self.__class__).inlet_pressure.fset(self, value)
-
-    @property
-    def discharge_pressure(self):
-        return super(_PressureChangers, self).outlet_pressure
-    @discharge_pressure.setter
-    def discharge_pressure(self, value):
-        super(_PressureChangers,self.__class__).outlet_pressure.fset(self, value)
-    
-    @property
-    def differential_pressure(self):
-        return prop.Pressure(-1 * self.pressure_drop.value,
-                             self.pressure_drop.unit)
-    @differential_pressure.setter
-    def differential_pressure(self, value):
-        _Validators.validate_arg_prop_value_type("differential_pressure", value, (prop.Pressure, int, float, tuple))
-        _Validators.validate_non_negative_value("differential_pressure", value)
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
-        if unit is None:
-            unit = self.pressure_drop.unit         
-        self.pressure_drop = prop.Pressure(-1 * value,
-                                           unit)   
-        self._update_equipment_object(self)   
-    
-    @property
-    def performance_curve(self):
-        self = self._get_equipment_object(self)
-        return self._perfomace_curve
-    @performance_curve.setter
-    def performance_curve(self,value):
-        _Validators.validate_arg_prop_value_type("performance_curve", value, DataFrame)
-        self = self._get_equipment_object(self)
-        if value.shape[1] == 2:
-                self._performance_curve = value
-        else:
-            raise Exception("Enter performance_curve as pandas dataframe of 2 columns.\nOne for Flow and other for head.")
-        self._update_equipment_object(self)
-    
-    @property
-    def efficiency(self):
-        self = self._get_equipment_object(self)
-        return self._efficiency
-    @efficiency.setter
-    def efficiency(self, value):
-        _Validators.validate_arg_prop_value_type("efficiency", value, (int, float, prop.Efficiency))
-        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
-        self = self._get_equipment_object(self)
-        if value <= 0:
-            raise Exception("Provide a positive value for efficiency.")
-        elif value <= 1:
-            self._efficiency = prop.Efficiency(value)
-        else:
-            self._efficiency = prop.Efficiency(value/100)
-            warn("Efficiency set to {} considering value provided in percent.".format(value/100))
-        self._update_equipment_object(self)
-    
-    @property
-    def power(self):
-        self = self._get_equipment_object(self)
-        return self._power
-    @power.setter
-    def power(self, value):
-        _Validators.validate_arg_prop_value_type("power", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self._power.unit         
-        self._power = prop.Power(value, unit)
-        self._update_equipment_object(self)  
-
-# Defining generic class for Compressors and Expanders.
-class _GasPressureChangers(_PressureChangers):
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Class for creating objects to represent a GasPressureChanger.
-        
-        PARAMETERS:
-            Read _PressureChangers class for more arguments for this class  
-            efficiency:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative values
-                Default value: 1.4
-                Description: Efficiency of the compressor. Efficiency can be set as
-                             adiabatic/isentropic or polytropic efficiency.
-            
-            adiabatic_efficiency:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative values
-                Default value: 0.7
-                Description: Efficiency of the compressor considering adiabatic/isentropic
-                             compression.
-            
-            polytropic_efficiency:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative values
-                Default value: 0.7
-                Description: Efficiency of the compressor considering polytropic
-                             compression.
-
-            polytropic_exponent:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative values
-                Default value: 1.4
-                Description: Polytropic exponent of the gas.
-        
-        PROPERTIES:
-            power:
-                Type: Power
-                Description: Power required by the compressor.
-
-        
-        RETURN VALUE:
-            Type: CentrifugalCompressor
-            Description: Returns an object of type CentrifugalCompressor with all properties of
-                         a Centrifugal Compressor used in process industries.
-        
-        ERROR RAISED:
-            Type:
-            Description:
-        
-        SAMPLE USE CASES:
-            >>> CC_1 = CentrifugalCompressor(tag="P1")
-            >>> print(CC_1)
-            Centrifugal Compressor with tag: P1
-        """
-        super().__init__( **inputs)
-        self.adiabatic_efficiency = 0.7 if 'efficiency' not in inputs else inputs['efficiency']
-        self.polytropic_exponent = 1.4 if 'polytropic_exponent' not in inputs else inputs['polytropic_exponent']
-        
-    @property
-    def temperature_change(self):
-        self = self._get_equipment_object(self)
-        k = self.polytropic_exponent
-        if (self._inlet_material_stream_index is not None or
-            self._outlet_material_stream_index is not None):
-            is_inlet = False if self._inlet_material_stream_index is None else True
-            k = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
-            if Settings.compression_process.lower() == "polytropic":
-                k = compressible_fluid.polytropic_exponent(k=k, eta_p=self.polytropic_efficiency)
-
-        T1 = self.inlet_temperature
-        P1 = self.inlet_pressure
-        P2 = self.outlet_pressure
-        T1.unit = "K"
-        P1.unit = P2.unit ="Pa"
-        eta = self.efficiency.value
-        value = prop.Temperature(compressible_fluid.isentropic_T_rise_compression(T1.value, P1.value, P2.value, k, eta))
-        value = value - T1
-        value.unit = self.inlet_temperature.unit
-        return value
-
-    @property
-    def efficiency(self):
-        self = self._get_equipment_object(self)
-        if Settings.compression_process.lower() == "polytropic":
-            return self.polytropic_efficiency
-        else:
-            return self.adiabatic_efficiency
-    @efficiency.setter
-    def efficiency(self, value):
-        _Validators.validate_arg_prop_value_type("efficiency", value, (int, float, prop.Efficiency))
-        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
-        self = self._get_equipment_object(self)
-        if value < 0:
-            raise Exception("Provide a positive value for efficiency.")
-        elif value <= 1:
-            value = value
-        else:
-            value = value/100
-        if Settings.compression_process.lower() in ["adiabatic", "isentropic"]:
-            self.adiabatic_efficiency = value
-        else:
-            self.polytropic_efficiency = value
-            
-        self._efficiency = value
-
-    @property
-    def adiabatic_efficiency(self):
-        self = self._get_equipment_object(self)
-        return self._adiabatic_efficiency
-    @adiabatic_efficiency.setter
-    def adiabatic_efficiency(self, value):
-        _Validators.validate_arg_prop_value_type("adiabatic_efficiency", value, (int, float, prop.Efficiency))
-        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
-        self = self._get_equipment_object(self)
-        if value == None:
-            value = 0.7
-        self._adiabatic_efficiency = prop.Efficiency(value)
-        self._update_equipment_object(self)
-    
-    @property
-    def polytropic_efficiency(self):
-        self = self._get_equipment_object(self)
-        if (self._inlet_material_stream_index is not None or
-            self._outlet_material_stream_index is not None):
-            is_inlet = False if self._inlet_material_stream_index is None else True
-            isentropic_exponent = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
-            pol_eff = compressible_fluid.isentropic_efficiency(P1 = self._inlet_pressure.value,
-                                                            P2 = self._outlet_pressure.value,
-                                                            k = isentropic_exponent,
-                                                            eta_s = self.adiabatic_efficiency.value)
-            return prop.Efficiency(pol_eff)
-        else:
-            return self.efficiency
-    @polytropic_efficiency.setter
-    def polytropic_efficiency(self, value):
-        _Validators.validate_arg_prop_value_type("polytropic_efficiency", value, (int, float, prop.Efficiency))
-        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
-        self = self._get_equipment_object(self)
-        is_inlet = False if self._intlet_material_stream_index is None else True
-        isentropic_exponent = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
-        self.adiabatic_efficiency = compressible_fluid.isentropic_efficiency(P1 = self._inlet_pressure.value,
-                                                                             P2 = self._outlet_pressure.value,
-                                                                             k = isentropic_exponent,
-                                                                             eta_p = value)
-        self._update_equipment_object(self)
-    
-    @property
-    def polytropic_exponent(self):
-        self = self._get_equipment_object(self)
-        if (self._inlet_material_stream_index is None and
-            self._outlet_material_stream_index is None):
-            return self._polytropic_exponent
-        is_inlet = False if self._inlet_material_stream_index is None else True
-        k = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
-        return compressible_fluid.polytropic_exponent(k=k, eta_p=self.polytropic_efficiency.value)
-    @polytropic_exponent.setter
-    def polytropic_exponent(self, value):
-        _Validators.validate_arg_prop_value_type("polytropic_exponent", value, (int, float))
-        self = self._get_equipment_object(self)
-        if (self._inlet_material_stream_index is None and
-            self._outlet_material_stream_index is None):
-            self._polytropic_exponent = value
-        else:
-            raise Exception("""Polytropic Exponent cannot be set as Compressor is connected to a MaterialStream object.\n
-                               Update Isentropic Exponent of the stream object instead.""")
-
-    @property
-    def power(self):
-        self = self._get_equipment_object(self)
-        is_inlet = False if self._inlet_material_stream_index is None else True
-        isentropic_exponent = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
-        Z = self._connected_stream_property_getter(is_inlet, "material", "Z_g")
-        MW = self._connected_stream_property_getter(is_inlet, "material", "molecular_weight")
-        work = compressible_fluid.isentropic_work_compression(T1 = self.inlet_temperature.value,
-                                                              k = isentropic_exponent,
-                                                              Z = Z,
-                                                              P1 = self._inlet_pressure.value,
-                                                              P2 = self._outlet_pressure.value,
-                                                              eta = self.adiabatic_efficiency.value)
-        return prop.Power(work * self.inlet_mass_flowrate.value / MW.value)
-    
-    @property
-    def head(self):
-        if (self._inlet_material_stream_index is None or
-            self._outlet_material_stream_index is None):
-            raise Exception("Head calculations only supported when Compressor is connected to a MaterialStream object.")
-        if Settings.compression_process.lower() in ["adiabatic", "isentropic"]:
-            isentropic_exponent = self._connected_stream_property_getter(True, "material", "isentropic_exponent")
-            ratio = (isentropic_exponent - 1)/isentropic_exponent
-        else:
-            ratio = (self.polytropic_exponent - 1)/self.polytropic_exponent
-        
-        P1 = self.inlet_pressure
-        P2 = self.outlet_pressure
-        P1.unit = "Pa"
-        P2.unit = "Pa"
-        Zi = self._connected_stream_property_getter(True, "material", "Z_g")
-        Zo = self._connected_stream_property_getter(False, "material", "Z_g")
-        Z = (Zi + Zo)/2
-        T1 = self.inlet_temperature
-        T1.unit = "K"
-        MW = self._connected_stream_property_getter(True, "material", "molecular_weight")
-        head = Z * Constants.R * T1.value * (pow((P2.value/P1.value), ratio) - 1)/(ratio * MW.value)
-        head_max_value = Z * Constants.R * T1.max_val * (pow((P2.max_val/P1.min_val), ratio) - 1)/(ratio * MW.value)
-        head_min_value = Z * Constants.R * T1.min_val * (pow((P2.min_val/P1.max_val), ratio) - 1)/(ratio * MW.value)
-        return prop.Length(head, max_val=head_max_value, min_val=head_min_value)
-        
-    
-#Defining generic class for all types of vessels. 
-class _Vessels(_EquipmentOneInletOutlet):
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Parent class for all equipment which has primary task to be a vessel
-            of a stream. For e.g. Tanks and reactors.
-        
-        PARAMETERS:
-            ID:
-                Required: No
-                Type: int or float or Length(recommended)
-                Acceptable values: Non-negative integer
-                Default value: 0 m   
-                Description: Internal diameter of the vessel.
-            
-            OD:
-                Required: No
-                Type: int or float or Length(recommended)
-                Acceptable values: Non-negative integer
-                Default value: 0 m    
-                Description: Outer diameter of the vessel.
-
-            thickness:
-                Required: No
-                Type: int or float or Length(recommended)
-                Acceptable values: Non-negative integer
-                Default value: 0 m    
-                Description: thickness of the vessel.
-            
-            length:
-                Required: No
-                Type: int or float or Length(recommended)
-                Acceptable values: Non-negative integer
-                Default value: 0 m   
-                Description: tan-line length of the vessel.
-            
-            LLL, LLLL, HLL, NLL and HHLL:
-                Required: No
-                Type: int or float or Length(recommended)
-                Acceptable values: Non-negative integer
-                Default value: 0 m    
-                Description: Low Liquid Level(LLL), Low-Low Liquid Level(LLLL), High Liquid Level(HLL),
-                             Normal Liquid Level(NLL), and High-high Liquid Level.
-            
-            head_type:
-                Required: No
-                Type: String
-                Acceptable values: {head_types}
-                Default value: elliptical    
-                Description: Type of head for the vessel.
-            
-            main_fluid:
-                Required: No
-                Type: String
-                Acceptable values: ["liquid", "gas"]
-                Default value: liquid    
-                Description: Type of fluid which the vessel stores.
-            
-            is_blanketed:
-                Required: No
-                Type: Boolean
-                Default value: False
-                Description: Specifies if the vessel is blanketed or not.
-            
-        RETURN VALUE:
-            Type: _Vessels
-            Description: object with all _EquipmentOneInletOutlet and other vessel related properties.
-        
-        PROPERTIES:
-            operating_pressure:
-                Type: int or float or Pressure(recommended)  
-                Acceptable values: Any
-                Default value: 101325 Pa  
-                Description: Operating pressure of the vessel. operating_pressure is
-                             considered equal to outlet_pressure and can be considered as
-                             alias of each other. Setting or getting one effects the other.
-            
-            operating_temperature:
-                Type: int or float or Pressure(recommended)   
-                Acceptable values: Any
-                Default value: 298 K 
-                Description: Operating temperature of the vessel. operating_temperature is
-                             considered equal to outlet_temperature and can be considered as
-                             alias of each other. Setting or getting one effects the other.
-
-            vessel_volume:
-                Type: int or float or Volume(recommended)   
-                Acceptable values: Any
-                Default value: 0 m^3 
-                Description:Total volumetric space of the vessel including heads.
-            
-            liquid_level:
-                Type: int or float or Length(recommended)
-                Acceptable values: Non-negative integer
-                Default value: 0 m   
-                Description: liquid level of the vessel.
-            
-        METHODS:
-            get_inventory(type="volume")
-            DESCRIPTION:
-                Function to get the inventory in the vessel.
-        
-            PARAMETERS:
-                type:
-                    Type: String
-                    Acceptable values: "volume" or "mass"
-                    Default value: "volume"  
-                    Description: The type of inventory to be calculated.
-                                 "volume" calculates volumetic inventroy and
-                                 "mass" calculates mass inventory of corresponding
-                                  volumetic inventory based on density of liquid.
-                                  Property main_fluid should be set for vessesl 
-                                  containging liquid.
-                                        
-        ERROR RAISED:
-            Type:
-            Description: 
-        
-        SAMPLE USE CASES:
-            >>>  class AwesomeReactor(_Vessels):
-            >>>     def __init__(**kwargs):
-            >>>         some_property = 20
-                
-    """.format(head_types=Constants.HEAD_TYPES)
-        super().__init__(**inputs)
-        self._ID = prop.Length()
-        self._OD = prop.Length()
-        self._length = prop.Length()
-        self._LLLL = prop.Length()
-        self._LLL = prop.Length()
-        self._NLL = prop.Length()
-        self._HLL = prop.Length()
-        self._HHLL = prop.Length()
-        self.blanketing = None
-        self._material = 1
-        self.operating_pressure = prop.Pressure()
-        self.operating_temperature = prop.Temperature()
-        if ('ID' in inputs and inputs['ID'] is not None):
-                self.ID = inputs['ID']
-                if 'OD' in inputs and inputs['OD'] is not None:
-                    self.OD = inputs['OD']
-                elif 'thickness' in inputs and inputs['thickness'] is not None:
-                    self.thickness = inputs['thickness']
-                else:
-                    self.thickness = self.calculate_thickness()
-                
-        elif ('OD' in inputs and 'thickness' in inputs):
-            self.OD = inputs['OD']
-            self.ID = inputs['thickness']
-            self.ID = self.OD - self.ID
-        
-        self.length = prop.Length() if 'length' not in inputs else inputs['length']
-        
-        self.LLLL = prop.Length() if 'LLLL' not in inputs else inputs['LLLL']
-        self.LLL = prop.Length() if 'LLL' not in inputs else inputs['LLL']
-        self.NLL = prop.Length() if 'NLL' not in inputs else inputs['NLL']
-        self.liquid_level = prop.Length() if 'NLL' not in inputs else inputs['NLL']
-        self.HLL = prop.Length() if 'HLL' not in inputs else inputs['HLL']
-        self.HHLL = prop.Length() if 'HHLL' not in inputs else inputs['HHLL']
-
-        if "head_type" not in inputs:
-            self._head_type = "torispherical"  
-        else:
-            _Validators.validate_arg_prop_value_type("head_type", inputs["head_type"], str)
-            _Validators.validate_arg_prop_value_list("head_type", inputs["head_type"], Constants.HEAD_TYPES)
-            self._head_type = inputs["head_type"]
-        
-        if "is_blanketed" in inputs and inputs["is_blanketed"]:
-            self.blanketing = _Blanketing(tag=self.tag)
-            self.blanketing.inlet_pressure = self.operating_pressure
-
-    @property
-    def ID(self):
-        self = self._get_equipment_object(self)
-        return self._ID
-    @ID.setter
-    def ID(self, value):
-        _Validators.validate_arg_prop_value_type("ID", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._ID.unit
-        self._ID = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    
-    @property
-    def OD(self):
-        self = self._get_equipment_object(self)
-        return self._OD
-    @OD.setter
-    def OD(self, value):
-        _Validators.validate_arg_prop_value_type("OD", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._OD.unit
-        self._OD =prop.Length(value, unit)
-        self._update_equipment_object(self)
-
-    @property
-    def thickness(self):
-        self = self._get_equipment_object(self)
-        # if self._OD - self._ID <= prop.Length(0):
-        #     raise Exception("ID is not less than OD! Change ID or OD or thickness.")
-        return self._OD - self._ID
-    @thickness.setter
-    def thickness(self, value):
-        _Validators.validate_arg_prop_value_type("thickness", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self.thickness
-        self._OD = self._ID + prop.Length(value, unit)
-        self._update_equipment_object(self)
-    
-    def calculate_thickness(self):
-        #TODO: Update calculations based on design pressure.
-        return prop.Length(0.01)
-
-    @property
-    def length(self):
-        self = self._get_equipment_object(self)
-        return self._length
-    @length.setter
-    def length(self, value):
-        _Validators.validate_arg_prop_value_type("length", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._length.unit
-        self._length = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @length.deleter
-    def length(self):
-        self = self._get_equipment_object(self)
-        del self._length
-        self._update_equipment_object(self)
-    
-    @property
-    def LLLL(self):
-        self = self._get_equipment_object(self)
-        return self._LLLL
-    @LLLL.setter
-    def LLLL(self, value):
-        _Validators.validate_arg_prop_value_type("LLLL", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._LLLL.unit
-        self._LLLL = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @LLLL.deleter
-    def LLLL(self):
-        self = self._get_equipment_object(self)
-        del self._LLLL
-        self._update_equipment_object(self)
-
-    @property
-    def LLL(self):
-        self = self._get_equipment_object(self)
-        return self._LLL
-    @LLL.setter
-    def LLL(self, value):
-        _Validators.validate_arg_prop_value_type("LLL", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._LLL.unit
-        self._LLL = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @LLL.deleter
-    def LLL(self):
-        self = self._get_equipment_object(self)
-        del self._LLL
-        self._update_equipment_object(self)
-
-    @property
-    def NLL(self):
-        self = self._get_equipment_object(self)
-        return self._NLL
-    @NLL.setter
-    def NLL(self, value):
-        _Validators.validate_arg_prop_value_type("NLL", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._NLL.unit
-        self._NLL = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @NLL.deleter
-    def NLL(self):
-        self = self._get_equipment_object(self)
-        del self._NLL
-        self._update_equipment_object(self)
-
-    @property
-    def HLL(self):
-        self = self._get_equipment_object(self)
-        return self._HLL
-    @HLL.setter
-    def HLL(self, value):
-        _Validators.validate_arg_prop_value_type("HLL", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._HLL.unit
-        self._HLL = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @HLL.deleter
-    def HLL(self):
-        self = self._get_equipment_object(self)
-        del self._HLL
-        self._update_equipment_object(self)
-
-    @property
-    def HHLL(self):
-        self = self._get_equipment_object(self)
-        return self._HHLL
-    @HHLL.setter
-    def HHLL(self, value):
-        _Validators.validate_arg_prop_value_type("HHLL", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._HHLL.unit
-        self._HHLL = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @HHLL.deleter
-    def HHLL(self):
-        self = self._get_equipment_object(self)
-        del self._HHLL
-        self._update_equipment_object(self)
-
-    @property
-    def head_type(self):
-        self = self._get_equipment_object(self)
-        return self._head_type
-    @head_type.setter
-    def head_type(self, value):
-        _Validators.validate_arg_prop_value_type("head_type", value, str)
-        _Validators.validate_arg_prop_value_list("head_type", value, Constants.HEAD_TYPES)
-        self = self._get_equipment_object(self)
-        if value not in Constants.HEAD_TYPES:
-            raise Exception("""Head type '{0}', not supported. Supported types are:\n
-            {1}""".format(value, Constants.HEAD_TYPES))
-        self._head_type = value
-        self._update_equipment_object(self)
-    @head_type.deleter
-    def head_type(self):
-        self = self._get_equipment_object(self)
-        del self._head_type
-        self._update_equipment_object(self)
-
-    @property
-    def material(self):
-        self = self._get_equipment_object(self)
-        return self._material
-    @material.setter
-    def material(self, value):
-        _Validators.validate_arg_prop_value_type("material", value, int)
-        _Validators.validate_arg_prop_value_range("head_type", value, [1, 4])
-        self = self._get_equipment_object(self)
-        materials = '''\nSegment material can be of following types and in range of numbers below:
-                    1. Raw Steel
-                    2. Carbon Steel
-                    3. Cast Iron
-                    4. Stainless Steel
-                    ''' 
-        if value not in range(1, 6):
-            raise Exception(materials)
-        self._material = value
-        self._update_equipment_object(self)
-
-    @property
-    def main_fluid(self):
-        self = self._get_equipment_object(self)
-        return self._main_fluid
-    @main_fluid.setter
-    def main_fluid(self, value):
-        _Validators.validate_arg_prop_value_type("main_fluid", value, str)
-        _Validators.validate_arg_prop_value_list("main_fluid", value, ("liquid", "gas"))
-        self = self._get_equipment_object(self)
-        self._main_fluid = value
-        self._update_equipment_object(self)
-
-    @property
-    def pressure_drop(self):
-        g = Constants.g
-        self = self._get_equipment_object(self)
-        if ((self._inlet_energy_stream_index is not None or
-             self._outlet_energy_stream_index is not None) and 
-             self.main_fluid == "liquid"):
-            is_inlet = False if self._inlet_material_stream_index is None else True
-            density = self._connected_stream_property_getter(is_inlet, "material", "density")
-            density.unit = "kg/m^3"
-            pd = density.value * g * self.liquid_level.value
-            pd_min = density.min_value * g * self.liquid_level.min_val
-            pd_max = density.max_value * g * self.liquid_level.max_val
-            return prop.Pressure(value=pd, min_val=pd_min, max_val=pd_max)
-        return self._pressure_drop
-    @pressure_drop.setter
-    def pressure_drop(self, value):
-        _Validators.validate_arg_prop_value_type("pressure_drop", value, (prop.Pressure, int, float, tuple))
-        if ((self._inlet_energy_stream_index is not None or
-             self._outlet_energy_stream_index is not None) and 
-             self.main_fluid == "liquid"):
-            raise Exception("Pressure drop cannot be set for vessels with main fluid as liquid.")
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
-        if unit is None:
-            unit = self._pressure_drop.unit
-        self._pressure_drop = prop.Pressure(value, unit)
-        self._outlet_pressure =  self._inlet_pressure - self._pressure_drop
-        self._update_equipment_object(self)
-               
-    @property
-    def operating_pressure(self):
-        return self.inlet_pressure
-    @operating_pressure.setter
-    def operating_pressure(self, value):
-        _Validators.validate_arg_prop_value_type("operating_pressure", value, (prop.Pressure, int, float, tuple))
-        self.inlet_pressure = value
-        if self.blanketing is not None:
-            self.blanketing.inlet_pressure = value
-    
-    @property
-    def operating_temperature(self):
-        return self.inlet_temperature
-    @operating_temperature.setter
-    def operating_temperature(self, value):
-        _Validators.validate_arg_prop_value_type("operating_temperature", value, (prop.Temperature, int, float, tuple))
-        self.inlet_temperature = value
-        if self.blanketing is not None:
-            self.blanketing.inlet_temperature = value
-    
-    @property
-    def vessel_volume(self):
-        D = self.ID.value
-        L = self.length.value
-        t = self.thickness.value
-        cylinder_volume = pi * D * D * L / 4
-        # Volume of both heads.
-        head_volume = 0
-        if self.head_type == "hemispherical":
-            # Spherical heads are not exact sphere but part of it.
-            # Dish depth = D/2
-            head_volume = pi * (D ** 3) / 6 
-        elif self.head_type == "elliptical":
-            # Dish depth = D/4
-            head_volume = pi * (D ** 3) / 12
-        elif self.head_type == "torispherical":
-            Rc = D + t
-            Rk = 3 * t
-            z = Rc - sqrt((Rc - Rk)**2 - (self.OD.value/2 - t - Rk)**2)
-            head_volume = 0.9 * 4 * pi * Rc * Rc * z / 3 
-        return prop.Volume(cylinder_volume + head_volume, "m^3")
-
-    @property
-    def liquid_level(self):
-        self = self._get_equipment_object(self)
-        return self._liquid_level
-    @liquid_level.setter
-    def liquid_level(self, value):
-        _Validators.validate_arg_prop_value_type("liquid_level", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._liquid_level.unit
-        self._liquid_level = prop.Length(value, unit)
-        self._update_equipment_object(self)
-
-    def get_inventory(self, type="volume"):
-        _Validators.validate_arg_prop_value_type("type", type, str)
-        _Validators.validate_arg_prop_value_list("type", type, ["volume", "mass"])
-        self = self._get_equipment_object(self)
-        if self.main_fluid == "gas":
-            if type == "volume":
-                liquid_volume = self._get_liquid_volume()
-                gas_volume = self.vessel_volume - liquid_volume
-                return gas_volume 
-            else:
-                is_inlet = False if self._inlet_material_stream_index is None else True
-                density = self._connected_stream_property_getter(is_inlet, "material", "density_g")
-                return prop.Mass(self.inventory().value * density) 
-        else:
-            if type == "volume":
-                return self._get_liquid_volume()
-            else:
-                is_inlet = False if self._inlet_material_stream_index is None else True
-                density = self._connected_stream_property_getter(is_inlet, "material", "density_l")
-                mass = self._get_liquid_volume().value * density.value
-    
-class _VerticalVessels(_Vessels):
-    def __init__(self, **inputs) -> None:
-        super().__init__(**inputs)
-    
-    def _get_head_volume(self):
-        head_volume = 0
-        D = self.ID.value
-        if self.head_type == "hemispherical":
-            # Dish depth = D/2
-            head_volume = pi * (D ** 3) / 12
-        elif self.head_type == "elliptical":
-            # Dish depth = D/4
-            head_volume = pi * (D ** 3) / 24
-        elif self.head_type == "torispherical":
-            Rc = (self.ID + self.thickness).value
-            Rk = 3 * self.thickness.value
-            z = Rc - sqrt((Rc - Rk)**2 - (self.OD.value/2 - self.thickness.value - Rk)**2)
-            head_volume = 0.9 * 4 * pi * Rc * Rc * z / 3
-        return prop.Volume(head_volume) 
-
-    def _get_cylinder_volume(self):
-        volume = pi * self.ID.value**2 * self.liquid_level.value / 4
-        return prop.Volume(volume)
-    
-    def _get_liquid_volume(self):
-        head_volume = self._get_head_volume()
-        cylinder_volume = self._get_cylinder_volume()
-        return cylinder_volume + head_volume
-
-class _HorizontalVessels(_Vessels):
-    def __init__(self, **inputs) -> None:
-        super().__init__(**inputs)
-    
-    def _get_head_volume(self):
-        self = self._get_equipment_object(self)
-        C = 0
-        if self.head_type == "hemispherical":
-            C = 1
-        elif self.head_type == "elliptical":
-            C = 0.5
-        elif self.head_type == "torispherical":
-            Rk = 3 * self.thickness.value
-            t_by_Dext = self.thickness/self.OD
-            C = 0.30939 + 1.7197 * (Rk - 0.06 * self.OD.value)/self.ID.value - 0.16116 * t_by_Dext + 0.98997 * t_by_Dext**2
-        head_volume = self._get_head_volume_by_type(C)
-        return prop.Volume(head_volume) 
-    
-    def _get_head_volume_by_type(self, C):
-        head_volume = (self.ID.value ** 3) * pi 
-        H_by_ID = self.liquid_level / self.ID
-        head_volume *= 3 * H_by_ID**2 - 2 * H_by_ID**3
-        head_volume /= 12
-        head_volume *= C
-        return head_volume
-
-    def _get_cylinder_volume(self):
-        self = self._get_equipment_object(self)
-        volume = 0
-        # alpha = cos-1(1-H/R)
-        R = self.ID.value / 2
-        H = self.liquid_level.value
-        L = self.length.value
-        radians = 1 - H / R
-        alpha = acos(radians)
-        volume = L * ((R ** 2) * alpha - (R - H) * sqrt(2*R*H - H*H))
-        return prop.Volume(volume)
-    
-    def _get_liquid_volume(self):
-        head_volume = self._get_head_volume()
-        cylinder_volume = self._get_cylinder_volume()
-        return cylinder_volume + head_volume + head_volume
-
-class _SphericalVessels(_Vessels):
-    def __init__(self, **inputs) -> None:
-        super().__init__(**inputs)
-        del self.head_type
-        del self.length
-    
-    @property
-    def vessel_volume(self):
-        self = self._get_equipment_object(self)
-        D = self.ID.value
-        volume = 2 * self._get_hemisphere_volume(D, D/2)
-        return prop.Volume(volume)
-    def _get_liquid_volume(self):
-        self = self._get_equipment_object(self)
-        H = self.liquid_level.value
-        D = self.ID.value
-        if H <= D/2:
-            volume = self._get_hemisphere_volume(D, H)
-        else:
-            volume = self._get_hemisphere_volume(D, D/2)
-            volume -=  self._get_hemisphere_volume(D, H)
-        return prop.Volume(volume)
-    
-    def _get_hemisphere_volume(self, D, H):
-        return pi * H**2 *(1.5 * D - H) / 3
-
-class _Blanketing(_EquipmentOneInletOutlet):
-    def __init__(self, **inputs) -> None:
-        inputs["tag"] += "_blanketing" 
-        super().__init__(**inputs)
-        del self.energy_in
-        del self.energy_out
-    
-    def __repr__(self):
-        return "Blanketing with tag: " + self.tag
-    @property
-    def pressure_drop(self):
-        return prop.Pressure(0)
-    @pressure_drop.setter
-    def pressure_drop(self, value):
-        raise Exception("Pressure drop setting for blanketing is not allowed as it is an intermittent process.")
-    
-    @property
-    def temperature_increase(self):
-        return prop.Temperature(0, "K")
-    @temperature_increase.setter
-    def temperature_increase(self, value):
-        raise Exception("Temperature increase setting for blanketing is not allowed as it is an intermittent process.")
-        
-    @property
-    def temperature_decrease(self):
-        return prop.Temperature(0, "K")
-    @temperature_decrease.setter
-    def temperature_decrease(self, value):
-        raise Exception("Temperature decrease setting for blanketing is not allowed as it is an intermittent process.")
-        
-
-#Defining generic class for all types of heat exchangers NEEDS SUPER CLASS WITH MULTI INPUT AND OUTPUT
-class _Exchangers(_EquipmentOneInletOutlet):
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Parent class for all equipment which has primary task to be an 
-            Temperature changer of a stream. For e.g. Heater and Cooler.
-        
-        PARAMETERS:
-            temperature_decrease:
-                Required: No
-                    Type: int/float or Temperature(recommended)
-                    Acceptable values: Non-negative integer
-                    Default value: based on unit    
-                    Description: Temperature decrease of stream in the equipment.
-                                 That is decrease from inlet stream to outlet stream.
-            
-            temperature_increase:
-                Required: No
-                    Type: int/float or Temperature(recommended)
-                    Acceptable values: Non-negative integer
-                    Default value: based on unit    
-                    Description: Temperature increase of stream in the equipment.
-                                 That is increase from inlet stream to outlet stream.
-                
-            efficiency:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative integer
-                Default value: based on unit    
-                Description: Efficiency of the equipment.
-
-        RETURN VALUE:
-            Type: _Exchangers
-            Description: object with all _EquipmentOneInletOutlet and other exchanger related properties.
-        
-        ERROR RAISED:
-            Type:
-            Description: 
-        
-        SAMPLE USE CASES:
-            >>>  class AwesomeNewExchanger(_Exchangers):
-            >>>     def __init__(**kwargs):
-            >>>         some_property = 20 
-        """
-        super().__init__(**inputs)
-        if ("temperature_increase" not in inputs and
-            "temperature_decrease" not in inputs):
-            self.temperature_increase = prop.Temperature(0, 'K')
-        elif "temperature_increase" in inputs:
-            self.temperature_increase = inputs["temperature_increase"]
-        else:
-            self.temperature_decrease = inputs["temperature_decrease"] 
-        if "energy_in" in inputs:
-            self.energy_in = inputs["energy_in"]
-        if "energy_out" in inputs:
-            self.energy_out = inputs["energy_out"]
-        self._efficiency = 100 if 'efficiency' not in inputs else inputs['efficiency']
-        
-    @property
-    def efficiency(self):
-        self = self._get_equipment_object(self)
-        return self._efficiency
-    @efficiency.setter
-    def efficiency(self, value):
-        _Validators.validate_arg_prop_value_type("efficiency", value, (int, float, prop.Efficiency))
-        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
-        self = self._get_equipment_object(self)
-        if value < 0:
-            raise Exception("Provide a positive value for efficiency.")
-        elif value <= 1:
-            self._efficiency = prop.Efficiency(value)
-        else:
-            self._efficiency = prop.Efficiency(value/100)
+from propylean.equipments.abstract_equipment_classes import _EquipmentOneInletOutlet, _EquipmentMultipleInletOutlet
+import propylean.properties as prop
+from propylean.constants import Constants
+from propylean.settings import Settings
+from pandas import DataFrame
+from propylean.validators import _Validators
+from math import pi, sqrt, acos
+import fluids.compressible as compressible_fluid
+from warnings import warn
+
+# Defining generic class for all types of pressure changers like Pumps, Compressors and Expanders.
+class _PressureChangers(_EquipmentOneInletOutlet):
+    def __init__(self,**inputs) -> None:
+        """ 
+            DESCRIPTION:
+                Parent class for all equipment which has primary task to change
+                pressure of a stream. For e.g. Pumps and compressors.
+            
+            PARAMETERS:                
+                pressure_drop or differential_pressure:
+                    Required: No
+                    Type: int/float or Pressure(recommended)
+                    Acceptable values: Non-negative integer
+                    Default value: based on unit    
+                    Description: Pressure drop or differential pressure of the equipment.
+                
+                efficiency:
+                    Required: No
+                    Type: int or float or Efficiency (recommended)
+                    Acceptable values: Non-negative integer
+                    Default value: 1    
+                    Description: Efficiency of the equipment.
+
+                performance_curve:
+                    Required: No
+                    Type: pandas DataFrame
+                    Acceptable values: Non-negative integer in dataframe with flow and head values.
+                    Default value: pandas.DataFrame()    
+                    Description: Performance curve of the pump. 
+                                 E.g. pd.DataFrame([{'flow':[2, 10, 30, 67], 'head':[45, 20, 10, 2]}]) 
+
+            RETURN VALUE:
+                Type: _PressureChangers
+                Description: object with all _EquipmentOneInletOutlet and other pressure changer properties.
+            
+            ERROR RAISED:
+                Type:
+                Description: 
+            
+            SAMPLE USE CASES:
+                >>>  class AwesomeCompressor(_PressureChangers):
+                >>>     def __init__(**kwargs):
+                >>>         some_property = 20
+                
+        """
+        
+        if 'pressure_drop' in inputs:
+            inputs['differential_pressure'] = -1 * inputs['pressure_drop']
+            del inputs['pressure_drop']
+        
+        super().__init__(**inputs)
+        
+        if 'differential_pressure' in inputs:
+            if ((self._inlet_pressure != None or self._outlet_pressure != None) and
+                 'performance_curve' in inputs):
+                 raise Exception('Input only one of differential pressure or performance_curve.')
+            diff_presure = inputs['differential_pressure'] 
+            if isinstance(diff_presure, prop.Pressure):
+                self._pressure_drop = prop.Pressure(-1 * diff_presure.value,
+                                                    diff_presure.unit)
+            elif isinstance(diff_presure, tuple):
+                self._pressure_drop = prop.Pressure(-1 * diff_presure[0],
+                                                     diff_presure[1])
+                 
+        self._performance_curve = DataFrame()
+        if 'performance_curve' in inputs:
+            self.performace_curve = inputs['performance_curve']
+        
+        self.efficiency = 1 if 'efficiency' not in inputs else inputs['efficiency']
+        
+    @property
+    def suction_pressure(self):
+        return super(_PressureChangers, self).inlet_pressure
+    @suction_pressure.setter
+    def suction_pressure(self, value):
+        super(_PressureChangers, self.__class__).inlet_pressure.fset(self, value)
+
+    @property
+    def discharge_pressure(self):
+        return super(_PressureChangers, self).outlet_pressure
+    @discharge_pressure.setter
+    def discharge_pressure(self, value):
+        super(_PressureChangers,self.__class__).outlet_pressure.fset(self, value)
+    
+    @property
+    def differential_pressure(self):
+        return prop.Pressure(-1 * self.pressure_drop.value,
+                             self.pressure_drop.unit)
+    @differential_pressure.setter
+    def differential_pressure(self, value):
+        _Validators.validate_arg_prop_value_type("differential_pressure", value, (prop.Pressure, int, float, tuple))
+        _Validators.validate_non_negative_value("differential_pressure", value)
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
+        if unit is None:
+            unit = self.pressure_drop.unit         
+        self.pressure_drop = prop.Pressure(-1 * value,
+                                           unit)   
+        self._update_equipment_object(self)   
+    
+    @property
+    def performance_curve(self):
+        self = self._get_equipment_object(self)
+        return self._perfomace_curve
+    @performance_curve.setter
+    def performance_curve(self,value):
+        _Validators.validate_arg_prop_value_type("performance_curve", value, DataFrame)
+        self = self._get_equipment_object(self)
+        if value.shape[1] == 2:
+                self._performance_curve = value
+        else:
+            raise Exception("Enter performance_curve as pandas dataframe of 2 columns.\nOne for Flow and other for head.")
+        self._update_equipment_object(self)
+    
+    @property
+    def efficiency(self):
+        self = self._get_equipment_object(self)
+        return self._efficiency
+    @efficiency.setter
+    def efficiency(self, value):
+        _Validators.validate_arg_prop_value_type("efficiency", value, (int, float, prop.Efficiency))
+        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
+        self = self._get_equipment_object(self)
+        if value <= 0:
+            raise Exception("Provide a positive value for efficiency.")
+        elif value <= 1:
+            self._efficiency = prop.Efficiency(value)
+        else:
+            self._efficiency = prop.Efficiency(value/100)
+            warn("Efficiency set to {} considering value provided in percent.".format(value/100))
+        self._update_equipment_object(self)
+    
+    @property
+    def power(self):
+        self = self._get_equipment_object(self)
+        return self._power
+    @power.setter
+    def power(self, value):
+        _Validators.validate_arg_prop_value_type("power", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self._power.unit         
+        self._power = prop.Power(value, unit)
+        self._update_equipment_object(self)  
+
+# Defining generic class for Compressors and Expanders.
+class _GasPressureChangers(_PressureChangers):
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Class for creating objects to represent a GasPressureChanger.
+        
+        PARAMETERS:
+            Read _PressureChangers class for more arguments for this class  
+            efficiency:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative values
+                Default value: 1.4
+                Description: Efficiency of the compressor. Efficiency can be set as
+                             adiabatic/isentropic or polytropic efficiency.
+            
+            adiabatic_efficiency:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative values
+                Default value: 0.7
+                Description: Efficiency of the compressor considering adiabatic/isentropic
+                             compression.
+            
+            polytropic_efficiency:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative values
+                Default value: 0.7
+                Description: Efficiency of the compressor considering polytropic
+                             compression.
+
+            polytropic_exponent:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative values
+                Default value: 1.4
+                Description: Polytropic exponent of the gas.
+        
+        PROPERTIES:
+            power:
+                Type: Power
+                Description: Power required by the compressor.
+
+        
+        RETURN VALUE:
+            Type: CentrifugalCompressor
+            Description: Returns an object of type CentrifugalCompressor with all properties of
+                         a Centrifugal Compressor used in process industries.
+        
+        ERROR RAISED:
+            Type:
+            Description:
+        
+        SAMPLE USE CASES:
+            >>> CC_1 = CentrifugalCompressor(tag="P1")
+            >>> print(CC_1)
+            Centrifugal Compressor with tag: P1
+        """
+        super().__init__( **inputs)
+        self.adiabatic_efficiency = 0.7 if 'efficiency' not in inputs else inputs['efficiency']
+        self.polytropic_exponent = 1.4 if 'polytropic_exponent' not in inputs else inputs['polytropic_exponent']
+        
+    @property
+    def temperature_change(self):
+        self = self._get_equipment_object(self)
+        k = self.polytropic_exponent
+        if (self._inlet_material_stream_index is not None or
+            self._outlet_material_stream_index is not None):
+            is_inlet = False if self._inlet_material_stream_index is None else True
+            k = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
+            if Settings.compression_process.lower() == "polytropic":
+                k = compressible_fluid.polytropic_exponent(k=k, eta_p=self.polytropic_efficiency)
+
+        T1 = self.inlet_temperature
+        P1 = self.inlet_pressure
+        P2 = self.outlet_pressure
+        T1.unit = "K"
+        P1.unit = P2.unit ="Pa"
+        eta = self.efficiency.value
+        value = prop.Temperature(compressible_fluid.isentropic_T_rise_compression(T1.value, P1.value, P2.value, k, eta))
+        value = value - T1
+        value.unit = self.inlet_temperature.unit
+        return value
+
+    @property
+    def efficiency(self):
+        self = self._get_equipment_object(self)
+        if Settings.compression_process.lower() == "polytropic":
+            return self.polytropic_efficiency
+        else:
+            return self.adiabatic_efficiency
+    @efficiency.setter
+    def efficiency(self, value):
+        _Validators.validate_arg_prop_value_type("efficiency", value, (int, float, prop.Efficiency))
+        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
+        self = self._get_equipment_object(self)
+        if value < 0:
+            raise Exception("Provide a positive value for efficiency.")
+        elif value <= 1:
+            value = value
+        else:
+            value = value/100
+        if Settings.compression_process.lower() in ["adiabatic", "isentropic"]:
+            self.adiabatic_efficiency = value
+        else:
+            self.polytropic_efficiency = value
+            
+        self._efficiency = value
+
+    @property
+    def adiabatic_efficiency(self):
+        self = self._get_equipment_object(self)
+        return self._adiabatic_efficiency
+    @adiabatic_efficiency.setter
+    def adiabatic_efficiency(self, value):
+        _Validators.validate_arg_prop_value_type("adiabatic_efficiency", value, (int, float, prop.Efficiency))
+        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
+        self = self._get_equipment_object(self)
+        if value == None:
+            value = 0.7
+        self._adiabatic_efficiency = prop.Efficiency(value)
+        self._update_equipment_object(self)
+    
+    @property
+    def polytropic_efficiency(self):
+        self = self._get_equipment_object(self)
+        if (self._inlet_material_stream_index is not None or
+            self._outlet_material_stream_index is not None):
+            is_inlet = False if self._inlet_material_stream_index is None else True
+            isentropic_exponent = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
+            pol_eff = compressible_fluid.isentropic_efficiency(P1 = self._inlet_pressure.value,
+                                                            P2 = self._outlet_pressure.value,
+                                                            k = isentropic_exponent,
+                                                            eta_s = self.adiabatic_efficiency.value)
+            return prop.Efficiency(pol_eff)
+        else:
+            return self.efficiency
+    @polytropic_efficiency.setter
+    def polytropic_efficiency(self, value):
+        _Validators.validate_arg_prop_value_type("polytropic_efficiency", value, (int, float, prop.Efficiency))
+        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
+        self = self._get_equipment_object(self)
+        is_inlet = False if self._intlet_material_stream_index is None else True
+        isentropic_exponent = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
+        self.adiabatic_efficiency = compressible_fluid.isentropic_efficiency(P1 = self._inlet_pressure.value,
+                                                                             P2 = self._outlet_pressure.value,
+                                                                             k = isentropic_exponent,
+                                                                             eta_p = value)
+        self._update_equipment_object(self)
+    
+    @property
+    def polytropic_exponent(self):
+        self = self._get_equipment_object(self)
+        if (self._inlet_material_stream_index is None and
+            self._outlet_material_stream_index is None):
+            return self._polytropic_exponent
+        is_inlet = False if self._inlet_material_stream_index is None else True
+        k = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
+        return compressible_fluid.polytropic_exponent(k=k, eta_p=self.polytropic_efficiency.value)
+    @polytropic_exponent.setter
+    def polytropic_exponent(self, value):
+        _Validators.validate_arg_prop_value_type("polytropic_exponent", value, (int, float))
+        self = self._get_equipment_object(self)
+        if (self._inlet_material_stream_index is None and
+            self._outlet_material_stream_index is None):
+            self._polytropic_exponent = value
+        else:
+            raise Exception("""Polytropic Exponent cannot be set as Compressor is connected to a MaterialStream object.\n
+                               Update Isentropic Exponent of the stream object instead.""")
+
+    @property
+    def power(self):
+        self = self._get_equipment_object(self)
+        is_inlet = False if self._inlet_material_stream_index is None else True
+        isentropic_exponent = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
+        Z = self._connected_stream_property_getter(is_inlet, "material", "Z_g")
+        MW = self._connected_stream_property_getter(is_inlet, "material", "molecular_weight")
+        work = compressible_fluid.isentropic_work_compression(T1 = self.inlet_temperature.value,
+                                                              k = isentropic_exponent,
+                                                              Z = Z,
+                                                              P1 = self._inlet_pressure.value,
+                                                              P2 = self._outlet_pressure.value,
+                                                              eta = self.adiabatic_efficiency.value)
+        return prop.Power(work * self.inlet_mass_flowrate.value / MW.value)
+    
+    @property
+    def head(self):
+        if (self._inlet_material_stream_index is None or
+            self._outlet_material_stream_index is None):
+            raise Exception("Head calculations only supported when Compressor is connected to a MaterialStream object.")
+        if Settings.compression_process.lower() in ["adiabatic", "isentropic"]:
+            isentropic_exponent = self._connected_stream_property_getter(True, "material", "isentropic_exponent")
+            ratio = (isentropic_exponent - 1)/isentropic_exponent
+        else:
+            ratio = (self.polytropic_exponent - 1)/self.polytropic_exponent
+        
+        P1 = self.inlet_pressure
+        P2 = self.outlet_pressure
+        P1.unit = "Pa"
+        P2.unit = "Pa"
+        Zi = self._connected_stream_property_getter(True, "material", "Z_g")
+        Zo = self._connected_stream_property_getter(False, "material", "Z_g")
+        Z = (Zi + Zo)/2
+        T1 = self.inlet_temperature
+        T1.unit = "K"
+        MW = self._connected_stream_property_getter(True, "material", "molecular_weight")
+        head = Z * Constants.R * T1.value * (pow((P2.value/P1.value), ratio) - 1)/(ratio * MW.value)
+        head_max_value = Z * Constants.R * T1.max_val * (pow((P2.max_val/P1.min_val), ratio) - 1)/(ratio * MW.value)
+        head_min_value = Z * Constants.R * T1.min_val * (pow((P2.min_val/P1.max_val), ratio) - 1)/(ratio * MW.value)
+        return prop.Length(head, max_val=head_max_value, min_val=head_min_value)
+        
+    
+#Defining generic class for all types of vessels. 
+class _Vessels(_EquipmentOneInletOutlet):
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Parent class for all equipment which has primary task to be a vessel
+            of a stream. For e.g. Tanks and reactors.
+        
+        PARAMETERS:
+            ID:
+                Required: No
+                Type: int or float or Length(recommended)
+                Acceptable values: Non-negative integer
+                Default value: 0 m   
+                Description: Internal diameter of the vessel.
+            
+            OD:
+                Required: No
+                Type: int or float or Length(recommended)
+                Acceptable values: Non-negative integer
+                Default value: 0 m    
+                Description: Outer diameter of the vessel.
+
+            thickness:
+                Required: No
+                Type: int or float or Length(recommended)
+                Acceptable values: Non-negative integer
+                Default value: 0 m    
+                Description: thickness of the vessel.
+            
+            length:
+                Required: No
+                Type: int or float or Length(recommended)
+                Acceptable values: Non-negative integer
+                Default value: 0 m   
+                Description: tan-line length of the vessel.
+            
+            LLL, LLLL, HLL, NLL and HHLL:
+                Required: No
+                Type: int or float or Length(recommended)
+                Acceptable values: Non-negative integer
+                Default value: 0 m    
+                Description: Low Liquid Level(LLL), Low-Low Liquid Level(LLLL), High Liquid Level(HLL),
+                             Normal Liquid Level(NLL), and High-high Liquid Level.
+            
+            head_type:
+                Required: No
+                Type: String
+                Acceptable values: {head_types}
+                Default value: elliptical    
+                Description: Type of head for the vessel.
+            
+            main_fluid:
+                Required: No
+                Type: String
+                Acceptable values: ["liquid", "gas"]
+                Default value: liquid    
+                Description: Type of fluid which the vessel stores.
+            
+            is_blanketed:
+                Required: No
+                Type: Boolean
+                Default value: False
+                Description: Specifies if the vessel is blanketed or not.
+            
+        RETURN VALUE:
+            Type: _Vessels
+            Description: object with all _EquipmentOneInletOutlet and other vessel related properties.
+        
+        PROPERTIES:
+            operating_pressure:
+                Type: int or float or Pressure(recommended)  
+                Acceptable values: Any
+                Default value: 101325 Pa  
+                Description: Operating pressure of the vessel. operating_pressure is
+                             considered equal to outlet_pressure and can be considered as
+                             alias of each other. Setting or getting one effects the other.
+            
+            operating_temperature:
+                Type: int or float or Pressure(recommended)   
+                Acceptable values: Any
+                Default value: 298 K 
+                Description: Operating temperature of the vessel. operating_temperature is
+                             considered equal to outlet_temperature and can be considered as
+                             alias of each other. Setting or getting one effects the other.
+
+            vessel_volume:
+                Type: int or float or Volume(recommended)   
+                Acceptable values: Any
+                Default value: 0 m^3 
+                Description:Total volumetric space of the vessel including heads.
+            
+            liquid_level:
+                Type: int or float or Length(recommended)
+                Acceptable values: Non-negative integer
+                Default value: 0 m   
+                Description: liquid level of the vessel.
+            
+        METHODS:
+            get_inventory(type="volume")
+            DESCRIPTION:
+                Function to get the inventory in the vessel.
+        
+            PARAMETERS:
+                type:
+                    Type: String
+                    Acceptable values: "volume" or "mass"
+                    Default value: "volume"  
+                    Description: The type of inventory to be calculated.
+                                 "volume" calculates volumetic inventroy and
+                                 "mass" calculates mass inventory of corresponding
+                                  volumetic inventory based on density of liquid.
+                                  Property main_fluid should be set for vessesl 
+                                  containging liquid.
+                                        
+        ERROR RAISED:
+            Type:
+            Description: 
+        
+        SAMPLE USE CASES:
+            >>>  class AwesomeReactor(_Vessels):
+            >>>     def __init__(**kwargs):
+            >>>         some_property = 20
+                
+    """.format(head_types=Constants.HEAD_TYPES)
+        super().__init__(**inputs)
+        self._ID = prop.Length()
+        self._OD = prop.Length()
+        self._length = prop.Length()
+        self._LLLL = prop.Length()
+        self._LLL = prop.Length()
+        self._NLL = prop.Length()
+        self._HLL = prop.Length()
+        self._HHLL = prop.Length()
+        self.blanketing = None
+        self._material = 1
+        self.operating_pressure = prop.Pressure()
+        self.operating_temperature = prop.Temperature()
+        if ('ID' in inputs and inputs['ID'] is not None):
+                self.ID = inputs['ID']
+                if 'OD' in inputs and inputs['OD'] is not None:
+                    self.OD = inputs['OD']
+                elif 'thickness' in inputs and inputs['thickness'] is not None:
+                    self.thickness = inputs['thickness']
+                else:
+                    self.thickness = self.calculate_thickness()
+                
+        elif ('OD' in inputs and 'thickness' in inputs):
+            self.OD = inputs['OD']
+            self.ID = inputs['thickness']
+            self.ID = self.OD - self.ID
+        
+        self.length = prop.Length() if 'length' not in inputs else inputs['length']
+        
+        self.LLLL = prop.Length() if 'LLLL' not in inputs else inputs['LLLL']
+        self.LLL = prop.Length() if 'LLL' not in inputs else inputs['LLL']
+        self.NLL = prop.Length() if 'NLL' not in inputs else inputs['NLL']
+        self.liquid_level = prop.Length() if 'NLL' not in inputs else inputs['NLL']
+        self.HLL = prop.Length() if 'HLL' not in inputs else inputs['HLL']
+        self.HHLL = prop.Length() if 'HHLL' not in inputs else inputs['HHLL']
+
+        if "head_type" not in inputs:
+            self._head_type = "torispherical"  
+        else:
+            _Validators.validate_arg_prop_value_type("head_type", inputs["head_type"], str)
+            _Validators.validate_arg_prop_value_list("head_type", inputs["head_type"], Constants.HEAD_TYPES)
+            self._head_type = inputs["head_type"]
+        
+        if "is_blanketed" in inputs and inputs["is_blanketed"]:
+            self.blanketing = _Blanketing(tag=self.tag)
+            self.blanketing.inlet_pressure = self.operating_pressure
+
+    @property
+    def ID(self):
+        self = self._get_equipment_object(self)
+        return self._ID
+    @ID.setter
+    def ID(self, value):
+        _Validators.validate_arg_prop_value_type("ID", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._ID.unit
+        self._ID = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    
+    @property
+    def OD(self):
+        self = self._get_equipment_object(self)
+        return self._OD
+    @OD.setter
+    def OD(self, value):
+        _Validators.validate_arg_prop_value_type("OD", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._OD.unit
+        self._OD =prop.Length(value, unit)
+        self._update_equipment_object(self)
+
+    @property
+    def thickness(self):
+        self = self._get_equipment_object(self)
+        # if self._OD - self._ID <= prop.Length(0):
+        #     raise Exception("ID is not less than OD! Change ID or OD or thickness.")
+        return self._OD - self._ID
+    @thickness.setter
+    def thickness(self, value):
+        _Validators.validate_arg_prop_value_type("thickness", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self.thickness
+        self._OD = self._ID + prop.Length(value, unit)
+        self._update_equipment_object(self)
+    
+    def calculate_thickness(self):
+        #TODO: Update calculations based on design pressure.
+        return prop.Length(0.01)
+
+    @property
+    def length(self):
+        self = self._get_equipment_object(self)
+        return self._length
+    @length.setter
+    def length(self, value):
+        _Validators.validate_arg_prop_value_type("length", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._length.unit
+        self._length = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @length.deleter
+    def length(self):
+        self = self._get_equipment_object(self)
+        del self._length
+        self._update_equipment_object(self)
+    
+    @property
+    def LLLL(self):
+        self = self._get_equipment_object(self)
+        return self._LLLL
+    @LLLL.setter
+    def LLLL(self, value):
+        _Validators.validate_arg_prop_value_type("LLLL", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._LLLL.unit
+        self._LLLL = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @LLLL.deleter
+    def LLLL(self):
+        self = self._get_equipment_object(self)
+        del self._LLLL
+        self._update_equipment_object(self)
+
+    @property
+    def LLL(self):
+        self = self._get_equipment_object(self)
+        return self._LLL
+    @LLL.setter
+    def LLL(self, value):
+        _Validators.validate_arg_prop_value_type("LLL", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._LLL.unit
+        self._LLL = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @LLL.deleter
+    def LLL(self):
+        self = self._get_equipment_object(self)
+        del self._LLL
+        self._update_equipment_object(self)
+
+    @property
+    def NLL(self):
+        self = self._get_equipment_object(self)
+        return self._NLL
+    @NLL.setter
+    def NLL(self, value):
+        _Validators.validate_arg_prop_value_type("NLL", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._NLL.unit
+        self._NLL = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @NLL.deleter
+    def NLL(self):
+        self = self._get_equipment_object(self)
+        del self._NLL
+        self._update_equipment_object(self)
+
+    @property
+    def HLL(self):
+        self = self._get_equipment_object(self)
+        return self._HLL
+    @HLL.setter
+    def HLL(self, value):
+        _Validators.validate_arg_prop_value_type("HLL", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._HLL.unit
+        self._HLL = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @HLL.deleter
+    def HLL(self):
+        self = self._get_equipment_object(self)
+        del self._HLL
+        self._update_equipment_object(self)
+
+    @property
+    def HHLL(self):
+        self = self._get_equipment_object(self)
+        return self._HHLL
+    @HHLL.setter
+    def HHLL(self, value):
+        _Validators.validate_arg_prop_value_type("HHLL", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._HHLL.unit
+        self._HHLL = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @HHLL.deleter
+    def HHLL(self):
+        self = self._get_equipment_object(self)
+        del self._HHLL
+        self._update_equipment_object(self)
+
+    @property
+    def head_type(self):
+        self = self._get_equipment_object(self)
+        return self._head_type
+    @head_type.setter
+    def head_type(self, value):
+        _Validators.validate_arg_prop_value_type("head_type", value, str)
+        _Validators.validate_arg_prop_value_list("head_type", value, Constants.HEAD_TYPES)
+        self = self._get_equipment_object(self)
+        if value not in Constants.HEAD_TYPES:
+            raise Exception("""Head type '{0}', not supported. Supported types are:\n
+            {1}""".format(value, Constants.HEAD_TYPES))
+        self._head_type = value
+        self._update_equipment_object(self)
+    @head_type.deleter
+    def head_type(self):
+        self = self._get_equipment_object(self)
+        del self._head_type
+        self._update_equipment_object(self)
+
+    @property
+    def material(self):
+        self = self._get_equipment_object(self)
+        return self._material
+    @material.setter
+    def material(self, value):
+        _Validators.validate_arg_prop_value_type("material", value, int)
+        _Validators.validate_arg_prop_value_range("head_type", value, [1, 4])
+        self = self._get_equipment_object(self)
+        materials = '''\nSegment material can be of following types and in range of numbers below:
+                    1. Raw Steel
+                    2. Carbon Steel
+                    3. Cast Iron
+                    4. Stainless Steel
+                    ''' 
+        if value not in range(1, 6):
+            raise Exception(materials)
+        self._material = value
+        self._update_equipment_object(self)
+
+    @property
+    def main_fluid(self):
+        self = self._get_equipment_object(self)
+        return self._main_fluid
+    @main_fluid.setter
+    def main_fluid(self, value):
+        _Validators.validate_arg_prop_value_type("main_fluid", value, str)
+        _Validators.validate_arg_prop_value_list("main_fluid", value, ("liquid", "gas"))
+        self = self._get_equipment_object(self)
+        self._main_fluid = value
+        self._update_equipment_object(self)
+
+    @property
+    def pressure_drop(self):
+        g = Constants.g
+        self = self._get_equipment_object(self)
+        if ((self._inlet_energy_stream_index is not None or
+             self._outlet_energy_stream_index is not None) and 
+             self.main_fluid == "liquid"):
+            is_inlet = False if self._inlet_material_stream_index is None else True
+            density = self._connected_stream_property_getter(is_inlet, "material", "density")
+            density.unit = "kg/m^3"
+            pd = density.value * g * self.liquid_level.value
+            pd_min = density.min_value * g * self.liquid_level.min_val
+            pd_max = density.max_value * g * self.liquid_level.max_val
+            return prop.Pressure(value=pd, min_val=pd_min, max_val=pd_max)
+        return self._pressure_drop
+    @pressure_drop.setter
+    def pressure_drop(self, value):
+        _Validators.validate_arg_prop_value_type("pressure_drop", value, (prop.Pressure, int, float, tuple))
+        if ((self._inlet_energy_stream_index is not None or
+             self._outlet_energy_stream_index is not None) and 
+             self.main_fluid == "liquid"):
+            raise Exception("Pressure drop cannot be set for vessels with main fluid as liquid.")
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
+        if unit is None:
+            unit = self._pressure_drop.unit
+        self._pressure_drop = prop.Pressure(value, unit)
+        self._outlet_pressure =  self._inlet_pressure - self._pressure_drop
+        self._update_equipment_object(self)
+               
+    @property
+    def operating_pressure(self):
+        return self.inlet_pressure
+    @operating_pressure.setter
+    def operating_pressure(self, value):
+        _Validators.validate_arg_prop_value_type("operating_pressure", value, (prop.Pressure, int, float, tuple))
+        self.inlet_pressure = value
+        if self.blanketing is not None:
+            self.blanketing.inlet_pressure = value
+    
+    @property
+    def operating_temperature(self):
+        return self.inlet_temperature
+    @operating_temperature.setter
+    def operating_temperature(self, value):
+        _Validators.validate_arg_prop_value_type("operating_temperature", value, (prop.Temperature, int, float, tuple))
+        self.inlet_temperature = value
+        if self.blanketing is not None:
+            self.blanketing.inlet_temperature = value
+    
+    @property
+    def vessel_volume(self):
+        D = self.ID.value
+        L = self.length.value
+        t = self.thickness.value
+        cylinder_volume = pi * D * D * L / 4
+        # Volume of both heads.
+        head_volume = 0
+        if self.head_type == "hemispherical":
+            # Spherical heads are not exact sphere but part of it.
+            # Dish depth = D/2
+            head_volume = pi * (D ** 3) / 6 
+        elif self.head_type == "elliptical":
+            # Dish depth = D/4
+            head_volume = pi * (D ** 3) / 12
+        elif self.head_type == "torispherical":
+            Rc = D + t
+            Rk = 3 * t
+            z = Rc - sqrt((Rc - Rk)**2 - (self.OD.value/2 - t - Rk)**2)
+            head_volume = 0.9 * 4 * pi * Rc * Rc * z / 3 
+        return prop.Volume(cylinder_volume + head_volume, "m^3")
+
+    @property
+    def liquid_level(self):
+        self = self._get_equipment_object(self)
+        return self._liquid_level
+    @liquid_level.setter
+    def liquid_level(self, value):
+        _Validators.validate_arg_prop_value_type("liquid_level", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._liquid_level.unit
+        self._liquid_level = prop.Length(value, unit)
+        self._update_equipment_object(self)
+
+    def get_inventory(self, type="volume"):
+        _Validators.validate_arg_prop_value_type("type", type, str)
+        _Validators.validate_arg_prop_value_list("type", type, ["volume", "mass"])
+        self = self._get_equipment_object(self)
+        if self.main_fluid == "gas":
+            if type == "volume":
+                liquid_volume = self._get_liquid_volume()
+                gas_volume = self.vessel_volume - liquid_volume
+                return gas_volume 
+            else:
+                is_inlet = False if self._inlet_material_stream_index is None else True
+                density = self._connected_stream_property_getter(is_inlet, "material", "density_g")
+                return prop.Mass(self.inventory().value * density) 
+        else:
+            if type == "volume":
+                return self._get_liquid_volume()
+            else:
+                is_inlet = False if self._inlet_material_stream_index is None else True
+                density = self._connected_stream_property_getter(is_inlet, "material", "density_l")
+                mass = self._get_liquid_volume().value * density.value
+    
+class _VerticalVessels(_Vessels):
+    def __init__(self, **inputs) -> None:
+        super().__init__(**inputs)
+    
+    def _get_head_volume(self):
+        head_volume = 0
+        D = self.ID.value
+        if self.head_type == "hemispherical":
+            # Dish depth = D/2
+            head_volume = pi * (D ** 3) / 12
+        elif self.head_type == "elliptical":
+            # Dish depth = D/4
+            head_volume = pi * (D ** 3) / 24
+        elif self.head_type == "torispherical":
+            Rc = (self.ID + self.thickness).value
+            Rk = 3 * self.thickness.value
+            z = Rc - sqrt((Rc - Rk)**2 - (self.OD.value/2 - self.thickness.value - Rk)**2)
+            head_volume = 0.9 * 4 * pi * Rc * Rc * z / 3
+        return prop.Volume(head_volume) 
+
+    def _get_cylinder_volume(self):
+        volume = pi * self.ID.value**2 * self.liquid_level.value / 4
+        return prop.Volume(volume)
+    
+    def _get_liquid_volume(self):
+        head_volume = self._get_head_volume()
+        cylinder_volume = self._get_cylinder_volume()
+        return cylinder_volume + head_volume
+
+class _HorizontalVessels(_Vessels):
+    def __init__(self, **inputs) -> None:
+        super().__init__(**inputs)
+    
+    def _get_head_volume(self):
+        self = self._get_equipment_object(self)
+        C = 0
+        if self.head_type == "hemispherical":
+            C = 1
+        elif self.head_type == "elliptical":
+            C = 0.5
+        elif self.head_type == "torispherical":
+            Rk = 3 * self.thickness.value
+            t_by_Dext = self.thickness/self.OD
+            C = 0.30939 + 1.7197 * (Rk - 0.06 * self.OD.value)/self.ID.value - 0.16116 * t_by_Dext + 0.98997 * t_by_Dext**2
+        head_volume = self._get_head_volume_by_type(C)
+        return prop.Volume(head_volume) 
+    
+    def _get_head_volume_by_type(self, C):
+        head_volume = (self.ID.value ** 3) * pi 
+        H_by_ID = self.liquid_level / self.ID
+        head_volume *= 3 * H_by_ID**2 - 2 * H_by_ID**3
+        head_volume /= 12
+        head_volume *= C
+        return head_volume
+
+    def _get_cylinder_volume(self):
+        self = self._get_equipment_object(self)
+        volume = 0
+        # alpha = cos-1(1-H/R)
+        R = self.ID.value / 2
+        H = self.liquid_level.value
+        L = self.length.value
+        radians = 1 - H / R
+        alpha = acos(radians)
+        volume = L * ((R ** 2) * alpha - (R - H) * sqrt(2*R*H - H*H))
+        return prop.Volume(volume)
+    
+    def _get_liquid_volume(self):
+        head_volume = self._get_head_volume()
+        cylinder_volume = self._get_cylinder_volume()
+        return cylinder_volume + head_volume + head_volume
+
+class _SphericalVessels(_Vessels):
+    def __init__(self, **inputs) -> None:
+        super().__init__(**inputs)
+        del self.head_type
+        del self.length
+    
+    @property
+    def vessel_volume(self):
+        self = self._get_equipment_object(self)
+        D = self.ID.value
+        volume = 2 * self._get_hemisphere_volume(D, D/2)
+        return prop.Volume(volume)
+    def _get_liquid_volume(self):
+        self = self._get_equipment_object(self)
+        H = self.liquid_level.value
+        D = self.ID.value
+        if H <= D/2:
+            volume = self._get_hemisphere_volume(D, H)
+        else:
+            volume = self._get_hemisphere_volume(D, D/2)
+            volume -=  self._get_hemisphere_volume(D, H)
+        return prop.Volume(volume)
+    
+    def _get_hemisphere_volume(self, D, H):
+        return pi * H**2 *(1.5 * D - H) / 3
+
+class _Blanketing(_EquipmentOneInletOutlet):
+    def __init__(self, **inputs) -> None:
+        inputs["tag"] += "_blanketing" 
+        super().__init__(**inputs)
+        del self.energy_in
+        del self.energy_out
+    
+    def __repr__(self):
+        return "Blanketing with tag: " + self.tag
+    @property
+    def pressure_drop(self):
+        return prop.Pressure(0)
+    @pressure_drop.setter
+    def pressure_drop(self, value):
+        raise Exception("Pressure drop setting for blanketing is not allowed as it is an intermittent process.")
+    
+    @property
+    def temperature_increase(self):
+        return prop.Temperature(0, "K")
+    @temperature_increase.setter
+    def temperature_increase(self, value):
+        raise Exception("Temperature increase setting for blanketing is not allowed as it is an intermittent process.")
+        
+    @property
+    def temperature_decrease(self):
+        return prop.Temperature(0, "K")
+    @temperature_decrease.setter
+    def temperature_decrease(self, value):
+        raise Exception("Temperature decrease setting for blanketing is not allowed as it is an intermittent process.")
+        
+
+#Defining generic class for all types of heat exchangers NEEDS SUPER CLASS WITH MULTI INPUT AND OUTPUT
+class _Exchangers(_EquipmentOneInletOutlet):
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Parent class for all equipment which has primary task to be an 
+            Temperature changer of a stream. For e.g. Heater and Cooler.
+        
+        PARAMETERS:
+            temperature_decrease:
+                Required: No
+                    Type: int/float or Temperature(recommended)
+                    Acceptable values: Non-negative integer
+                    Default value: based on unit    
+                    Description: Temperature decrease of stream in the equipment.
+                                 That is decrease from inlet stream to outlet stream.
+            
+            temperature_increase:
+                Required: No
+                    Type: int/float or Temperature(recommended)
+                    Acceptable values: Non-negative integer
+                    Default value: based on unit    
+                    Description: Temperature increase of stream in the equipment.
+                                 That is increase from inlet stream to outlet stream.
+                
+            efficiency:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative integer
+                Default value: based on unit    
+                Description: Efficiency of the equipment.
+
+        RETURN VALUE:
+            Type: _Exchangers
+            Description: object with all _EquipmentOneInletOutlet and other exchanger related properties.
+        
+        ERROR RAISED:
+            Type:
+            Description: 
+        
+        SAMPLE USE CASES:
+            >>>  class AwesomeNewExchanger(_Exchangers):
+            >>>     def __init__(**kwargs):
+            >>>         some_property = 20 
+        """
+        super().__init__(**inputs)
+        if ("temperature_increase" not in inputs and
+            "temperature_decrease" not in inputs):
+            self.temperature_increase = prop.Temperature(0, 'K')
+        elif "temperature_increase" in inputs:
+            self.temperature_increase = inputs["temperature_increase"]
+        else:
+            self.temperature_decrease = inputs["temperature_decrease"] 
+        if "energy_in" in inputs:
+            self.energy_in = inputs["energy_in"]
+        if "energy_out" in inputs:
+            self.energy_out = inputs["energy_out"]
+        self._efficiency = 100 if 'efficiency' not in inputs else inputs['efficiency']
+        
+    @property
+    def efficiency(self):
+        self = self._get_equipment_object(self)
+        return self._efficiency
+    @efficiency.setter
+    def efficiency(self, value):
+        _Validators.validate_arg_prop_value_type("efficiency", value, (int, float, prop.Efficiency))
+        value, _ = self._tuple_property_value_unit_returner(value, prop.Efficiency)
+        self = self._get_equipment_object(self)
+        if value < 0:
+            raise Exception("Provide a positive value for efficiency.")
+        elif value <= 1:
+            self._efficiency = prop.Efficiency(value)
+        else:
+            self._efficiency = prop.Efficiency(value/100)
         self._update_equipment_object(self)
```

### Comparing `propylean-0.2.5/src/propylean/equipments/rotary.py` & `propylean-0.2.6/src/propylean/equipments/rotary.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,590 +1,590 @@
-from propylean.equipments.generic_equipment_classes import _PressureChangers, _GasPressureChangers
-from propylean import streams
-import propylean.properties as prop
-
-from math import pow
-from propylean.validators import _Validators
-
-# Start of final classes of pumps.
-class CentrifugalPump(_PressureChangers):
-    items = []    
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Final class for creating objects to represent Centrifugal Pump.
-        
-        PARAMETERS:
-            Read _PressureChangers class for more arguments for this class
-            min_flow:
-                Required: No
-                Type: int/float or tuple(value, unit) or VolumetricFlowrate(recommended)
-                Acceptable values: Non-negative values
-                Default value: None # TODO: Add industry standard
-                Description: Minimum flow requirement of the pump
-
-            NPSHr:
-                Required: No
-                Type: int/float or tuple(value, unit) or Length(recommended)
-                Acceptable values: Non-negative values
-                Default value: None
-                Description: NPSHr of the pump
-        
-        PROPERTIES:
-            NPSHa:
-                Type: Length
-                Description: NPSH available to the pump.
-            
-            head:
-                Type: Length
-                Description: Differential head generated by the pump.
-
-            hydraulic_power:
-                Type: Power
-                Description: Hydraulic power generated by the pump.
-            
-            power/energy_in:
-                Type: Power
-                Description: Power required by the pump.
-
-        
-        RETURN VALUE:
-            Type: CentrifugalPump
-            Description: Returns an object of type CentrifugalPump with all properties of
-                         a centrifugal pump used in process industries.
-        
-        ERROR RAISED:
-            Type:
-            Description:
-        
-        SAMPLE USE CASES:
-            >>> pump_1 = CentrifugalPump(tag="P1")
-            >>> print(pump_1)
-            Centrifugal Pump with tag: P1
-        """
-        super().__init__( **inputs)
-        self._NPSHr = prop.Length()
-        self._NPSHa = prop.Length()
-        self._min_flow = prop.VolumetricFlowRate()
-        del self.energy_out
-        
-        if 'min_flow' in inputs:
-            self.min_flow = inputs['min_flow']
-        if "NPSHr" in inputs:
-            self.NPSHr = inputs['NPSHr']
-        
-        self._index = len(CentrifugalPump.items)
-        CentrifugalPump.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Centrifugal Pump with tag: " + self.tag
-    def __hash__(self):
-        return hash(self.__repr__())
-
-    @property
-    def min_flow(self):
-        self = self._get_equipment_object(self)
-        return self._min_flow
-    @min_flow.setter
-    def min_flow(self, value):
-        _Validators.validate_arg_prop_value_type("min_flow", value, (prop.VolumetricFlowRate, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.VolumetricFlowRate)
-        if unit is None:
-            unit = self._min_flow.unit
-        self._min_flow = prop.VolumetricFlowRate(value, unit)
-        self._update_equipment_object(self)
-
-    @property
-    def NPSHr(self):
-        self = self._get_equipment_object(self)
-        return self._NPSHr
-    @NPSHr.setter
-    def NPSHr(self, value):
-        _Validators.validate_arg_prop_value_type("min_flow", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._NPSHr.unit
-        self._NPSHr = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    
-    @property
-    def NPSHa(self):
-        self = self._get_equipment_object(self)
-        if self._inlet_material_stream_tag is None:
-            raise Exception("Pump should be connected with MaterialStream at the inlet")
-        density = self._connected_stream_property_getter(True, "material", "density")
-        density.unit = "kg/m^3"
-        old_p_unit = self.inlet_pressure.unit
-        self.inlet_pressure.unit = 'Pa'
-        value = self.inlet_pressure.value/(9.8 * density.value)
-        self.inlet_pressure.unit = old_p_unit
-        return prop.Length(value, "m")
-
-    @property
-    def head(self):
-        self = self._get_equipment_object(self)
-        if (self._outlet_material_stream_tag is None and
-            self._inlet_material_stream_tag is None):
-            raise Exception("Pump should be connected with MaterialStream either at inlet or outlet")
-        is_inlet = False if self._inlet_material_stream_index is None else True
-        density = self._connected_stream_property_getter(is_inlet, "material", "density")
-        density.unit = "kg/m^3"
-        dp = self.differential_pressure
-        dp.unit = "Pa"
-        value = dp.value / (9.8 * density.value)
-        return prop.Length(value, "m")
-    @property
-    def hydraulic_power(self):
-        self = self._get_equipment_object(self)
-        if (self._outlet_material_stream_tag is None and
-            self._inlet_material_stream_tag is None):
-            raise Exception("Centrifugal Pump should be connected with MaterialStream either at inlet or outlet")
-        is_inlet = False if self._inlet_material_stream_index is None else True
-        vol_flowrate = self._connected_stream_property_getter(is_inlet, "material", "vol_flowrate")
-        vol_flowrate.unit = "m^3/h"
-        dp = self.differential_pressure
-        dp.unit = "Pa"
-        value = vol_flowrate.value * dp.value / (3.6e3)
-        return prop.Power(value, 'W')
-    @property
-    def power(self):
-        self = self._get_equipment_object(self)
-        self.hydraulic_power.unit = "W"
-        value = self.hydraulic_power.value / self.efficiency.value
-        return prop.Power(value, "W")
-    @power.setter
-    def power(self, value):
-        #TODO Proived setting feature for power
-        raise Exception("Pump power value setting is not yet supported. Modify differential pressure to get required power.")
-    @property
-    def energy_in(self):
-        return self.power
-    @energy_in.setter
-    def energy_in(self, value):
-        # This is needed for property matching with the stream.
-        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self.energy_in.unit
-        self._energy_in = prop.Power(value, unit)
-        self._update_equipment_object(self)
-    
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-    
-    def connect_stream(self, 
-                       stream_object=None, 
-                       direction=None, 
-                       stream_tag=None, 
-                       stream_type=None,
-                       stream_governed=True):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'power', 'e', 'p']):
-            if direction is not None and 'out' in direction:
-                raise Exception('CentrifugalPump only supports energy inlet.')
-            direction = 'in'
-            stream_governed = False
-        return super().connect_stream(direction=direction, 
-                                      stream_object=stream_object, 
-                                      stream_tag=stream_tag, 
-                                      stream_type=stream_type,
-                                      stream_governed=stream_governed)
-    
-    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'power', 'e', 'p']):
-            if direction is not None and 'out' in direction:
-                raise Exception('CentrifugalPump only supports energy inlet.')
-            direction = 'in'
-            stream_type = "e"
-        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
-
-
-class PositiveDisplacementPump(_PressureChangers):
-    items = []
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Final class for creating objects to represent a Positive Displacement Pump.
-        
-        PARAMETERS:
-            Read _PressureChangers class for more arguments for this class
-            min_flow:
-                Required: No
-                Type: int/float or tuple(value, unit) or VolumetricFlowrate(recommended)
-                Acceptable values: Non-negative values
-                Default value: None # TODO: Add industry standard
-                Description: Minimum flow requirement of the pump
-
-            NPSHr:
-                Required: No
-                Type: int/float or tuple(value, unit) or Length(recommended)
-                Acceptable values: Non-negative values
-                Default value: None
-                Description: NPSHr of the pump
-        
-        PROPERTIES:
-            NPSHa:
-                Type: Length
-                Description: NPSH available to the pump.
-            
-            head:
-                Type: Length
-                Description: Differential head generated by the pump.
-
-            accel_head:
-                Type: Length
-                Description: Acceleration head loss at the inlet of pump.
-            
-            power/energy_in:
-                Type: Power
-                Description: Power required by the pump.
-
-        RETURN VALUE:
-            Type: PositiveDisplacementPump
-            Description: Returns an object of type PositiveDisplacementPump with all properties of
-                         a positive displacement pump used in process industries.
-        
-        ERROR RAISED:
-            Type:
-            Description:
-        
-        SAMPLE USE CASES:
-            >>> pump_1 = PositiveDisplacementlPump(tag="P1")
-            >>> print(pump_1)
-            Positive Displacement Pump with tag: P1
-        """
-        super().__init__( **inputs)
-        self._speed = prop.Frequency()
-        self._NPSHr = prop.Length()
-        if "NPSHr" in inputs:
-            self.NPSHr = inputs['NPSHr']
-        del self.energy_out
-
-        self._index = len(PositiveDisplacementPump.items)
-        PositiveDisplacementPump.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Positive Displacement Pump with tag: " + self.tag
-    def __hash__(self):
-        return hash(self.__repr__())
-    
-    @property
-    def NPSHa(self):
-        self = self._get_equipment_object(self)
-        if self._inlet_material_stream_tag is None:
-            raise Exception("Pump should be connected with MaterialStream at the inlet")
-        density = self._connected_stream_property_getter(True, "material", "density")
-        density.unit = "kg/m^3"
-        old_p_unit = self.inlet_pressure.unit
-        old_acc_head_unit = self.accel_head.unit
-        self.inlet_pressure.unit = self.accel_head = 'Pa'
-        
-        value = (self.inlet_pressure.value - self.accel_head.value)/(9.8 * density.value)
-        self.inlet_pressure.unit = old_p_unit
-        self.accel_head.unit = old_acc_head_unit
-        return prop.Length(value, "m")
-    @property
-    def NPSHr(self):
-        self = self._get_equipment_object(self)
-        return self._NPSHr
-    @NPSHr.setter
-    def NPSHr(self, value):
-        _Validators.validate_arg_prop_value_type("min_flow", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
-        if unit is None:
-            unit = self._NPSHr.unit
-        self._NPSHr = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    
-    @property
-    def head(self):
-        self = self._get_equipment_object(self)
-        if (self._outlet_material_stream_tag is None and
-            self._inlet_material_stream_tag is None):
-            raise Exception("Pump should be connected with MaterialStream either at inlet or outlet")
-        is_inlet = False if self._inlet_material_stream_index is None else True
-        density = self._connected_stream_property_getter(is_inlet, "material", "density")
-        density.unit = "kg/m^3"
-        dp = self.differential_pressure
-        dp.unit = "Pa"
-        value = dp.value / (9.8 * density.value)
-        return prop.Length(value, "m")
-    
-    @property
-    def accel_head(self):
-        L, V = self._get_suction_length_velocity()
-        density = self._connected_stream_property_getter(True, "material", "density")
-        density.unit = "kg/m^3"
-        SG = density.value/1000
-        k = 1
-        head_loss = L.value * V.value * self.speed * SG / (k * 9.8) 
-        return prop.Length(head_loss, 'm')
-    
-    @property
-    def power(self):
-        self = self._get_equipment_object(self)
-        is_inlet = False if self._inlet_material_stream_index is None else True
-        vol_flow = self._connected_stream_property_getter(is_inlet, "material", "vol_flowrate")
-        vol_flow.unit = "gal/min"
-        old_dp_unit = self.differential_pressure.unit
-        self.differential_pressure.unit = 'psi'
-        value = vol_flow.value * self.differential_pressure.value /(1714 * self.efficiency.value)
-        return prop.Power(value, "hp")
-    @power.setter
-    def power(self, value):
-        #TODO Proived setting feature for power
-        raise Exception("Pump power value setting is not yet supported. Modify differential pressure to get required power.")
-    @property
-    def energy_in(self):
-        return self.power
-    @energy_in.setter
-    def energy_in(self, value):
-        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self.energy_in.unit
-        self._energy_in = prop.Power(value, unit)
-        self._update_equipment_object(self)
-        
-    
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-
-    def connect_stream(self, 
-                       stream_object=None, 
-                       direction=None, 
-                       stream_tag=None, 
-                       stream_type=None,
-                       stream_governed=True):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'power', 'e', 'p']):
-            if direction is not None and 'out' in direction:
-                raise Exception('PositiveDisplacementPump only supports energy inlet.')
-            direction = 'in'
-        return super().connect_stream(direction=direction, 
-                                      stream_object=stream_object, 
-                                      stream_tag=stream_tag, 
-                                      stream_type=stream_type,
-                                      stream_governed=stream_governed)
-    
-    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'power', 'e', 'p']):
-            if direction is not None and 'out' in direction:
-                raise Exception('PositiveDisplacementPump only supports energy inlet.')
-            direction = 'in'
-            stream_type = "e"
-        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
-# End of final classes of pumps
-
-# Start of final classes of Compressors and TurboExpanders.
-class CentrifugalCompressor(_GasPressureChangers):
-    items = []
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Final class for creating objects to represent a Centrifugal Compressors.
-        
-        PARAMETERS:
-            Read _PressureChangers class for more arguments for this class  
-            efficiency:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative values
-                Default value: 1.4
-                Description: Efficiency of the compressor. Efficency can be set as
-                             adiabatic/isentropic or polytropic efficiency.
-            
-            adiabatic_efficiency:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative values
-                Default value: 0.7
-                Description: Efficiency of the compressor considering adiabatic/isentropic
-                             compression.
-            
-            polytropic_efficiency:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative values
-                Default value: 0.7
-                Description: Efficiency of the compressor considering polytropic
-                             compression.
-
-            polytropic_exponent:
-                Required: No
-                Type: int or float (recommended)
-                Acceptable values: Non-negative values
-                Default value: 1.4
-                Description: Polytropic exponent of the gas.
-        
-        PROPERTIES:
-            power:
-                Type: Power
-                Description: Power required by the compressor.
-
-        
-        RETURN VALUE:
-            Type: CentrifugalCompressor
-            Description: Returns an object of type CentrifugalCompressor with all properties of
-                         a Centrifugal Compressor used in process industries.
-        
-        ERROR RAISED:
-            Type:
-            Description:
-        
-        SAMPLE USE CASES:
-            >>> CC_1 = CentrifugalCompressor(tag="P1")
-            >>> print(CC_1)
-            Centrifugal Compressor with tag: P1
-        """
-        super().__init__( **inputs)
-        del self.energy_out
-        self._index = len(CentrifugalCompressor.items)
-        CentrifugalCompressor.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Centrifugal Compressor with tag: " + self.tag
-    def __hash__(self):
-        return hash(self.__repr__())
-    
-    @property
-    def temperature_increase(self):
-        return super().temperature_change
-    
-    @property
-    def energy_in(self):
-        return self.power
-    @energy_in.setter
-    def energy_in(self, value):
-        # This is needed for property matching with the stream.
-        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
-        _Validators.validate_non_negative_value("energy_in", value)
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self.energy_in.unit
-        self._energy_in = prop.Power(value, unit)
-        self._update_equipment_object(self)
-    
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-    
-    def connect_stream(self, 
-                       stream_object=None, 
-                       direction=None, 
-                       stream_tag=None, 
-                       stream_type=None,
-                       stream_governed=True):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'power', 'e', 'p']):
-            if direction is not None and 'out' in direction:
-                raise Exception('CentrifugalCompressor only supports energy inlet.')
-            direction = 'in'
-            stream_governed = False
-            stream_type = "e"
-        return super().connect_stream(direction=direction, 
-                                      stream_object=stream_object, 
-                                      stream_tag=stream_tag, 
-                                      stream_type=stream_type,
-                                      stream_governed=stream_governed)
-    
-    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'power', 'e', 'p']):
-            if direction is not None and 'out' in direction:
-                raise Exception('CentrifugalCompressor only supports energy inlet.')
-            direction = 'in'
-            stream_type = 'e'
-        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
-
-class TurboExpander(_GasPressureChangers):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__( **inputs)
-        del self.energy_in
-        self._index = len(TurboExpander.items)
-        TurboExpander.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "TurboExpander with tag: " + self.tag
-    def __hash__(self):
-        return hash(self.__repr__())
-
-    @property
-    def temperature_decrease(self):
-        return super().temperature_change
-    @property
-    def temperature_increase(self):
-        t_increase = super().temperature_change
-        t_increase.value *= -1
-        return t_increase
-
-    @property
-    def energy_out(self):
-        return self.power
-    @energy_out.setter
-    def energy_out(self, value):
-        # This is needed for property matching with the stream.
-        _Validators.validate_arg_prop_value_type("energy_out", value, (prop.Power, int, float, tuple))
-        _Validators.validate_non_negative_value("energy_out", value)
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
-        if unit is None:
-            unit = self.energy_out.unit
-        self._energy_out = prop.Power(value, unit)
-        self._update_equipment_object(self)
-
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-    
-    def connect_stream(self,
-                       stream_object=None, 
-                       direction=None, 
-                       stream_tag=None, 
-                       stream_type=None,
-                       stream_governed=True):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'power', 'e', 'p']):
-            if direction is not None and 'in' in direction:
-                raise Exception('TurboExpander only supports energy outlet.')
-            direction = 'out'
-            stream_type = 'e'
-            stream_governed = False
-        return super().connect_stream(direction=direction, 
-                                      stream_object=stream_object, 
-                                      stream_tag=stream_tag, 
-                                      stream_type=stream_type,
-                                      stream_governed=stream_governed)
-    
-    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'power', 'e', 'p']):
-            if direction is not None and 'in' in direction:
-                raise Exception('TurboExpander only supports energy outlet.')
-            direction = 'out'
-            stream_type = 'e'
-        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
-
+from propylean.equipments.generic_equipment_classes import _PressureChangers, _GasPressureChangers
+from propylean import streams
+import propylean.properties as prop
+
+from math import pow
+from propylean.validators import _Validators
+
+# Start of final classes of pumps.
+class CentrifugalPump(_PressureChangers):
+    items = []    
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Final class for creating objects to represent Centrifugal Pump.
+        
+        PARAMETERS:
+            Read _PressureChangers class for more arguments for this class
+            min_flow:
+                Required: No
+                Type: int/float or tuple(value, unit) or VolumetricFlowrate(recommended)
+                Acceptable values: Non-negative values
+                Default value: None # TODO: Add industry standard
+                Description: Minimum flow requirement of the pump
+
+            NPSHr:
+                Required: No
+                Type: int/float or tuple(value, unit) or Length(recommended)
+                Acceptable values: Non-negative values
+                Default value: None
+                Description: NPSHr of the pump
+        
+        PROPERTIES:
+            NPSHa:
+                Type: Length
+                Description: NPSH available to the pump.
+            
+            head:
+                Type: Length
+                Description: Differential head generated by the pump.
+
+            hydraulic_power:
+                Type: Power
+                Description: Hydraulic power generated by the pump.
+            
+            power/energy_in:
+                Type: Power
+                Description: Power required by the pump.
+
+        
+        RETURN VALUE:
+            Type: CentrifugalPump
+            Description: Returns an object of type CentrifugalPump with all properties of
+                         a centrifugal pump used in process industries.
+        
+        ERROR RAISED:
+            Type:
+            Description:
+        
+        SAMPLE USE CASES:
+            >>> pump_1 = CentrifugalPump(tag="P1")
+            >>> print(pump_1)
+            Centrifugal Pump with tag: P1
+        """
+        super().__init__( **inputs)
+        self._NPSHr = prop.Length()
+        self._NPSHa = prop.Length()
+        self._min_flow = prop.VolumetricFlowRate()
+        del self.energy_out
+        
+        if 'min_flow' in inputs:
+            self.min_flow = inputs['min_flow']
+        if "NPSHr" in inputs:
+            self.NPSHr = inputs['NPSHr']
+        
+        self._index = len(CentrifugalPump.items)
+        CentrifugalPump.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Centrifugal Pump with tag: " + self.tag
+    def __hash__(self):
+        return hash(self.__repr__())
+
+    @property
+    def min_flow(self):
+        self = self._get_equipment_object(self)
+        return self._min_flow
+    @min_flow.setter
+    def min_flow(self, value):
+        _Validators.validate_arg_prop_value_type("min_flow", value, (prop.VolumetricFlowRate, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.VolumetricFlowRate)
+        if unit is None:
+            unit = self._min_flow.unit
+        self._min_flow = prop.VolumetricFlowRate(value, unit)
+        self._update_equipment_object(self)
+
+    @property
+    def NPSHr(self):
+        self = self._get_equipment_object(self)
+        return self._NPSHr
+    @NPSHr.setter
+    def NPSHr(self, value):
+        _Validators.validate_arg_prop_value_type("min_flow", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._NPSHr.unit
+        self._NPSHr = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    
+    @property
+    def NPSHa(self):
+        self = self._get_equipment_object(self)
+        if self._inlet_material_stream_tag is None:
+            raise Exception("Pump should be connected with MaterialStream at the inlet")
+        density = self._connected_stream_property_getter(True, "material", "density")
+        density.unit = "kg/m^3"
+        old_p_unit = self.inlet_pressure.unit
+        self.inlet_pressure.unit = 'Pa'
+        value = self.inlet_pressure.value/(9.8 * density.value)
+        self.inlet_pressure.unit = old_p_unit
+        return prop.Length(value, "m")
+
+    @property
+    def head(self):
+        self = self._get_equipment_object(self)
+        if (self._outlet_material_stream_tag is None and
+            self._inlet_material_stream_tag is None):
+            raise Exception("Pump should be connected with MaterialStream either at inlet or outlet")
+        is_inlet = False if self._inlet_material_stream_index is None else True
+        density = self._connected_stream_property_getter(is_inlet, "material", "density")
+        density.unit = "kg/m^3"
+        dp = self.differential_pressure
+        dp.unit = "Pa"
+        value = dp.value / (9.8 * density.value)
+        return prop.Length(value, "m")
+    @property
+    def hydraulic_power(self):
+        self = self._get_equipment_object(self)
+        if (self._outlet_material_stream_tag is None and
+            self._inlet_material_stream_tag is None):
+            raise Exception("Centrifugal Pump should be connected with MaterialStream either at inlet or outlet")
+        is_inlet = False if self._inlet_material_stream_index is None else True
+        vol_flowrate = self._connected_stream_property_getter(is_inlet, "material", "vol_flowrate")
+        vol_flowrate.unit = "m^3/h"
+        dp = self.differential_pressure
+        dp.unit = "Pa"
+        value = vol_flowrate.value * dp.value / (3.6e3)
+        return prop.Power(value, 'W')
+    @property
+    def power(self):
+        self = self._get_equipment_object(self)
+        self.hydraulic_power.unit = "W"
+        value = self.hydraulic_power.value / self.efficiency.value
+        return prop.Power(value, "W")
+    @power.setter
+    def power(self, value):
+        #TODO Proived setting feature for power
+        raise Exception("Pump power value setting is not yet supported. Modify differential pressure to get required power.")
+    @property
+    def energy_in(self):
+        return self.power
+    @energy_in.setter
+    def energy_in(self, value):
+        # This is needed for property matching with the stream.
+        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self.energy_in.unit
+        self._energy_in = prop.Power(value, unit)
+        self._update_equipment_object(self)
+    
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+    
+    def connect_stream(self, 
+                       stream_object=None, 
+                       direction=None, 
+                       stream_tag=None, 
+                       stream_type=None,
+                       stream_governed=True):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'power', 'e', 'p']):
+            if direction is not None and 'out' in direction:
+                raise Exception('CentrifugalPump only supports energy inlet.')
+            direction = 'in'
+            stream_governed = False
+        return super().connect_stream(direction=direction, 
+                                      stream_object=stream_object, 
+                                      stream_tag=stream_tag, 
+                                      stream_type=stream_type,
+                                      stream_governed=stream_governed)
+    
+    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'power', 'e', 'p']):
+            if direction is not None and 'out' in direction:
+                raise Exception('CentrifugalPump only supports energy inlet.')
+            direction = 'in'
+            stream_type = "e"
+        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
+
+
+class PositiveDisplacementPump(_PressureChangers):
+    items = []
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Final class for creating objects to represent a Positive Displacement Pump.
+        
+        PARAMETERS:
+            Read _PressureChangers class for more arguments for this class
+            min_flow:
+                Required: No
+                Type: int/float or tuple(value, unit) or VolumetricFlowrate(recommended)
+                Acceptable values: Non-negative values
+                Default value: None # TODO: Add industry standard
+                Description: Minimum flow requirement of the pump
+
+            NPSHr:
+                Required: No
+                Type: int/float or tuple(value, unit) or Length(recommended)
+                Acceptable values: Non-negative values
+                Default value: None
+                Description: NPSHr of the pump
+        
+        PROPERTIES:
+            NPSHa:
+                Type: Length
+                Description: NPSH available to the pump.
+            
+            head:
+                Type: Length
+                Description: Differential head generated by the pump.
+
+            accel_head:
+                Type: Length
+                Description: Acceleration head loss at the inlet of pump.
+            
+            power/energy_in:
+                Type: Power
+                Description: Power required by the pump.
+
+        RETURN VALUE:
+            Type: PositiveDisplacementPump
+            Description: Returns an object of type PositiveDisplacementPump with all properties of
+                         a positive displacement pump used in process industries.
+        
+        ERROR RAISED:
+            Type:
+            Description:
+        
+        SAMPLE USE CASES:
+            >>> pump_1 = PositiveDisplacementlPump(tag="P1")
+            >>> print(pump_1)
+            Positive Displacement Pump with tag: P1
+        """
+        super().__init__( **inputs)
+        self._speed = prop.Frequency()
+        self._NPSHr = prop.Length()
+        if "NPSHr" in inputs:
+            self.NPSHr = inputs['NPSHr']
+        del self.energy_out
+
+        self._index = len(PositiveDisplacementPump.items)
+        PositiveDisplacementPump.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Positive Displacement Pump with tag: " + self.tag
+    def __hash__(self):
+        return hash(self.__repr__())
+    
+    @property
+    def NPSHa(self):
+        self = self._get_equipment_object(self)
+        if self._inlet_material_stream_tag is None:
+            raise Exception("Pump should be connected with MaterialStream at the inlet")
+        density = self._connected_stream_property_getter(True, "material", "density")
+        density.unit = "kg/m^3"
+        old_p_unit = self.inlet_pressure.unit
+        old_acc_head_unit = self.accel_head.unit
+        self.inlet_pressure.unit = self.accel_head = 'Pa'
+        
+        value = (self.inlet_pressure.value - self.accel_head.value)/(9.8 * density.value)
+        self.inlet_pressure.unit = old_p_unit
+        self.accel_head.unit = old_acc_head_unit
+        return prop.Length(value, "m")
+    @property
+    def NPSHr(self):
+        self = self._get_equipment_object(self)
+        return self._NPSHr
+    @NPSHr.setter
+    def NPSHr(self, value):
+        _Validators.validate_arg_prop_value_type("min_flow", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Pressure)
+        if unit is None:
+            unit = self._NPSHr.unit
+        self._NPSHr = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    
+    @property
+    def head(self):
+        self = self._get_equipment_object(self)
+        if (self._outlet_material_stream_tag is None and
+            self._inlet_material_stream_tag is None):
+            raise Exception("Pump should be connected with MaterialStream either at inlet or outlet")
+        is_inlet = False if self._inlet_material_stream_index is None else True
+        density = self._connected_stream_property_getter(is_inlet, "material", "density")
+        density.unit = "kg/m^3"
+        dp = self.differential_pressure
+        dp.unit = "Pa"
+        value = dp.value / (9.8 * density.value)
+        return prop.Length(value, "m")
+    
+    @property
+    def accel_head(self):
+        L, V = self._get_suction_length_velocity()
+        density = self._connected_stream_property_getter(True, "material", "density")
+        density.unit = "kg/m^3"
+        SG = density.value/1000
+        k = 1
+        head_loss = L.value * V.value * self.speed * SG / (k * 9.8) 
+        return prop.Length(head_loss, 'm')
+    
+    @property
+    def power(self):
+        self = self._get_equipment_object(self)
+        is_inlet = False if self._inlet_material_stream_index is None else True
+        vol_flow = self._connected_stream_property_getter(is_inlet, "material", "vol_flowrate")
+        vol_flow.unit = "gal/min"
+        old_dp_unit = self.differential_pressure.unit
+        self.differential_pressure.unit = 'psi'
+        value = vol_flow.value * self.differential_pressure.value /(1714 * self.efficiency.value)
+        return prop.Power(value, "hp")
+    @power.setter
+    def power(self, value):
+        #TODO Proived setting feature for power
+        raise Exception("Pump power value setting is not yet supported. Modify differential pressure to get required power.")
+    @property
+    def energy_in(self):
+        return self.power
+    @energy_in.setter
+    def energy_in(self, value):
+        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self.energy_in.unit
+        self._energy_in = prop.Power(value, unit)
+        self._update_equipment_object(self)
+        
+    
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+
+    def connect_stream(self, 
+                       stream_object=None, 
+                       direction=None, 
+                       stream_tag=None, 
+                       stream_type=None,
+                       stream_governed=True):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'power', 'e', 'p']):
+            if direction is not None and 'out' in direction:
+                raise Exception('PositiveDisplacementPump only supports energy inlet.')
+            direction = 'in'
+        return super().connect_stream(direction=direction, 
+                                      stream_object=stream_object, 
+                                      stream_tag=stream_tag, 
+                                      stream_type=stream_type,
+                                      stream_governed=stream_governed)
+    
+    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'power', 'e', 'p']):
+            if direction is not None and 'out' in direction:
+                raise Exception('PositiveDisplacementPump only supports energy inlet.')
+            direction = 'in'
+            stream_type = "e"
+        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
+# End of final classes of pumps
+
+# Start of final classes of Compressors and TurboExpanders.
+class CentrifugalCompressor(_GasPressureChangers):
+    items = []
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Final class for creating objects to represent a Centrifugal Compressors.
+        
+        PARAMETERS:
+            Read _PressureChangers class for more arguments for this class  
+            efficiency:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative values
+                Default value: 1.4
+                Description: Efficiency of the compressor. Efficency can be set as
+                             adiabatic/isentropic or polytropic efficiency.
+            
+            adiabatic_efficiency:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative values
+                Default value: 0.7
+                Description: Efficiency of the compressor considering adiabatic/isentropic
+                             compression.
+            
+            polytropic_efficiency:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative values
+                Default value: 0.7
+                Description: Efficiency of the compressor considering polytropic
+                             compression.
+
+            polytropic_exponent:
+                Required: No
+                Type: int or float (recommended)
+                Acceptable values: Non-negative values
+                Default value: 1.4
+                Description: Polytropic exponent of the gas.
+        
+        PROPERTIES:
+            power:
+                Type: Power
+                Description: Power required by the compressor.
+
+        
+        RETURN VALUE:
+            Type: CentrifugalCompressor
+            Description: Returns an object of type CentrifugalCompressor with all properties of
+                         a Centrifugal Compressor used in process industries.
+        
+        ERROR RAISED:
+            Type:
+            Description:
+        
+        SAMPLE USE CASES:
+            >>> CC_1 = CentrifugalCompressor(tag="P1")
+            >>> print(CC_1)
+            Centrifugal Compressor with tag: P1
+        """
+        super().__init__( **inputs)
+        del self.energy_out
+        self._index = len(CentrifugalCompressor.items)
+        CentrifugalCompressor.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Centrifugal Compressor with tag: " + self.tag
+    def __hash__(self):
+        return hash(self.__repr__())
+    
+    @property
+    def temperature_increase(self):
+        return super().temperature_change
+    
+    @property
+    def energy_in(self):
+        return self.power
+    @energy_in.setter
+    def energy_in(self, value):
+        # This is needed for property matching with the stream.
+        _Validators.validate_arg_prop_value_type("energy_in", value, (prop.Power, int, float, tuple))
+        _Validators.validate_non_negative_value("energy_in", value)
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self.energy_in.unit
+        self._energy_in = prop.Power(value, unit)
+        self._update_equipment_object(self)
+    
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+    
+    def connect_stream(self, 
+                       stream_object=None, 
+                       direction=None, 
+                       stream_tag=None, 
+                       stream_type=None,
+                       stream_governed=True):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'power', 'e', 'p']):
+            if direction is not None and 'out' in direction:
+                raise Exception('CentrifugalCompressor only supports energy inlet.')
+            direction = 'in'
+            stream_governed = False
+            stream_type = "e"
+        return super().connect_stream(direction=direction, 
+                                      stream_object=stream_object, 
+                                      stream_tag=stream_tag, 
+                                      stream_type=stream_type,
+                                      stream_governed=stream_governed)
+    
+    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'power', 'e', 'p']):
+            if direction is not None and 'out' in direction:
+                raise Exception('CentrifugalCompressor only supports energy inlet.')
+            direction = 'in'
+            stream_type = 'e'
+        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
+
+class TurboExpander(_GasPressureChangers):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__( **inputs)
+        del self.energy_in
+        self._index = len(TurboExpander.items)
+        TurboExpander.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "TurboExpander with tag: " + self.tag
+    def __hash__(self):
+        return hash(self.__repr__())
+
+    @property
+    def temperature_decrease(self):
+        return super().temperature_change
+    @property
+    def temperature_increase(self):
+        t_increase = super().temperature_change
+        t_increase.value *= -1
+        return t_increase
+
+    @property
+    def energy_out(self):
+        return self.power
+    @energy_out.setter
+    def energy_out(self, value):
+        # This is needed for property matching with the stream.
+        _Validators.validate_arg_prop_value_type("energy_out", value, (prop.Power, int, float, tuple))
+        _Validators.validate_non_negative_value("energy_out", value)
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Power)
+        if unit is None:
+            unit = self.energy_out.unit
+        self._energy_out = prop.Power(value, unit)
+        self._update_equipment_object(self)
+
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+    
+    def connect_stream(self,
+                       stream_object=None, 
+                       direction=None, 
+                       stream_tag=None, 
+                       stream_type=None,
+                       stream_governed=True):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'power', 'e', 'p']):
+            if direction is not None and 'in' in direction:
+                raise Exception('TurboExpander only supports energy outlet.')
+            direction = 'out'
+            stream_type = 'e'
+            stream_governed = False
+        return super().connect_stream(direction=direction, 
+                                      stream_object=stream_object, 
+                                      stream_tag=stream_tag, 
+                                      stream_type=stream_type,
+                                      stream_governed=stream_governed)
+    
+    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'power', 'e', 'p']):
+            if direction is not None and 'in' in direction:
+                raise Exception('TurboExpander only supports energy outlet.')
+            direction = 'out'
+            stream_type = 'e'
+        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
+
 # End of final classes of compressors
```

### Comparing `propylean-0.2.5/src/propylean/equipments/separators.py` & `propylean-0.2.6/src/propylean/equipments/separators.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from propylean.equipments.generic_equipment_classes import _VerticalVessels, _HorizontalVessels
-from propylean.settings import Settings
-from propylean.constants import Constants
-from propylean import properties as prop
-
-class VerticalSeparator(_VerticalVessels):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__( **inputs)
-        self._index = len(VerticalSeparator.items)
-        VerticalSeparator.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Vertical Separator with tag: " + self.tag   
-    def __hash__(self):
-        return hash(self.__repr__())
-
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-
-class HorizontalSeparator(_HorizontalVessels):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__( **inputs)
-        self._index = len(HorizontalSeparator.items)
-        HorizontalSeparator.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Horizontal Separator with tag: " + self.tag   
-    def __hash__(self):
-        return hash(self.__repr__())
-
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-
-class Column(_VerticalVessels):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__( **inputs)
-        self._index = len(Column.items)
-        Column.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Column with tag: " + self.tag   
-    def __hash__(self):
-        return hash(self.__repr__())
-    
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-
-class FlareKOD(_HorizontalVessels):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__(**inputs)
-        self._index = len(FlareKOD.items)
+from propylean.equipments.generic_equipment_classes import _VerticalVessels, _HorizontalVessels
+from propylean.settings import Settings
+from propylean.constants import Constants
+from propylean import properties as prop
+
+class VerticalSeparator(_VerticalVessels):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__( **inputs)
+        self._index = len(VerticalSeparator.items)
+        VerticalSeparator.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Vertical Separator with tag: " + self.tag   
+    def __hash__(self):
+        return hash(self.__repr__())
+
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+
+class HorizontalSeparator(_HorizontalVessels):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__( **inputs)
+        self._index = len(HorizontalSeparator.items)
+        HorizontalSeparator.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Horizontal Separator with tag: " + self.tag   
+    def __hash__(self):
+        return hash(self.__repr__())
+
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+
+class Column(_VerticalVessels):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__( **inputs)
+        self._index = len(Column.items)
+        Column.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Column with tag: " + self.tag   
+    def __hash__(self):
+        return hash(self.__repr__())
+    
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+
+class FlareKOD(_HorizontalVessels):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__(**inputs)
+        self._index = len(FlareKOD.items)
         FlareKOD.items.append(self)
```

### Comparing `propylean-0.2.5/src/propylean/equipments/static.py` & `propylean-0.2.6/src/propylean/equipments/static.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,456 +1,456 @@
-from propylean.equipments.generic_equipment_classes import _EquipmentOneInletOutlet
-from propylean.settings import Settings
-from propylean.constants import Constants
-from propylean import properties as prop
-from math import pi
-import pandas as pd
-from propylean.validators import _Validators
-
-class PipeSegment(_EquipmentOneInletOutlet):
-    items = []
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Final class for creating objects to represent a Pipe Segmenet.
-        
-        PARAMETERS:
-            Read _EquipmentOneInletOutlet class for more arguments for this class
-            ID:
-                Required: Yes, if OD and thickness not provided
-                Type: int or float or property.Lenght(recommended)
-                Acceptable values: Non-negative values
-                Default value: None
-                Description: Internal Diameter of the pipe segment.
-
-            OD:
-                Required: Yes, if ID not provided
-                Type: int or float or property.Lenght(recommended)
-                Acceptable values: Non-negative values
-                Default value: None
-                Description: Outer Diameter of the pipe segment.
-            
-            thickness:
-                Required: Yes, if ID not provided
-                Type: int or float or property.Lenght(recommended)
-                Acceptable values: Non-negative values
-                Default value: None
-                Description: Wall thickness of the pipe segment.
-            
-            length:
-                Required: Yes, for straight tube
-                Type: int or float or property.Lenght(recommended)
-                Acceptable values: Non-negative values
-                Default value: None
-                Description: length of the pipe segment.
-            
-            elevation:
-                Required: No
-                Type: int or float or property.Lenght(recommended)
-                Acceptable values: All values
-                Default value: 0 m
-                Description: elevation of the pipe segment.
-
-            segment_type:
-                Required: No
-                Type: int
-                Acceptable values: 1 to 13.
-                Default value: 1
-                Description: Segment type/fitting type of the pipe segment.
-            
-            material:
-                Required: No
-                Type: int
-                Acceptable values: 1 to 5.
-                Default value: 1
-                Description: Material type of the pipe segment.
-            
-            shape:
-                Required: Yes, only if segment_type is 12 or 13
-                Type: tuple
-                Description: Only in segment type is reducer or expander 
-            
-            segment_frame:
-                Required: No
-                Type: Pandas DataFrame
-                Description: List of PipeSegment objects in with columns as above arguments.
-                             >>> import pandas as pd
-                             For below list of segements, DataFrame to be created is as follows:
-                                +-----------------------------------------------------------------------------+
-                                | Segment Type   |  ID    |  length   |  material     | elevation  | Shape    |
-                                | Straight Tube  | 20 cm  |  10 m     | Carbon Steel  | 2 m down   |          |
-                                | Elbow          | 20 cm  |  NA       | Carbon Steel  | NA         |          |
-                                | Ball Valve     | 20 cm  |  NA       | Carbon Steel  | NA         |          |
-                                | Reducer        |        |  NA       | Carbon Steel  | NA         | (20, 18) |
-                                +-----------------------------------------------------------------------------+
-                                Note: OD and tickness can also be sepcified instead of ID. If all are provided,
-                                      ID will be considered
-                             >>> segment_frame = pd.DataFrame({'segment_type': [1, 2, 6, 12],
-                                                               'ID': [(20, 'cm'), (20, 'cm'), (20, 'cm'), (18, 'cm')],
-                                                               'length': [(10, 'm'), None, None, None],
-                                                               'material': [2, 2, 2, 2],
-                                                               'elevation': [(-2, 'm'), None, None, None],
-                                                               'shape': [None, None, None, (20, 18)]})
-        
-        RETURN VALUE:
-            Type: PipeSegment
-            Description: Returns an object of type PipeSegment with all properties of
-                         a pipe segments and fittings used in process industry piping.
-        
-        ERROR RAISED:
-            Type:
-            Description:
-        
-        SAMPLE USE CASES:
-            >>> PS_1 = PipeSegment(ID=(20, "cm"), 
-                                   OD=prop.Length(2200, "mm"),
-                                   length=10)
-            >>> print(PS_1)
-            Pipe Segment with tag: P1
-        """
-        super().__init__( **inputs)
-        self._pressure_drop = prop.Pressure(0)
-        self._ID = prop.Length()
-        self._OD = prop.Length()
-        self._length = prop.Length(0)
-        self._elevation = prop.Length(0)
-        self._segment_type = 1
-        self._material = 1
-        from pandas import DataFrame
-        self._segment_frame = DataFrame()
-        self._segment_obj_list = None
-        
-        if 'segment_frame' not in inputs:
-            del self.segment_frame
-            self.segment_type = 1 if 'segment_type' not in inputs else inputs['segment_type']
-            if self.segment_type == 1:
-                if 'length' in inputs:
-                    self.length = inputs['length']               
-                else:
-                    raise Exception('Straight Tube segment requires "length" value.')
-                if 'elevation' in inputs:
-                    self.elevation = inputs['elevation']
-            elif self.segment_type in range(12, 14):
-                self._shape = inputs['shape']
-            
-            if 'material' in inputs:
-                self.material = inputs['material']
-            
-            if ('ID' in inputs and inputs['ID'] is not None):
-                self.ID = inputs['ID']
-                if 'OD' in inputs and inputs['OD'] is not None:
-                    self.OD = inputs['OD']
-                elif 'thickness' in inputs and inputs['thickness'] is not None:
-                    self.thickness = inputs['thickness']
-            elif ('OD' in inputs and 'thickness' in inputs):
-                self.OD = inputs['OD']
-                self.ID = inputs['thickness']
-                self.ID = self.OD - self.ID
-            else:
-                raise Exception('Define atleast ID or OD with thickness to define a pipe segment object') 
-            
-        else:
-            self.segment_frame = inputs['segment_frame']   
-            self._segment_obj_list = []                                     
-            del self.ID
-            del self.OD
-            del self.material
-            del self.segment_type
-        self._index = len(PipeSegment.items)
-        PipeSegment.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Pipe Segment with tag: " + self.tag   #ADD SEGMENT TYPE!!
-    def __hash__(self):
-        return hash(self.__repr__())
-    
-    @property
-    def segment_frame(self):
-        self = self._get_equipment_object(self)
-        return self._segment_frame
-    @segment_frame.setter
-    def segment_frame(self, value):
-        _Validators.validate_arg_prop_value_type("segment_frame", value, pd.DataFrame)
-        self = self._get_equipment_object(self)
-        self._segment_frame = value
-        self._update_equipment_object(self)
-    @segment_frame.deleter
-    def segment_frame(self):
-        self = self._get_equipment_object(self)
-        del self._segment_frame
-        self._update_equipment_object(self)
-
-    @property
-    def length(self):
-        self = self._get_equipment_object(self)
-        return self._length
-    @length.setter
-    def length(self, value):
-        _Validators.validate_arg_prop_value_type("length", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._length.unit
-        self._length = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @property
-    def equivalent_length(self):
-        self = self._get_equipment_object(self)
-        ID = self.ID
-        ID.unit = 'm'
-        if self.material==5:
-            Le_by_D = Constants.Le_BY_D["plastic"]
-            if self.segment_type in range(13, 15):
-                Le_by_D = Constants.REDUCER_Le_BY_D_PLASTIC
-            else:
-                Le_by_D = Constants.REDUCER_Le_BY_D_STEEL
-        else:
-            Le_by_D = Constants.Le_BY_D["steel"]
-        if self.segment_type == 1:
-            equivalent_length = self.length
-        elif self.segment_type in range(2, 12):
-            equivalent_length = Le_by_D[self.segment_type-2] * ID.value
-            equivalent_length = prop.Length(equivalent_length)
-        elif self.segment_type in range(12, 14):
-            ratio = int(10*self._shape[1]/self._shape[0])
-            if ratio > 9:
-                ratio = 9
-            elif ratio < 4:
-                ratio = 4
-            equivalent_length = Le_by_D[ratio] * self._shape[0]
-            equivalent_length = prop.Length(equivalent_length)
-        return equivalent_length
-    @property
-    def elevation(self):
-        self = self._get_equipment_object(self)
-        return self._elevation
-    @elevation.setter
-    def elevation(self, value):
-        _Validators.validate_arg_prop_value_type("elevation", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._elevation.unit
-        self._elevation = prop.Length(value, unit)
-        self._update_equipment_object(self)
-
-    @property
-    def ID(self):
-        self = self._get_equipment_object(self)
-        return self._ID
-    @ID.setter
-    def ID(self, value):
-        _Validators.validate_arg_prop_value_type("ID", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._ID.unit
-        self._ID = prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @ID.deleter
-    def ID(self):
-        self = self._get_equipment_object(self)
-        del self._ID
-        self._update_equipment_object(self)
-    
-    @property
-    def OD(self):
-        self = self._get_equipment_object(self)
-        return self._OD
-    @OD.setter
-    def OD(self, value):
-        _Validators.validate_arg_prop_value_type("OD", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self._OD.unit
-        self._OD =prop.Length(value, unit)
-        self._update_equipment_object(self)
-    @OD.deleter
-    def OD(self):
-        self = self._get_equipment_object(self)
-        del self._OD
-        self._update_equipment_object(self)
-    
-    @property
-    def thickness(self):
-        self = self._get_equipment_object(self)
-        # if self._OD - self._ID <= prop.Length(0):
-        #     raise Exception("ID is not less than OD! Change ID or OD or thickness.")
-        return self._OD - self._ID
-    @thickness.setter
-    def thickness(self, value):
-        _Validators.validate_arg_prop_value_type("thickness", value, (prop.Length, int, float, tuple))
-        self = self._get_equipment_object(self)
-        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
-        if unit is None:
-            unit = self.thickness
-        self._OD = self._ID + prop.Length(value, unit)
-        self._update_equipment_object(self)
-
-    @property
-    def segment_type(self):
-        self = self._get_equipment_object(self)
-        return self._segment_type
-    @segment_type.setter
-    def segment_type(self, value):
-        _Validators.validate_arg_prop_value_type("segment_type", value, int)
-        _Validators.validate_arg_prop_value_range("segment_type", value, [1, 13])
-        self = self._get_equipment_object(self)
-        segments = '''\nSegments can be of following types and in range of numbers below:
-                    1. Straight Tube
-                    2. Elbow
-                    3. Tee (straight through)
-                    4. Tee (through branch)
-                    5. Butterfly valve 
-                    6. Ball valve (full bore)
-                    7. Gate valve(full open)
-                    8. Globe valve (full open)
-                    9. Swing check valve
-                    10. Wafer disk check valve
-                    11. Lift check valve
-                    12. Reducer
-                    13. Expander'''
-        if value not in range(1,14):
-            raise Exception(segments)
-        self._segment_type = value
-        self._update_equipment_object(self)
-    @segment_type.deleter
-    def segment_type(self):
-        self = self._get_equipment_object(self)
-        del self._segment_type
-        self._update_equipment_object(self)
-    
-    @property
-    def material(self):
-        self = self._get_equipment_object(self)
-        return self._material
-    @material.setter
-    def material(self, value):
-        _Validators.validate_arg_prop_value_type("material", value, int)
-        _Validators.validate_arg_prop_value_range("material", value, [1, 5])
-        self = self._get_equipment_object(self)
-        materials = '''\nSegment material can be of following types and in range of numbers below:
-                    1. Raw Steel
-                    2. Carbon Steel
-                    3. Cast Iron
-                    4. Stainless Steel
-                    5. PVC''' 
-        if value not in range(1, 6):
-            raise Exception(materials)
-        self._material = value
-        self._update_equipment_object(self)
-    @material.deleter
-    def material(self):
-        self = self._get_equipment_object(self)
-        del self._material
-        self._update_equipment_object(self)
-
-    @property
-    def pressure_drop(self):
-        self = self._get_equipment_object(self)
-        pressure_drop = prop.Pressure(0, self.inlet_pressure.unit)
-        if self.inlet_mass_flowrate.value == 0:
-            return prop.Pressure(0, self._inlet_pressure.unit)
-        if (self._outlet_material_stream_tag is None and
-            self._inlet_material_stream_tag is None):
-            raise Exception("PipeSegment should be connected with MaterialStream either at inlet or outlet")
-       
-        is_inlet = False if self._inlet_material_stream_index is None else True
-        density = self._connected_stream_property_getter(is_inlet, "material", "density")
-        viscosity = self._connected_stream_property_getter(is_inlet, "material", "d_viscosity")
-        vol_flowrate = self._connected_stream_property_getter(is_inlet, "material", "vol_flowrate")
-        density.unit = "kg/m^3"
-        viscosity.unit = "Pa-s"
-        vol_flowrate.unit = "m^3/s"
-        if self._segment_obj_list is None:
-            ID = self.ID
-            ID.unit = 'm'
-            length = self.equivalent_length
-            length.unit = 'm'
-            drop_friction = self.dp_friction(vol_flowrate, ID, length, density, viscosity)
-            drop_hydrostatic = self.dp_hydrostatic(density)
-            pressure_drop = drop_friction + drop_hydrostatic
-        else:
-            for column in ['segment_type', 'ID', 'OD', 'thickness', 'length', 'material', 'elevation', 'shape']:
-                if column not in list(self.segment_frame.columns):
-                    self.segment_frame[column] = None
-            rows = zip(self.segment_frame['segment_type'],
-                        self.segment_frame['ID'],
-                        self.segment_frame['OD'],
-                        self.segment_frame['thickness'],
-                        self.segment_frame['length'],
-                        self.segment_frame['material'],
-                        self.segment_frame['elevation'],
-                        self.segment_frame['shape'])
-            for row in rows:
-                ps = PipeSegment(segment_type=row[0],
-                                 ID=row[1],
-                                 OD=row[2],
-                                 thickness=row[3],
-                                 length=row[4],
-                                 material=row[5],
-                                 elevation=row[6],
-                                 shape=row[7])
-                ID = ps.ID
-                ID.unit = 'm'
-                length = ps.equivalent_length
-                length.unit = 'm'
-                drop_friction = ps.dp_friction(vol_flowrate, ID, length, density, viscosity)
-                drop_hydrostatic = ps.dp_hydrostatic(density)
-                pressure_drop += drop_friction + drop_hydrostatic
-        return pressure_drop
-        
-    @pressure_drop.setter
-    def pressure_drop(self, value):
-        raise Exception('''Cannot manually set pressure drop for PipeSegment!\n
-                         Pressure drop depends on physical properties of the PipeSegment and MaterialStream connected.''')
-    
-    def dp_hydrostatic(self, density):
-        self = self._get_equipment_object(self)
-        elevation_old_unit = self.elevation.unit
-        self.elevation.unit = "m"
-        hydro_drop = prop.Pressure(self.elevation.value * density.value * 9.8)
-        hydro_drop.unit = self.inlet_pressure.unit
-        self.elevation.unit = elevation_old_unit
-        return hydro_drop
-
-    def dp_friction(self, vol_flowrate, ID, length, density, viscosity,
-                    method=Settings.pipe_dp_method, Darcy=Settings.Darcy):
-        self = self._get_equipment_object(self)
-        from fluids.friction import friction_factor
-        from fluids.core import Reynolds, K_from_f, dP_from_K
-        from propylean.constants import Constants
-
-        V=(vol_flowrate.value)/(pi* ID.value**2)/4
-        Re = Reynolds(V=V,
-                    D=ID.value, 
-                    rho=density.value, 
-                    mu=viscosity.value)
-        fd = friction_factor(Re=Re, 
-                            eD=Constants.ROUGHNESS[self.material-1]/ID.value,
-                            Method=method,
-                            Darcy=Darcy)
-        K = K_from_f(fd=fd, L=length.value, D=ID.value)        
-        drop = round(dP_from_K(K, rho=1000, V=V),3)
-        drop = prop.Pressure(drop, 'Pa')
-        drop.unit = self._inlet_pressure.unit
-        return drop
-            
-    @classmethod
-    def list_objects(cls):
-        return cls.items
-
-class Strainers(_EquipmentOneInletOutlet):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__(**inputs)
-        self._index = len(Strainers.items)
-        Strainers.items.append(self)
-        
-class Filters(_EquipmentOneInletOutlet):
-    items = []
-    def __init__(self, **inputs) -> None:
-        super().__init__(**inputs)
-        self._index = len(Filters.items)
+from propylean.equipments.generic_equipment_classes import _EquipmentOneInletOutlet
+from propylean.settings import Settings
+from propylean.constants import Constants
+from propylean import properties as prop
+from math import pi
+import pandas as pd
+from propylean.validators import _Validators
+
+class PipeSegment(_EquipmentOneInletOutlet):
+    items = []
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Final class for creating objects to represent a Pipe Segmenet.
+        
+        PARAMETERS:
+            Read _EquipmentOneInletOutlet class for more arguments for this class
+            ID:
+                Required: Yes, if OD and thickness not provided
+                Type: int or float or property.Lenght(recommended)
+                Acceptable values: Non-negative values
+                Default value: None
+                Description: Internal Diameter of the pipe segment.
+
+            OD:
+                Required: Yes, if ID not provided
+                Type: int or float or property.Lenght(recommended)
+                Acceptable values: Non-negative values
+                Default value: None
+                Description: Outer Diameter of the pipe segment.
+            
+            thickness:
+                Required: Yes, if ID not provided
+                Type: int or float or property.Lenght(recommended)
+                Acceptable values: Non-negative values
+                Default value: None
+                Description: Wall thickness of the pipe segment.
+            
+            length:
+                Required: Yes, for straight tube
+                Type: int or float or property.Lenght(recommended)
+                Acceptable values: Non-negative values
+                Default value: None
+                Description: length of the pipe segment.
+            
+            elevation:
+                Required: No
+                Type: int or float or property.Lenght(recommended)
+                Acceptable values: All values
+                Default value: 0 m
+                Description: elevation of the pipe segment.
+
+            segment_type:
+                Required: No
+                Type: int
+                Acceptable values: 1 to 13.
+                Default value: 1
+                Description: Segment type/fitting type of the pipe segment.
+            
+            material:
+                Required: No
+                Type: int
+                Acceptable values: 1 to 5.
+                Default value: 1
+                Description: Material type of the pipe segment.
+            
+            shape:
+                Required: Yes, only if segment_type is 12 or 13
+                Type: tuple
+                Description: Only in segment type is reducer or expander 
+            
+            segment_frame:
+                Required: No
+                Type: Pandas DataFrame
+                Description: List of PipeSegment objects in with columns as above arguments.
+                             >>> import pandas as pd
+                             For below list of segements, DataFrame to be created is as follows:
+                                +-----------------------------------------------------------------------------+
+                                | Segment Type   |  ID    |  length   |  material     | elevation  | Shape    |
+                                | Straight Tube  | 20 cm  |  10 m     | Carbon Steel  | 2 m down   |          |
+                                | Elbow          | 20 cm  |  NA       | Carbon Steel  | NA         |          |
+                                | Ball Valve     | 20 cm  |  NA       | Carbon Steel  | NA         |          |
+                                | Reducer        |        |  NA       | Carbon Steel  | NA         | (20, 18) |
+                                +-----------------------------------------------------------------------------+
+                                Note: OD and tickness can also be sepcified instead of ID. If all are provided,
+                                      ID will be considered
+                             >>> segment_frame = pd.DataFrame({'segment_type': [1, 2, 6, 12],
+                                                               'ID': [(20, 'cm'), (20, 'cm'), (20, 'cm'), (18, 'cm')],
+                                                               'length': [(10, 'm'), None, None, None],
+                                                               'material': [2, 2, 2, 2],
+                                                               'elevation': [(-2, 'm'), None, None, None],
+                                                               'shape': [None, None, None, (20, 18)]})
+        
+        RETURN VALUE:
+            Type: PipeSegment
+            Description: Returns an object of type PipeSegment with all properties of
+                         a pipe segments and fittings used in process industry piping.
+        
+        ERROR RAISED:
+            Type:
+            Description:
+        
+        SAMPLE USE CASES:
+            >>> PS_1 = PipeSegment(ID=(20, "cm"), 
+                                   OD=prop.Length(2200, "mm"),
+                                   length=10)
+            >>> print(PS_1)
+            Pipe Segment with tag: P1
+        """
+        super().__init__( **inputs)
+        self._pressure_drop = prop.Pressure(0)
+        self._ID = prop.Length()
+        self._OD = prop.Length()
+        self._length = prop.Length(0)
+        self._elevation = prop.Length(0)
+        self._segment_type = 1
+        self._material = 1
+        from pandas import DataFrame
+        self._segment_frame = DataFrame()
+        self._segment_obj_list = None
+        
+        if 'segment_frame' not in inputs:
+            del self.segment_frame
+            self.segment_type = 1 if 'segment_type' not in inputs else inputs['segment_type']
+            if self.segment_type == 1:
+                if 'length' in inputs:
+                    self.length = inputs['length']               
+                else:
+                    raise Exception('Straight Tube segment requires "length" value.')
+                if 'elevation' in inputs:
+                    self.elevation = inputs['elevation']
+            elif self.segment_type in range(12, 14):
+                self._shape = inputs['shape']
+            
+            if 'material' in inputs:
+                self.material = inputs['material']
+            
+            if ('ID' in inputs and inputs['ID'] is not None):
+                self.ID = inputs['ID']
+                if 'OD' in inputs and inputs['OD'] is not None:
+                    self.OD = inputs['OD']
+                elif 'thickness' in inputs and inputs['thickness'] is not None:
+                    self.thickness = inputs['thickness']
+            elif ('OD' in inputs and 'thickness' in inputs):
+                self.OD = inputs['OD']
+                self.ID = inputs['thickness']
+                self.ID = self.OD - self.ID
+            else:
+                raise Exception('Define atleast ID or OD with thickness to define a pipe segment object') 
+            
+        else:
+            self.segment_frame = inputs['segment_frame']   
+            self._segment_obj_list = []                                     
+            del self.ID
+            del self.OD
+            del self.material
+            del self.segment_type
+        self._index = len(PipeSegment.items)
+        PipeSegment.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Pipe Segment with tag: " + self.tag   #ADD SEGMENT TYPE!!
+    def __hash__(self):
+        return hash(self.__repr__())
+    
+    @property
+    def segment_frame(self):
+        self = self._get_equipment_object(self)
+        return self._segment_frame
+    @segment_frame.setter
+    def segment_frame(self, value):
+        _Validators.validate_arg_prop_value_type("segment_frame", value, pd.DataFrame)
+        self = self._get_equipment_object(self)
+        self._segment_frame = value
+        self._update_equipment_object(self)
+    @segment_frame.deleter
+    def segment_frame(self):
+        self = self._get_equipment_object(self)
+        del self._segment_frame
+        self._update_equipment_object(self)
+
+    @property
+    def length(self):
+        self = self._get_equipment_object(self)
+        return self._length
+    @length.setter
+    def length(self, value):
+        _Validators.validate_arg_prop_value_type("length", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._length.unit
+        self._length = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @property
+    def equivalent_length(self):
+        self = self._get_equipment_object(self)
+        ID = self.ID
+        ID.unit = 'm'
+        if self.material==5:
+            Le_by_D = Constants.Le_BY_D["plastic"]
+            if self.segment_type in range(13, 15):
+                Le_by_D = Constants.REDUCER_Le_BY_D_PLASTIC
+            else:
+                Le_by_D = Constants.REDUCER_Le_BY_D_STEEL
+        else:
+            Le_by_D = Constants.Le_BY_D["steel"]
+        if self.segment_type == 1:
+            equivalent_length = self.length
+        elif self.segment_type in range(2, 12):
+            equivalent_length = Le_by_D[self.segment_type-2] * ID.value
+            equivalent_length = prop.Length(equivalent_length)
+        elif self.segment_type in range(12, 14):
+            ratio = int(10*self._shape[1]/self._shape[0])
+            if ratio > 9:
+                ratio = 9
+            elif ratio < 4:
+                ratio = 4
+            equivalent_length = Le_by_D[ratio] * self._shape[0]
+            equivalent_length = prop.Length(equivalent_length)
+        return equivalent_length
+    @property
+    def elevation(self):
+        self = self._get_equipment_object(self)
+        return self._elevation
+    @elevation.setter
+    def elevation(self, value):
+        _Validators.validate_arg_prop_value_type("elevation", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._elevation.unit
+        self._elevation = prop.Length(value, unit)
+        self._update_equipment_object(self)
+
+    @property
+    def ID(self):
+        self = self._get_equipment_object(self)
+        return self._ID
+    @ID.setter
+    def ID(self, value):
+        _Validators.validate_arg_prop_value_type("ID", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._ID.unit
+        self._ID = prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @ID.deleter
+    def ID(self):
+        self = self._get_equipment_object(self)
+        del self._ID
+        self._update_equipment_object(self)
+    
+    @property
+    def OD(self):
+        self = self._get_equipment_object(self)
+        return self._OD
+    @OD.setter
+    def OD(self, value):
+        _Validators.validate_arg_prop_value_type("OD", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self._OD.unit
+        self._OD =prop.Length(value, unit)
+        self._update_equipment_object(self)
+    @OD.deleter
+    def OD(self):
+        self = self._get_equipment_object(self)
+        del self._OD
+        self._update_equipment_object(self)
+    
+    @property
+    def thickness(self):
+        self = self._get_equipment_object(self)
+        # if self._OD - self._ID <= prop.Length(0):
+        #     raise Exception("ID is not less than OD! Change ID or OD or thickness.")
+        return self._OD - self._ID
+    @thickness.setter
+    def thickness(self, value):
+        _Validators.validate_arg_prop_value_type("thickness", value, (prop.Length, int, float, tuple))
+        self = self._get_equipment_object(self)
+        value, unit = self._tuple_property_value_unit_returner(value, prop.Length)
+        if unit is None:
+            unit = self.thickness
+        self._OD = self._ID + prop.Length(value, unit)
+        self._update_equipment_object(self)
+
+    @property
+    def segment_type(self):
+        self = self._get_equipment_object(self)
+        return self._segment_type
+    @segment_type.setter
+    def segment_type(self, value):
+        _Validators.validate_arg_prop_value_type("segment_type", value, int)
+        _Validators.validate_arg_prop_value_range("segment_type", value, [1, 13])
+        self = self._get_equipment_object(self)
+        segments = '''\nSegments can be of following types and in range of numbers below:
+                    1. Straight Tube
+                    2. Elbow
+                    3. Tee (straight through)
+                    4. Tee (through branch)
+                    5. Butterfly valve 
+                    6. Ball valve (full bore)
+                    7. Gate valve(full open)
+                    8. Globe valve (full open)
+                    9. Swing check valve
+                    10. Wafer disk check valve
+                    11. Lift check valve
+                    12. Reducer
+                    13. Expander'''
+        if value not in range(1,14):
+            raise Exception(segments)
+        self._segment_type = value
+        self._update_equipment_object(self)
+    @segment_type.deleter
+    def segment_type(self):
+        self = self._get_equipment_object(self)
+        del self._segment_type
+        self._update_equipment_object(self)
+    
+    @property
+    def material(self):
+        self = self._get_equipment_object(self)
+        return self._material
+    @material.setter
+    def material(self, value):
+        _Validators.validate_arg_prop_value_type("material", value, int)
+        _Validators.validate_arg_prop_value_range("material", value, [1, 5])
+        self = self._get_equipment_object(self)
+        materials = '''\nSegment material can be of following types and in range of numbers below:
+                    1. Raw Steel
+                    2. Carbon Steel
+                    3. Cast Iron
+                    4. Stainless Steel
+                    5. PVC''' 
+        if value not in range(1, 6):
+            raise Exception(materials)
+        self._material = value
+        self._update_equipment_object(self)
+    @material.deleter
+    def material(self):
+        self = self._get_equipment_object(self)
+        del self._material
+        self._update_equipment_object(self)
+
+    @property
+    def pressure_drop(self):
+        self = self._get_equipment_object(self)
+        pressure_drop = prop.Pressure(0, self.inlet_pressure.unit)
+        if self.inlet_mass_flowrate.value == 0:
+            return prop.Pressure(0, self._inlet_pressure.unit)
+        if (self._outlet_material_stream_tag is None and
+            self._inlet_material_stream_tag is None):
+            raise Exception("PipeSegment should be connected with MaterialStream either at inlet or outlet")
+       
+        is_inlet = False if self._inlet_material_stream_index is None else True
+        density = self._connected_stream_property_getter(is_inlet, "material", "density")
+        viscosity = self._connected_stream_property_getter(is_inlet, "material", "d_viscosity")
+        vol_flowrate = self._connected_stream_property_getter(is_inlet, "material", "vol_flowrate")
+        density.unit = "kg/m^3"
+        viscosity.unit = "Pa-s"
+        vol_flowrate.unit = "m^3/s"
+        if self._segment_obj_list is None:
+            ID = self.ID
+            ID.unit = 'm'
+            length = self.equivalent_length
+            length.unit = 'm'
+            drop_friction = self.dp_friction(vol_flowrate, ID, length, density, viscosity)
+            drop_hydrostatic = self.dp_hydrostatic(density)
+            pressure_drop = drop_friction + drop_hydrostatic
+        else:
+            for column in ['segment_type', 'ID', 'OD', 'thickness', 'length', 'material', 'elevation', 'shape']:
+                if column not in list(self.segment_frame.columns):
+                    self.segment_frame[column] = None
+            rows = zip(self.segment_frame['segment_type'],
+                        self.segment_frame['ID'],
+                        self.segment_frame['OD'],
+                        self.segment_frame['thickness'],
+                        self.segment_frame['length'],
+                        self.segment_frame['material'],
+                        self.segment_frame['elevation'],
+                        self.segment_frame['shape'])
+            for row in rows:
+                ps = PipeSegment(segment_type=row[0],
+                                 ID=row[1],
+                                 OD=row[2],
+                                 thickness=row[3],
+                                 length=row[4],
+                                 material=row[5],
+                                 elevation=row[6],
+                                 shape=row[7])
+                ID = ps.ID
+                ID.unit = 'm'
+                length = ps.equivalent_length
+                length.unit = 'm'
+                drop_friction = ps.dp_friction(vol_flowrate, ID, length, density, viscosity)
+                drop_hydrostatic = ps.dp_hydrostatic(density)
+                pressure_drop += drop_friction + drop_hydrostatic
+        return pressure_drop
+        
+    @pressure_drop.setter
+    def pressure_drop(self, value):
+        raise Exception('''Cannot manually set pressure drop for PipeSegment!\n
+                         Pressure drop depends on physical properties of the PipeSegment and MaterialStream connected.''')
+    
+    def dp_hydrostatic(self, density):
+        self = self._get_equipment_object(self)
+        elevation_old_unit = self.elevation.unit
+        self.elevation.unit = "m"
+        hydro_drop = prop.Pressure(self.elevation.value * density.value * 9.8)
+        hydro_drop.unit = self.inlet_pressure.unit
+        self.elevation.unit = elevation_old_unit
+        return hydro_drop
+
+    def dp_friction(self, vol_flowrate, ID, length, density, viscosity,
+                    method=Settings.pipe_dp_method, Darcy=Settings.Darcy):
+        self = self._get_equipment_object(self)
+        from fluids.friction import friction_factor
+        from fluids.core import Reynolds, K_from_f, dP_from_K
+        from propylean.constants import Constants
+
+        V=(vol_flowrate.value)/(pi* ID.value**2)/4
+        Re = Reynolds(V=V,
+                    D=ID.value, 
+                    rho=density.value, 
+                    mu=viscosity.value)
+        fd = friction_factor(Re=Re, 
+                            eD=Constants.ROUGHNESS[self.material-1]/ID.value,
+                            Method=method,
+                            Darcy=Darcy)
+        K = K_from_f(fd=fd, L=length.value, D=ID.value)        
+        drop = round(dP_from_K(K, rho=1000, V=V),3)
+        drop = prop.Pressure(drop, 'Pa')
+        drop.unit = self._inlet_pressure.unit
+        return drop
+            
+    @classmethod
+    def list_objects(cls):
+        return cls.items
+
+class Strainers(_EquipmentOneInletOutlet):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__(**inputs)
+        self._index = len(Strainers.items)
+        Strainers.items.append(self)
+        
+class Filters(_EquipmentOneInletOutlet):
+    items = []
+    def __init__(self, **inputs) -> None:
+        super().__init__(**inputs)
+        self._index = len(Filters.items)
         Filters.items.append(self)
```

### Comparing `propylean-0.2.5/src/propylean/instruments/control.py` & `propylean-0.2.6/src/propylean/instruments/control.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-from propylean import streams
-import propylean.properties as prop
-from propylean.equipments.generic_equipment_classes import _EquipmentOneInletOutlet
-from propylean.settings import Settings
-from propylean.constants import Constants
-from fluids import control_valve as cv_calculations
-
-class ControlValve(_EquipmentOneInletOutlet):
-    items = []
-    def __init__(self, **inputs) -> None:
-        """ 
-        DESCRIPTION:
-            Final class for creating objects to represent a Control Valve.
-        
-        PARAMETERS:
-            Read _EquipmentOneInletOutlet class for more arguments for this class
-        
-        RETURN VALUE:
-            Type: ControlValve
-            Description: Returns an object of type ControlValve with all properties of
-                         a control valve used in process industry.
-        
-        ERROR RAISED:
-            Type:
-            Description:
-        
-        SAMPLE USE CASES:
-            >>> CV_1 = ControlValve(tag="CV1")
-            >>> print(CV_1)
-            Contrl Valve with tag: CV1
-        """
-        super().__init__( **inputs)
-        del self.energy_in
-        del self.energy_out
-        self._index = len(ControlValve.items)
-        ControlValve.items.append(self)
-    
-    def __repr__(self):
-        self = self._get_equipment_object(self)
-        return "Control Valve with tag: " + self.tag   
-    def __hash__(self):
-        return hash(self.__repr__())
-
-    @property
-    def Cv(self):
-        self = self._get_equipment_object(self)
-        if (self._outlet_material_stream_tag is None and
-            self._inlet_material_stream_tag is None):
-            raise Exception("PipeSegment should be connected with MaterialStream either at inlet or outlet")
-        P1 = self.inlet_pressure
-        P2 = self.outlet_pressure
-        P1.unit = P2.unit = "Pa"
-        is_inlet = True if self._outlet_material_stream_tag is None else False
-        density = self._connected_stream_property_getter(is_inlet, "material", "density")
-        phase = self._connected_stream_property_getter(is_inlet, "material", "phase")
-        d_viscosity = self._connected_stream_property_getter(is_inlet, "material", "d_viscosity")
-        isentropic_exponent = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
-        MW = self._connected_stream_property_getter(is_inlet, "material", "molecular_weight")
-        Psat = self._connected_stream_property_getter(is_inlet, "material", "Psat")
-        Pc = self._connected_stream_property_getter(is_inlet, "material", "Pc")
-        if phase == 'l':
-            return cv_calculations.size_control_valve_l(density.value, Psat.value, Pc.value, d_viscosity.value,
-                                                        P1.value, P2.value, 
-                                                        self.inlet_mass_flowrate.value/density.value)
-        elif phase == 'g' or phase == 'l/g':
-            Z_g = self._connected_stream_property_getter(is_inlet, "material", "Z_g")
-            return cv_calculations.size_control_valve_g(T = self.inlet_temperature.value, 
-                                                        MW = MW.value,
-                                                        mu= d_viscosity.value,
-                                                        gamma = isentropic_exponent, 
-                                                        Z = Z_g,
-                                                        P1 = P1.value, 
-                                                        P2 = P2.value, 
-                                                        Q = self.inlet_mass_flowrate.value/density.value)
-        else:
-            raise Exception('Possibility of fluid solification inside the control valve')
-
-    def connect_stream(self, 
-                       stream_object=None, 
-                       direction=None, 
-                       stream_tag=None, 
-                       stream_type=None,
-                       stream_governed=True):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'e']):
-            raise Exception("No energy stream is associated  with control valve.")
-        return super().connect_stream(direction=direction, 
-                                      stream_object=stream_object, 
-                                      stream_tag=stream_tag, 
-                                      stream_type=stream_type,
-                                      stream_governed=stream_governed)
-    
-    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
-        if ((stream_object is not None and 
-            isinstance(stream_object, streams.EnergyStream)) or
-            stream_type in ['energy', 'e']):
-            raise Exception("No energy stream is associated  with control valve.")
-        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
-
-    @classmethod
-    def list_objects(cls):
-        return cls.items
+from propylean import streams
+import propylean.properties as prop
+from propylean.equipments.generic_equipment_classes import _EquipmentOneInletOutlet
+from propylean.settings import Settings
+from propylean.constants import Constants
+from fluids import control_valve as cv_calculations
+
+class ControlValve(_EquipmentOneInletOutlet):
+    items = []
+    def __init__(self, **inputs) -> None:
+        """ 
+        DESCRIPTION:
+            Final class for creating objects to represent a Control Valve.
+        
+        PARAMETERS:
+            Read _EquipmentOneInletOutlet class for more arguments for this class
+        
+        RETURN VALUE:
+            Type: ControlValve
+            Description: Returns an object of type ControlValve with all properties of
+                         a control valve used in process industry.
+        
+        ERROR RAISED:
+            Type:
+            Description:
+        
+        SAMPLE USE CASES:
+            >>> CV_1 = ControlValve(tag="CV1")
+            >>> print(CV_1)
+            Contrl Valve with tag: CV1
+        """
+        super().__init__( **inputs)
+        del self.energy_in
+        del self.energy_out
+        self._index = len(ControlValve.items)
+        ControlValve.items.append(self)
+    
+    def __repr__(self):
+        self = self._get_equipment_object(self)
+        return "Control Valve with tag: " + self.tag   
+    def __hash__(self):
+        return hash(self.__repr__())
+
+    @property
+    def Cv(self):
+        self = self._get_equipment_object(self)
+        if (self._outlet_material_stream_tag is None and
+            self._inlet_material_stream_tag is None):
+            raise Exception("PipeSegment should be connected with MaterialStream either at inlet or outlet")
+        P1 = self.inlet_pressure
+        P2 = self.outlet_pressure
+        P1.unit = P2.unit = "Pa"
+        is_inlet = True if self._outlet_material_stream_tag is None else False
+        density = self._connected_stream_property_getter(is_inlet, "material", "density")
+        phase = self._connected_stream_property_getter(is_inlet, "material", "phase")
+        d_viscosity = self._connected_stream_property_getter(is_inlet, "material", "d_viscosity")
+        isentropic_exponent = self._connected_stream_property_getter(is_inlet, "material", "isentropic_exponent")
+        MW = self._connected_stream_property_getter(is_inlet, "material", "molecular_weight")
+        Psat = self._connected_stream_property_getter(is_inlet, "material", "Psat")
+        Pc = self._connected_stream_property_getter(is_inlet, "material", "Pc")
+        if phase == 'l':
+            return cv_calculations.size_control_valve_l(density.value, Psat.value, Pc.value, d_viscosity.value,
+                                                        P1.value, P2.value, 
+                                                        self.inlet_mass_flowrate.value/density.value)
+        elif phase == 'g' or phase == 'l/g':
+            Z_g = self._connected_stream_property_getter(is_inlet, "material", "Z_g")
+            return cv_calculations.size_control_valve_g(T = self.inlet_temperature.value, 
+                                                        MW = MW.value,
+                                                        mu= d_viscosity.value,
+                                                        gamma = isentropic_exponent, 
+                                                        Z = Z_g,
+                                                        P1 = P1.value, 
+                                                        P2 = P2.value, 
+                                                        Q = self.inlet_mass_flowrate.value/density.value)
+        else:
+            raise Exception('Possibility of fluid solification inside the control valve')
+
+    def connect_stream(self, 
+                       stream_object=None, 
+                       direction=None, 
+                       stream_tag=None, 
+                       stream_type=None,
+                       stream_governed=True):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'e']):
+            raise Exception("No energy stream is associated  with control valve.")
+        return super().connect_stream(direction=direction, 
+                                      stream_object=stream_object, 
+                                      stream_tag=stream_tag, 
+                                      stream_type=stream_type,
+                                      stream_governed=stream_governed)
+    
+    def disconnect_stream(self, stream_object=None, direction=None, stream_tag=None, stream_type=None):
+        if ((stream_object is not None and 
+            isinstance(stream_object, streams.EnergyStream)) or
+            stream_type in ['energy', 'e']):
+            raise Exception("No energy stream is associated  with control valve.")
+        return super().disconnect_stream(stream_object, direction, stream_tag, stream_type)
+
+    @classmethod
+    def list_objects(cls):
+        return cls.items
```

### Comparing `propylean-0.2.5/src/propylean/properties.py` & `propylean-0.2.6/src/propylean/properties.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,586 +1,547 @@
-from pandas import Series, DataFrame
-from propylean.validators import _Validators
-from propylean.constants import ConversionFactors
-from warnings import warn
-
-class _Property(object):
-    def __init__(self, value=None, unit=None, time_series=None, min_val=None, max_val=None):
-        _Validators.validate_arg_prop_value_type("value", value, (int, float))
-        _Validators.validate_arg_prop_value_type("unit", unit, str)
-        _Validators.validate_arg_prop_value_type("time_series", time_series, 
-            (Series, DataFrame, dict))
-        self._value = value
-        self._min_val = min_val
-        self._max_val = max_val
-        self._unit = unit
-        self._time_series = time_series
-    def __eq__(self, other):
-        if (isinstance(other, _Property) and
-            self.value == other.value and
-            self.unit == other.unit):
-                return True
-        return False
-    @property
-    def value(self):
-        return self._value
-    @value.setter
-    def value(self, value):
-        _Validators.validate_arg_prop_value_type("value", value, (int, float))
-        self._value = value
-    
-    @property
-    def max_val(self):
-        return self._max_val if self._max_val is not None else self._value
-    @max_val.setter
-    def max_val(self, value):
-        _Validators.validate_arg_prop_value_type("max_val", value, (int, float))
-        self._max_val = value
-    
-    @property
-    def min_val(self):
-        return self._min_val if self._min_val is not None else self._value
-    @min_val.setter
-    def min_val(self, value):
-        _Validators.validate_arg_prop_value_type("min_val", value, (int, float))
-        self._min_val = value
-    
-    @property
-    def unit(self):
-        return self._unit
-    @unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        self._unit = unit
-    
-    @property
-    def time_series(self):
-        return self._time_series
-    @time_series.setter
-    def time_series(self, time_series):
-        _Validators.validate_arg_prop_value_type("time_series", time_series, 
-            (Series, DataFrame, dict))
-            
-        if isinstance(time_series, dict):
-            time_series = Series(data=time_series, index=list(time_series.keys()))
-        elif isinstance(time_series, DataFrame):
-            if len(time_series.columns) == 2:
-                time_index = time_series[time_series.columns[0]]
-                data = time_series[time_series.columns[1]]
-                time_series = DataFrame(data=list(data), index=time_index)
-
-            if len(time_series.columns) == 1:
-                time_series = time_series[time_series.columns[0]]
-            else:
-                raise Exception("""Incorrect number of columns provided in DataFrame.
-                Should be either one with index as time-series or two with first column as time-series and second as property data.""")
-
-        self._time_series = time_series
-
-    def __getattr__(self, name):
-        if not name.startswith("_") and self.time_series is None:
-            time_series = {0: self.value}
-            if self.min_val is not None:
-                time_series[1] = self.min_val
-            if self.max_val is not None:
-                time_series[2] = self.max_val
-            time_series = Series(data=time_series, index=list(time_series.keys()))
-            warn("Time series of the property is not set. Series attribute is considerd using 'value', 'max_val', or 'min_val' if provided.")
-        else:
-            time_series = self.time_series
-        return getattr(time_series, name)
-
-    def __repr__(self) -> str:
-        return str(self.value) + ' ' + self.unit
-    
-    def __add__(self, other):
-        if self.unit != other.unit:
-            other.unit = self.unit
-        return type(self)(value=self.value + other.value, 
-                          unit=self.unit,
-                          min_val=self.max_val + other.min_val,
-                          max_val=self.max_val + other.max_val)
-    
-    def __sub__(self, other):
-        if self.unit != other.unit:
-            other.unit = self.unit
-        return type(self)(value=self.value - other.value,
-                          unit=self.unit,
-                          min_val=self.min_val - other.min_val, 
-                          max_val=self.max_val - other.min_val)
-    
-    def __truediv__(self, other):
-        if self.unit != other.unit:
-            other.unit = self.unit
-        return self.value / other.value
-
-    def __eq__(self, other):
-        if isinstance(other, type(self)):
-            if self.unit != other.unit:
-                other.unit = self.unit
-            return self.value == other.value
-        else:
-            return False
-    
-    def _convert_values_for_unit_change(self, unit, invert_factor=False):
-        """
-        Internal function to convert all values (min, norm and max values) for any unit change.
-        """
-        conversion_factor = getattr(ConversionFactors, self.__class__.__name__.upper())
-        conversion_factor = conversion_factor[unit] / conversion_factor[self._unit]
-        if invert_factor:
-            conversion_factor = 1 / conversion_factor
-        if self._value is not None:
-            self._value *= conversion_factor
-        if self._max_val is not None:
-            self._max_val *= conversion_factor
-        if self._min_val is not None:
-            self._min_val *= conversion_factor 
-        self._unit = unit
-
-class Length(_Property):
-    def __init__(self, value=0, unit='m', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit, True)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Length.
-                               Supported units are:
-                               1. m for meters
-                               2. mm for millimeters
-                               3. km for Kilometers
-                               4. cm for centimeters
-                               5. inch
-                               6. mile
-                               7. yard
-                               8. foot
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class Time(_Property):
-    def __init__(self, value=0, unit='sec', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit, True)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Time.
-                               Supported units are:
-                               1. s for seconds
-                               2. min for minutes
-                               3. hour
-                               4. day
-                               5. week
-                               6. month
-                               7. year
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-    
-class Pressure(_Property):
-    def __init__(self, value=101325, unit='Pa', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit, True)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Length.
-                               Supported units are:
-                               1. Pa for Pascals
-                               2. m water for meters of water column
-                               3. in water for inches of water column
-                               4. mm Hg for millimeters of Mercury
-                               5. Torr
-                               6. ata
-                               7. kg/cm^2 for kilogram per square centimeter 
-                               8. MPa for Mega Pascal
-                               9. kPa for Kilo Pascal
-                               10. psi for Pound per square inch
-                               11. bar
-                               12. atm for Atmospheres
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class Temperature(_Property):
-    def __init__(self, value=298, unit='K', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        if unit in ['K', 'C', 'F', 'R']:
-            while unit != self._unit:
-                if self._unit == 'K':
-                    self._value -= 273.15
-                    self._unit = 'C'
-                    if unit == self._unit:
-                        break
-                if self._unit == 'C':
-                    self._value = self._value * 9/5 + 32
-                    self._unit = 'F'
-                    if unit == self._unit:
-                        break
-                if self._unit == 'F':
-                    self._value = self._value  + 459.67
-                    self._unit = 'R'
-                    if unit == self._unit:
-                        break
-                if self._unit == 'R':
-                    self._value = self._value  * 5 / 9
-                    self._unit = 'K'
-                    if unit == self._unit:
-                        break
-            self._value = round(self.value,5)
-        else:
-            raise Exception('''Selected unit is not supported or a correct unit of Temperature.
-                               Supported units are:
-                               1. K for Kelvin
-                               2. C for Degrees Celsius
-                               3. F for Degree Fahrenheit
-                               4. R for Degree Rankine
-                               You selected '{}'.
-                               '''.format(unit))
-
-    def __add__(self, other):
-        old_unit = self.unit
-        self.unit = other.unit
-        addition = self.value + other.value
-        addition = Temperature(addition, other.unit)
-        self.unit = old_unit
-        addition.unit = old_unit
-        return addition
-    
-    def __sub__(self, other):
-        old_unit = self.unit
-        self.unit = other.unit
-        subtraction = self.value - other.value
-        subtraction = Temperature(subtraction, other.unit)
-        self.unit = old_unit
-        subtraction.unit = old_unit
-        return subtraction
-        
-class MassFlowRate(_Property):
-    def __init__(self, value=0, unit='kg/s', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Mass Flow Rate.
-                               Supported units are:
-                               1. kg/s for kilogram per seconds
-                               2. kg/min for kilogram per minutes
-                               3. kg/h for kilogram per hour
-                               4. kg/d for kilogram per day
-                               5. g/s for gram per second
-                               6. lb/s for pound per second
-                               7. lb/min for pound per minutes
-                               8. lb/h for pound per hour
-                               9. lb/d for pound per day
-                               10. ton/d for metric ton per day
-                               11. ton/h for metric ton per hour
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-    
-    def __add__(self, other):
-        return super().__add__(other)
-
-class Mass(_Property):
-    def __init__(self, value=0, unit='kg', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Mass Flow Rate.
-                               Supported units are:
-                               1. kg for kilogram 
-                               2. g for gram
-                               3. lb for pound
-                               4. ton for metric ton
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-    
-    def __add__(self, other):
-        return super().__add__(other)
-
-class MolecularWeigth(_Property):
-    def __init__(self, value=0, unit='g/mol', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Molecular Weight.
-                               Following are the supported units:
-                               1. g/mol for gram per mol
-                               2. kg/mol for kilogram per mol
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class MolarFlowRate(_Property):
-    def __init__(self, value=1, unit='mol/s', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Molar Flow Rate.
-                               Supported units are:
-                               1. mol/s for moles per seconds
-                               2. mol/min for moles per minutes
-                               3. mol/h for moles per hour
-                               4. mol/d for moles per day
-                               5. lbmol/s for poundmole per second
-                               6. lbmol/min for poundmole per minute
-                               7. lbmol/d for poundmole per day
-                               8. kmol/h for kilomole per hour
-                               9. kmol/d for kilomole per day
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class VolumetricFlowRate(_Property):
-    def __init__(self, value = 1, unit='m^3/s', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Volumetric Flow Rate.
-                               Following are the supported units:
-                               1. m^3/s for cubic meter per second
-                               2. ft^3/s for cubic feet per second
-                               3. cm^3/s for cubic centimeter per second
-                               4. m^3/min for cubic meter per minute
-                               5. m^3/h for cubic meter per hour
-                               6. m^3/d for cubic meter per day,
-                               7. ft^3/min for cubic feet per minute,
-                               8. ft^3/h for cubic feet per hour
-                               9. ft^3/d for cubic feet per day
-                               10. gal/s for US Gallons per second
-                               11. gal/min for US Gallon per minute
-                               12. gal/h for US Gallon per hour
-                               13. gal/d for US Gallin per day
-                               14. lit/s for Liters per second
-                               15. lit/min for Liters per minute
-                               16. lit/h for Liters per hour
-                               17. lit/d  for Liters per day
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class Volume(_Property):
-    def __init__(self, value = 0, unit= 'm^3', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Volumetric Flow Rate.
-                               Following are the supported units:
-                               1. m^3 for cubic meter
-                               2. ft^3 for cubic feet
-                               3. cm^3 for cubic centimeter
-                               4. gal for US Gallons
-                               5. lit for Liters
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class Density(_Property):
-    def __init__(self, value = 0, unit= 'kg/m^3', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Density.
-                               Following are the supported units:
-                               1. kg/m^3 for kilograms per cubic meter
-                               2. g/cm^3 for grams per per cubic centimeter
-                               3. lbm/ft^3 for pound mass per cubic feet
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class DViscosity(_Property):
-    def __init__(self, value = 0, unit= 'Pa-s', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Dynamic Viscosity.
-                               Following are the supported units:
-                               1. Pa-s for Pascal second
-                               2. cP for centipoise
-                               3. lb/(ft-s) for pound mass per cubic feet
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class Power(_Property):
-    def __init__(self, value = 0, unit= 'W', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit, True)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Power. 
-                               Following units are supported:
-                               1. W for Watts
-                               2. BTU/h for British Termal Units per hour
-                               3. BTU/min for Brititsh Termal Units per minutes
-                               4. BTU/s for British Termal Units per second
-                               5. cal/h for calories per hour
-                               6. cal/s for calories per second
-                               7. erg/h for ergs per hour
-                               8. erg/min for ergs per minutes
-                               9. erg/s for ergs per second
-                               10. hp for Horse Power
-                               11. MMBTU/h for Million Metric BTU/h
-                               12. MMBTU/min
-                               13. MMBTU/s
-                               14. kW for kilo watts
-                               15. MW for mega watts
-                               16. GW for giga watts
-                               17. TW for tera watts
-                               18. kWh/d for kilo watt hours per day
-                               19. MWh/d for Mega watt hours per day
-                               20. GWh/d for Giga watt hour per day
-                               21. TWh/d for Tera watt hour per day
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class Frequency(_Property):
-    def __init__(self, value=0, unit='Hz', time_series=None, min_val=None, max_val=None):
-        super().__init__(value, unit, time_series=time_series, max_val=max_val, min_val=min_val)
-        self.unit = unit
-    @_Property.unit.setter
-    def unit(self, unit):
-        _Validators.validate_arg_prop_value_type("unit", unit, (str))
-        try:
-            self._convert_values_for_unit_change(unit)
-        except KeyError:
-            raise Exception('''Selected unit is not supported or a correct unit of Dynamic Viscosity.
-                               Following are the supported units:
-                               1. Hz for Hertz(cycle per second)
-                               2. /min for cylce per minute
-                               3. /hour for cycle per hour
-                               You selected '{}'.
-                               '''.format(unit))
-        except:
-            raise
-
-class Components(object):
-    def __init__(self, fractions=None, type="mass"):
-        if fractions is not None:
-            _Validators.validate_arg_prop_value_type("fractions", fractions, (dict))
-        _Validators.validate_arg_prop_value_type("type", type, (str))        
-        self.fractions = fractions
-        self.type = type
-    def __eq__(self, other):
-        if self.type==other.type and self.fractions==other.fractions:
-            return True
-        return False
-
-class Dimensionless(_Property):
-    def __init__(self, value=None, name=None, time_series=None, min_val=None, max_val=None):
-        super().__init__(value=value, unit=None, time_series=time_series, max_val=max_val, min_val=min_val)
-        self._name = name
-    
-    @property
-    def name(self):
-        return self._name if self._name is not None else str(self.__class__.__name__)
-    @name.setter
-    def name(self, value):
-        self._name = value
-
-    @property
-    def unit(self):
-        return None
-    @unit.setter
-    def unit(self, unit):
-        raise Exception("{} does not have unit.".format(self.name))
-    
-    def __repr__(self) -> str:
-        return "{} with value {}".format(self.name, self.value)
-
-class Efficiency(Dimensionless):
-    def __init__(self, value=1, time_series=None, min_val=0, max_val=1):
-        super().__init__(value=value, name="Efficiency", time_series=time_series, max_val=max_val, min_val=min_val)
-        if value < 0 or min_val < 0 or max_val < 0:
-            raise Exception("Provide a non-negative value for efficiency.")
-        else:
-            if value > 1:
-                self.value =  value/100
-                warn("Efficiency value set to {} considering value provided in percent.".format(value/100))
-            if max_val > 1:
-                self.max_val = max_val/100
-                warn("Efficiency max_val set to {} considering value provided in percent.".format(max_val/100))
-            if min_val > 1:
-                self.min_val = min_val/100
+from propylean.validators import _Validators
+from propylean.constants import ConversionFactors
+from warnings import warn
+
+class _Property(object):
+    def __init__(self, value=None, unit=None, min_val=None, max_val=None):
+        _Validators.validate_arg_prop_value_type("value", value, (int, float))
+        _Validators.validate_arg_prop_value_type("unit", unit, str)
+        self._value = value
+        self._min_val = min_val
+        self._max_val = max_val
+        self._unit = unit
+    
+    def __eq__(self, other):
+        if (isinstance(other, _Property) and
+            self.value == other.value and
+            self.unit == other.unit):
+                return True
+        return False
+    
+    @property
+    def value(self):
+        return self._value
+    @value.setter
+    def value(self, value):
+        _Validators.validate_arg_prop_value_type("value", value, (int, float))
+        self._value = value
+    
+    @property
+    def max_val(self):
+        return self._max_val if self._max_val is not None else self._value
+    @max_val.setter
+    def max_val(self, value):
+        _Validators.validate_arg_prop_value_type("max_val", value, (int, float))
+        self._max_val = value
+    
+    @property
+    def min_val(self):
+        return self._min_val if self._min_val is not None else self._value
+    @min_val.setter
+    def min_val(self, value):
+        _Validators.validate_arg_prop_value_type("min_val", value, (int, float))
+        self._min_val = value
+    
+    @property
+    def unit(self):
+        return self._unit
+    @unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        self._unit = unit
+
+    def __repr__(self) -> str:
+        return str(self.value) + ' ' + self.unit
+    
+    def __add__(self, other):
+        if self.unit != other.unit:
+            other.unit = self.unit
+        return type(self)(value=self.value + other.value, 
+                          unit=self.unit,
+                          min_val=self.max_val + other.min_val,
+                          max_val=self.max_val + other.max_val)
+    
+    def __sub__(self, other):
+        if self.unit != other.unit:
+            other.unit = self.unit
+        return type(self)(value=self.value - other.value,
+                          unit=self.unit,
+                          min_val=self.min_val - other.min_val, 
+                          max_val=self.max_val - other.min_val)
+    
+    def __truediv__(self, other):
+        if self.unit != other.unit:
+            other.unit = self.unit
+        return self.value / other.value
+
+    def __eq__(self, other):
+        if isinstance(other, type(self)):
+            if self.unit != other.unit:
+                other.unit = self.unit
+            return self.value == other.value
+        else:
+            return False
+    
+    def _convert_values_for_unit_change(self, unit, invert_factor=False):
+        """
+        Internal function to convert all values (min, norm and max values) for any unit change.
+        """
+        conversion_factor = getattr(ConversionFactors, self.__class__.__name__.upper())
+        conversion_factor = conversion_factor[unit] / conversion_factor[self._unit]
+        if invert_factor:
+            conversion_factor = 1 / conversion_factor
+        if self._value is not None:
+            self._value *= conversion_factor
+        if self._max_val is not None:
+            self._max_val *= conversion_factor
+        if self._min_val is not None:
+            self._min_val *= conversion_factor 
+        self._unit = unit
+
+class Length(_Property):
+    def __init__(self, value=0, unit='m', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit, True)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Length.
+                               Supported units are:
+                               1. m for meters
+                               2. mm for millimeters
+                               3. km for Kilometers
+                               4. cm for centimeters
+                               5. inch
+                               6. mile
+                               7. yard
+                               8. foot
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class Time(_Property):
+    def __init__(self, value=0, unit='sec', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit, True)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Time.
+                               Supported units are:
+                               1. s for seconds
+                               2. min for minutes
+                               3. hour
+                               4. day
+                               5. week
+                               6. month
+                               7. year
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+    
+class Pressure(_Property):
+    def __init__(self, value=101325, unit='Pa', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit, True)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Length.
+                               Supported units are:
+                               1. Pa for Pascals
+                               2. m water for meters of water column
+                               3. in water for inches of water column
+                               4. mm Hg for millimeters of Mercury
+                               5. Torr
+                               6. ata
+                               7. kg/cm^2 for kilogram per square centimeter 
+                               8. MPa for Mega Pascal
+                               9. kPa for Kilo Pascal
+                               10. psi for Pound per square inch
+                               11. bar
+                               12. atm for Atmospheres
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class Temperature(_Property):
+    def __init__(self, value=298, unit='K', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        if unit in ['K', 'C', 'F', 'R']:
+            while unit != self._unit:
+                if self._unit == 'K':
+                    self._value -= 273.15
+                    self._unit = 'C'
+                    if unit == self._unit:
+                        break
+                if self._unit == 'C':
+                    self._value = self._value * 9/5 + 32
+                    self._unit = 'F'
+                    if unit == self._unit:
+                        break
+                if self._unit == 'F':
+                    self._value = self._value  + 459.67
+                    self._unit = 'R'
+                    if unit == self._unit:
+                        break
+                if self._unit == 'R':
+                    self._value = self._value  * 5 / 9
+                    self._unit = 'K'
+                    if unit == self._unit:
+                        break
+            self._value = round(self.value,5)
+        else:
+            raise Exception('''Selected unit is not supported or a correct unit of Temperature.
+                               Supported units are:
+                               1. K for Kelvin
+                               2. C for Degrees Celsius
+                               3. F for Degree Fahrenheit
+                               4. R for Degree Rankine
+                               You selected '{}'.
+                               '''.format(unit))
+
+    def __add__(self, other):
+        old_unit = self.unit
+        self.unit = other.unit
+        addition = self.value + other.value
+        addition = Temperature(addition, other.unit)
+        self.unit = old_unit
+        addition.unit = old_unit
+        return addition
+    
+    def __sub__(self, other):
+        old_unit = self.unit
+        self.unit = other.unit
+        subtraction = self.value - other.value
+        subtraction = Temperature(subtraction, other.unit)
+        self.unit = old_unit
+        subtraction.unit = old_unit
+        return subtraction
+        
+class MassFlowRate(_Property):
+    def __init__(self, value=0, unit='kg/s', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Mass Flow Rate.
+                               Supported units are:
+                               1. kg/s for kilogram per seconds
+                               2. kg/min for kilogram per minutes
+                               3. kg/h for kilogram per hour
+                               4. kg/d for kilogram per day
+                               5. g/s for gram per second
+                               6. lb/s for pound per second
+                               7. lb/min for pound per minutes
+                               8. lb/h for pound per hour
+                               9. lb/d for pound per day
+                               10. ton/d for metric ton per day
+                               11. ton/h for metric ton per hour
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+    
+    def __add__(self, other):
+        return super().__add__(other)
+
+class Mass(_Property):
+    def __init__(self, value=0, unit='kg', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Mass Flow Rate.
+                               Supported units are:
+                               1. kg for kilogram 
+                               2. g for gram
+                               3. lb for pound
+                               4. ton for metric ton
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+    
+    def __add__(self, other):
+        return super().__add__(other)
+
+class MolecularWeigth(_Property):
+    def __init__(self, value=0, unit='g/mol', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Molecular Weight.
+                               Following are the supported units:
+                               1. g/mol for gram per mol
+                               2. kg/mol for kilogram per mol
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class MolarFlowRate(_Property):
+    def __init__(self, value=1, unit='mol/s', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Molar Flow Rate.
+                               Supported units are:
+                               1. mol/s for moles per seconds
+                               2. mol/min for moles per minutes
+                               3. mol/h for moles per hour
+                               4. mol/d for moles per day
+                               5. lbmol/s for poundmole per second
+                               6. lbmol/min for poundmole per minute
+                               7. lbmol/d for poundmole per day
+                               8. kmol/h for kilomole per hour
+                               9. kmol/d for kilomole per day
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class VolumetricFlowRate(_Property):
+    def __init__(self, value = 1, unit='m^3/s', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Volumetric Flow Rate.
+                               Following are the supported units:
+                               1. m^3/s for cubic meter per second
+                               2. ft^3/s for cubic feet per second
+                               3. cm^3/s for cubic centimeter per second
+                               4. m^3/min for cubic meter per minute
+                               5. m^3/h for cubic meter per hour
+                               6. m^3/d for cubic meter per day,
+                               7. ft^3/min for cubic feet per minute,
+                               8. ft^3/h for cubic feet per hour
+                               9. ft^3/d for cubic feet per day
+                               10. gal/s for US Gallons per second
+                               11. gal/min for US Gallon per minute
+                               12. gal/h for US Gallon per hour
+                               13. gal/d for US Gallin per day
+                               14. lit/s for Liters per second
+                               15. lit/min for Liters per minute
+                               16. lit/h for Liters per hour
+                               17. lit/d  for Liters per day
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class Volume(_Property):
+    def __init__(self, value = 0, unit= 'm^3', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Volumetric Flow Rate.
+                               Following are the supported units:
+                               1. m^3 for cubic meter
+                               2. ft^3 for cubic feet
+                               3. cm^3 for cubic centimeter
+                               4. gal for US Gallons
+                               5. lit for Liters
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class Density(_Property):
+    def __init__(self, value = 0, unit= 'kg/m^3', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Density.
+                               Following are the supported units:
+                               1. kg/m^3 for kilograms per cubic meter
+                               2. g/cm^3 for grams per per cubic centimeter
+                               3. lbm/ft^3 for pound mass per cubic feet
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class DViscosity(_Property):
+    def __init__(self, value = 0, unit= 'Pa-s', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Dynamic Viscosity.
+                               Following are the supported units:
+                               1. Pa-s for Pascal second
+                               2. cP for centipoise
+                               3. lb/(ft-s) for pound mass per cubic feet
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class Power(_Property):
+    def __init__(self, value = 0, unit= 'W', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit, True)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Power. 
+                               Following units are supported:
+                               1. W for Watts
+                               2. BTU/h for British Termal Units per hour
+                               3. BTU/min for Brititsh Termal Units per minutes
+                               4. BTU/s for British Termal Units per second
+                               5. cal/h for calories per hour
+                               6. cal/s for calories per second
+                               7. erg/h for ergs per hour
+                               8. erg/min for ergs per minutes
+                               9. erg/s for ergs per second
+                               10. hp for Horse Power
+                               11. MMBTU/h for Million Metric BTU/h
+                               12. MMBTU/min
+                               13. MMBTU/s
+                               14. kW for kilo watts
+                               15. MW for mega watts
+                               16. GW for giga watts
+                               17. TW for tera watts
+                               18. kWh/d for kilo watt hours per day
+                               19. MWh/d for Mega watt hours per day
+                               20. GWh/d for Giga watt hour per day
+                               21. TWh/d for Tera watt hour per day
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class Frequency(_Property):
+    def __init__(self, value=0, unit='Hz', min_val=None, max_val=None):
+        super().__init__(value, unit, max_val=max_val, min_val=min_val)
+        self.unit = unit
+    @_Property.unit.setter
+    def unit(self, unit):
+        _Validators.validate_arg_prop_value_type("unit", unit, (str))
+        try:
+            self._convert_values_for_unit_change(unit)
+        except KeyError:
+            raise Exception('''Selected unit is not supported or a correct unit of Dynamic Viscosity.
+                               Following are the supported units:
+                               1. Hz for Hertz(cycle per second)
+                               2. /min for cylce per minute
+                               3. /hour for cycle per hour
+                               You selected '{}'.
+                               '''.format(unit))
+        except:
+            raise
+
+class Components(object):
+    def __init__(self, fractions=None, type="mass"):
+        if fractions is not None:
+            _Validators.validate_arg_prop_value_type("fractions", fractions, (dict))
+        _Validators.validate_arg_prop_value_type("type", type, (str))        
+        self.fractions = fractions
+        self.type = type
+    def __eq__(self, other):
+        if self.type==other.type and self.fractions==other.fractions:
+            return True
+        return False
+
+class Dimensionless(_Property):
+    def __init__(self, value=None, name=None, min_val=None, max_val=None):
+        super().__init__(value=value, unit=None, max_val=max_val, min_val=min_val)
+        self._name = name
+    
+    @property
+    def name(self):
+        return self._name if self._name is not None else str(self.__class__.__name__)
+    @name.setter
+    def name(self, value):
+        self._name = value
+
+    @property
+    def unit(self):
+        return None
+    @unit.setter
+    def unit(self, unit):
+        raise Exception("{} does not have unit.".format(self.name))
+    
+    def __repr__(self) -> str:
+        return "{} with value {}".format(self.name, self.value)
+
+class Efficiency(Dimensionless):
+    def __init__(self, value=1, min_val=0, max_val=1):
+        super().__init__(value=value, name="Efficiency", max_val=max_val, min_val=min_val)
+        if value < 0 or min_val < 0 or max_val < 0:
+            raise Exception("Provide a non-negative value for efficiency.")
+        else:
+            if value > 1:
+                self.value =  value/100
+                warn("Efficiency value set to {} considering value provided in percent.".format(value/100))
+            if max_val > 1:
+                self.max_val = max_val/100
+                warn("Efficiency max_val set to {} considering value provided in percent.".format(max_val/100))
+            if min_val > 1:
+                self.min_val = min_val/100
                 warn("Efficiency min_val set to {} considering value provided in percent.".format(min_val/100))
```

### Comparing `propylean-0.2.5/src/propylean.egg-info/PKG-INFO` & `propylean-0.2.6/src/propylean.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,100 @@
-Metadata-Version: 2.1
-Name: propylean
-Version: 0.2.5
-Summary: The open-source calculations and analytics package for chemical process industries.
-Home-page: https://github.com/abhishekvraman/Propylean
-Author: Abhishek V Raman
-Author-email: 
-Project-URL: Bug Tracker, https://github.com/abhishekvraman/Propylean/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Manufacturing
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Windows](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml)
-[![macOS](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml)
-[![Ubuntu](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml)
-[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/abhishekvraman/Propylean/blob/main/LICENSE)
-[![PythonVersions](https://img.shields.io/pypi/pyversions/propylean.svg?style=flat)](https://pypi.python.org/pypi/propylean)
-# Propylean
-#### The open-source analytics and calculation package for chemical process industries.
-
-## What is Propylean
-Propylean name is derived from words Process/Production + Python + lean programming/manufacturing.
-Propylean is a Python library which will help engineers analyse production plants focusing on chemical and related process industries using only Python environments.
-Supports for general calculations like hydraulics, vessel sizing and other process engineering calculations is provided and constantly updated.
-By coupling this library with available data analysis/machine learning frameworks, engineers will be able to enhance operations of their plants. Ultimate aspiration of this project is to enable process industries transit to zero carbon operation.
-
-## Objective
-To increase the utilization of open-source software and analytics tools in the chemical and related industries.
-
-## Vision
-Vision of Propylean is to:
-- Enable chemical and related industries to use analytics and ML frameworks
-- Improve operational agility and efficiency of the plant
-- Be a cheap simulation-software alternative for small manufacturers
-- One-stop shop for all process engineering calculations
-- Help the industry transition to Net-Zero emissions
-- Inculcate coding/programing skills in manufacturing engineers
-
-## Installation and Requirements
-To download use below command or download the wheel file from PyPi page.
-
-Pip command:
-`pip install propylean`
-
-PyPi page:
-https://pypi.org/project/propylean/
-
-## Getting Started and Documentation
-To get started with Propylean, have a look at the getting started documenation.
-https://github.com/abhishekvraman/Propylean/wiki/Getting-started-with-Propylean
-
-## Supported objects that can be imported:
-
-* equipments.rotary
-    1. CentrifugalPump
-    2. PositiveDisplacementPump
-    3. CentrifugalCompressor
-    4. TurboExpander
-* equipments.static
-    1. PipeSegment
-* equipments.storage
-    1. VerticalStorage
-    2. Bullet
-    3. Tank
-    4. Sphere
-* equipments.exchangers
-    1. AirCooler
-    2. ElectricHeater
-* instruments
-    1. ControlValve
-    2. FlowMeter
-* streams
-    1. MaterialStream
-    2. EnergyStream
-* properties
-    1. Pressure
-    2. Temperature
-    3. MassFlowRate
-    4. Components (Molecular components)
-    5. Length
-    6. Time
-    7. Mass
-    8. MolecularWeigth
-    9. MolarFlowRate
-    10. VolumetricFlowRate
-    11. Volume
-    12. Density
-    13. DViscosity
-    14. Power
-    15. Frequency
+Metadata-Version: 2.1
+Name: propylean
+Version: 0.2.6
+Summary: The open-source calculations and analytics package for chemical process industries.
+Home-page: https://github.com/abhishekvraman/Propylean
+Author: Abhishek V Raman
+Author-email: 
+Project-URL: Bug Tracker, https://github.com/abhishekvraman/Propylean/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Manufacturing
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: fluids
+Requires-Dist: thermo
+
+[![Windows](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-windows.yml)
+[![macOS](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-macos.yml)
+[![Ubuntu](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml/badge.svg?branch=main)](https://github.com/abhishekvraman/Propylean/actions/workflows/build-ubuntu.yml)
+[![License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/abhishekvraman/Propylean/blob/main/LICENSE)
+[![PythonVersions](https://img.shields.io/pypi/pyversions/propylean.svg?style=flat)](https://pypi.python.org/pypi/propylean)
+# Propylean
+#### The open-source analytics and calculation package for chemical process industries.
+
+## What is Propylean
+Propylean name is derived from words Process/Production + Python + lean programming/manufacturing.
+Propylean is a Python library which will help engineers analyse production plants focusing on chemical and related process industries using only Python environments.
+Supports for general calculations like hydraulics, vessel sizing and other process engineering calculations is provided and constantly updated.
+By coupling this library with available data analysis/machine learning frameworks, engineers will be able to enhance operations of their plants. Ultimate aspiration of this project is to enable process industries transit to zero carbon operation.
+
+## Objective
+To increase the utilization of open-source software and analytics tools in the chemical and related industries.
+
+## Vision
+Vision of Propylean is to:
+- Enable chemical and related industries to use analytics and ML frameworks
+- Improve operational agility and efficiency of the plant
+- Be a cheap simulation-software alternative for small manufacturers
+- One-stop shop for all process engineering calculations
+- Help the industry transition to Net-Zero emissions
+- Inculcate coding/programing skills in manufacturing engineers
+
+## Installation and Requirements
+To download use below command or download the wheel file from PyPi page.
+
+Pip command:
+`pip install propylean`
+
+PyPi page:
+https://pypi.org/project/propylean/
+
+## Getting Started and Documentation
+To get started with Propylean, have a look at the getting started documenation.
+https://github.com/abhishekvraman/Propylean/wiki/Getting-started-with-Propylean
+
+## Supported objects that can be imported:
+
+* equipments.rotary
+    1. CentrifugalPump
+    2. PositiveDisplacementPump
+    3. CentrifugalCompressor
+    4. TurboExpander
+* equipments.static
+    1. PipeSegment
+* equipments.storage
+    1. VerticalStorage
+    2. Bullet
+    3. Tank
+    4. Sphere
+* equipments.exchangers
+    1. AirCooler
+    2. ElectricHeater
+* instruments
+    1. ControlValve
+    2. FlowMeter
+* streams
+    1. MaterialStream
+    2. EnergyStream
+* properties
+    1. Pressure
+    2. Temperature
+    3. MassFlowRate
+    4. Components (Molecular components)
+    5. Length
+    6. Time
+    7. Mass
+    8. MolecularWeigth
+    9. MolarFlowRate
+    10. VolumetricFlowRate
+    11. Volume
+    12. Density
+    13. DViscosity
+    14. Power
+    15. Frequency
```

### Comparing `propylean-0.2.5/src/propylean.egg-info/SOURCES.txt` & `propylean-0.2.6/src/propylean.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/propylean/__init__.py
 src/propylean/constants.py
 src/propylean/properties.py
+src/propylean/series.py
 src/propylean/settings.py
 src/propylean/streams.py
 src/propylean/validators.py
 src/propylean.egg-info/PKG-INFO
 src/propylean.egg-info/SOURCES.txt
 src/propylean.egg-info/dependency_links.txt
 src/propylean.egg-info/requires.txt
```

