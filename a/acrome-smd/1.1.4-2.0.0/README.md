# Comparing `tmp/acrome-smd-1.1.4.tar.gz` & `tmp/acrome_smd-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrome-smd-1.1.4.tar", last modified: Fri Jan  5 12:02:23 2024, max compression
+gzip compressed data, was "acrome_smd-2.0.0.tar", last modified: Fri May 24 07:29:37 2024, max compression
```

## Comparing `acrome-smd-1.1.4.tar` & `acrome_smd-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 12:02:23.767119 acrome-smd-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-05 12:02:14.000000 acrome-smd-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    33381 2024-01-05 12:02:23.767119 acrome-smd-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    33546 2024-01-05 12:02:14.000000 acrome-smd-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 12:02:23.767119 acrome-smd-1.1.4/acrome_smd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    33381 2024-01-05 12:02:23.000000 acrome-smd-1.1.4/acrome_smd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-05 12:02:23.000000 acrome-smd-1.1.4/acrome_smd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 12:02:23.000000 acrome-smd-1.1.4/acrome_smd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-05 12:02:23.000000 acrome-smd-1.1.4/acrome_smd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-05 12:02:23.000000 acrome-smd-1.1.4/acrome_smd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-05 12:02:23.767119 acrome-smd-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-05 12:02:14.000000 acrome-smd-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 12:02:23.767119 acrome-smd-1.1.4/smd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 12:02:14.000000 acrome-smd-1.1.4/smd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-01-05 12:02:14.000000 acrome-smd-1.1.4/smd/_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)    52785 2024-01-05 12:02:14.000000 acrome-smd-1.1.4/smd/red.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 12:02:23.767119 acrome-smd-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-01-05 12:02:14.000000 acrome-smd-1.1.4/tests/test_red.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    34174 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34326 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/acrome_smd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34174 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-24 07:29:37.000000 acrome_smd-2.0.0/acrome_smd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:37.414240 acrome_smd-2.0.0/smd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/smd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/smd/_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64185 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/smd/red.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:29:37.418239 acrome_smd-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 07:29:30.000000 acrome_smd-2.0.0/tests/test_red.py
```

### Comparing `acrome-smd-1.1.4/LICENSE` & `acrome_smd-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acrome-smd-1.1.4/PKG-INFO` & `acrome_smd-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrome-smd
-Version: 1.1.4
+Version: 2.0.0
 Summary: Python library for interfacing with Acrome Smart Motor Drivers (SMD) products.
 Home-page: https://github.com/Acrome-Smart-Motor-Driver/python-library
 Author: Furkan Kırlangıç
 Author-email: furkankirlangic@acrome.net
 Project-URL: Bug Tracker, https://github.com/Acrome-Smart-Motor-Driver/python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -51,15 +51,15 @@
 
 2. Install SMD library using `pip` (Python package manager) by running the following command:
 
   ```shell
   pip install acrome-smd
   ```
 
