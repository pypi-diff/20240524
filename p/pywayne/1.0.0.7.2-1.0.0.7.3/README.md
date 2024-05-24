# Comparing `tmp/pywayne-1.0.0.7.2.tar.gz` & `tmp/pywayne-1.0.0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywayne-1.0.0.7.2.tar", last modified: Tue May 14 07:36:18 2024, max compression
+gzip compressed data, was "pywayne-1.0.0.7.3.tar", last modified: Fri May 24 03:28:40 2024, max compression
```

## Comparing `pywayne-1.0.0.7.2.tar` & `pywayne-1.0.0.7.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.223890 pywayne-1.0.0.7.2/
--rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/LICENSE
--rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-14 07:36:18.223550 pywayne-1.0.0.7.2/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/README.md
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.219124 pywayne-1.0.0.7.2/bin/
--rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.7.2/bin/gettool
--rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.7.2/bin/gettool.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.220616 pywayne-1.0.0.7.2/pywayne/
--rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/pywayne/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)      242 2024-05-14 07:35:57.000000 pywayne-1.0.0.7.2/pywayne/__version__.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.221591 pywayne-1.0.0.7.2/pywayne/adb/
--rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.2/pywayne/adb/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.2/pywayne/adb/logcat_reader.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.221846 pywayne-1.0.0.7.2/pywayne/ahrs/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/pywayne/ahrs/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/pywayne/ahrs/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.222343 pywayne-1.0.0.7.2/pywayne/calibration/
--rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/pywayne/calibration/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.7.2/pywayne/calibration/magnetometer_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.7.2/pywayne/calibration/temporal_calibration.py
--rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/pywayne/data_structure.py
--rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.7.2/pywayne/dsp.py
--rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.7.2/pywayne/gui.py
--rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/pywayne/math.py
--rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.2/pywayne/plot.py
--rw-r--r--   0 wayne      (503) staff       (20)    18054 2024-05-14 07:36:09.000000 pywayne-1.0.0.7.2/pywayne/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.222763 pywayne-1.0.0.7.2/pywayne/vio/
--rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.2/pywayne/vio/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.2/pywayne/vio/tools.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.223036 pywayne-1.0.0.7.2/pywayne/visualization/
--rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.7.2/pywayne/visualization/__init__.py
--rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.7.2/pywayne/visualization/pangolin.py
-drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-14 07:36:18.223245 pywayne-1.0.0.7.2/pywayne.egg-info/
--rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-14 07:36:18.000000 pywayne-1.0.0.7.2/pywayne.egg-info/PKG-INFO
--rw-r--r--   0 wayne      (503) staff       (20)      692 2024-05-14 07:36:18.000000 pywayne-1.0.0.7.2/pywayne.egg-info/SOURCES.txt
--rw-r--r--   0 wayne      (503) staff       (20)      184 2024-05-14 07:36:18.000000 pywayne-1.0.0.7.2/pywayne.egg-info/dependency_links.txt
--rw-r--r--   0 wayne      (503) staff       (20)      162 2024-05-14 07:36:18.000000 pywayne-1.0.0.7.2/pywayne.egg-info/requires.txt
--rw-r--r--   0 wayne      (503) staff       (20)        8 2024-05-14 07:36:18.000000 pywayne-1.0.0.7.2/pywayne.egg-info/top_level.txt
--rw-r--r--   0 wayne      (503) staff       (20)       38 2024-05-14 07:36:18.223945 pywayne-1.0.0.7.2/setup.cfg
--rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.7.2/setup.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.843858 pywayne-1.0.0.7.3/
+-rw-r--r--   0 wayne      (503) staff       (20)     1064 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/LICENSE
+-rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-24 03:28:40.843591 pywayne-1.0.0.7.3/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      600 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/README.md
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.839822 pywayne-1.0.0.7.3/bin/
+-rw-r--r--   0 wayne      (503) staff       (20)       63 2023-11-01 16:27:11.000000 pywayne-1.0.0.7.3/bin/gettool
+-rw-r--r--   0 wayne      (503) staff       (20)     4261 2023-11-06 12:31:36.000000 pywayne-1.0.0.7.3/bin/gettool.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.841081 pywayne-1.0.0.7.3/pywayne/
+-rw-r--r--   0 wayne      (503) staff       (20)      207 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/pywayne/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)      242 2024-05-24 03:26:24.000000 pywayne-1.0.0.7.3/pywayne/__version__.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.841972 pywayne-1.0.0.7.3/pywayne/adb/
+-rw-r--r--   0 wayne      (503) staff       (20)      278 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.3/pywayne/adb/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2168 2023-11-07 03:21:11.000000 pywayne-1.0.0.7.3/pywayne/adb/logcat_reader.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.842234 pywayne-1.0.0.7.3/pywayne/ahrs/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/pywayne/ahrs/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4038 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/pywayne/ahrs/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.842628 pywayne-1.0.0.7.3/pywayne/calibration/
+-rw-r--r--   0 wayne      (503) staff       (20)      211 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/pywayne/calibration/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     4269 2023-12-05 12:13:27.000000 pywayne-1.0.0.7.3/pywayne/calibration/magnetometer_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)      223 2023-12-05 11:52:18.000000 pywayne-1.0.0.7.3/pywayne/calibration/temporal_calibration.py
+-rw-r--r--   0 wayne      (503) staff       (20)     6948 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/pywayne/data_structure.py
+-rw-r--r--   0 wayne      (503) staff       (20)    16705 2023-11-11 07:27:50.000000 pywayne-1.0.0.7.3/pywayne/dsp.py
+-rw-r--r--   0 wayne      (503) staff       (20)     7535 2023-11-11 18:58:57.000000 pywayne-1.0.0.7.3/pywayne/gui.py
+-rw-r--r--   0 wayne      (503) staff       (20)     2433 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/pywayne/math.py
+-rw-r--r--   0 wayne      (503) staff       (20)    14981 2023-11-01 17:13:21.000000 pywayne-1.0.0.7.3/pywayne/plot.py
+-rw-r--r--   0 wayne      (503) staff       (20)    18046 2024-05-24 03:26:24.000000 pywayne-1.0.0.7.3/pywayne/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.842887 pywayne-1.0.0.7.3/pywayne/vio/
+-rw-r--r--   0 wayne      (503) staff       (20)      243 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.3/pywayne/vio/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3281 2024-01-13 09:21:45.000000 pywayne-1.0.0.7.3/pywayne/vio/tools.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.843171 pywayne-1.0.0.7.3/pywayne/visualization/
+-rw-r--r--   0 wayne      (503) staff       (20)      271 2023-11-06 04:42:24.000000 pywayne-1.0.0.7.3/pywayne/visualization/__init__.py
+-rw-r--r--   0 wayne      (503) staff       (20)     3766 2023-11-11 18:56:53.000000 pywayne-1.0.0.7.3/pywayne/visualization/pangolin.py
+drwxr-xr-x   0 wayne      (503) staff       (20)        0 2024-05-24 03:28:40.843354 pywayne-1.0.0.7.3/pywayne.egg-info/
+-rw-r--r--   0 wayne      (503) staff       (20)     1485 2024-05-24 03:28:40.000000 pywayne-1.0.0.7.3/pywayne.egg-info/PKG-INFO
+-rw-r--r--   0 wayne      (503) staff       (20)      692 2024-05-24 03:28:40.000000 pywayne-1.0.0.7.3/pywayne.egg-info/SOURCES.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      184 2024-05-24 03:28:40.000000 pywayne-1.0.0.7.3/pywayne.egg-info/dependency_links.txt
+-rw-r--r--   0 wayne      (503) staff       (20)      162 2024-05-24 03:28:40.000000 pywayne-1.0.0.7.3/pywayne.egg-info/requires.txt
+-rw-r--r--   0 wayne      (503) staff       (20)        8 2024-05-24 03:28:40.000000 pywayne-1.0.0.7.3/pywayne.egg-info/top_level.txt
+-rw-r--r--   0 wayne      (503) staff       (20)       38 2024-05-24 03:28:40.843907 pywayne-1.0.0.7.3/setup.cfg
+-rw-r--r--   0 wayne      (503) staff       (20)     1555 2023-11-05 05:52:08.000000 pywayne-1.0.0.7.3/setup.py
```

### Comparing `pywayne-1.0.0.7.2/LICENSE` & `pywayne-1.0.0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/PKG-INFO` & `pywayne-1.0.0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.7.2
+Version: 1.0.0.7.3
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.7.2/README.md` & `pywayne-1.0.0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/bin/gettool.py` & `pywayne-1.0.0.7.3/bin/gettool.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/adb/logcat_reader.py` & `pywayne-1.0.0.7.3/pywayne/adb/logcat_reader.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/ahrs/tools.py` & `pywayne-1.0.0.7.3/pywayne/ahrs/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/calibration/magnetometer_calibration.py` & `pywayne-1.0.0.7.3/pywayne/calibration/magnetometer_calibration.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/data_structure.py` & `pywayne-1.0.0.7.3/pywayne/data_structure.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/dsp.py` & `pywayne-1.0.0.7.3/pywayne/dsp.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/gui.py` & `pywayne-1.0.0.7.3/pywayne/gui.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/math.py` & `pywayne-1.0.0.7.3/pywayne/math.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/plot.py` & `pywayne-1.0.0.7.3/pywayne/plot.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/tools.py` & `pywayne-1.0.0.7.3/pywayne/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,20 +371,20 @@
 
     class ColoredFormatter(logging.Formatter):
         """
         A Formatter that adds color codes to log levels for console output.
         """
         # ANSI escape sequences for colors.
         COLORS = {
-            'DEBUG': '\033[36m\033[1m',     # Cyan
-            'INFO': '\033[32m\033[1m',      # Bright green
-            'WARNING': '\033[33m\033[1m',   # Bright yellow
-            'ERROR': '\033[31m\033[1m',     # Bright red
+            'DEBUG': '\033[36m\033[1m',  # Cyan
+            'INFO': '\033[32m\033[1m',  # Bright green
+            'WARNING': '\033[33m\033[1m',  # Bright yellow
+            'ERROR': '\033[31m\033[1m',  # Bright red
             'CRITICAL': '\033[35m\033[1m',  # Purple
-            'ENDC': '\033[0m',              # Reset to default color
+            'ENDC': '\033[0m',  # Reset to default color
         }
 
         def format(self, record):
             levelname = record.levelname
             if levelname in self.COLORS:
                 record.levelname = f"{self.COLORS[levelname]}{levelname}{self.COLORS['ENDC']}"
             return super().format(record)
