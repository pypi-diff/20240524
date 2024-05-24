# Comparing `tmp/abeewayconfig-0.2.2.9.tar.gz` & `tmp/abeewayconfig-0.2.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abeewayconfig-0.2.2.9.tar", last modified: Thu May 23 16:33:55 2024, max compression
+gzip compressed data, was "abeewayconfig-0.2.2.9.1.tar", last modified: Thu May 23 20:19:07 2024, max compression
```

## Comparing `abeewayconfig-0.2.2.9.tar` & `abeewayconfig-0.2.2.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/
--rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.2.9/LICENSE
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1695 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1307 2024-05-23 15:33:30.000000 abeewayconfig-0.2.2.9/README.md
--rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/setup.cfg
--rw-r--r--   0 lucas     (1001) lucas     (1001)      851 2024-05-23 16:29:40.000000 abeewayconfig-0.2.2.9/setup.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 16:33:55.004683 abeewayconfig-0.2.2.9/src/
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/src/AbeewayConfig/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4700 2024-05-23 16:09:37.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/CSVFile.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     3430 2024-05-22 20:24:17.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/Config.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     2906 2024-05-23 16:27:23.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/Device.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/__init__.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     6138 2024-05-23 15:33:47.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/abeewayconfig.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/smartbadgecfgdict.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1695 2024-05-23 16:33:54.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)      463 2024-05-23 16:33:55.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-23 16:33:54.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)      121 2024-05-23 16:33:55.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       12 2024-05-23 16:33:55.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/requires.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-23 16:33:55.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 20:19:07.074667 abeewayconfig-0.2.2.9.1/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.2.9.1/LICENSE
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1721 2024-05-23 20:19:07.074667 abeewayconfig-0.2.2.9.1/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1307 2024-05-23 15:33:30.000000 abeewayconfig-0.2.2.9.1/README.md
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-23 20:19:07.074667 abeewayconfig-0.2.2.9.1/setup.cfg
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      873 2024-05-23 20:18:02.000000 abeewayconfig-0.2.2.9.1/setup.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 20:19:07.071334 abeewayconfig-0.2.2.9.1/src/
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 20:19:07.071334 abeewayconfig-0.2.2.9.1/src/AbeewayConfig/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     6566 2024-05-23 20:08:49.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig/CSVFile.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     3492 2024-05-23 20:11:22.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig/Config.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     2906 2024-05-23 16:48:09.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig/Device.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig/__init__.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     6185 2024-05-23 20:18:36.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig/abeewayconfig.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig/smartbadgecfgdict.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 20:19:07.071334 abeewayconfig-0.2.2.9.1/src/AbeewayConfig.egg-info/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1721 2024-05-23 20:19:07.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      463 2024-05-23 20:19:07.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-23 20:19:07.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      121 2024-05-23 20:19:07.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       21 2024-05-23 20:19:07.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-23 20:19:07.000000 abeewayconfig-0.2.2.9.1/src/AbeewayConfig.egg-info/top_level.txt
```

### Comparing `abeewayconfig-0.2.2.9/LICENSE` & `abeewayconfig-0.2.2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.9/PKG-INFO` & `abeewayconfig-0.2.2.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.2.9
+Version: 0.2.2.9.1
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: tk
+Requires-Dist: requests
 
 # Abeeway Tracker Configurator
 
 ## About
 Python project useful if you want to configure multiple serial devices at once through their CLI. Right now, it's designed to be used to configure Abeeway's trackers.
 
 ![](https://i.ibb.co/HptPP0S/Screenshot-2024-05-15-15-25-08.png)
```

### Comparing `abeewayconfig-0.2.2.9/README.md` & `abeewayconfig-0.2.2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.9/setup.py` & `abeewayconfig-0.2.2.9.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="AbeewayConfig",
-    version="0.2.2.9",
+    version="0.2.2.9.1",
     description="Abeeway configuration tool",
     author="João Lucas",
     url="https://github.com/jlabbude/AbeewayConfig",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "pyserial",
         "tk",
+        "requests",
     ],
     entry_points={
         "console_scripts": [
             "abeewayconfig = AbeewayConfig.abeewayconfig:main",
             "abeewayupload = AbeewayConfig.abeewayconfig:nw_sv_gui"
         ],
     },
```

### Comparing `abeewayconfig-0.2.2.9/src/AbeewayConfig/Config.py` & `abeewayconfig-0.2.2.9.1/src/AbeewayConfig/Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,18 @@
                 for line in config:
                     config_parameter_cfg = Config.get_config_parameter_from_cfg(line)
                     config_value_cfg = Config.get_config_value_from_cfg(config_parameter_cfg, line)
                     config_name = config_dict.get(config_parameter_cfg)
                     if config_parameter_cfg is not None or config_value_cfg is not None:
                         config_value_dev = Device.get_config_value_from_dev(device_config, config_name)
 
-                        if config_parameter_cfg is 249 and config_value_dev is 5:
+                        if config_parameter_cfg == 249 and config_value_dev == 5:
                             console_output.insert(tk.END, f"Config error: {deveui} \n")
-                            console_output.insert(tk.END, f"An error occurred. Please try starting the device, then configuring again. \n")
+                            console_output.insert(tk.END, f"An error occurred. Please try starting the device, "
+                                                          f"then configuring again. \n")
                             return False
 
                         if config_value_cfg != config_value_dev:
                             console_output.insert(tk.END, f"Config error: {deveui} \n")
                             console_output.insert(tk.END, f"[Parameter : {config_name}] - Current: [{config_value_dev}] | Correct: [{config_value_cfg}] \n")
                             return False
         except FileNotFoundError:
```

### Comparing `abeewayconfig-0.2.2.9/src/AbeewayConfig/Device.py` & `abeewayconfig-0.2.2.9.1/src/AbeewayConfig/Device.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.9/src/AbeewayConfig/abeewayconfig.py` & `abeewayconfig-0.2.2.9.1/src/AbeewayConfig/abeewayconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 def define_os_specific_startingdir() -> str:
     match operating_system:
         case "Linux":
             return "~/Desktop"
         case "Windows":
             return "~\\Desktop"
+        case _:
+            return "~/Desktop"
 
 
 def serial_parallel_process(target) -> None:
     threads = []
     for serial_port in serial_port_array:
         thread = Thread(target=target, args=(serial_port, baud_rate))
         threads.append(thread)
```

### Comparing `abeewayconfig-0.2.2.9/src/AbeewayConfig/smartbadgecfgdict.py` & `abeewayconfig-0.2.2.9.1/src/AbeewayConfig/smartbadgecfgdict.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/PKG-INFO` & `abeewayconfig-0.2.2.9.1/src/AbeewayConfig.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.2.9
+Version: 0.2.2.9.1
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: tk
+Requires-Dist: requests
 
 # Abeeway Tracker Configurator
 
 ## About
 Python project useful if you want to configure multiple serial devices at once through their CLI. Right now, it's designed to be used to configure Abeeway's trackers.
 
 ![](https://i.ibb.co/HptPP0S/Screenshot-2024-05-15-15-25-08.png)
```

