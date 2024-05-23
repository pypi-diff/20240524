# Comparing `tmp/SiEPIC_TestCreator-0.1.1.tar.gz` & `tmp/SiEPIC_TestCreator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SiEPIC_TestCreator-0.1.1.tar", last modified: Thu May 23 23:35:58 2024, max compression
+gzip compressed data, was "SiEPIC_TestCreator-0.1.2.tar", last modified: Thu May 23 23:42:32 2024, max compression
```

## Comparing `SiEPIC_TestCreator-0.1.1.tar` & `SiEPIC_TestCreator-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.944779 SiEPIC_TestCreator-0.1.1/
--rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 SiEPIC_TestCreator-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2497 2024-05-23 23:35:58.943779 SiEPIC_TestCreator-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.846778 SiEPIC_TestCreator-0.1.1/app/
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.866782 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/
--rw-rw-rw-   0        0        0     2497 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-23 23:35:58.000000 SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.878777 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/
--rw-rw-rw-   0        0        0      114 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/__init__.py
--rw-rw-rw-   0        0        0    91527 2024-05-23 23:32:07.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencecreator.py
--rw-rw-rw-   0        0        0       68 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencecreatorvariables.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.881777 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.883778 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/BIO/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:24.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/BIO/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.902778 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:03.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/__init__.py
--rw-rw-rw-   0        0        0     2728 2024-05-01 18:00:31.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/current_sweep.py
--rw-rw-rw-   0        0        0     3285 2024-05-01 18:00:19.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py
--rw-rw-rw-   0        0        0     3404 2024-04-29 21:16:26.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py
--rw-rw-rw-   0        0        0     3056 2024-05-01 18:09:04.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py
--rw-rw-rw-   0        0        0     3575 2024-05-01 18:08:51.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py
--rw-rw-rw-   0        0        0     2802 2024-05-01 18:06:34.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py
--rw-rw-rw-   0        0        0     2807 2024-05-01 18:05:34.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.925779 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/
--rw-rw-rw-   0        0        0        0 2024-04-30 23:49:17.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/__init__.py
--rw-rw-rw-   0        0        0     2415 2024-05-01 22:40:23.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py
--rw-rw-rw-   0        0        0     3488 2024-05-01 18:01:26.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     3565 2024-05-01 23:03:32.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0     2952 2024-05-01 18:03:17.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py
--rw-rw-rw-   0        0        0     3034 2024-05-23 22:51:07.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2318 2024-05-23 22:50:40.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py
--rw-rw-rw-   0        0        0     2490 2024-05-01 23:03:54.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py
--rw-rw-rw-   0        0        0      112 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.938781 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/
--rw-rw-rw-   0        0        0      106 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/__init__.py
--rw-rw-rw-   0        0        0    10207 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/laser_sweep.py
--rw-rw-rw-   0        0        0    15635 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/results.py
--rw-rw-rw-   0        0        0     3086 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/sequence.py
--rw-rw-rw-   0        0        0     7492 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/smu_sweep.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:35:58.941780 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/template/
--rw-rw-rw-   0        0        0      971 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/template/__init__.py
--rw-rw-rw-   0        0        0     3071 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencetracker.py
--rw-rw-rw-   0        0        0     4994 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/yamlcheck.py
--rw-rw-rw-   0        0        0       42 2024-05-23 23:35:58.945778 SiEPIC_TestCreator-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1229 2024-05-23 23:34:54.000000 SiEPIC_TestCreator-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.335191 SiEPIC_TestCreator-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-03-18 02:28:05.000000 SiEPIC_TestCreator-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2497 2024-05-23 23:42:32.334195 SiEPIC_TestCreator-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.229198 SiEPIC_TestCreator-0.1.2/app/
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.248193 SiEPIC_TestCreator-0.1.2/app/SiEPIC_TestCreator.egg-info/
+-rw-rw-rw-   0        0        0     2497 2024-05-23 23:42:31.000000 SiEPIC_TestCreator-0.1.2/app/SiEPIC_TestCreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2024-05-23 23:42:31.000000 SiEPIC_TestCreator-0.1.2/app/SiEPIC_TestCreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 23:42:31.000000 SiEPIC_TestCreator-0.1.2/app/SiEPIC_TestCreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2024-05-23 23:42:31.000000 SiEPIC_TestCreator-0.1.2/app/SiEPIC_TestCreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-23 23:42:31.000000 SiEPIC_TestCreator-0.1.2/app/SiEPIC_TestCreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.261192 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/
+-rw-rw-rw-   0        0        0      114 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/__init__.py
+-rw-rw-rw-   0        0        0    91527 2024-05-23 23:32:07.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequencecreator.py
+-rw-rw-rw-   0        0        0       68 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequencecreatorvariables.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.263193 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.265194 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/BIO/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:24.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/BIO/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.285194 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:03.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/__init__.py
+-rw-rw-rw-   0        0        0     2734 2024-05-23 23:38:49.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/current_sweep.py
+-rw-rw-rw-   0        0        0     3291 2024-05-23 23:39:01.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     3410 2024-05-23 23:39:06.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py
+-rw-rw-rw-   0        0        0     3062 2024-05-23 23:39:11.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py
+-rw-rw-rw-   0        0        0     3581 2024-05-23 23:39:17.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py
+-rw-rw-rw-   0        0        0     2808 2024-05-23 23:39:21.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py
+-rw-rw-rw-   0        0        0     2813 2024-05-23 23:39:26.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.307200 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/
+-rw-rw-rw-   0        0        0        0 2024-04-30 23:49:17.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/__init__.py
+-rw-rw-rw-   0        0        0     2421 2024-05-23 23:39:32.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py
+-rw-rw-rw-   0        0        0     3494 2024-05-23 23:39:37.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     3571 2024-05-23 23:39:42.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0     2958 2024-05-23 23:39:46.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py
+-rw-rw-rw-   0        0        0     3040 2024-05-23 23:39:51.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py
+-rw-rw-rw-   0        0        0     2324 2024-05-23 23:39:55.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py
+-rw-rw-rw-   0        0        0     2496 2024-05-23 23:40:00.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py
+-rw-rw-rw-   0        0        0      112 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.328195 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/
+-rw-rw-rw-   0        0        0      106 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/__init__.py
+-rw-rw-rw-   0        0        0    10207 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/laser_sweep.py
+-rw-rw-rw-   0        0        0    15635 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/results.py
+-rw-rw-rw-   0        0        0     3086 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/sequence.py
+-rw-rw-rw-   0        0        0     7492 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/smu_sweep.py
+drwxrwxrwx   0        0        0        0 2024-05-23 23:42:32.332194 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/template/
+-rw-rw-rw-   0        0        0      971 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/template/__init__.py
+-rw-rw-rw-   0        0        0     3071 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequencetracker.py
+-rw-rw-rw-   0        0        0     4994 2024-04-04 20:31:52.000000 SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/yamlcheck.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 23:42:32.336193 SiEPIC_TestCreator-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2024-05-23 23:42:18.000000 SiEPIC_TestCreator-0.1.2/setup.py
```

### Comparing `SiEPIC_TestCreator-0.1.1/LICENSE` & `SiEPIC_TestCreator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/PKG-INFO` & `SiEPIC_TestCreator-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiEPIC_TestCreator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/SiEPIC/SiEPIC_testcreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/PKG-INFO` & `SiEPIC_TestCreator-0.1.2/app/SiEPIC_TestCreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SiEPIC-TestCreator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for creating YAML files for use in Dream Photonics and edx course
 Home-page: https://github.com/SiEPIC/SiEPIC_testcreator.git
 Author: Jonathan Barnes
 Author-email: jonathanyorkbarnes@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/SiEPIC_TestCreator.egg-info/SOURCES.txt` & `SiEPIC_TestCreator-0.1.2/app/SiEPIC_TestCreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencecreator.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequencecreator.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/current_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/current_sweep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
