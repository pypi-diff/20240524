# Comparing `tmp/cdbt-0.2.7.tar.gz` & `tmp/cdbt-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.2.7.tar", last modified: Fri May 24 03:04:36 2024, max compression
+gzip compressed data, was "cdbt-0.2.8.tar", last modified: Fri May 24 03:10:20 2024, max compression
```

## Comparing `cdbt-0.2.7.tar` & `cdbt-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:04:36.805381 cdbt-0.2.7/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:04:36.804657 cdbt-0.2.7/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.7/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:04:36.795362 cdbt-0.2.7/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.7/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4790 2024-05-24 03:04:34.000000 cdbt-0.2.7/cdbt/ai_core.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.2.7/cdbt/build_dbt_docs_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.2.7/cdbt/build_unit_test_data_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 02:51:51.000000 cdbt-0.2.7/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.2.7/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    17569 2024-05-24 02:39:54.000000 cdbt-0.2.7/cdbt/prompts.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:04:36.804067 cdbt-0.2.7/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:04:36.000000 cdbt-0.2.7/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 03:04:36.000000 cdbt-0.2.7/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 03:04:36.000000 cdbt-0.2.7/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 03:04:36.000000 cdbt-0.2.7/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 03:04:36.000000 cdbt-0.2.7/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 03:04:36.000000 cdbt-0.2.7/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 03:04:36.805453 cdbt-0.2.7/setup.cfg
--rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 03:04:22.000000 cdbt-0.2.7/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:04:36.803189 cdbt-0.2.7/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.7/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:10:20.729904 cdbt-0.2.8/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:10:20.728012 cdbt-0.2.8/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.8/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:10:20.702132 cdbt-0.2.8/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.8/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     5002 2024-05-24 03:09:54.000000 cdbt-0.2.8/cdbt/ai_core.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.2.8/cdbt/build_dbt_docs_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.2.8/cdbt/build_unit_test_data_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 02:51:51.000000 cdbt-0.2.8/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.2.8/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    17569 2024-05-24 02:39:54.000000 cdbt-0.2.8/cdbt/prompts.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:10:20.725697 cdbt-0.2.8/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 03:10:20.000000 cdbt-0.2.8/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 03:10:20.730033 cdbt-0.2.8/setup.cfg
+-rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 03:09:54.000000 cdbt-0.2.8/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 03:10:20.723532 cdbt-0.2.8/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.8/tests/test_main.py
```

### Comparing `cdbt-0.2.7/PKG-INFO` & `cdbt-0.2.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.2.7
+Version: 0.2.8
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.2.7/README.md` & `cdbt-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.7/cdbt/ai_core.py` & `cdbt-0.2.8/cdbt/ai_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             sample_sql = self.build_sample_sql(extracted_sql)
             try:
                 self._cur.execute(sample_sql)
             except snow.DatabaseError as e:
                 print(f'Error executing sample SQL for {model_name}')
                 print(e)
                 print('\n\n'+sample_sql+'\n\n')
-                continue
+                raise e
             tmp_df = self._cur.fetch_pandas_all()
             sample_results[model_name] = tmp_df.to_csv(index=False)
 
         return sample_results
 
     @staticmethod
     def build_sample_sql(sql: str) -> str:
@@ -117,10 +117,12 @@
             sample (20 rows)
             '''
         return sql
 
     @staticmethod
     def extract_sql(log):
         sql_lines = [line for line in log.splitlines() if not re.match(r'^\x1b\[0m\d{2}:\d{2}:\d{2}', line)]
+        sql_lines = [line for line in log.splitlines() if not re.match(r'There are \d+ unused configuration paths:', line)]
+        sql_lines = [line for line in log.splitlines() if not re.match(r'--\s.*', line)]
         # Join the remaining lines and remove escape sequences
         sql = '\n'.join(sql_lines).replace('\x1b[0m', '').strip()
         return sql
```

### Comparing `cdbt-0.2.7/cdbt/build_dbt_docs_ai.py` & `cdbt-0.2.8/cdbt/build_dbt_docs_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.7/cdbt/build_unit_test_data_ai.py` & `cdbt-0.2.8/cdbt/build_unit_test_data_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.7/cdbt/cmdline.py` & `cdbt-0.2.8/cdbt/cmdline.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.7/cdbt/main.py` & `cdbt-0.2.8/cdbt/main.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.7/cdbt/prompts.py` & `cdbt-0.2.8/cdbt/prompts.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.7/cdbt.egg-info/PKG-INFO` & `cdbt-0.2.8/cdbt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.2.7
+Version: 0.2.8
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.2.7/setup.py` & `cdbt-0.2.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.2.7',
+    version='0.2.8',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
         'pyperclip',
```

### Comparing `cdbt-0.2.7/tests/test_main.py` & `cdbt-0.2.8/tests/test_main.py`

 * *Files identical despite different names*

