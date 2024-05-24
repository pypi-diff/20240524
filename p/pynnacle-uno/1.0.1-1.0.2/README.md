# Comparing `tmp/pynnacle_uno-1.0.1.tar.gz` & `tmp/pynnacle_uno-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynnacle_uno-1.0.1.tar", last modified: Fri May 17 08:21:34 2024, max compression
+gzip compressed data, was "pynnacle_uno-1.0.2.tar", last modified: Fri May 24 07:33:10 2024, max compression
```

## Comparing `pynnacle_uno-1.0.1.tar` & `pynnacle_uno-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 08:21:34.014593 pynnacle_uno-1.0.1/
--rw-rw-rw-   0        0        0    35549 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     3086 2024-05-17 08:21:34.013594 pynnacle_uno-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2017 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 08:21:33.995589 pynnacle_uno-1.0.1/pynnacle_uno/
--rw-rw-rw-   0        0        0      862 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.1/pynnacle_uno/__init__.py
--rw-rw-rw-   0        0        0    14014 2024-05-17 08:19:23.000000 pynnacle_uno-1.0.1/pynnacle_uno/main.py
-drwxrwxrwx   0        0        0        0 2024-05-17 08:21:34.010595 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/
--rw-rw-rw-   0        0        0     3086 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-17 08:21:33.000000 pynnacle_uno-1.0.1/pynnacle_uno.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 08:21:34.014593 pynnacle_uno-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1294 2024-05-17 08:20:51.000000 pynnacle_uno-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:33:10.635100 pynnacle_uno-1.0.2/
+-rw-rw-rw-   0        0        0    35549 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3086 2024-05-24 07:33:10.633099 pynnacle_uno-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2017 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 07:33:10.613095 pynnacle_uno-1.0.2/pynnacle_uno/
+-rw-rw-rw-   0        0        0      862 2024-05-11 13:51:43.000000 pynnacle_uno-1.0.2/pynnacle_uno/__init__.py
+-rw-rw-rw-   0        0        0    14086 2024-05-24 07:30:19.000000 pynnacle_uno-1.0.2/pynnacle_uno/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:33:10.630099 pynnacle_uno-1.0.2/pynnacle_uno.egg-info/
+-rw-rw-rw-   0        0        0     3086 2024-05-24 07:33:10.000000 pynnacle_uno-1.0.2/pynnacle_uno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-24 07:33:10.000000 pynnacle_uno-1.0.2/pynnacle_uno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:33:10.000000 pynnacle_uno-1.0.2/pynnacle_uno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 07:33:10.000000 pynnacle_uno-1.0.2/pynnacle_uno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-24 07:33:10.000000 pynnacle_uno-1.0.2/pynnacle_uno.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:33:10.635100 pynnacle_uno-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2024-05-24 07:32:28.000000 pynnacle_uno-1.0.2/setup.py
```

### Comparing `pynnacle_uno-1.0.1/LICENSE` & `pynnacle_uno-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynnacle_uno-1.0.1/PKG-INFO` & `pynnacle_uno-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynnacle_uno
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module that provides hands-on robotics coding experience in Python that closely mirrors the structure and functionality of Arduino's programming language.
 Home-page: https://github.com/Red-Pula/Pynnacle-Uno
 Author: Rafael Red Angelo M. Hizon, Jenel M. Justo, Serena Mae C.S. Lee
 Author-email: redhizon@gmail.com, jenel.just88@gmail.com, nmae.lee@gmail.com
 License: GNU Affero General Public License
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pynnacle_uno-1.0.1/README.md` & `pynnacle_uno-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pynnacle_uno-1.0.1/pynnacle_uno/__init__.py` & `pynnacle_uno-1.0.2/pynnacle_uno/__init__.py`

 * *Files identical despite different names*

### Comparing `pynnacle_uno-1.0.1/pynnacle_uno/main.py` & `pynnacle_uno-1.0.2/pynnacle_uno/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,25 +40,28 @@
 # Import statements
 from pymata4 import pymata4
 from time import sleep
 import re
 
 # CONSTANTS
 
+# Delay in ms before performing a write operation
+DELAY_WRITE = 10
+
 # States
 HIGH = 1
 LOW = 0
 
 # Modes
 OUTPUT = 'O'
 INPUT = 'I'
 INPUT_PULLUP = 'IP'
 
 # Maximum number of digital pins on the Arduino UNO
