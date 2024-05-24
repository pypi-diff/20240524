# Comparing `tmp/wmul_logger-0.5.1.tar.gz` & `tmp/wmul_logger-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmul_logger-0.5.1.tar", last modified: Fri Jan 20 18:06:29 2023, max compression
+gzip compressed data, was "wmul_logger-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wmul_logger-0.5.1.tar` & `wmul_logger-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      106 2023-01-20 18:02:02.962132 wmul_logger-0.5.1/.gitignore
--rw-r--r--   0        0        0       91 2023-01-20 18:00:16.745193 wmul_logger-0.5.1/CHANGELOG.txt
--rw-r--r--   0        0        0    18431 2023-01-20 17:28:47.872017 wmul_logger-0.5.1/LICENSE
--rw-r--r--   0        0        0       18 2023-01-20 17:28:47.873018 wmul_logger-0.5.1/README.txt
--rw-r--r--   0        0        0      888 2023-01-20 17:57:40.118351 wmul_logger-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1299 2023-01-20 17:28:47.873018 wmul_logger-0.5.1/setup.py
--rw-r--r--   0        0        0      987 2023-01-20 18:00:39.763045 wmul_logger-0.5.1/src/wmul_logger/__init__.py
--rw-r--r--   0        0        0     4277 2023-01-20 18:00:47.184278 wmul_logger-0.5.1/src/wmul_logger/logger.py
--rw-r--r--   0        0        0     9352 2023-01-20 18:00:55.728864 wmul_logger-0.5.1/tests/test_logger.py
--rw-r--r--   0        0        0     2119 2023-01-20 18:01:31.476370 wmul_logger-0.5.1/tests/test_multiprocess_logging.py
--rw-r--r--   0        0        0     1153 2023-01-20 17:58:30.027497 wmul_logger-0.5.1/tox.ini
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 wmul_logger-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2023-01-20 18:02:02.962132 wmul_logger-0.6.0/.gitignore
+-rw-r--r--   0        0        0       91 2023-01-20 18:00:16.745193 wmul_logger-0.6.0/CHANGELOG.txt
+-rw-r--r--   0        0        0    18431 2023-01-20 17:28:47.872017 wmul_logger-0.6.0/LICENSE
+-rw-r--r--   0        0        0       18 2023-01-20 17:28:47.873018 wmul_logger-0.6.0/README.txt
+-rw-r--r--   0        0        0      888 2023-01-20 17:57:40.118351 wmul_logger-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      987 2024-05-24 17:44:39.521754 wmul_logger-0.6.0/src/wmul_logger/__init__.py
+-rw-r--r--   0        0        0     4373 2024-05-24 17:32:27.772780 wmul_logger-0.6.0/src/wmul_logger/logger.py
+-rw-r--r--   0        0        0     9352 2023-01-20 18:00:55.728864 wmul_logger-0.6.0/tests/test_logger.py
+-rw-r--r--   0        0        0     2119 2023-01-20 18:01:31.476370 wmul_logger-0.6.0/tests/test_multiprocess_logging.py
+-rw-r--r--   0        0        0      785 2024-05-24 17:36:10.806103 wmul_logger-0.6.0/tox.ini
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 wmul_logger-0.6.0/setup.py
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 wmul_logger-0.6.0/PKG-INFO
```

### Comparing `wmul_logger-0.5.1/LICENSE` & `wmul_logger-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wmul_logger-0.5.1/pyproject.toml` & `wmul_logger-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wmul_logger-0.5.1/setup.py` & `wmul_logger-0.6.0/src/wmul_logger/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ============ Change Log ============
 2022-May-06 = Changed License from MIT to GPLv2.
 
 2018-Apr-13 = Created.
 
 ============ License ============
