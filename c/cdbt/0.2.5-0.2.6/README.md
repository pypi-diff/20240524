# Comparing `tmp/cdbt-0.2.5.tar.gz` & `tmp/cdbt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.2.5.tar", last modified: Fri May 24 02:51:54 2024, max compression
+gzip compressed data, was "cdbt-0.2.6.tar", last modified: Fri May 24 02:53:57 2024, max compression
```

## Comparing `cdbt-0.2.5.tar` & `cdbt-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:51:54.705940 cdbt-0.2.5/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:51:54.705254 cdbt-0.2.5/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.5/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:51:54.695681 cdbt-0.2.5/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.5/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4634 2024-05-24 02:44:30.000000 cdbt-0.2.5/cdbt/ai_core.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.2.5/cdbt/build_dbt_docs_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.2.5/cdbt/build_unit_test_data_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 02:51:51.000000 cdbt-0.2.5/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.2.5/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    17569 2024-05-24 02:39:54.000000 cdbt-0.2.5/cdbt/prompts.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:51:54.704740 cdbt-0.2.5/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 02:51:54.706010 cdbt-0.2.5/setup.cfg
--rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 02:51:51.000000 cdbt-0.2.5/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:51:54.703994 cdbt-0.2.5/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.5/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:53:57.005233 cdbt-0.2.6/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:53:57.004326 cdbt-0.2.6/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.6/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:53:56.995094 cdbt-0.2.6/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.6/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4574 2024-05-24 02:53:34.000000 cdbt-0.2.6/cdbt/ai_core.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.2.6/cdbt/build_dbt_docs_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.2.6/cdbt/build_unit_test_data_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 02:51:51.000000 cdbt-0.2.6/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.2.6/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    17569 2024-05-24 02:39:54.000000 cdbt-0.2.6/cdbt/prompts.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:53:57.003803 cdbt-0.2.6/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:53:56.000000 cdbt-0.2.6/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 02:53:56.000000 cdbt-0.2.6/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 02:53:56.000000 cdbt-0.2.6/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 02:53:56.000000 cdbt-0.2.6/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 02:53:56.000000 cdbt-0.2.6/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 02:53:56.000000 cdbt-0.2.6/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 02:53:57.005323 cdbt-0.2.6/setup.cfg
+-rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 02:53:52.000000 cdbt-0.2.6/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:53:57.002676 cdbt-0.2.6/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.6/tests/test_main.py
```

### Comparing `cdbt-0.2.5/PKG-INFO` & `cdbt-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.2.5
+Version: 0.2.6
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.2.5/README.md` & `cdbt-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.5/cdbt/ai_core.py` & `cdbt-0.2.6/cdbt/ai_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         """
         cdbt_main = ColdBoreCapitalDBT()
         sample_results = {}
         for model_name in model_names:
             print(f'Getting sample data for {model_name}')
             args = ['--select', model_name]
             cmd = 'compile'
-            cdbt_main.execute_dbt_command_stream(cmd, args)
             results = cdbt_main.execute_dbt_command_capture(cmd, args)
             extracted_sql = self.extract_sql(results)
             sample_sql = self.build_sample_sql(extracted_sql)
             self._cur.execute(sample_sql)
             tmp_df = self._cur.fetch_pandas_all()
             sample_results[model_name] = tmp_df.to_csv(index=False)
             a = 0
```

### Comparing `cdbt-0.2.5/cdbt/build_dbt_docs_ai.py` & `cdbt-0.2.6/cdbt/build_dbt_docs_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.5/cdbt/build_unit_test_data_ai.py` & `cdbt-0.2.6/cdbt/build_unit_test_data_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.5/cdbt/cmdline.py` & `cdbt-0.2.6/cdbt/cmdline.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.5/cdbt/main.py` & `cdbt-0.2.6/cdbt/main.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.5/cdbt/prompts.py` & `cdbt-0.2.6/cdbt/prompts.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.5/cdbt.egg-info/PKG-INFO` & `cdbt-0.2.6/cdbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.2.5
+Version: 0.2.6
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.2.5/setup.py` & `cdbt-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.2.5',
+    version='0.2.6',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
         'pyperclip',
```

### Comparing `cdbt-0.2.5/tests/test_main.py` & `cdbt-0.2.6/tests/test_main.py`

 * *Files identical despite different names*