@@ -481,20 +481,19 @@
             else:
                 original[key] = value
         return original
 
     lock_file = config_yaml_file + ".lock"
     lock = FileLock(lock_file)
 
-    if update and os.path.exists(config_yaml_file):
-        existing_config = read_yaml_config(config_yaml_file)
-    else:
-        existing_config = {}
-
     with lock:
+        if update and os.path.exists(config_yaml_file):
+            existing_config = read_yaml_config(config_yaml_file)
+        else:
+            existing_config = {}
         if update:
             config = deep_merge_dicts(existing_config, config)
         with open(config_yaml_file, 'w', encoding='UTF-8') as f:
             yaml.dump(config, f, default_flow_style=False)
 
 
 def read_yaml_config(config_yaml_file: str):
```

### Comparing `pywayne-1.0.0.7.2/pywayne/vio/tools.py` & `pywayne-1.0.0.7.3/pywayne/vio/tools.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne/visualization/pangolin.py` & `pywayne-1.0.0.7.3/pywayne/visualization/pangolin.py`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/pywayne.egg-info/PKG-INFO` & `pywayne-1.0.0.7.3/pywayne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywayne
-Version: 1.0.0.7.2
+Version: 1.0.0.7.3
 Summary: Some useful tools
 Home-page: https://github.com/wangyendt/wangye_algorithm_lib
 Author: Wayne
 Author-email: wang121ye@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pywayne-1.0.0.7.2/pywayne.egg-info/SOURCES.txt` & `pywayne-1.0.0.7.3/pywayne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywayne-1.0.0.7.2/setup.py` & `pywayne-1.0.0.7.3/setup.py`

 * *Files identical despite different names*