+from siepic_testcreator.sequences.core.smu_sweep import SmuSweep
 
 class CurrentSweep(SmuSweep):
     """
     Current sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/set_current_wavelength_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.laser_sweep import LaserSweep
+from siepic_testcreator.sequences.core.laser_sweep import LaserSweep
 
 class SetCurrentWavelengthSweep(LaserSweep):
     """
     Sets the current and then performs a laser sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/set_voltage_wavelength_sweep.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.laser_sweep import LaserSweep
+from siepic_testcreator.sequences.core.laser_sweep import LaserSweep
 
 class SetVoltageWavelengthSweep(LaserSweep):
     """
     Sets the voltage and then performs a laser sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/set_wavelength_current_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
+from siepic_testcreator.sequences.core.smu_sweep import SmuSweep
 
 class SetWavelengthCurrentSweep(SmuSweep):
     """
     Sets the wavelength then performs a current sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/set_wavelength_voltage_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
+from siepic_testcreator.sequences.core.smu_sweep import SmuSweep
 import time
 
 class SetWavelengthVoltageSweep(SmuSweep):
     """
     Sets the wavelength then performs a voltage sweep.
 
     Args:
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/voltage_sweep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
+from siepic_testcreator.sequences.core.smu_sweep import SmuSweep
 
 class VoltageSweep(SmuSweep):
     """
     Voltage sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/DREAM/wavelength_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.laser_sweep import LaserSweep
