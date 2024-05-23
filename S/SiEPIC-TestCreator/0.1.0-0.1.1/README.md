# Comparing `tmp/SiEPIC_TestCreator-0.1.0.tar.gz` & `tmp/SiEPIC_TestCreator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiEPIC_TestCreator-0.1.0.tar", last modified: Thu May 23 23:11:35 2024, max compression
+gzip compressed data, was "SiEPIC_TestCreator-0.1.1.tar", last modified: Thu May 23 23:35:58 2024, max compression
```

## Comparing `SiEPIC_TestCreator-0.1.0.tar` & `SiEPIC_TestCreator-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.655845 SiEPIC_TestCreator-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 SiEPIC_TestCreator-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2497 2024-05-23 23:11:35.654842 SiEPIC_TestCreator-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.521409 SiEPIC_TestCreator-0.1.0/app/
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.545409 SiEPIC_TestCreator-0.1.0/app/SiEPIC_TestCreator.egg-info/
--rw-rw-rw-   0        0        0     2497 2024-05-23 23:11:34.000000 SiEPIC_TestCreator-0.1.0/app/SiEPIC_TestCreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2024-05-23 23:11:34.000000 SiEPIC_TestCreator-0.1.0/app/SiEPIC_TestCreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 23:11:34.000000 SiEPIC_TestCreator-0.1.0/app/SiEPIC_TestCreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2024-05-23 23:11:34.000000 SiEPIC_TestCreator-0.1.0/app/SiEPIC_TestCreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-23 23:11:34.000000 SiEPIC_TestCreator-0.1.0/app/SiEPIC_TestCreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.562410 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/
--rw-rw-rw-   0        0        0      114 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/__init__.py
--rw-rw-rw-   0        0        0    91546 2024-05-23 23:09:24.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequencecreator.py
--rw-rw-rw-   0        0        0       68 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequencecreatorvariables.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.564410 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.567410 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/BIO/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:24.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/BIO/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.596410 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:03.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/__init__.py
--rw-rw-rw-   0        0        0     2728 2024-05-01 18:00:31.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/current_sweep.py
--rw-rw-rw-   0        0        0     3285 2024-05-01 18:00:19.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py
--rw-rw-rw-   0        0        0     3404 2024-04-29 21:16:26.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py
--rw-rw-rw-   0        0        0     3056 2024-05-01 18:09:04.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py
--rw-rw-rw-   0        0        0     3575 2024-05-01 18:08:51.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py
--rw-rw-rw-   0        0        0     2802 2024-05-01 18:06:34.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py
--rw-rw-rw-   0        0        0     2807 2024-05-01 18:05:34.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.627418 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:17.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/__init__.py
--rw-rw-rw-   0        0        0     2415 2024-05-01 22:40:23.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py
--rw-rw-rw-   0        0        0     3488 2024-05-01 18:01:26.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     3565 2024-05-01 23:03:32.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     2952 2024-05-01 18:03:17.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py
--rw-rw-rw-   0        0        0     3034 2024-05-23 22:51:07.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2318 2024-05-23 22:50:40.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2490 2024-05-01 23:03:54.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0      112 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.642842 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/
--rw-rw-rw-   0        0        0      106 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/__init__.py
--rw-rw-rw-   0        0        0    10207 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/laser_sweep.py
--rw-rw-rw-   0        0        0    15635 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/results.py
--rw-rw-rw-   0        0        0     3086 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/sequence.py
--rw-rw-rw-   0        0        0     7492 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/smu_sweep.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:11:35.645843 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/template/
--rw-rw-rw-   0        0        0      971 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/template/__init__.py
--rw-rw-rw-   0        0        0     3071 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequencetracker.py
--rw-rw-rw-   0        0        0     4994 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/yamlcheck.py
--rw-rw-rw-   0        0        0       42 2024-05-23 23:11:35.655845 SiEPIC_TestCreator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1229 2024-05-23 23:11:17.000000 SiEPIC_TestCreator-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.944779 SiEPIC_TestCreator-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 SiEPIC_TestCreator-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2497 2024-05-23 23:35:58.943779 SiEPIC_TestCreator-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.846778 SiEPIC_TestCreator-0.1.1/app/
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.866782 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/
+-rw-rw-rw-   0        0        0     2497 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.878777 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/
+-rw-rw-rw-   0        0        0      114 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/__init__.py
+-rw-rw-rw-   0        0        0    91527 2024-05-23 23:32:07.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencecreator.py
+-rw-rw-rw-   0        0        0       68 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencecreatorvariables.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.881777 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.883778 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/BIO/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:24.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/BIO/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.902778 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:03.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/__init__.py
+-rw-rw-rw-   0        0        0     2728 2024-05-01 18:00:31.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/current_sweep.py
+-rw-rw-rw-   0        0        0     3285 2024-05-01 18:00:19.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     3404 2024-04-29 21:16:26.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     3056 2024-05-01 18:09:04.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py
+-rw-rw-rw-   0        0        0     3575 2024-05-01 18:08:51.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py
+-rw-rw-rw-   0        0        0     2802 2024-05-01 18:06:34.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py
+-rw-rw-rw-   0        0        0     2807 2024-05-01 18:05:34.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.925779 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:17.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/__init__.py
+-rw-rw-rw-   0        0        0     2415 2024-05-01 22:40:23.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py
+-rw-rw-rw-   0        0        0     3488 2024-05-01 18:01:26.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     3565 2024-05-01 23:03:32.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     2952 2024-05-01 18:03:17.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py
+-rw-rw-rw-   0        0        0     3034 2024-05-23 22:51:07.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py
+-rw-rw-rw-   0        0        0     2318 2024-05-23 22:50:40.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py
+-rw-rw-rw-   0        0        0     2490 2024-05-01 23:03:54.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0      112 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.938781 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/
+-rw-rw-rw-   0        0        0      106 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/__init__.py
+-rw-rw-rw-   0        0        0    10207 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/laser_sweep.py
+-rw-rw-rw-   0        0        0    15635 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/results.py
+-rw-rw-rw-   0        0        0     3086 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/sequence.py
+-rw-rw-rw-   0        0        0     7492 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/smu_sweep.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.941780 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/template/
+-rw-rw-rw-   0        0        0      971 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/template/__init__.py
+-rw-rw-rw-   0        0        0     3071 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencetracker.py
+-rw-rw-rw-   0        0        0     4994 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/yamlcheck.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 23:35:58.945778 SiEPIC_TestCreator-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2024-05-23 23:34:54.000000 SiEPIC_TestCreator-0.1.1/setup.py
```

### Comparing `SiEPIC_TestCreator-0.1.0/LICENSE` & `SiEPIC_TestCreator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/PKG-INFO` & `SiEPIC_TestCreator-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiEPIC_TestCreator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/SiEPIC/SiEPIC_testcreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SiEPIC_TestCreator-0.1.0/app/SiEPIC_TestCreator.egg-info/PKG-INFO` & `SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiEPIC-TestCreator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/SiEPIC/SiEPIC_testcreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SiEPIC_TestCreator-0.1.0/app/SiEPIC_TestCreator.egg-info/SOURCES.txt` & `SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequencecreator.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencecreator.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import yaml
 import importlib
 import importlib.util
 import inspect
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 import logging
-from siepic_testcreator.yamlcheck import yaml_check
+from yamlcheck import yaml_check
 
 
 def launch():
     app = QApplication([])
     ex = GUI()
     ex.show()
     app.exec_()
```

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/current_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/current_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/laser_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/laser_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/results.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/results.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/sequence.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/sequence.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/core/smu_sweep.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/smu_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequences/template/__init__.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/template/__init__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/sequencetracker.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencetracker.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/app/siepic_testcreator/yamlcheck.py` & `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.0/setup.py` & `SiEPIC_TestCreator-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "SiEPIC_TestCreator",
-    version = "0.1.0",
+    version = "0.1.1",
     description = "A tool for creating YAML files for use in Dream Photonics and edx course",
     package_dir = {"": "app"},
     packages = find_packages(where="app"),
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/SiEPIC/SiEPIC_testcreator.git",
     author = "Jonathan Barnes",
```

