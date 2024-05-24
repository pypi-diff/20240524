# Comparing `tmp/cdbt-0.2.8.tar.gz` & `tmp/cdbt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.2.8.tar", last modified: Fri May 24 03:10:20 2024, max compression
+gzip compressed data, was "cdbt-0.3.0.tar", last modified: Fri May 24 03:33:52 2024, max compression
```

## Comparing `cdbt-0.2.8.tar` & `cdbt-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:10:20.729904 cdbt-0.2.8/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:10:20.728012 cdbt-0.2.8/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.8/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:10:20.702132 cdbt-0.2.8/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.8/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     5002 2024-05-24 03:09:54.000000 cdbt-0.2.8/cdbt/ai_core.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.2.8/cdbt/build_dbt_docs_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.2.8/cdbt/build_unit_test_data_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 02:51:51.000000 cdbt-0.2.8/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.2.8/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    17569 2024-05-24 02:39:54.000000 cdbt-0.2.8/cdbt/prompts.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:10:20.725697 cdbt-0.2.8/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 03:10:20.730033 cdbt-0.2.8/setup.cfg
--rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 03:09:54.000000 cdbt-0.2.8/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:10:20.723532 cdbt-0.2.8/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.8/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:33:52.547986 cdbt-0.3.0/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:33:52.547217 cdbt-0.3.0/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.3.0/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:33:52.532129 cdbt-0.3.0/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.3.0/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     5290 2024-05-24 03:23:49.000000 cdbt-0.3.0/cdbt/ai_core.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.3.0/cdbt/build_dbt_docs_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.3.0/cdbt/build_unit_test_data_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 02:51:51.000000 cdbt-0.3.0/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.3.0/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    17495 2024-05-24 03:28:48.000000 cdbt-0.3.0/cdbt/prompts.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:33:52.546464 cdbt-0.3.0/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 03:33:52.000000 cdbt-0.3.0/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 03:33:52.548093 cdbt-0.3.0/setup.cfg
+-rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 03:33:42.000000 cdbt-0.3.0/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:33:52.545484 cdbt-0.3.0/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.3.0/tests/test_main.py
```

### Comparing `cdbt-0.2.8/PKG-INFO` & `cdbt-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.2.8
+Version: 0.3.0
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.2.8/README.md` & `cdbt-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.8/cdbt/ai_core.py` & `cdbt-0.3.0/cdbt/ai_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,12 +117,22 @@
             sample (20 rows)
             '''
         return sql
 
     @staticmethod
     def extract_sql(log):
         sql_lines = [line for line in log.splitlines() if not re.match(r'^\x1b\[0m\d{2}:\d{2}:\d{2}', line)]
+        # Edge case when there are unused config paths
         sql_lines = [line for line in log.splitlines() if not re.match(r'There are \d+ unused configuration paths:', line)]
         sql_lines = [line for line in log.splitlines() if not re.match(r'--\s.*', line)]
+
+        keyword_line_index = 0
+        for i, line in enumerate(sql_lines):
+            if 'Compiled node' in line:
+                keyword_line_index = i+1
+                break
+
+        sql_lines = sql_lines[keyword_line_index:]
+
         # Join the remaining lines and remove escape sequences
         sql = '\n'.join(sql_lines).replace('\x1b[0m', '').strip()
         return sql
```

### Comparing `cdbt-0.2.8/cdbt/build_dbt_docs_ai.py` & `cdbt-0.3.0/cdbt/build_dbt_docs_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.8/cdbt/build_unit_test_data_ai.py` & `cdbt-0.3.0/cdbt/build_unit_test_data_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.8/cdbt/cmdline.py` & `cdbt-0.3.0/cdbt/cmdline.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.8/cdbt/main.py` & `cdbt-0.3.0/cdbt/main.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.8/cdbt/prompts.py` & `cdbt-0.3.0/cdbt/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 
 
 class Prompts:
+    '''
+Holding: @ todo: something with this like a local config.
+    1. These models are all veterinary related.
+    2. VS is shorthand for Vetspire. Vetspire is a veterinary software practice management company.
+'''
 
     @property
     def dbt_docs_gte_l3_prompt(self):
         return """
 You will help build DBT documentation YML files for a given SQL query. Sometimes you will be asked to generate a description from scratch, other times you will be asked to fill in missing columns that exist in the model, but not in the documentation.
 
 
 Primary DBT Guidelines:
-    1. These models are all veterinary related.
-    2. VS is shorthand for Vetspire. Vetspire is a veterinary software practice management company.
+
     3. Include a config block for each model:
         a. Set `materialized` to `table`
         b. Do not include a `sort` key.
     4. Do not add any tests. This model is part of the L1 or L2 layer and does not get tested.
     5. For long descriptions, use the following format so the lines are not too long:
         ```
         - name: replacement_plan_id
@@ -205,23 +209,24 @@
               compact: thousands
               group_label: "Count"
 ```
 
 This is a CSV data sample from the model:        
         """
 
+
+
     @property
     def dbt_docs_lte_l2_prompt(self):
         return """
         You will help build DBT documentation YML files for a given SQL query. Sometimes you will be asked to generate a description from scratch, other times you will be asked to fill in missing columns that exist in the model, but not in the documentation.
 
 
 Primary DBT Guidelines:
-    1. These models are all veterinary related.
-    2. VS is shorthand for Vetspire. Vetspire is a veterinary software practice management company.
+
     3. Include a config block for each model:
         a. Set `materialized` to `view`
         b. Do not include a `sort` key.
         c. If the model name ends in `_mat` set materialized to `table`.
     4. Add tests `unique` and `not_null` to the primary key only. Do not add tests to any other columns.
     5. For long descriptions, use the following format so the lines are not too long:
         ```
```

### Comparing `cdbt-0.2.8/cdbt.egg-info/PKG-INFO` & `cdbt-0.3.0/cdbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.2.8
+Version: 0.3.0
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.2.8/setup.py` & `cdbt-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.2.8',
+    version='0.3.0',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
         'pyperclip',
```

### Comparing `cdbt-0.2.8/tests/test_main.py` & `cdbt-0.3.0/tests/test_main.py`

 * *Files identical despite different names*

