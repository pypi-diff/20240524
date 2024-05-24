# Comparing `tmp/cdbt-0.2.4.tar.gz` & `tmp/cdbt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdbt-0.2.4.tar", last modified: Fri May 24 02:48:40 2024, max compression
+gzip compressed data, was "cdbt-0.2.5.tar", last modified: Fri May 24 02:51:54 2024, max compression
```

## Comparing `cdbt-0.2.4.tar` & `cdbt-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:48:40.731193 cdbt-0.2.4/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:48:40.730385 cdbt-0.2.4/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.4/README.md
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:48:40.716118 cdbt-0.2.4/cdbt/
--rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.4/cdbt/__init__.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4634 2024-05-24 02:44:30.000000 cdbt-0.2.4/cdbt/ai_core.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.2.4/cdbt/build_dbt_docs_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.2.4/cdbt/build_unit_test_data_ai.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)     6704 2024-05-23 17:30:10.000000 cdbt-0.2.4/cdbt/cmdline.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.2.4/cdbt/main.py
--rw-r--r--   0 craiglathrop   (501) staff       (20)    17569 2024-05-24 02:39:54.000000 cdbt-0.2.4/cdbt/prompts.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:48:40.729723 cdbt-0.2.4/cdbt.egg-info/
--rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/PKG-INFO
--rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/SOURCES.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/dependency_links.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/entry_points.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/requires.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 02:48:40.000000 cdbt-0.2.4/cdbt.egg-info/top_level.txt
--rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 02:48:40.731327 cdbt-0.2.4/setup.cfg
--rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 02:48:37.000000 cdbt-0.2.4/setup.py
-drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:48:40.728887 cdbt-0.2.4/tests/
--rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.4/tests/test_main.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:51:54.705940 cdbt-0.2.5/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:51:54.705254 cdbt-0.2.5/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4072 2024-05-17 13:41:23.000000 cdbt-0.2.5/README.md
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:51:54.695681 cdbt-0.2.5/cdbt/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        0 2024-05-15 13:54:01.000000 cdbt-0.2.5/cdbt/__init__.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4634 2024-05-24 02:44:30.000000 cdbt-0.2.5/cdbt/ai_core.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4591 2024-05-24 02:45:14.000000 cdbt-0.2.5/cdbt/build_dbt_docs_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     4070 2024-05-24 02:39:54.000000 cdbt-0.2.5/cdbt/build_unit_test_data_ai.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     6856 2024-05-24 02:51:51.000000 cdbt-0.2.5/cdbt/cmdline.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    19551 2024-05-24 02:39:54.000000 cdbt-0.2.5/cdbt/main.py
+-rw-r--r--   0 craiglathrop   (501) staff       (20)    17569 2024-05-24 02:39:54.000000 cdbt-0.2.5/cdbt/prompts.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:51:54.704740 cdbt-0.2.5/cdbt.egg-info/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      517 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/PKG-INFO
+-rw-r--r--   0 craiglathrop   (501) staff       (20)      343 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        1 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       43 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/entry_points.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       72 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/requires.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)        5 2024-05-24 02:51:54.000000 cdbt-0.2.5/cdbt.egg-info/top_level.txt
+-rw-r--r--   0 craiglathrop   (501) staff       (20)       38 2024-05-24 02:51:54.706010 cdbt-0.2.5/setup.cfg
+-rwxr-xr-x   0 craiglathrop   (501) staff       (20)      753 2024-05-24 02:51:51.000000 cdbt-0.2.5/setup.py
+drwxr-xr-x   0 craiglathrop   (501) staff       (20)        0 2024-05-24 02:51:54.703994 cdbt-0.2.5/tests/
+-rw-r--r--   0 craiglathrop   (501) staff       (20)     7050 2024-05-15 13:54:01.000000 cdbt-0.2.5/tests/test_main.py
```

### Comparing `cdbt-0.2.4/PKG-INFO` & `cdbt-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.2.4/README.md` & `cdbt-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.4/cdbt/ai_core.py` & `cdbt-0.2.5/cdbt/ai_core.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.4/cdbt/build_dbt_docs_ai.py` & `cdbt-0.2.5/cdbt/build_dbt_docs_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.4/cdbt/build_unit_test_data_ai.py` & `cdbt-0.2.5/cdbt/build_unit_test_data_ai.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.4/cdbt/cmdline.py` & `cdbt-0.2.5/cdbt/cmdline.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
             ctx.obj['build_parents'] = True
             ctx.obj['build_parents_count'] = int(count) if count else None  # Default to 1 if no number is specified
 
         return click.Group.get_command(self, ctx, cmd_name)
 
     def list_commands(self, ctx):
         # List of all commands