-3. Wait for the installation to complete. Pip willmnmnmnmn automatically download and install the library along with any required dependencies.
+3. Wait for the installation to complete. Pip will automatically download and install the library along with any required dependencies.
 
 #### Linux
 1. Open a terminal.
 
 2. Install SMD library using pip (Python package manager) by running the following command:
 
   ```shell
@@ -745,67 +745,67 @@
     `id` argument is the device ID of the connected driver.
 
 
 
 # SMD Modules
 ### SMD Modules Basic
 To use SMD modules, you should initially utilize the following scanning function. This function returns which modules are connected to the SMD. Each module has a type and an ID, and through this scanning process, you can learn these properties of the connected modules. When the board is powered up for the first time, this scan is automatically performed once, but afterward, this command should be used manually.
-  - #### `scan_sensors(self, id: int)`
+  - #### `scan_modules(self, id: int):`
 
-    **`Return:`** *List of connected sensors*
+    **`Return:`** *List of connected modules*
     
-    This method scans and returns the sensor IDs which are currently connected to a driver.
+    This method scans and returns the module IDs which are currently connected to a driver.
 
     `id` argument is the device ID of the connected driver.
 
 #### Button Module
-  - ####  `get_button(self, id: int, index: Index)`
+  - ####  `get_button(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the button state*
 
       This method gets the button module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the button module.
+      `module_id` argument is the module ID of the button. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Light Module
-  - ####  `get_light(self, id: int, index: Index):`
+  - ####  `get_light(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the ambient light measurement (in lux)*
 
       This method gets the ambient light module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the ambient light module.
+      `module_id` argument is the module ID of the ambient light. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Buzzer Module
-  - ####  `set_buzzer(self, id: int, index: Index, en: bool):`
+  - ####  `set_buzzer(self, id: int, module_id: int, note_frequency: int)`
 
     **`Return:`** *None*
 
       This method enables/disables the buzzer module with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the buzzer module.
+      `module_id` argument is the module ID of the buzzer. It takes values in the range of 1 - 5 (including 1 and 5).
 
-      `en` argument enables or disables the buzzer. (Enable = 1, Disable = 0)
+      `note_frequency` argument specifies the frequency of the tone in Hertz. 0 Hertz will result in no tone.
 
 #### Joystick Module
-  - ####  `get_joystick(self, id: int, index: Index):`
+  - ####  `get_joystick(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the joystick module analogs and button data*
 
       This method gets the joystick module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the joystick module.
+      `module_id` argument is the module ID of the joystick. It takes values in the range of 1 - 5 (including 1 and 5).
 
   #### Example of Joystick Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
@@ -816,119 +816,106 @@
     joystick = m.get_joystick(0, Index.Joystick_1)
     joystick_X = joystick[0]
     joystick_Y = joystick[1]
     joystick_button = joystick[2]
   ```
 
 #### Distance Module
-  - ####  `get_distance(self, id: int, index: Index):`
+  - ####  `get_distance(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the distance from the ultrasonic distance module (in cm)*
 
       This method gets the ultrasonic distance module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the ultrasonic distance module.
+      `module_id` argument is the module ID of the ultrasonic distance module. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### QTR Module
-  - ####  `get_qtr(self, id: int, index: Index):`
+  - ####  `get_qtr(self, id: int, module_id: int):`
 
-    **`Return:`** *Returns qtr module data: [Left(bool), Middle(bool), Right(bool)]*
+    **`Return:`** *Returns QTR module data: [Left(bool), Middle(bool), Right(bool)]*
 
-      This method gets the qtr module data with given index.
+      This method gets the QTR module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the qtr module.
+      `module_id` argument is the module ID of the QTR. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Servo Module
-  - ####  `set_servo(self, id: int, index: Index, val: int):`
+  - ####  `set_servo(self, id: int, module_id: int, val: int):`
 
     **`Return:`** *None*
 
       This method moves servo module to a desired position.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the servo module.
+      `module_id` argument is the module ID of the servo. It takes values in the range of 1 - 5 (including 1 and 5)
 
-      `val`argument is the value to write to the servo (0, 255).
+      `val` argument is the value to write to the servo. It takes values in the range of 0 - 255 (including 0 and 255).
 
-#### Potantiometer Module
-  - ####  `get_potantiometer(self, id: int, index: Index):`
+#### Potentiometer Module
+  - ####  `get_potentiometer(self, id: int, module_id: int):`
 
-    **`Return:`** *Returns the ADC conversion from the potantiometer module*
+    **`Return:`** *Returns the ADC conversion from the potentiometer module*
 
-      This method gets the potantiometer module data with given index.
+      This method gets the potentiometer module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the potantiometer module.
+      `module_id` argument is the module ID of the potentiometer. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### RGB Led Module
 The setRGB() method is used to control an RGB Led module by specifying the intensity or color values for each of the RGB components.
 
-  - ####  `set_rgb(self, id: int, index: Index, color: Colors):`
+  - ####  `set_rgb(self, id: int, module_id: int, red: int, green: int, blue: int):`
 
     **`Return:`** *None*
 
       This method sets the colour emitted from the RGB module.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the RGB module.
+      `module_id` argument is the module ID of the RGB. It takes values in the range of 1 - 5 (including 1 and 5).
 
-      `color` argument is the color for RGB from Colors class.
+      `red` argument is representing red color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
+      `green` argument is representing green color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
-  Colors available in RGB sensor module :
-  - NO_COLOR,
-  - RED,
-  - GREEN,
-  - BLUE,
-  - WHITE,
-  - YELLOW,
-  - CYAN,
-  - MAGENTA,
-  - ORANGE,
-  - PURPLE,
-  - PINK,
-  - AMBER,
-  - TEAL,
-  - INDIGO
+      `blue` argument is representing blue color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
   The method and colors can be used as in the example below for the RGB module.
   #### Example of RGB Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
   m.scan_modules(0)
 
-  m.set_rgb(0, Index.RGB_1, Colors.RED)
+  m.set_rgb(0, Index.RGB_1, 255, 0, 0) # Red color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.GREEN)
+  m.set_rgb(0, Index.RGB_1, 0, 255, 0) # Green color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.BLUE)
+  m.set_rgb(0, Index.RGB_1, 0, 0, 255) # Blue color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.PURPLE)
+  m.set_rgb(0, Index.RGB_1, 128, 0, 128) # Purple color
   time.sleep(0.5)
   ```
 #### IMU Module
-  - ####  `get_imu(self, id: int, index: Index):`
+  - ####  `get_imu(self, id: int, module_id: int):`
 
     **`Return:`** *Returns roll, pitch angles*
 
       This method gets the IMU module data (roll, pitch).
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the IMU module.
+      `module_id` argument is the module ID of the IMU. It takes values in the range of 1 - 5 (including 1 and 5).
 
   #### Example of IMU Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
```

### Comparing `acrome-smd-1.1.4/README.md` & `acrome_smd-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 2. Install SMD library using `pip` (Python package manager) by running the following command:
 
   ```shell
   pip install acrome-smd
   ```
 
-3. Wait for the installation to complete. Pip willmnmnmnmn automatically download and install the library along with any required dependencies.
+3. Wait for the installation to complete. Pip will automatically download and install the library along with any required dependencies.
 
 #### Linux
 1. Open a terminal.
 
 2. Install SMD library using pip (Python package manager) by running the following command:
 
   ```shell
@@ -725,67 +725,67 @@
     `id` argument is the device ID of the connected driver.
 
 
 
 # SMD Modules
 ### SMD Modules Basic
 To use SMD modules, you should initially utilize the following scanning function. This function returns which modules are connected to the SMD. Each module has a type and an ID, and through this scanning process, you can learn these properties of the connected modules. When the board is powered up for the first time, this scan is automatically performed once, but afterward, this command should be used manually.
-  - #### `scan_sensors(self, id: int)`
+  - #### `scan_modules(self, id: int):`
 
-    **`Return:`** *List of connected sensors*
+    **`Return:`** *List of connected modules*
     
-    This method scans and returns the sensor IDs which are currently connected to a driver.
+    This method scans and returns the module IDs which are currently connected to a driver.
 
     `id` argument is the device ID of the connected driver.
 
 #### Button Module
-  - ####  `get_button(self, id: int, index: Index)`
+  - ####  `get_button(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the button state*
 
       This method gets the button module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the button module.
+      `module_id` argument is the module ID of the button. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Light Module
-  - ####  `get_light(self, id: int, index: Index):`
+  - ####  `get_light(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the ambient light measurement (in lux)*
 
       This method gets the ambient light module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the ambient light module.
+      `module_id` argument is the module ID of the ambient light. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Buzzer Module
-  - ####  `set_buzzer(self, id: int, index: Index, en: bool):`
+  - ####  `set_buzzer(self, id: int, module_id: int, note_frequency: int)`
 
     **`Return:`** *None*
 
       This method enables/disables the buzzer module with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the buzzer module.
+      `module_id` argument is the module ID of the buzzer. It takes values in the range of 1 - 5 (including 1 and 5).
 
-      `en` argument enables or disables the buzzer. (Enable = 1, Disable = 0)
+      `note_frequency` argument specifies the frequency of the tone in Hertz. 0 Hertz will result in no tone.
 
 #### Joystick Module
-  - ####  `get_joystick(self, id: int, index: Index):`
+  - ####  `get_joystick(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the joystick module analogs and button data*
 
       This method gets the joystick module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the joystick module.
+      `module_id` argument is the module ID of the joystick. It takes values in the range of 1 - 5 (including 1 and 5).
 
   #### Example of Joystick Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
@@ -796,119 +796,106 @@
     joystick = m.get_joystick(0, Index.Joystick_1)
     joystick_X = joystick[0]
     joystick_Y = joystick[1]
     joystick_button = joystick[2]
   ```
 
 #### Distance Module
-  - ####  `get_distance(self, id: int, index: Index):`
+  - ####  `get_distance(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the distance from the ultrasonic distance module (in cm)*
 
       This method gets the ultrasonic distance module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the ultrasonic distance module.
+      `module_id` argument is the module ID of the ultrasonic distance module. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### QTR Module
-  - ####  `get_qtr(self, id: int, index: Index):`
+  - ####  `get_qtr(self, id: int, module_id: int):`
 
-    **`Return:`** *Returns qtr module data: [Left(bool), Middle(bool), Right(bool)]*
+    **`Return:`** *Returns QTR module data: [Left(bool), Middle(bool), Right(bool)]*
 
-      This method gets the qtr module data with given index.
+      This method gets the QTR module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the qtr module.
+      `module_id` argument is the module ID of the QTR. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Servo Module
-  - ####  `set_servo(self, id: int, index: Index, val: int):`
+  - ####  `set_servo(self, id: int, module_id: int, val: int):`
 
     **`Return:`** *None*
 
       This method moves servo module to a desired position.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the servo module.
+      `module_id` argument is the module ID of the servo. It takes values in the range of 1 - 5 (including 1 and 5)
 
-      `val`argument is the value to write to the servo (0, 255).
+      `val` argument is the value to write to the servo. It takes values in the range of 0 - 255 (including 0 and 255).
 
-#### Potantiometer Module
-  - ####  `get_potantiometer(self, id: int, index: Index):`
+#### Potentiometer Module
+  - ####  `get_potentiometer(self, id: int, module_id: int):`
 
-    **`Return:`** *Returns the ADC conversion from the potantiometer module*
+    **`Return:`** *Returns the ADC conversion from the potentiometer module*
 
-      This method gets the potantiometer module data with given index.
+      This method gets the potentiometer module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the potantiometer module.
+      `module_id` argument is the module ID of the potentiometer. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### RGB Led Module
 The setRGB() method is used to control an RGB Led module by specifying the intensity or color values for each of the RGB components.
 
-  - ####  `set_rgb(self, id: int, index: Index, color: Colors):`
+  - ####  `set_rgb(self, id: int, module_id: int, red: int, green: int, blue: int):`
 
     **`Return:`** *None*
 
       This method sets the colour emitted from the RGB module.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the RGB module.
+      `module_id` argument is the module ID of the RGB. It takes values in the range of 1 - 5 (including 1 and 5).
 
-      `color` argument is the color for RGB from Colors class.
+      `red` argument is representing red color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
+      `green` argument is representing green color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
-  Colors available in RGB sensor module :
-  - NO_COLOR,
-  - RED,
-  - GREEN,
-  - BLUE,
-  - WHITE,
-  - YELLOW,
-  - CYAN,
-  - MAGENTA,
-  - ORANGE,
-  - PURPLE,
-  - PINK,
-  - AMBER,
-  - TEAL,
-  - INDIGO
+      `blue` argument is representing blue color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
   The method and colors can be used as in the example below for the RGB module.
   #### Example of RGB Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
   m.scan_modules(0)
 
-  m.set_rgb(0, Index.RGB_1, Colors.RED)
+  m.set_rgb(0, Index.RGB_1, 255, 0, 0) # Red color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.GREEN)
+  m.set_rgb(0, Index.RGB_1, 0, 255, 0) # Green color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.BLUE)
+  m.set_rgb(0, Index.RGB_1, 0, 0, 255) # Blue color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.PURPLE)
+  m.set_rgb(0, Index.RGB_1, 128, 0, 128) # Purple color
   time.sleep(0.5)
   ```
 #### IMU Module
-  - ####  `get_imu(self, id: int, index: Index):`
+  - ####  `get_imu(self, id: int, module_id: int):`
 
     **`Return:`** *Returns roll, pitch angles*
 
       This method gets the IMU module data (roll, pitch).
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the IMU module.
+      `module_id` argument is the module ID of the IMU. It takes values in the range of 1 - 5 (including 1 and 5).
 
   #### Example of IMU Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
```

### Comparing `acrome-smd-1.1.4/acrome_smd.egg-info/PKG-INFO` & `acrome_smd-2.0.0/acrome_smd.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrome-smd
-Version: 1.1.4
+Version: 2.0.0
 Summary: Python library for interfacing with Acrome Smart Motor Drivers (SMD) products.
 Home-page: https://github.com/Acrome-Smart-Motor-Driver/python-library
 Author: Furkan Kırlangıç
 Author-email: furkankirlangic@acrome.net
 Project-URL: Bug Tracker, https://github.com/Acrome-Smart-Motor-Driver/python-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -51,15 +51,15 @@
 
 2. Install SMD library using `pip` (Python package manager) by running the following command:
 
   ```shell
   pip install acrome-smd
   ```
 
-3. Wait for the installation to complete. Pip willmnmnmnmn automatically download and install the library along with any required dependencies.
+3. Wait for the installation to complete. Pip will automatically download and install the library along with any required dependencies.
 
 #### Linux
 1. Open a terminal.
 
 2. Install SMD library using pip (Python package manager) by running the following command:
 
   ```shell
@@ -745,67 +745,67 @@
     `id` argument is the device ID of the connected driver.
 
 
 
 # SMD Modules
 ### SMD Modules Basic
 To use SMD modules, you should initially utilize the following scanning function. This function returns which modules are connected to the SMD. Each module has a type and an ID, and through this scanning process, you can learn these properties of the connected modules. When the board is powered up for the first time, this scan is automatically performed once, but afterward, this command should be used manually.
-  - #### `scan_sensors(self, id: int)`
+  - #### `scan_modules(self, id: int):`
 
-    **`Return:`** *List of connected sensors*
+    **`Return:`** *List of connected modules*
     
-    This method scans and returns the sensor IDs which are currently connected to a driver.
+    This method scans and returns the module IDs which are currently connected to a driver.
 
     `id` argument is the device ID of the connected driver.
 
 #### Button Module
-  - ####  `get_button(self, id: int, index: Index)`
+  - ####  `get_button(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the button state*
 
       This method gets the button module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the button module.
+      `module_id` argument is the module ID of the button. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Light Module
-  - ####  `get_light(self, id: int, index: Index):`
+  - ####  `get_light(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the ambient light measurement (in lux)*
 
       This method gets the ambient light module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the ambient light module.
+      `module_id` argument is the module ID of the ambient light. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Buzzer Module
-  - ####  `set_buzzer(self, id: int, index: Index, en: bool):`
+  - ####  `set_buzzer(self, id: int, module_id: int, note_frequency: int)`
 
     **`Return:`** *None*
 
       This method enables/disables the buzzer module with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the buzzer module.
+      `module_id` argument is the module ID of the buzzer. It takes values in the range of 1 - 5 (including 1 and 5).
 
-      `en` argument enables or disables the buzzer. (Enable = 1, Disable = 0)
+      `note_frequency` argument specifies the frequency of the tone in Hertz. 0 Hertz will result in no tone.
 
 #### Joystick Module
-  - ####  `get_joystick(self, id: int, index: Index):`
+  - ####  `get_joystick(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the joystick module analogs and button data*
 
       This method gets the joystick module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the joystick module.
+      `module_id` argument is the module ID of the joystick. It takes values in the range of 1 - 5 (including 1 and 5).
 
   #### Example of Joystick Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
@@ -816,119 +816,106 @@
     joystick = m.get_joystick(0, Index.Joystick_1)
     joystick_X = joystick[0]
     joystick_Y = joystick[1]
     joystick_button = joystick[2]
   ```
 
 #### Distance Module
-  - ####  `get_distance(self, id: int, index: Index):`
+  - ####  `get_distance(self, id: int, module_id: int):`
 
     **`Return:`** *Returns the distance from the ultrasonic distance module (in cm)*
 
       This method gets the ultrasonic distance module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the ultrasonic distance module.
+      `module_id` argument is the module ID of the ultrasonic distance module. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### QTR Module
-  - ####  `get_qtr(self, id: int, index: Index):`
+  - ####  `get_qtr(self, id: int, module_id: int):`
 
-    **`Return:`** *Returns qtr module data: [Left(bool), Middle(bool), Right(bool)]*
+    **`Return:`** *Returns QTR module data: [Left(bool), Middle(bool), Right(bool)]*
 
-      This method gets the qtr module data with given index.
+      This method gets the QTR module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the qtr module.
+      `module_id` argument is the module ID of the QTR. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### Servo Module
-  - ####  `set_servo(self, id: int, index: Index, val: int):`
+  - ####  `set_servo(self, id: int, module_id: int, val: int):`
 
     **`Return:`** *None*
 
       This method moves servo module to a desired position.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the servo module.
+      `module_id` argument is the module ID of the servo. It takes values in the range of 1 - 5 (including 1 and 5)
 
-      `val`argument is the value to write to the servo (0, 255).
+      `val` argument is the value to write to the servo. It takes values in the range of 0 - 255 (including 0 and 255).
 
-#### Potantiometer Module
-  - ####  `get_potantiometer(self, id: int, index: Index):`
+#### Potentiometer Module
+  - ####  `get_potentiometer(self, id: int, module_id: int):`
 
-    **`Return:`** *Returns the ADC conversion from the potantiometer module*
+    **`Return:`** *Returns the ADC conversion from the potentiometer module*
 
-      This method gets the potantiometer module data with given index.
+      This method gets the potentiometer module data with given index.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the potantiometer module.
+      `module_id` argument is the module ID of the potentiometer. It takes values in the range of 1 - 5 (including 1 and 5).
 
 #### RGB Led Module
 The setRGB() method is used to control an RGB Led module by specifying the intensity or color values for each of the RGB components.
 
-  - ####  `set_rgb(self, id: int, index: Index, color: Colors):`
+  - ####  `set_rgb(self, id: int, module_id: int, red: int, green: int, blue: int):`
 
     **`Return:`** *None*
 
       This method sets the colour emitted from the RGB module.
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the RGB module.
+      `module_id` argument is the module ID of the RGB. It takes values in the range of 1 - 5 (including 1 and 5).
 
-      `color` argument is the color for RGB from Colors class.
+      `red` argument is representing red color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
+      `green` argument is representing green color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
-  Colors available in RGB sensor module :
-  - NO_COLOR,
-  - RED,
-  - GREEN,
-  - BLUE,
-  - WHITE,
-  - YELLOW,
-  - CYAN,
-  - MAGENTA,
-  - ORANGE,
-  - PURPLE,
-  - PINK,
-  - AMBER,
-  - TEAL,
-  - INDIGO
+      `blue` argument is representing blue color's level. It takes values in the range of 0 - 255 (including 0 and 255).
 
   The method and colors can be used as in the example below for the RGB module.
   #### Example of RGB Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
   m.scan_modules(0)
 
-  m.set_rgb(0, Index.RGB_1, Colors.RED)
+  m.set_rgb(0, Index.RGB_1, 255, 0, 0) # Red color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.GREEN)
+  m.set_rgb(0, Index.RGB_1, 0, 255, 0) # Green color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.BLUE)
+  m.set_rgb(0, Index.RGB_1, 0, 0, 255) # Blue color
   time.sleep(0.5)
-  m.set_rgb(0, Index.RGB_1, Colors.PURPLE)
+  m.set_rgb(0, Index.RGB_1, 128, 0, 128) # Purple color
   time.sleep(0.5)
   ```
 #### IMU Module
-  - ####  `get_imu(self, id: int, index: Index):`
+  - ####  `get_imu(self, id: int, module_id: int):`
 
     **`Return:`** *Returns roll, pitch angles*
 
       This method gets the IMU module data (roll, pitch).
 
       `id` argument is the device ID of the driver.
 
-      `index` argument is the protocol index of the IMU module.
+      `module_id` argument is the module ID of the IMU. It takes values in the range of 1 - 5 (including 1 and 5).
 
   #### Example of IMU Module Usage
   ``` python
   from smd.red import*
   import time
   m = Master("/dev/ttyUSB0")
   m.attach(Red(0))
```

### Comparing `acrome-smd-1.1.4/setup.py` & `acrome_smd-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="acrome-smd",
-    version="1.1.4",
+    version="2.0.0",
     author="Furkan Kırlangıç",
     author_email="furkankirlangic@acrome.net",
     description="Python library for interfacing with Acrome Smart Motor Drivers (SMD) products.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Acrome-Smart-Motor-Driver/python-library",
     project_urls={
```

### Comparing `acrome-smd-1.1.4/smd/_internals.py` & `acrome_smd-2.0.0/smd/_internals.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,178 @@
-import struct
-import enum
-
-
-class Commands(enum.IntEnum):
-    PING = 0x00
-    WRITE = 0x01
-    WRITE_ACK = 0x80 | 0x01
-    READ = 0x02,
-    EEPROM_WRITE = 0x03
-    MODULE_SCAN = 0x04
-    REBOOT = 0x05
-    RESET_ENC = 0x06
-    TUNE = 0x07
-    HARD_RESET = 0x17
-    ERROR_CLEAR = 0x18
-    BL_JUMP = 0x30
-    SYNC_WRITE = 0x40 | 0x01
-    BULK_WRITE = 0x20 | 0x01
-    BULK_READ = 0x20 | 0x02
-    ACK = 0x80
-    __EEPROM_WRITE_ACK = -1
-
-
-class OperationMode():
-    PWM = 0
-    Position = 1
-    Velocity = 2
-    Torque = 3
-
-
-Index = enum.IntEnum('Index', [
-    'Header',
-    'DeviceID',
-    'DeviceFamily',
-    'PackageSize',
-    'Command',
-    'Status',
-    'HardwareVersion',
-    'SoftwareVersion',
-    'Baudrate',
-    'OperationMode',
-    'TorqueEnable',
-    'OutputShaftCPR',
-    'OutputShaftRPM',
-    'UserIndicator',
-    'MinimumPositionLimit',
-    'MaximumPositionLimit',
-    'TorqueLimit',
-    'VelocityLimit',
-    'PositionFF',
-    'VelocityFF',
-    'TorqueFF',
-    'PositionDeadband',
-    'VelocityDeadband',
-    'TorqueDeadband',
-    'PositionOutputLimit',
-    'VelocityOutputLimit',
-    'TorqueOutputLimit',
-    'PositionScalerGain',
-    'PositionPGain',
-    'PositionIGain',
-    'PositionDGain',
-    'VelocityScalerGain',
-    'VelocityPGain',
-    'VelocityIGain',
-    'VelocityDGain',
-    'TorqueScalerGain',
-    'TorquePGain',
-    'TorqueIGain',
-    'TorqueDGain',
-    'SetPosition',
-    'SetVelocity',
-    'SetTorque',
-    'SetDutyCycle',
-    'Buzzer_1',
-    'Buzzer_2',
-    'Buzzer_3',
-    'Buzzer_4',
-    'Buzzer_5',
-    'Servo_1',                      
-    'Servo_2',
-    'Servo_3',
-    'Servo_4',
-    'Servo_5',
-    'RGB_1',                        
-    'RGB_2',
-    'RGB_3',
-    'RGB_4',
-    'RGB_5',
-    'PresentPosition',              
-    'PresentVelocity',
-    'MotorCurrent',
-    'AnalogPort',
-    'Button_1',                     
-    'Button_2',
-    'Button_3',
-    'Button_4',
-    'Button_5',
-    'Light_1',                      
-    'Light_2',
-    'Light_3',
-    'Light_4',
-    'Light_5',
-    'Joystick_1',
-    'Joystick_2',
-    'Joystick_3',
-    'Joystick_4',
-    'Joystick_5',                   
-    'Distance_1',                   
-    'Distance_2',
-    'Distance_3',
-    'Distance_4',
-    'Distance_5',
-    'QTR_1',                        
-    'QTR_2',
-    'QTR_3',
-    'QTR_4',
-    'QTR_5',
-    'Pot_1',                        
-    'Pot_2',
-    'Pot_3',
-    'Pot_4',
-    'Pot_5',
-    'IMU_1',                        
-    'IMU_2',
-    'IMU_3',
-    'IMU_4',
-    'IMU_5',
-    'CRCValue',
-    ], start=0)
-
-
-class _Data():
-    def __init__(self, index, var_type, rw=True, value=0):
-        self.__index = index
-        self.__type = var_type
-        self.__size = struct.calcsize(self.__type)
-        self.__value = value
-        self.__rw = rw
-
-    def value(self, value=None):
-        if value is None:
-            return self.__value
-        elif self.__rw:
-            if len(self.__type) > 1:
-                self.__value = list(struct.unpack('<' + self.__type, struct.pack('<' + self.__type, *value)))
-            else:
-                self.__value = struct.unpack('<' + self.__type, struct.pack('<' + self.__type, value))[0]
-
-    def index(self) -> enum.IntEnum:
-        return self.__index
-
-    def size(self) -> int:
-        return self.__size
-
-    def type(self) -> str:
-        return self.__type
+import struct
+import enum
+
+class Commands(enum.IntEnum):
+    PING = 0x00
+    WRITE = 0x01
+    WRITE_ACK = 0x80 | 0x01
+    READ = 0x02,
+    EEPROM_WRITE = 0x03
+    MODULE_SCAN = 0x04
+    REBOOT = 0x05
+    RESET_ENC = 0x06
+    TUNE = 0x07
+    HARD_RESET = 0x17
+    ERROR_CLEAR = 0x18
+    BL_JUMP = 0x30
+    SYNC_WRITE = 0x40 | 0x01
+    BULK_WRITE = 0x20 | 0x01
+    BULK_READ = 0x20 | 0x02
+    ACK = 0x80
+    __EEPROM_WRITE_ACK = -1
+
+
+class OperationMode():
+    PWM = 0
+    Position = 1
+    Velocity = 2
+    Torque = 3
+
+
+class MotorConstants():
+    MAX_ACCEL = 999999.9999
+
+
+Index = enum.IntEnum('Index', [
+    'Header',
+    'DeviceID',
+    'DeviceFamily',
+    'PackageSize',
+    'Command',
+    'Status',
+    'HardwareVersion',
+    'SoftwareVersion',
+    'Baudrate',
+    'OperationMode',
+    'TorqueEnable',
+    'OutputShaftCPR',
+    'OutputShaftRPM',
+    'UserIndicator',
+    'MinimumPositionLimit',
+    'MaximumPositionLimit',
+    'TorqueLimit',
+    'VelocityLimit',
+    'PositionFF',
+    'VelocityFF',
+    'TorqueFF',
+    'PositionDeadband',
+    'VelocityDeadband',
+    'TorqueDeadband',
+    'PositionOutputLimit',
+    'VelocityOutputLimit',
+    'TorqueOutputLimit',
+    'PositionScalerGain',
+    'PositionPGain',
+    'PositionIGain',
+    'PositionDGain',
+    'VelocityScalerGain',
+    'VelocityPGain',
+    'VelocityIGain',
+    'VelocityDGain',
+    'TorqueScalerGain',
+    'TorquePGain',
+    'TorqueIGain',
+    'TorqueDGain',
+    'SetPosition',
+    'PositionControlMode',
+	'SCurveSetpoint',
+	'ScurveAccel',
+	'SCurveMaxVelocity',
+	'SCurveTime',
+    'SetVelocity',
+    'SetVelocityAcceleration',
+    'SetTorque',
+    'SetDutyCycle',
+    'SetScanModuleMode',
+    'SetManualBuzzer',
+    'SetManualServo',
+    'SetManualRGB',
+    'SetManualButton',
+    'SetManualLight',
+    'SetManualJoystick',
+    'SetManualDistance',
+    'SetManualQTR',
+    'SetManualPot',
+    'SetManualIMU',
+    'Buzzer_1',
+    'Buzzer_2',
+    'Buzzer_3',
+    'Buzzer_4',
+    'Buzzer_5',
+    'Servo_1',                      
+    'Servo_2',
+    'Servo_3',
+    'Servo_4',
+    'Servo_5',
+    'RGB_1',                        
+    'RGB_2',
+    'RGB_3',
+    'RGB_4',
+    'RGB_5',
+    'PresentPosition',              
+    'PresentVelocity',
+    'MotorCurrent',
+    'AnalogPort',
+    'Button_1',                     
+    'Button_2',
+    'Button_3',
+    'Button_4',
+    'Button_5',
+    'Light_1',                      
+    'Light_2',
+    'Light_3',
+    'Light_4',
+    'Light_5',
+    'Joystick_1',
+    'Joystick_2',
+    'Joystick_3',
+    'Joystick_4',
+    'Joystick_5',                   
+    'Distance_1',                   
+    'Distance_2',
+    'Distance_3',
+    'Distance_4',
+    'Distance_5',
+    'QTR_1',                        
+    'QTR_2',
+    'QTR_3',
+    'QTR_4',
+    'QTR_5',
+    'Pot_1',                        
+    'Pot_2',
+    'Pot_3',
+    'Pot_4',
+    'Pot_5',
+    'IMU_1',                        
+    'IMU_2',
+    'IMU_3',
+    'IMU_4',
+    'IMU_5',
+    'CRCValue',
+    ], start=0)
+
+
+class _Data():
+    def __init__(self, index, var_type, rw=True, value=0):
+        self.__index = index
+        self.__type = var_type
+        self.__size = struct.calcsize(self.__type)
+        self.__value = value
+        self.__rw = rw
+
+    def value(self, value=None):
+        if value is None:
+            return self.__value
+        elif self.__rw:
+            if len(self.__type) > 1:
+                self.__value = list(struct.unpack('<' + self.__type, struct.pack('<' + self.__type, *value)))
+            else:
+                self.__value = struct.unpack('<' + self.__type, struct.pack('<' + self.__type, value))[0]
+
+    def index(self) -> enum.IntEnum:
+        return self.__index
+
+    def size(self) -> int:
+        return self.__size
+
+    def type(self) -> str:
+        return self.__type
```

### Comparing `acrome-smd-1.1.4/smd/red.py` & `acrome_smd-2.0.0/smd/red.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from smd._internals import (_Data, Index, Commands,
-                            OperationMode)
+                            OperationMode, MotorConstants)
 import struct
 from crccheck.crc import Crc32Mpeg2 as CRC32
 import serial
 import time
 from packaging.version import parse as parse_version
 import requests
 import hashlib
@@ -71,17 +71,34 @@
             _Data(Index.VelocityIGain, 'f'),
             _Data(Index.VelocityDGain, 'f'),
             _Data(Index.TorqueScalerGain, 'f'),
             _Data(Index.TorquePGain, 'f'),
             _Data(Index.TorqueIGain, 'f'),
             _Data(Index.TorqueDGain, 'f'),
             _Data(Index.SetPosition, 'f'),
+            _Data(Index.PositionControlMode, 'B'),      # S Curve Position Control / 1 is SCurve(goTo function) 0 is direct control.
+            _Data(Index.SCurveSetpoint, 'f'),
+            _Data(Index.ScurveAccel, 'f'),
+            _Data(Index.SCurveMaxVelocity, 'f'),
+            _Data(Index.SCurveTime, 'f'),
             _Data(Index.SetVelocity, 'f'),
+            _Data(Index.SetVelocityAcceleration, 'f'),
             _Data(Index.SetTorque, 'f'),
             _Data(Index.SetDutyCycle, 'f'),
+            _Data(Index.SetScanModuleMode, 'B'),        # Modules
+            _Data(Index.SetManualBuzzer, 'B'),
+            _Data(Index.SetManualServo, 'B'),
+            _Data(Index.SetManualRGB, 'B'),
+            _Data(Index.SetManualButton, 'B'),
+            _Data(Index.SetManualLight, 'B'),
+            _Data(Index.SetManualJoystick, 'B'),
+            _Data(Index.SetManualDistance, 'B'),
+            _Data(Index.SetManualQTR, 'B'),
+            _Data(Index.SetManualPot, 'B'),
+            _Data(Index.SetManualIMU, 'B'),
             _Data(Index.Buzzer_1, 'i'),
             _Data(Index.Buzzer_2, 'i'),
             _Data(Index.Buzzer_3, 'i'),
             _Data(Index.Buzzer_4, 'i'),
             _Data(Index.Buzzer_5, 'i'),
             _Data(Index.Servo_1, 'B'),
             _Data(Index.Servo_2, 'B'),
@@ -156,14 +173,15 @@
         struct_out = list(struct.pack(fmt_str, *[*[var.value() for var in self.vars[:6]], *[val for pair in zip(index_list, [self.vars[int(index)].value() for index in index_list]) for val in pair]]))
 
         struct_out[int(Index.PackageSize)] = len(struct_out) + self.vars[int(Index.CRCValue)].size()
 
         self.vars[Index.CRCValue].value(CRC32.calc(struct_out))
 
         return bytes(struct_out) + struct.pack('<' + self.vars[Index.CRCValue].type(), self.vars[Index.CRCValue].value())
+    
 
     def get_variables(self, index_list=[]):
         self.vars[Index.Command].value(Commands.READ)
 
         fmt_str = '<' + ''.join([var.type() for var in self.vars[:6]])
         fmt_str += 'B' * len(index_list)
 
@@ -720,14 +738,113 @@
                 addrs = [i for i in range(64) if (data & (1 << i)) == (1 << i)]
                 result = []
                 for addr in addrs:
                     result.append((Index(addr - _ID_OFFSETS[int((addr - 1) / 5)][0] + _ID_OFFSETS[int((addr - 1) / 5)][1])).name)
                 return result
         else:
             return None
+        
+    def set_connected_modules(self, id: int, modules: list):
+        """ Set the list of sensor IDs which are connected to the driver.
+
+        Args:
+            id (int): The device ID of the driver.
+            modules (list): List of the protocol IDs of the connected sensors.
+        """
+
+
+        #remove elements that has multiple ones in modules list
+        filtered_modules = list(set(modules))
+        print(filtered_modules)
+
+        ManualBuzzer_Byte = 0
+        ManualServo_Byte = 0
+        ManualRGB_Byte = 0
+        ManualButton_Byte = 0
+        ManualLight_Byte = 0
+        ManualJoystick_Byte = 0
+        ManualDistance_Byte = 0
+        ManualQTR_Byte = 0
+        ManualPot_Byte = 0
+        ManualIMU_Byte = 0
+        try:
+            for module in filtered_modules:
+                if "Buzzer" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'Buzzer_2' ".format(module))
+                    ManualBuzzer_Byte += 2**(module_id - 1)
+                elif "Servo" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'Servo_2' ".format(module))
+                    ManualServo_Byte += 2**(module_id - 1)
+                elif "RGB" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'RGB_2' ".format(module))
+                    ManualRGB_Byte += 2**(module_id - 1)
+                elif "Button" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'Button_2' ".format(module))
+                    ManualButton_Byte += 2**(module_id - 1)
+                elif "Light" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'Light_2' ".format(module))
+                    ManualLight_Byte += 2**(module_id - 1)
+                elif "Joystick" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'Joystick_2' ".format(module))
+                    ManualJoystick_Byte += 2**(module_id - 1)
+                elif "Distance" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'Distance_2' ".format(module))
+                    ManualDistance_Byte += 2**(module_id - 1)
+                elif "QTR" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'QTR_2' ".format(module))
+                    ManualQTR_Byte += 2**(module_id - 1)
+                elif "Pot" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'Pot_2' ".format(module))
+                    ManualPot_Byte += 2**(module_id - 1)
+                elif "IMU" in module:
+                    module_id = int(module[-1])
+                    if module_id <= 0 or module_id > 5:
+                        raise ValueError("{} invalid module ID! it should be between 1 and 5. for ex: 'IMU_2' ".format(module))
+                    ManualIMU_Byte += 2**(module_id - 1)           
+                else:
+                    raise ValueError("{} is not a Module with ID! for ex: 'Button_2' ".format(module))
+        except Exception as e:
+            raise e
+        
+        self.set_variables(id, [[Index.SetScanModuleMode, 1]])
+
+        self.set_variables(id, [[Index.SetManualBuzzer, ManualBuzzer_Byte]])
+        self.set_variables(id, [[Index.SetManualServo, ManualServo_Byte]])
+        self.set_variables(id, [[Index.SetManualRGB, ManualRGB_Byte]])
+        self.set_variables(id, [[Index.SetManualButton, ManualButton_Byte]])
+        self.set_variables(id, [[Index.SetManualLight, ManualLight_Byte]])
+        self.set_variables(id, [[Index.SetManualJoystick, ManualJoystick_Byte]])
+        self.set_variables(id, [[Index.SetManualDistance, ManualDistance_Byte]])
+        self.set_variables(id, [[Index.SetManualQTR, ManualQTR_Byte]])
+        self.set_variables(id, [[Index.SetManualPot, ManualPot_Byte]])
+        self.set_variables(id, [[Index.SetManualIMU, ManualIMU_Byte]])
+    
+        self.__write_bus(self.__driver_list[id].scan_modules())
+        time.sleep(self.__post_sleep)
+
+
+
 
     def enter_bootloader(self, id: int):
         """ Put the driver into bootloader mode.
 
         Args:
             id (int): The device ID of the driver.
         """
@@ -946,36 +1063,123 @@
     def set_position(self, id: int, sp: int):
         """ Set the desired setpoint for the position control in terms of encoder ticks.
 
         Args:
             id (int): The device ID of the driver.
             sp (int | float): Position control setpoint.
         """
-        self.set_variables(id, [[Index.SetPosition, sp]])
+        self.set_variables(id, [[Index.PositionControlMode, 0],[Index.SetPosition, sp]])
         time.sleep(self.__post_sleep)
 
     def get_position(self, id: int):
         """ Get the current position of the motor from the driver in terms of encoder ticks.
 
         Args:
             id (int): The device ID of the driver.
 
         Returns:
             list | None: Returns the list containing the current position, otherwise None.
         """
         return self.get_variables(id, [Index.PresentPosition])[0]
+    
+    def goTo(self, id: int, target_position, time_ = 0, maxSpeed = 0, accel = 0, 
+             blocking: bool = False, encoder_tick_close_counter = 10):
+        """
+            # goTo: 
+
+            Sets the target position in S Curve mode. Since this function controls motor in position, 
+            device should be in Position Mode to use this func.
+
+            If you just want to drive the motor to target point smoothly, you can use just the target_position parameter only.
+            If other parameters are not given or they are 0 (time, maxSpeed, accel), it will use default speed and acceleration values based on the motor's RPM.
+            
+            If the setpoint, time, maxSpeed, and accel parameters are specified in a way that makes it impossible to reach the target in the given time, 
+            the time variable will be ignored.
 
-    def set_velocity(self, id: int, sp: float):
+            If only the time is not provided, the movement will be executed according to the other given parameters.
+
+            It is not necessary for the speed to reach the maxSpeed value during the movement. 
+            The maxSpeed parameter is only a limitation. Due to the other given parameters, it might be impossible to reach the maxSpeed value during the movement. 
+            Note: The motor's RPM value is defined as maxSpeed within the SMD.
+
+            If blocking is True, the function will wait until the motor reaches the target position.
+            If blocking is False, the function will return immediately.
+
+            Args:
+                id (int): The device ID of the driver.
+                target_position (int | float): Position control setpoint.
+                time (int | float): Time in seconds.
+                maxSpeed (int | float): Maximum speed in RPM.
+                accel (int | float): Acceleration in RPM/s.
+                blocking (bool): If True, the function will wait until the motor reaches the target position.
+                encoder_tick_close_counter (int): The number of encoder ticks that the motor should close enough to the target position to be considered reached.
+        """
+
+        self.set_variables(id, [[Index.PositionControlMode, 1]])
+        self.set_variables(id, [[Index.SCurveTime, time_],[Index.SCurveMaxVelocity, maxSpeed],[Index.ScurveAccel, accel]])
+        self.set_variables(id, [[Index.SCurveSetpoint, target_position]])
+
+        time.sleep(self.__post_sleep)
+
+        while(blocking):
+            if (abs(target_position - self.get_position(id)) <= encoder_tick_close_counter):
+                break
+        
+    def goTo_ConstantSpeed(self, id: int, target_position, speed,
+                           blocking: bool = False, encoder_tick_close_counter = 10):
+        """
+            # goTo_ConstantSpeed: 
+
+            Sets the target position and sets the accel to max accel in S Curve mode. So velocity reaches given speed immediately.
+
+            If blocking is True, the function will wait until the motor reaches the target position.
+            If blocking is False, the function will return immediately.
+
+            Args:
+                id (int): The device ID of the driver.
+                target_position (int | float): Position control setpoint.
+                speed (int | float): Maximum speed in RPM.
+                blocking (bool): If True, the function will wait until the motor reaches the target position.
+                encoder_tick_close_counter (int): The number of encoder ticks that the motor should close enough to the target position to be considered reached.
+        """
+        
+        self.set_variables(id, [[Index.VelocityControlMode, 1]])
+        self.set_variables(id, [[Index.SCurveMaxVelocity, speed],[Index.ScurveAccel, MotorConstants.MAX_ACCEL]])
+        self.set_variables(id, [[Index.SCurveSetpoint, target_position]])
+
+        time.sleep(self.__post_sleep)
+
+        while(blocking):
+            if (abs(target_position - self.get_position(id)) <= encoder_tick_close_counter):
+                break
+
+    def set_velocity(self, id: int, sp: float, accel = 0):
         """ Set the desired setpoint for the velocity control in terms of RPM.
 
         Args:
             id (int): The device ID of the driver.
             sp (int | float): Velocity control setpoint.
-        """
-        self.set_variables(id, [[Index.SetVelocity, sp]])
+            accel(float): sets the acceleration value for the velocity control in terms of (RPM/seconds). if accel is not given, it will be ignored. 
+            So previously set accel value will be used.
+            In initial SMD-RED Velocity Control Mode, accel will be set to MAX_ACCEL.
+
+        Hint: 
+            It can be used to set the acceleration value by "MotorConstants.MAX_ACCEL" to reach the target velocity immediately.
+        """
+        if accel == MotorConstants.MAX_ACCEL:
+            accel = 0
+            self.set_variables(id, [[Index.SetVelocityAcceleration, accel]])
+            self.set_variables(id, [[Index.SetVelocity, sp]])
+
+        elif accel == 0:
+            self.set_variables(id, [[Index.SetVelocity, sp]])
+        else:
+            self.set_variables(id, [[Index.SetVelocityAcceleration, accel]])
+            self.set_variables(id, [[Index.SetVelocity, sp]])
+        
         time.sleep(self.__post_sleep)
 
     def get_velocity(self, id: int):
         """ Get the current velocity of the motor output shaft from the driver in terms of RPM.
 
         Args:
             id (int): The device ID of the driver.
@@ -1120,19 +1324,19 @@
 
         Returns:
             list | None: Returns the list [P, I, D, FF, DB, OUTPUT_LIMIT], otherwise None.
         """
         return self.get_variables(id, [Index.TorquePGain, Index.TorqueIGain, Index.TorqueDGain, Index.TorqueDeadband, Index.TorqueFF, Index.TorqueOutputLimit])
 
     def get_button(self, id: int, module_id: int):
-        """ Get the button module data with given index.
+        """ Get the button module data with given module ID.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the button module.
+            module_id (int): The module ID of the button.
 
         Raises:
             InvalidIndexError: Index is not a button module index
 
         Returns:
             int: Returns the button state
         """
@@ -1142,19 +1346,19 @@
 
         ret = self.get_variables(id, [index])
         if ret is None:
             return ret
         return ret[0]
 
     def get_light(self, id: int, module_id: int):
-        """ Get the ambient light module data with given index.
+        """ Get the ambient light module data with given module ID.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the ambient light module.
+            module_id (int): The module ID of the ambient light.
 
         Raises:
             InvalidIndexError: Index is not a light module index
 
         Returns:
             float: Returns the ambient light measurement (in lux)
         """
@@ -1164,20 +1368,20 @@
 
         ret = self.get_variables(id, [index])
         if ret is None:
             return ret
         return ret[0]
 
     def set_buzzer(self, id: int, module_id: int, note_frequency: int):
-        """ Enable/disable the buzzer module with given index.
+        """ Set the note frequency of the buzzer module with given module ID.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the buzzer module.
-            en (bool): Enable = 1, Disable = 0
+            module_id (int): The module ID of the buzzer.
+            note_frequency (int): The frequency of the tone in Hertz.
 
         Raises:
             InvalidIndexError: Index is not a buzzer module index
         """
         if note_frequency < 0 :
             print("note frequency cannot be negative!")
             raise InvalidIndexError()
@@ -1185,19 +1389,19 @@
         index =  module_id + Index.Buzzer_1 - 1
         if (index < Index.Buzzer_1) or (index > Index.Buzzer_5):
             raise InvalidIndexError()
         self.set_variables(id, [[index, note_frequency]])
         time.sleep(self.__post_sleep)
 
     def get_joystick(self, id: int, module_id: int):
-        """ Get the joystick module data with given index.
+        """ Get the joystick module data with given module ID.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the joystick module.
+            module_id (int): The module ID of the joystick.
 
         Raises:
             InvalidIndexError: Index is not a joystick module index
 
         Returns:
             list: Returns the joystick module analogs and button data
         """
@@ -1207,19 +1411,19 @@
 
         ret = self.get_variables(id, [index])
         if ret is None:
             return ret
         return ret[0]
 
     def get_distance(self, id: int, module_id: int):
-        """ Get the ultrasonic distance module data with given index.
+        """ Get the ultrasonic distance module data with given module ID.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the ultrasonic distance module.
+            module_id (int): The module ID of the ultrasonic distance module.
 
         Raises:
             InvalidIndexError: Index is not a ultrasonic distance module index
 
         Returns:
             int: Returns the distance from the ultrasonic distance module (in cm)
         """
@@ -1229,25 +1433,25 @@
 
         ret = self.get_variables(id, [index])
         if ret is None:
             return ret
         return ret[0]
 
     def get_qtr(self, id: int, module_id: int):
-        """ Get the qtr module data with given index.
+        """ Get the QTR module data with given module ID.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the qtr module.
+            module_id (int): The module ID of the QTR.
 
         Raises:
-            InvalidIndexError: Index is not a qtr module index
+            InvalidIndexError: Index is not a QTR module index
 
         Returns:
-            list: Returns qtr module data: [Left(bool), Middle(bool), Right(bool)]
+            list: Returns QTR module data: [Left(bool), Middle(bool), Right(bool)]
         """
         index =  module_id + Index.QTR_1 - 1
         if (index < Index.QTR_1) or (index > Index.QTR_5):
             raise InvalidIndexError()
 
         data = self.get_variables(id, [index])
         if data is not None:
@@ -1256,41 +1460,41 @@
             return None
 
     def set_servo(self, id: int, module_id: int, val: int):
         """ Move servo module to a position.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the servo module.
+            module_id (int): The module ID of the servo.
             val (int): The value to write to the servo
 
         Raises:
             ValueError: Value should be in range [0, 255]
             InvalidIndexError: Index is not a servo module index
         """
         if val < 0 or val > 255:
             raise ValueError()
         index =  module_id + Index.Servo_1 - 1
         if (index < Index.Servo_1) or (index > Index.Servo_5):
             raise InvalidIndexError()
         self.set_variables(id, [[index, val]])
         time.sleep(self.__post_sleep)
 
-    def get_potantiometer(self, id: int, module_id: int):
-        """ Get the potantiometer module data with given index.
+    def get_potentiometer(self, id: int, module_id: int):
+        """ Get the potentiometer module data with given module ID.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the potantiometer module.
+            module_id (int): The module ID of the potentiometer.
 
         Raises:
-            InvalidIndexError: Index is not a potantiometer module index
+            InvalidIndexError: Index is not a potentiometer module index
 
         Returns:
-            int: Returns the ADC conversion from the potantiometer module
+            int: Returns the ADC conversion from the potentiometer module
         """
         index =  module_id + Index.Pot_1 - 1
         if (index < Index.Pot_1) or (index > Index.Pot_5):
             raise InvalidIndexError()
 
         ret = self.get_variables(id, [index])
         if ret is None:
@@ -1298,16 +1502,18 @@
         return ret[0]
 
     def set_rgb(self, id: int, module_id: int, red: int, green: int, blue: int):
         """ Set the colour emitted from the RGB module.
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the RGB module.
-            color (Colors): Color for RGB from Colors class
+            module_id (int): The module ID of the RGB.
+            red (int): The color level of red. [0,255]
+            green (int): The color level of green. [0,255]
+            blue (int): The color level of blue. [0,255]
         Raises:
             ValueError: Color is invalid
             InvalidIndexError: Index is not a RGB module index
         """
 
 
         if red < 0 or red > 255:
@@ -1326,15 +1532,15 @@
         time.sleep(self.__post_sleep)
 
     def get_imu(self, id: int, module_id: int):
         """ Get IMU module data (roll, pitch)
 
         Args:
             id (int): The device ID of the driver.
-            index (Index): The index of the IMU module.
+            module_id (int): The module ID of the IMU.
 
         Raises:
             InvalidIndexError: Index is not a IMU module index
 
         Returns:
             list: Returns roll, pitch angles
         """
```

### Comparing `acrome-smd-1.1.4/tests/test_red.py` & `acrome_smd-2.0.0/tests/test_red.py`

 * *Files identical despite different names*

