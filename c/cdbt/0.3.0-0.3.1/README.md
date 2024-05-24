# Comparing `tmp/cdbt-0.3.0.tar.gz` & `tmp/cdbt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.3.0.tar", last modified: Fri May 24 03:33:52 2024, max compression
+gzip compressed data, was "cdbt-0.3.1.tar", last modified: Fri May 24 16:35:34 2024, max compression
```

## Comparing `cdbt-0.3.0.tar` & `cdbt-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:33:52.547986 cdbt-0.3.0/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:33:52.547217 cdbt-0.3.0/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.3.0/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:33:52.532129 cdbt-0.3.0/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.3.0/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     5290 2024-05-24 03:23:49.000000 cdbt-0.3.0/cdbt/ai_core.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.3.0/cdbt/build_dbt_docs_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.3.0/cdbt/build_unit_test_data_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 02:51:51.000000 cdbt-0.3.0/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.3.0/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    17495 2024-05-24 03:28:48.000000 cdbt-0.3.0/cdbt/prompts.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:33:52.546464 cdbt-0.3.0/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 03:33:52.548093 cdbt-0.3.0/setup.cfg
--rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 03:33:42.000000 cdbt-0.3.0/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:33:52.545484 cdbt-0.3.0/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.3.0/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 16:35:34.380075 cdbt-0.3.1/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 16:35:34.379680 cdbt-0.3.1/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.3.1/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 16:35:34.372788 cdbt-0.3.1/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.3.1/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     5290 2024-05-24 16:21:23.000000 cdbt-0.3.1/cdbt/ai_core.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 16:21:23.000000 cdbt-0.3.1/cdbt/build_dbt_docs_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 16:21:23.000000 cdbt-0.3.1/cdbt/build_unit_test_data_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 16:21:23.000000 cdbt-0.3.1/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 16:21:23.000000 cdbt-0.3.1/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    17594 2024-05-24 16:35:28.000000 cdbt-0.3.1/cdbt/prompts.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 16:35:34.379340 cdbt-0.3.1/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 16:35:34.000000 cdbt-0.3.1/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 16:35:34.000000 cdbt-0.3.1/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 16:35:34.000000 cdbt-0.3.1/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 16:35:34.000000 cdbt-0.3.1/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 16:35:34.000000 cdbt-0.3.1/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 16:35:34.000000 cdbt-0.3.1/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 16:35:34.380131 cdbt-0.3.1/setup.cfg
+-rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 16:35:28.000000 cdbt-0.3.1/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 16:35:34.378913 cdbt-0.3.1/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.3.1/tests/test_main.py
```

### Comparing `cdbt-0.3.0/PKG-INFO` & `cdbt-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.3.0
+Version: 0.3.1
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.3.0/README.md` & `cdbt-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cdbt-0.3.0/cdbt/ai_core.py` & `cdbt-0.3.1/cdbt/ai_core.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.3.0/cdbt/build_dbt_docs_ai.py` & `cdbt-0.3.1/cdbt/build_dbt_docs_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.3.0/cdbt/build_unit_test_data_ai.py` & `cdbt-0.3.1/cdbt/build_unit_test_data_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.3.0/cdbt/cmdline.py` & `cdbt-0.3.1/cdbt/cmdline.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.3.0/cdbt/main.py` & `cdbt-0.3.1/cdbt/main.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.3.0/cdbt/prompts.py` & `cdbt-0.3.1/cdbt/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,9 +368,10 @@
 8. Output the data in the same format as the example. Use as many `dbt_unit_testing.mock_ref` blocks as needed.
 9. Use enough rows with variation that at least one aggregation can be created. For example, if the model groups by date and ID, you will need at least two rows with the same date and ID but different values for the columns being aggregated. 
 10. Location names are always three uppercase letters followed by three numbers. For example, "ABC123" or "DEF123". Network names are always the first three uppercase letters of the network name, like "ABC" or "DEF"
 11. At the top of the file as in the example, add a --depends-on line for each moc_ref model used in the input SQL. Example, --depends-on: {{ ref('fct_appointments') }}
 12. Encapsulate any string in single or date in single quotes. Even if the sample data has long strings, truncate to no more than 30 characters, preferably even less unless the logic requires something more.
 13. Try to limit the date range in the input data to one or two days of time span, unless more is needed to fully test the logic of the model.
 14. Do not include timezones in mockup data unless the sample data provided for that model includes timezones.
+15. Do not include columns in the mock_ref blocks that are not used by the SQL model being tested.
 Do not provide an explanation, only return the code for the test.
         """
```

### Comparing `cdbt-0.3.0/cdbt.egg-info/PKG-INFO` & `cdbt-0.3.1/cdbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.3.0
+Version: 0.3.1
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.3.0/setup.py` & `cdbt-0.3.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.3.0',
+    version='0.3.1',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
         'pyperclip',
```

### Comparing `cdbt-0.3.0/tests/test_main.py` & `cdbt-0.3.1/tests/test_main.py`

 * *Files identical despite different names*