-        return ['help', 'build', 'trun', 'run', 'test', 'compile', 'clip-compile', 'unittest', 'sbuild', 'pbuild', 'build-docs', 'build-unit']
+        return ['help', 'build', 'trun', 'run', 'test', 'compile', 'clip-compile', 'unittest', 'sbuild', 'pbuild',
+                'gbuild', 'build-docs', 'build-unit', 'lightdash']
 
 
 cdbt = CustomCmdLoader()
 
 
 @cdbt.command()
 @click.option('--full-refresh', '-f', is_flag=True, help='Run a full refresh on all models.')
@@ -121,31 +122,31 @@
 
 
 @cdbt.command()
 @click.option('--full-refresh', '-f', is_flag=True, help='Force a full refresh on all models in build scope.')
 @click.option('--threads', '-t', type=int, help='Number of threads to use during DBT operations.')
 @click.pass_context
 def gbuild(ctx, full_refresh, threads):
-    """Build models based on changes from production to current branch."""
+    """Build models based on Git changes from production to current branch."""
     cdbt_class.gbuild(ctx, full_refresh, threads)
 
 @cdbt.command()
+@click.option('--select', '-s', type=str, required=True, help='Name of the model to build unit test data for.')
 @click.pass_context
-@click.option('--select', '-s', type=str, help='Name of the model to build unit test data for.')
 def build_docs(ctx, select):
-    """Build dbt YML model docs for a model"""
+    """Build dbt YML model docs for a model. This command will sample the database."""
     dbt_docs = BuildDBTDocs()
     dbt_docs.main(select)
 
 
 @cdbt.command()
-@click.option('--select', '-s', type=str, help='Name of the model to build unit test data for.')
+@click.option('--select', '-s', type=str, required=True, help='Name of the model to build unit test data for.')
 @click.pass_context
 def build_unit(ctx, select):
-    """Build unit test mock and expect data for a model."""
+    """Build unit test mock and expect data for a model. This command will sample the database."""
     build_unit_test_data = BuildUnitTestDataAI()
     build_unit_test_data.main(select)
 
 @cdbt.command()
 @click.option('--select', '-s', type=str, help='Name of the model to start a lightdash preview for. If not provided, all models will be previewed.')
 @click.option('--name', '-n', type=str, required=True, help='Name of the lightdash preview. Required.')
 @click.pass_context
```

### Comparing `cdbt-0.2.4/cdbt/main.py` & `cdbt-0.2.5/cdbt/main.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.4/cdbt/prompts.py` & `cdbt-0.2.5/cdbt/prompts.py`

 * *Files identical despite different names*

### Comparing `cdbt-0.2.4/cdbt.egg-info/PKG-INFO` & `cdbt-0.2.5/cdbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdbt
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI tool to manage dbt builds with state handling and manifest management
 Author: Craig Lathrop
 Author-email: development@coldborecapital.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `cdbt-0.2.4/setup.py` & `cdbt-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdbt',
-    version='0.2.4',
+    version='0.2.5',
     description='A CLI tool to manage dbt builds with state handling and manifest management',
     author='Craig Lathrop',
     author_email='development@coldborecapital.com',
     packages=find_packages(),
     install_requires=[
         'click',
         'pyperclip',
```

### Comparing `cdbt-0.2.4/tests/test_main.py` & `cdbt-0.2.5/tests/test_main.py`

 * *Files identical despite different names*