+from siepic_testcreator.sequences.core.laser_sweep import LaserSweep
 
 class WavelengthSweep(LaserSweep):
     """
     Wavelength sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/current_sweep_ida.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
+from siepic_testcreator.sequences.core.smu_sweep import SmuSweep
 
 class CurrentSweepIda(SmuSweep):
     """
     Current sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/set_current_wavelength_sweep_ida.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.laser_sweep import LaserSweep
+from siepic_testcreator.sequences.core.laser_sweep import LaserSweep
 
 class SetCurrentWavelengthSweepIda(LaserSweep):
     """
     Sets the current and then performs a laser sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/set_voltage_wavelength_sweep_ida.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.laser_sweep import LaserSweep
+from siepic_testcreator.sequences.core.laser_sweep import LaserSweep
 
 class SetVoltageWavelengthSweepIda(LaserSweep):
     """
     Sets the voltage and then performs a laser sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/set_wavelength_current_sweep_ida.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
+from siepic_testcreator.sequences.core.smu_sweep import SmuSweep
 
 class SetWavelengthCurrentSweepIda(SmuSweep):
     """
     Sets the wavelength then performs a current sweep.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/set_wavelength_voltage_sweep_ida.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
+from siepic_testcreator.sequences.core.smu_sweep import SmuSweep
 import time
 
 class SetWavelengthVoltageSweepIda(SmuSweep):
     """
     Sets the wavelength then performs a voltage sweep.
 
     Args:
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/voltage_sweep_ida.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.smu_sweep import SmuSweep
+from siepic_testcreator.sequences.core.smu_sweep import SmuSweep
 
 class VoltageSweepIda(SmuSweep):
     """
     Voltage sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/IDA/wavelength_sweep_ida.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dreamcreator.sequences.core.laser_sweep import LaserSweep
+from siepic_testcreator.sequences.core.laser_sweep import LaserSweep
 
 class WavelengthSweepIda(LaserSweep):
     """
     Wavelength sweep sequence class.
 
     Args:
         ps (Dreams Lab probe station object): the probe station performing the sweep.
```

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/laser_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/laser_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/results.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/results.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/sequence.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/sequence.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/core/smu_sweep.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/core/smu_sweep.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequences/template/__init__.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequences/template/__init__.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/sequencetracker.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/sequencetracker.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/app/siepic_testcreator/yamlcheck.py` & `SiEPIC_TestCreator-0.1.2/app/siepic_testcreator/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `SiEPIC_TestCreator-0.1.1/setup.py` & `SiEPIC_TestCreator-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = "SiEPIC_TestCreator",
-    version = "0.1.1",
+    version = "0.1.2",
     description = "A tool for creating YAML files for use in Dream Photonics and edx course",
     package_dir = {"": "app"},
     packages = find_packages(where="app"),
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/SiEPIC/SiEPIC_testcreator.git",
     author = "Jonathan Barnes",
```

