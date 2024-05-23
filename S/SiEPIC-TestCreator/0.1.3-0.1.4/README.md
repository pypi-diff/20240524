# Comparing `tmp/SiEPIC_TestCreator-0.1.3.tar.gz` & `tmp/SiEPIC_TestCreator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiEPIC_TestCreator-0.1.3.tar", last modified: Thu May 23 23:46:21 2024, max compression
+gzip compressed data, was "SiEPIC_TestCreator-0.1.4.tar", last modified: Thu May 23 23:50:31 2024, max compression
```

## Comparing `SiEPIC_TestCreator-0.1.3.tar` & `SiEPIC_TestCreator-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.376794 SiEPIC_TestCreator-0.1.3/
--rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 SiEPIC_TestCreator-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2497 2024-05-23 23:46:21.375781 SiEPIC_TestCreator-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.292616 SiEPIC_TestCreator-0.1.3/app/
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.309618 SiEPIC_TestCreator-0.1.3/app/SiEPIC_TestCreator.egg-info/
--rw-rw-rw-   0        0        0     2497 2024-05-23 23:46:20.000000 SiEPIC_TestCreator-0.1.3/app/SiEPIC_TestCreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2024-05-23 23:46:20.000000 SiEPIC_TestCreator-0.1.3/app/SiEPIC_TestCreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 23:46:20.000000 SiEPIC_TestCreator-0.1.3/app/SiEPIC_TestCreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2024-05-23 23:46:20.000000 SiEPIC_TestCreator-0.1.3/app/SiEPIC_TestCreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-23 23:46:20.000000 SiEPIC_TestCreator-0.1.3/app/SiEPIC_TestCreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.319622 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/
--rw-rw-rw-   0        0        0      114 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/__init__.py
--rw-rw-rw-   0        0        0    91527 2024-05-23 23:32:07.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequencecreator.py
--rw-rw-rw-   0        0        0       68 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequencecreatorvariables.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.321617 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.322618 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/BIO/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:24.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/BIO/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.341617 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:03.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/__init__.py
--rw-rw-rw-   0        0        0     2734 2024-05-23 23:38:49.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/current_sweep.py
--rw-rw-rw-   0        0        0     3291 2024-05-23 23:39:01.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py
--rw-rw-rw-   0        0        0     3410 2024-05-23 23:39:06.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py
--rw-rw-rw-   0        0        0     3062 2024-05-23 23:39:11.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py
--rw-rw-rw-   0        0        0     3581 2024-05-23 23:39:17.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py
--rw-rw-rw-   0        0        0     2808 2024-05-23 23:39:21.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py
--rw-rw-rw-   0        0        0     2813 2024-05-23 23:39:26.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.360796 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:17.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/__init__.py
--rw-rw-rw-   0        0        0     2421 2024-05-23 23:39:32.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py
--rw-rw-rw-   0        0        0     3494 2024-05-23 23:39:37.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     3571 2024-05-23 23:39:42.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     2958 2024-05-23 23:39:46.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py
--rw-rw-rw-   0        0        0     3040 2024-05-23 23:39:51.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2324 2024-05-23 23:39:55.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2496 2024-05-23 23:40:00.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0      112 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.371787 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/
--rw-rw-rw-   0        0        0      106 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/__init__.py
--rw-rw-rw-   0        0        0    10207 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/laser_sweep.py
--rw-rw-rw-   0        0        0    15635 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/results.py
--rw-rw-rw-   0        0        0     3086 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/sequence.py
--rw-rw-rw-   0        0        0     7492 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/smu_sweep.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:46:21.374781 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/template/
--rw-rw-rw-   0        0        0      971 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/template/__init__.py
--rw-rw-rw-   0        0        0     3071 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequencetracker.py
--rw-rw-rw-   0        0        0     4994 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/yamlcheck.py
--rw-rw-rw-   0        0        0       42 2024-05-23 23:46:21.376794 SiEPIC_TestCreator-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1229 2024-05-23 23:45:48.000000 SiEPIC_TestCreator-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.816543 SiEPIC_TestCreator-0.1.4/
+-rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 SiEPIC_TestCreator-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2497 2024-05-23 23:50:31.815548 SiEPIC_TestCreator-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.722546 SiEPIC_TestCreator-0.1.4/app/
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.741546 SiEPIC_TestCreator-0.1.4/app/SiEPIC_TestCreator.egg-info/
+-rw-rw-rw-   0        0        0     2497 2024-05-23 23:50:31.000000 SiEPIC_TestCreator-0.1.4/app/SiEPIC_TestCreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2024-05-23 23:50:31.000000 SiEPIC_TestCreator-0.1.4/app/SiEPIC_TestCreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 23:50:31.000000 SiEPIC_TestCreator-0.1.4/app/SiEPIC_TestCreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2024-05-23 23:50:31.000000 SiEPIC_TestCreator-0.1.4/app/SiEPIC_TestCreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 23:50:31.000000 SiEPIC_TestCreator-0.1.4/app/SiEPIC_TestCreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.755546 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/
+-rw-rw-rw-   0        0        0      114 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/__init__.py
+-rw-rw-rw-   0        0        0    91546 2024-05-23 23:49:04.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequencecreator.py
+-rw-rw-rw-   0        0        0       68 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequencecreatorvariables.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.757545 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.759549 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/BIO/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:24.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/BIO/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.782545 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:03.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/__init__.py
+-rw-rw-rw-   0        0        0     2734 2024-05-23 23:38:49.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/current_sweep.py
+-rw-rw-rw-   0        0        0     3291 2024-05-23 23:39:01.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     3410 2024-05-23 23:39:06.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     3062 2024-05-23 23:39:11.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py
+-rw-rw-rw-   0        0        0     3581 2024-05-23 23:39:17.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py
+-rw-rw-rw-   0        0        0     2808 2024-05-23 23:39:21.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py
+-rw-rw-rw-   0        0        0     2813 2024-05-23 23:39:26.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.800545 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:17.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/__init__.py
+-rw-rw-rw-   0        0        0     2421 2024-05-23 23:39:32.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py
+-rw-rw-rw-   0        0        0     3494 2024-05-23 23:39:37.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     3571 2024-05-23 23:39:42.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     2958 2024-05-23 23:39:46.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py
+-rw-rw-rw-   0        0        0     3040 2024-05-23 23:39:51.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py
+-rw-rw-rw-   0        0        0     2324 2024-05-23 23:39:55.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py
+-rw-rw-rw-   0        0        0     2496 2024-05-23 23:40:00.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0      112 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.809579 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/
+-rw-rw-rw-   0        0        0      106 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/__init__.py
+-rw-rw-rw-   0        0        0    10207 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/laser_sweep.py
+-rw-rw-rw-   0        0        0    15635 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/results.py
+-rw-rw-rw-   0        0        0     3086 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/sequence.py
+-rw-rw-rw-   0        0        0     7492 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/smu_sweep.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:50:31.812545 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/template/
+-rw-rw-rw-   0        0        0      971 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/template/__init__.py
+-rw-rw-rw-   0        0        0     3071 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequencetracker.py
+-rw-rw-rw-   0        0        0     4994 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/yamlcheck.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 23:50:31.816543 SiEPIC_TestCreator-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2024-05-23 23:50:06.000000 SiEPIC_TestCreator-0.1.4/setup.py
```

### Comparing `SiEPIC_TestCreator-0.1.3/LICENSE` & `SiEPIC_TestCreator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/PKG-INFO` & `SiEPIC_TestCreator-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiEPIC_TestCreator
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/SiEPIC/SiEPIC_testcreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SiEPIC_TestCreator-0.1.3/app/SiEPIC_TestCreator.egg-info/PKG-INFO` & `SiEPIC_TestCreator-0.1.4/app/SiEPIC_TestCreator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiEPIC-TestCreator
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/SiEPIC/SiEPIC_testcreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SiEPIC_TestCreator-0.1.3/app/SiEPIC_TestCreator.egg-info/SOURCES.txt` & `SiEPIC_TestCreator-0.1.4/app/SiEPIC_TestCreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequencecreator.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequencecreator.py`

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
-from yamlcheck import yaml_check
+from siepic_testcreator.yamlcheck import yaml_check
 
 
 def launch():
     app = QApplication([])
     ex = GUI()
     ex.show()
     app.exec_()
```

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/current_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/current_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/laser_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/laser_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/results.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/results.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/sequence.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/sequence.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/core/smu_sweep.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/core/smu_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequences/template/__init__.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequences/template/__init__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/sequencetracker.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/sequencetracker.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/app/siepic_testcreator/yamlcheck.py` & `SiEPIC_TestCreator-0.1.4/app/siepic_testcreator/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.3/setup.py` & `SiEPIC_TestCreator-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "SiEPIC_TestCreator",
-    version = "0.1.3",
+    version = "0.1.4",
     description = "A tool for creating YAML files for use in Dream Photonics and edx course",
     package_dir = {"": "app"},
     packages = find_packages(where="app"),
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/SiEPIC/SiEPIC_testcreator.git",
     author = "Jonathan Barnes",
```

