# Comparing `tmp/my_data_preprocessor_mz-0.1.0.tar.gz` & `tmp/my_data_preprocessor_mz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_data_preprocessor_mz-0.1.0.tar", last modified: Thu May 23 16:31:32 2024, max compression
+gzip compressed data, was "my_data_preprocessor_mz-0.2.0.tar", last modified: Fri May 24 03:37:36 2024, max compression
```

## Comparing `my_data_preprocessor_mz-0.1.0.tar` & `my_data_preprocessor_mz-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:32.935631 my_data_preprocessor_mz-0.1.0/
--rw-rw-rw-   0        0        0     1103 2024-05-23 14:28:00.000000 my_data_preprocessor_mz-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5879 2024-05-23 16:31:32.919632 my_data_preprocessor_mz-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5233 2024-05-23 15:45:21.000000 my_data_preprocessor_mz-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:32.828395 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/
--rw-rw-rw-   0        0        0        0 2024-05-19 16:49:28.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/__init__.py
--rw-rw-rw-   0        0        0      873 2024-05-23 16:17:21.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/categorical_encoder.py
--rw-rw-rw-   0        0        0      346 2024-05-23 16:20:04.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/data_type_converter.py
--rw-rw-rw-   0        0        0      627 2024-05-23 16:20:43.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/datetime_handler.py
--rw-rw-rw-   0        0        0     1054 2024-05-23 13:11:49.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/missing_value_handler.py
--rw-rw-rw-   0        0        0     1343 2024-05-23 16:22:01.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/outlier_handler.py
--rw-rw-rw-   0        0        0      906 2024-05-23 11:37:54.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/scaler.py
--rw-rw-rw-   0        0        0     1134 2024-05-23 11:28:51.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:32.911630 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz.egg-info/
--rw-rw-rw-   0        0        0     5879 2024-05-23 16:31:32.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2024-05-23 16:31:32.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:31:32.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-23 16:31:32.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-05-23 16:31:32.000000 my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 16:31:32.936636 my_data_preprocessor_mz-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      944 2024-05-23 15:50:25.000000 my_data_preprocessor_mz-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:32.901634 my_data_preprocessor_mz-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-23 15:59:35.000000 my_data_preprocessor_mz-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      916 2024-05-23 16:01:29.000000 my_data_preprocessor_mz-0.1.0/tests/test_data_type_converter.py
--rw-rw-rw-   0        0        0      947 2024-05-23 16:01:43.000000 my_data_preprocessor_mz-0.1.0/tests/test_datetime_handler.py
--rw-rw-rw-   0        0        0     1063 2024-05-23 16:01:57.000000 my_data_preprocessor_mz-0.1.0/tests/test_missing_value_handler.py
--rw-rw-rw-   0        0        0      714 2024-05-23 16:02:11.000000 my_data_preprocessor_mz-0.1.0/tests/test_outlier_handler.py
--rw-rw-rw-   0        0        0     1005 2024-05-23 16:02:21.000000 my_data_preprocessor_mz-0.1.0/tests/test_scaler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 03:37:36.861041 my_data_preprocessor_mz-0.2.0/
+-rw-rw-rw-   0        0        0     1103 2024-05-23 14:28:00.000000 my_data_preprocessor_mz-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5754 2024-05-24 03:37:36.858047 my_data_preprocessor_mz-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2024-05-24 03:37:05.000000 my_data_preprocessor_mz-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 03:37:36.830047 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/
+-rw-rw-rw-   0        0        0        0 2024-05-19 16:49:28.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/__init__.py
+-rw-rw-rw-   0        0        0      873 2024-05-23 16:17:21.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/categorical_encoder.py
+-rw-rw-rw-   0        0        0      346 2024-05-23 16:20:04.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/data_type_converter.py
+-rw-rw-rw-   0        0        0      627 2024-05-23 16:20:43.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/datetime_handler.py
+-rw-rw-rw-   0        0        0     1054 2024-05-23 13:11:49.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/missing_value_handler.py
+-rw-rw-rw-   0        0        0     1343 2024-05-23 16:22:01.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/outlier_handler.py
+-rw-rw-rw-   0        0        0      906 2024-05-23 11:37:54.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/scaler.py
+-rw-rw-rw-   0        0        0     1134 2024-05-23 11:28:51.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-24 03:37:36.856034 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz.egg-info/
+-rw-rw-rw-   0        0        0     5754 2024-05-24 03:37:36.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2024-05-24 03:37:36.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 03:37:36.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-24 03:37:36.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-05-24 03:37:36.000000 my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 03:37:36.862034 my_data_preprocessor_mz-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      948 2024-05-24 03:37:05.000000 my_data_preprocessor_mz-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 03:37:36.853043 my_data_preprocessor_mz-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-23 15:59:35.000000 my_data_preprocessor_mz-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      916 2024-05-23 16:01:29.000000 my_data_preprocessor_mz-0.2.0/tests/test_data_type_converter.py
+-rw-rw-rw-   0        0        0      947 2024-05-23 16:01:43.000000 my_data_preprocessor_mz-0.2.0/tests/test_datetime_handler.py
+-rw-rw-rw-   0        0        0     1063 2024-05-23 16:01:57.000000 my_data_preprocessor_mz-0.2.0/tests/test_missing_value_handler.py
+-rw-rw-rw-   0        0        0      714 2024-05-23 16:02:11.000000 my_data_preprocessor_mz-0.2.0/tests/test_outlier_handler.py
+-rw-rw-rw-   0        0        0     1005 2024-05-23 16:02:21.000000 my_data_preprocessor_mz-0.2.0/tests/test_scaler.py
```

### Comparing `my_data_preprocessor_mz-0.1.0/LICENSE.txt` & `my_data_preprocessor_mz-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/PKG-INFO` & `my_data_preprocessor_mz-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: my_data_preprocessor_mz
-Version: 0.1.0
+Version: 0.2.0
 Summary: A comprehensive data preprocessing library for data engineering tasks
 Home-page: https://github.com/meyvadem/my_data_preprocessor
 Author:  Merve Demir, Zeynep Dagtekin
