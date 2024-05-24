# Comparing `tmp/ziptimezone-1.1.1.tar.gz` & `tmp/ziptimezone-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-1.1.1.tar", max compression
+gzip compressed data, was "ziptimezone-1.1.2.tar", max compression
```

## Comparing `ziptimezone-1.1.1.tar` & `ziptimezone-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.1.1/LICENSE
--rw-r--r--   0        0        0      846 2024-05-13 11:03:40.070042 ziptimezone-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1818 2024-04-24 12:24:15.572521 ziptimezone-1.1.1/README.rst
--rw-r--r--   0        0        0     1395 2024-05-13 11:45:23.443070 ziptimezone-1.1.1/ziptimezone/__init__.py
--rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.1.1/ziptimezone/batch_processor.py
--rw-r--r--   0        0        0     4294 2024-05-13 14:58:07.970304 ziptimezone-1.1.1/ziptimezone/core.py
--rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.1.1/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.1.1/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.1.1/ziptimezone/globals.py
--rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.1.1/ziptimezone/mappings.py
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 ziptimezone-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.1.2/LICENSE
+-rw-r--r--   0        0        0      817 2024-05-24 17:10:42.718838 ziptimezone-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1944 2024-05-19 09:21:03.238230 ziptimezone-1.1.2/README.rst
+-rw-r--r--   0        0        0     1395 2024-05-13 11:45:23.443070 ziptimezone-1.1.2/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.1.2/ziptimezone/batch_processor.py
+-rw-r--r--   0        0        0     4325 2024-05-19 09:28:26.628819 ziptimezone-1.1.2/ziptimezone/core.py
+-rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.1.2/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.1.2/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.1.2/ziptimezone/globals.py
+-rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.1.2/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 ziptimezone-1.1.2/PKG-INFO
```

### Comparing `ziptimezone-1.1.1/pyproject.toml` & `ziptimezone-1.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "1.1.1"
+version = "1.1.2"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.rst"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
 requests = "^2.31.0"
 timezonefinder = ">=6.1.5, <=6.5.0"
-pandas = ">=1.3.3, <=2.2.2"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ziptimezone-1.1.1/README.rst` & `ziptimezone-1.1.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -47,13 +47,15 @@
     # returns 'Eastern' the timezone has been reduced to the more popular zones 
     # for United States Regions
     zpt.get_timezone_by_zip('02138') 
 
     # returns a dictionary, {'02138': 'Eastern', '85260': 'Mountain'}
     zpt.get_timezone_for_many_zips(['02138', '85260']) 
 
+    # returns a a string, '02138 is ahead of 72201 by 1.00 hours."}
+    zpt.get_timezone_for_many_zips(['02138', '72201']) 
 
 For more refer to the `Documentation <https://ziptimezone.readthedocs.io/en/latest/>`__.
 
 Also check:
 
 `PyPI <https://pypi.python.org/pypi/ziptimezone/>`__
```

### Comparing `ziptimezone-1.1.1/ziptimezone/__init__.py` & `ziptimezone-1.1.2/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.1/ziptimezone/batch_processor.py` & `ziptimezone-1.1.2/ziptimezone/batch_processor.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.1/ziptimezone/core.py` & `ziptimezone-1.1.2/ziptimezone/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     except ValueError as e:
         return str(e)
 
 
 def get_timezone_without_map_by_zip(zip_code):
     """
     Retrieves the timezone based on the provided ZIP code using geographic coordinates.
-
+    Without any Custom mapping.
     Parameters:
         zip_code (str): The ZIP code for which the timezone is requested.
 
     Returns:
         str: The timezone string (e.g., 'America/New_York') if found,
              returns 'Unknown' if the timezone cannot be determined.
     """
```

### Comparing `ziptimezone-1.1.1/ziptimezone/data_manager.py` & `ziptimezone-1.1.2/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.1/ziptimezone/geocode.py` & `ziptimezone-1.1.2/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.1/ziptimezone/globals.py` & `ziptimezone-1.1.2/ziptimezone/globals.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.1/ziptimezone/mappings.py` & `ziptimezone-1.1.2/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.1/PKG-INFO` & `ziptimezone-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pandas (>=1.3.3,<=2.2.2)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: timezonefinder (>=6.1.5,<=6.5.0)
 Description-Content-Type: text/x-rst
 
 ==============
 timezonefinder
 ==============
@@ -66,14 +65,16 @@
     # returns 'Eastern' the timezone has been reduced to the more popular zones 
     # for United States Regions
     zpt.get_timezone_by_zip('02138') 
 
     # returns a dictionary, {'02138': 'Eastern', '85260': 'Mountain'}
     zpt.get_timezone_for_many_zips(['02138', '85260']) 
 
+    # returns a a string, '02138 is ahead of 72201 by 1.00 hours."}
+    zpt.get_timezone_for_many_zips(['02138', '72201']) 
 
 For more refer to the `Documentation <https://ziptimezone.readthedocs.io/en/latest/>`__.
 
 Also check:
 
 `PyPI <https://pypi.python.org/pypi/ziptimezone/>`__
```