-DIGITAL_PINS_COUNT = 14
+_DIGITAL_PINS_COUNT = 14
 
 # Analog Pins on Arduino UNO. Add more if you want to 
 A0 = 'A0'
 A1 = 'A1'
 A2 = 'A2'
 A3 = 'A3'
 A4 = 'A4'
@@ -201,14 +204,21 @@
     _board = pymata4.Pymata4()
     _Style.info()
 except:
     _Style.info()
     _Style.print_error_message()
 
 
+# This function accepts a pin as a parameter.
+# This function converts the analog pin to its digital pin equivalent.
+# It returns the calculated digital pin equivalent.
+def _analogToDigital(pin):
+    integer_only = int(pin[1:])
+    pin = _DIGITAL_PINS_COUNT + integer_only
+    return pin
 
 
 # In Arduino's pinMode function, there are only 3 modes:
 #   1. INPUT
 #   2. OUTPUT
 #   3. INPUT_PULLUP
 # See more at: https://www.arduino.cc/reference/en/language/functions/digital-io/pinmode/
@@ -231,15 +241,15 @@
     # 2. <https://mryslab.github.io/pymata4/pin_modes/#set_pin_mode_analog_input>
     elif pin.startswith('A'):
         integer_only = int(pin[1:])
         if mode == INPUT:
             _board.set_pin_mode_analog_input(integer_only)
 
         else:
-            digital_pin_equivalent = DIGITAL_PINS_COUNT + integer_only
+            digital_pin_equivalent = _analogToDigital(pin)
             if mode == OUTPUT:
                 _board.set_pin_mode_digital_output(digital_pin_equivalent)
 
             elif mode == INPUT_PULLUP:
                 _board.set_pin_mode_digital_input_pullup(digital_pin_equivalent)
 
             else:
@@ -251,72 +261,61 @@
 # This simulates the Arduino's delay function.
 # In Arduino, the said function takes a delay time in milliseconds.
 # It is implemented here using the sleep method.
 def delay(ms):
     sleep(ms / 1000)  # The sleep method takes a delay time in seconds so we divide by 1000.
 
 
-# This function accepts a pin as a parameter.
-# This function converts the analog pin to its digital pin equivalent.
-# It returns the calculated digital pin equivalent.
-def analogToDigital(pin):
-    integer_only = int(pin[1:])
-    pin = DIGITAL_PINS_COUNT + integer_only
-    return pin
-
-
 # This function sets (writes) a digital pin's state into HIGH or LOW.
 # This function takes in 2 parameters:
 #   1. pin
 #   2. state (HIGH or LOW)
 def digitalWrite(pin, state):
+    delay(DELAY_WRITE)
     if isinstance(pin, str) and pin.startswith('A'):
-        pin = analogToDigital(pin)  # convert analog pin to digital pin equivalent
+        pin = _analogToDigital(pin)  # convert analog pin to digital pin equivalent
     _board.digital_write(pin, state)
 
 
 # This function allows users to write PWM wave (analog value) to a pin.
 # This function takes in 2 parameters:
 #   1. pin
 #   2. val (ranges from 0-255)
 # In Arduino, the analogWrite function does not require the programmer to
 # invoke pinMode in order to set the pin as OUTPUT. We simulate this effect
 # using the set_pin_mode_pwm_output method before calling pwm_write.
 # See more at: <https://www.arduino.cc/reference/en/language/functions/analog-io/analogwrite/>
 def analogWrite(pin, val):
+    delay(DELAY_WRITE)
     if isinstance(pin, str) and pin.startswith('A'):
-        pin = analogToDigital(pin)  # convert analog pin to digital pin equivalent
+        pin = _analogToDigital(pin)  # convert analog pin to digital pin equivalent
     _board.set_pin_mode_pwm_output(pin)  # set the pin's mode as a pwm output pin
     _board.pwm_write(pin, val)  # write an output value
 
 
 # This function accepts a pin as a parameter.
 # This function allows to read a digital pin's state whether HIGH or LOW.
-# It returns a list with two values:
-#   1. last value change
-#   2. time_stamp
+# This returns the last digital value change.
 # See more at: <https://mryslab.github.io/pymata4/pin_changes/#digital_read>
 def digitalRead(pin):
     if isinstance(pin, str) and pin.startswith('A'):
