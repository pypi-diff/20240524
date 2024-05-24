# Comparing `tmp/ch9329-1.0.9.tar.gz` & `tmp/ch9329-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ch9329-1.0.9.tar", last modified: Wed May  8 10:49:10 2024, max compression
+gzip compressed data, was "ch9329-1.1.0.tar", last modified: Fri May 24 15:21:21 2024, max compression
```

## Comparing `ch9329-1.0.9.tar` & `ch9329-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:10.631512 ch9329-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-08 10:49:06.000000 ch9329-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 10:49:06.000000 ch9329-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-08 10:49:10.631512 ch9329-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-08 10:49:06.000000 ch9329-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:10.631512 ch9329-1.0.9/ch9329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/hid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-08 10:49:06.000000 ch9329-1.0.9/ch9329/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:49:10.631512 ch9329-1.0.9/ch9329.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 10:49:10.000000 ch9329-1.0.9/ch9329.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-08 10:49:06.000000 ch9329-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:49:10.631512 ch9329-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:21:21.479537 ch9329-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-24 15:21:17.000000 ch9329-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 15:21:17.000000 ch9329-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 15:21:21.479537 ch9329-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-24 15:21:17.000000 ch9329-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:21:21.479537 ch9329-1.1.0/ch9329/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:21:17.000000 ch9329-1.1.0/ch9329/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-05-24 15:21:17.000000 ch9329-1.1.0/ch9329/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 15:21:17.000000 ch9329-1.1.0/ch9329/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-05-24 15:21:17.000000 ch9329-1.1.0/ch9329/hid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-24 15:21:17.000000 ch9329-1.1.0/ch9329/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-24 15:21:17.000000 ch9329-1.1.0/ch9329/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:21:17.000000 ch9329-1.1.0/ch9329/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-24 15:21:17.000000 ch9329-1.1.0/ch9329/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:21:21.479537 ch9329-1.1.0/ch9329.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 15:21:21.000000 ch9329-1.1.0/ch9329.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-24 15:21:21.000000 ch9329-1.1.0/ch9329.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:21:21.000000 ch9329-1.1.0/ch9329.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 15:21:21.000000 ch9329-1.1.0/ch9329.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 15:21:21.000000 ch9329-1.1.0/ch9329.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-24 15:21:17.000000 ch9329-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:21:21.479537 ch9329-1.1.0/setup.cfg
```

### Comparing `ch9329-1.0.9/LICENSE` & `ch9329-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.9/PKG-INFO` & `ch9329-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -46,28 +46,38 @@
 ## Usage
 
 ```py
 from serial import Serial
 
 from ch9329 import keyboard
 from ch9329 import mouse
+from ch9329.config import get_manufacturer
+from ch9329.config import get_product
+from ch9329.config import get_serial_number
 
 ser = Serial("COM3", 9600, timeout=1)
 
 keyboard.press_and_release(ser, "a", modifier="ctrl")
 keyboard.write(ser, "Hello World\n")
 keyboard.write(ser, "abcdefghijklmnopqrstuvwxyz\n")
 keyboard.write(ser, "ABCDEFGHIJKLMNOPQRSTUVWXYZ\n")
 keyboard.write(ser, "0123456789\n")
 keyboard.write(ser, "!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~\n")
 
 mouse.move(ser, x=500, y=500)
 mouse.move(ser, x=50, y=50, relative=True)
 mouse.click(ser, button="left")
 
+print(get_serial_number(ser))
+# 20193152CFBF
+print(get_product(ser))
+# WCH UART TO KB-MS_V1.7
+print(get_manufacturer(ser))
+# WWW.WCH.CN
+
 ser.close()
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `ch9329-1.0.9/ch9329/hid.py` & `ch9329-1.1.0/ch9329/hid.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.9/ch9329/keyboard.py` & `ch9329-1.1.0/ch9329/keyboard.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.9/ch9329/mouse.py` & `ch9329-1.1.0/ch9329/mouse.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.9/ch9329/utils.py` & `ch9329-1.1.0/ch9329/utils.py`

 * *Files identical despite different names*

### Comparing `ch9329-1.0.9/ch9329.egg-info/PKG-INFO` & `ch9329-1.1.0/ch9329.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ch9329
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python module to control ch9329
 Author-email: Pradish Bijukchhe <pradish@sandbox.com.np>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -46,28 +46,38 @@
 ## Usage
 
 ```py
 from serial import Serial
 
 from ch9329 import keyboard
 from ch9329 import mouse
+from ch9329.config import get_manufacturer
+from ch9329.config import get_product
+from ch9329.config import get_serial_number
 
 ser = Serial("COM3", 9600, timeout=1)
 
 keyboard.press_and_release(ser, "a", modifier="ctrl")
 keyboard.write(ser, "Hello World\n")
 keyboard.write(ser, "abcdefghijklmnopqrstuvwxyz\n")
 keyboard.write(ser, "ABCDEFGHIJKLMNOPQRSTUVWXYZ\n")
 keyboard.write(ser, "0123456789\n")
 keyboard.write(ser, "!\"#$%&'()*+,-./:;<=>?@[\\]^_`{|}~\n")
 
 mouse.move(ser, x=500, y=500)
 mouse.move(ser, x=50, y=50, relative=True)
 mouse.click(ser, button="left")
 
+print(get_serial_number(ser))
+# 20193152CFBF
+print(get_product(ser))
+# WCH UART TO KB-MS_V1.7
+print(get_manufacturer(ser))
+# WWW.WCH.CN
+
 ser.close()
 ```
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `ch9329-1.0.9/pyproject.toml` & `ch9329-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ch9329"
-version = "1.0.9"
+version = "1.1.0"
 dependencies = ["pyserial"]
 requires-python = ">=3"
 authors = [{ name = "Pradish Bijukchhe", email = "pradish@sandbox.com.np" }]
 description = "Python module to control ch9329"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = []
```