-Copyright (c) 2018 Michael Stanley
+Copyright (C) 2018, 2022 Michael Stanley
 
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation; either version 2
 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -19,23 +19,10 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program; if not, write to the Free Software
 Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """
-from setuptools import setup, find_packages
+from wmul_logger.logger import *
 
-setup(
-    name='wmul_logger',
-    version='0.5.0',
-    license='GPLv2',
-    description='Logging Module for WMUL-FM Developed Projects',
-
-    author='Michael Stanley',
-    author_email='stanley50@marshall.edu',
-
-    packages=find_packages(where='src'),
-    package_dir={'': 'src'},
-
-    tests_require=["pytest"],
-)
+__version__ = "0.6.0"
```

### Comparing `wmul_logger-0.5.1/src/wmul_logger/logger.py` & `wmul_logger-0.6.0/src/wmul_logger/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 @Author = 'Mike Stanley'
 
 Logging wrapper.
 
 ============ Change Log ============
+2024-May-28 = Add errors="replace" to the file handler.
+
 2022-May-06 = Changed License from MIT to GPLv2.
 
 2017-Aug-18 = Created.
 
               Moved logging from Utilities to here.
 
 ============ License ============
-Copyright (c) 2017, 2022 Michael Stanley
+Copyright (c) 2017, 2022, 2024 Michael Stanley
 
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License
 as published by the Free Software Foundation; either version 2
 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
@@ -60,15 +62,16 @@
     )
     stdout_handler.setFormatter(log_formatter)
 
     if file_name:
         file_handler = logging.handlers.RotatingFileHandler(
             filename=file_name,
             maxBytes=1_048_576,
-            backupCount=5
+            backupCount=5,
+            errors="replace"
         )
         file_handler.setFormatter(log_formatter)
         file_handler.setLevel(log_level)
         this_logger.addHandler(file_handler)
 
         stdout_handler.setLevel(logging.WARNING)
     else:
```

### Comparing `wmul_logger-0.5.1/tests/test_logger.py` & `wmul_logger-0.6.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `wmul_logger-0.5.1/tests/test_multiprocess_logging.py` & `wmul_logger-0.6.0/tests/test_multiprocess_logging.py`

 * *Files identical despite different names*

### Comparing `wmul_logger-0.5.1/tox.ini` & `wmul_logger-0.6.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,43 @@
 [tox]
 env_list =
+    py312
     py311
     py310
     py39
-    py38
-    py37
-    py36
 minversion = 4.2.8
 
-[testenv:py311]
-description = run the tests with pytest
-package = wheel
-wheel_build_env = .pkg
-deps =
-    pytest>=6
-commands =
-    pytest {tty:--color=yes} {posargs}
-
-[testenv:py310]
-description = run the tests with pytest
-package = wheel
-wheel_build_env = .pkg
-deps =
-    pytest>=6
-commands =
-    pytest {tty:--color=yes} {posargs}
-
-[testenv:py39]
+[testenv:py312]
 description = run the tests with pytest
 package = wheel
 wheel_build_env = .pkg
 deps =
     pytest>=6
 commands =
     pytest {tty:--color=yes} {posargs}
 
-[testenv:py38]
+[testenv:py311]
 description = run the tests with pytest
 package = wheel
 wheel_build_env = .pkg
 deps =
     pytest>=6
 commands =
     pytest {tty:--color=yes} {posargs}
 
-[testenv:py37]
+[testenv:py310]
 description = run the tests with pytest
 package = wheel
 wheel_build_env = .pkg
 deps =
     pytest>=6
 commands =
     pytest {tty:--color=yes} {posargs}
 
-[testenv:py36]
+[testenv:py39]
 description = run the tests with pytest
 package = wheel
 wheel_build_env = .pkg
 deps =
     pytest>=6
 commands =
     pytest {tty:--color=yes} {posargs}
```

### Comparing `wmul_logger-0.5.1/PKG-INFO` & `wmul_logger-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmul_logger
-Version: 0.5.1
+Version: 0.6.0
 Summary: Logging Module for WMUL-FM Developed Projects
 Author-email: Michael Stanley <stanley50@marshall.edu>
 Requires-Python: >=3.6
 Description-Content-Type: text/plain
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
```