-        pin = analogToDigital(pin)  # convert analog pin to digital pin equivalent
+        pin = _analogToDigital(pin)  # convert analog pin to digital pin equivalent
         _board.set_pin_mode_digital_input(pin)  # set the pin's mode as a digital input pin
-    val = _board.digital_read(pin)  # read the digital value
+    val = _board.digital_read(pin)[0]  # store the digital reading
     return val
 
 
 # This function accepts a pin as a parameter.
 # This function allows to read the value from an analog pin.
-# It returns a list with two values:
-#   1. last value change
-#   2. time_stamp
+# This returns the last analog value change.
 # See more at: <https://mryslab.github.io/pymata4/pin_changes/#analog_read>
 def analogRead(pin):
     if isinstance(pin, str) and pin.startswith('A'):
         pin = int(pin[1:])
-    val = _board.analog_read(pin)  # read the analog value
+    val = _board.analog_read(pin)[0]  # store the analog reading
     return val
 
 
 # That pin will then be set for ultrasonic operations.
 # This accepts 2 parameters:
 #   1. trigger_pin
 #   2. echo_pin
@@ -325,22 +324,20 @@
 # It is added here for educational purposes in line with the authors' book.
 def ultrasonicAttach(trigger_pin, echo_pin):
     _board.set_pin_mode_sonar(trigger_pin, echo_pin)
 
 
 # This function accepts a trigger_pin as a parameter.
 # This function retrieves ping data from the ultrasonic (HC-SR04 type).
-# This returns a list with 2 values:
-#   1. last value
-#   2. raw time_stamp
+# This returns the last read value.
 # See more at: <https://mryslab.github.io/pymata4/pin_changes/#sonar_read>
 # This function is not part of the original programming language of Arduino.
 # It is added here for educational purposes in line with the authors' book.
 def ultrasonicRead(trigger_pin):
-    val = _board.sonar_read(trigger_pin)
+    val = _board.sonar_read(trigger_pin)[0] # store the ultrasonic sensor's reading
     return val
 
 
 # That pin will then be set for servo operations.
 # This accepts 3 parameters:
 #   1. pin of the servo
 #   2. min pulse width in ms. (if no value was passed, value is 544)
@@ -356,14 +353,15 @@
 # This accepts 2 parameters:
 #   1. pin of the buzzer
 #   2. frequency
 # See more at:
 #   1. <https://www.arduino.cc/reference/en/libraries/servo/write/>
 #   2. <https://mryslab.github.io/pymata4/device_writes/#servo_write>
 def servoWrite(pin, position):
+    delay(DELAY_WRITE)
     _board.servo_write(pin, position)
 
 
 # This function accepts a pin as a parameter.
 # That pin will then be set for tone operations.
 # See more at: <https://mryslab.github.io/pymata4/pin_modes/#set_pin_mode_tone>
 # This function is not part of the original programming language of Arduino.
```

### Comparing `pynnacle_uno-1.0.1/pynnacle_uno.egg-info/PKG-INFO` & `pynnacle_uno-1.0.2/pynnacle_uno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynnacle_uno
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python module that provides hands-on robotics coding experience in Python that closely mirrors the structure and functionality of Arduino's programming language.
 Home-page: https://github.com/Red-Pula/Pynnacle-Uno
 Author: Rafael Red Angelo M. Hizon, Jenel M. Justo, Serena Mae C.S. Lee
 Author-email: redhizon@gmail.com, jenel.just88@gmail.com, nmae.lee@gmail.com
 License: GNU Affero General Public License
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pynnacle_uno-1.0.1/setup.py` & `pynnacle_uno-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='pynnacle_uno',
-    version='1.0.1', 
+    version='1.0.2', 
     packages=find_packages(),
     description='A Python module that provides hands-on robotics coding experience in Python that closely mirrors the structure and functionality of Arduino\'s programming language.',
     url='https://github.com/Red-Pula/Pynnacle-Uno',
     author='Rafael Red Angelo M. Hizon, Jenel M. Justo, Serena Mae C.S. Lee',
     author_email='redhizon@gmail.com, jenel.just88@gmail.com, nmae.lee@gmail.com',
     license='GNU Affero General Public License',
     install_requires=['pymata4>=1.15'],
```