-Author-email: merve_demir@stu.fsm.edu.tr
+Author-email: zeynep.dagtekin@stu.fsm.edu.tr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -81,18 +81,15 @@
 df_converted = DateTimeManipulator.convert_to_datetime(df, columns=['Release Date'])
 print("DataFrame after converting to datetime:")
 print(df_converted)
 
 df_date_info = DateTimeManipulator.extract_date_info(df_converted, column='Release Date')
 print("\nDataFrame with extracted date information:")
 print(df_date_info)
-For MissingValueHandler
-```bash
-from my_data_preprocessor_mz.data_type_converter import DataFrameConverter
-import pandas as pd
+
 ```
 
 
 For MissingValueHandler
 ```bash
 from my_data_preprocessor_mz.missing_value_handler import Imputer
 import pandas as pd
```

### Comparing `my_data_preprocessor_mz-0.1.0/README.md` & `my_data_preprocessor_mz-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,15 @@
 df_converted = DateTimeManipulator.convert_to_datetime(df, columns=['Release Date'])
 print("DataFrame after converting to datetime:")
 print(df_converted)
 
 df_date_info = DateTimeManipulator.extract_date_info(df_converted, column='Release Date')
 print("\nDataFrame with extracted date information:")
 print(df_date_info)
-For MissingValueHandler
-```bash
-from my_data_preprocessor_mz.data_type_converter import DataFrameConverter
-import pandas as pd
+
 ```
 
 
 For MissingValueHandler
 ```bash
 from my_data_preprocessor_mz.missing_value_handler import Imputer
 import pandas as pd
```

### Comparing `my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/categorical_encoder.py` & `my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/datetime_handler.py` & `my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/datetime_handler.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/missing_value_handler.py` & `my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/outlier_handler.py` & `my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/scaler.py` & `my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/scaler.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz/text_cleaner.py` & `my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz.egg-info/PKG-INFO` & `my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: my_data_preprocessor_mz
-Version: 0.1.0
+Version: 0.2.0
 Summary: A comprehensive data preprocessing library for data engineering tasks
 Home-page: https://github.com/meyvadem/my_data_preprocessor
 Author:  Merve Demir, Zeynep Dagtekin
-Author-email: merve_demir@stu.fsm.edu.tr
+Author-email: zeynep.dagtekin@stu.fsm.edu.tr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -81,18 +81,15 @@
 df_converted = DateTimeManipulator.convert_to_datetime(df, columns=['Release Date'])
 print("DataFrame after converting to datetime:")
 print(df_converted)
 
 df_date_info = DateTimeManipulator.extract_date_info(df_converted, column='Release Date')
 print("\nDataFrame with extracted date information:")
 print(df_date_info)
-For MissingValueHandler
-```bash
-from my_data_preprocessor_mz.data_type_converter import DataFrameConverter
-import pandas as pd
+
 ```
 
 
 For MissingValueHandler
 ```bash
 from my_data_preprocessor_mz.missing_value_handler import Imputer
 import pandas as pd
```

### Comparing `my_data_preprocessor_mz-0.1.0/my_data_preprocessor_mz.egg-info/SOURCES.txt` & `my_data_preprocessor_mz-0.2.0/my_data_preprocessor_mz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/tests/test_data_type_converter.py` & `my_data_preprocessor_mz-0.2.0/tests/test_data_type_converter.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/tests/test_datetime_handler.py` & `my_data_preprocessor_mz-0.2.0/tests/test_datetime_handler.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/tests/test_missing_value_handler.py` & `my_data_preprocessor_mz-0.2.0/tests/test_missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/tests/test_outlier_handler.py` & `my_data_preprocessor_mz-0.2.0/tests/test_outlier_handler.py`

 * *Files identical despite different names*

### Comparing `my_data_preprocessor_mz-0.1.0/tests/test_scaler.py` & `my_data_preprocessor_mz-0.2.0/tests/test_scaler.py`

 * *Files identical despite different names*

