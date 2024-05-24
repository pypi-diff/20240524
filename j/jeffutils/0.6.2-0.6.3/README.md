# Comparing `tmp/jeffutils-0.6.2.tar.gz` & `tmp/jeffutils-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.6.2.tar", last modified: Wed May 22 19:01:07 2024, max compression
+gzip compressed data, was "jeffutils-0.6.3.tar", last modified: Fri May 24 14:42:35 2024, max compression
```

## Comparing `jeffutils-0.6.2.tar` & `jeffutils-0.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-22 19:01:07.337368 jeffutils-0.6.2/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.2/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-22 19:01:07.337368 jeffutils-0.6.2/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.6.2/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.2/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-22 19:01:07.337368 jeffutils-0.6.2/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-22 19:01:04.000000 jeffutils-0.6.2/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-22 19:01:07.337368 jeffutils-0.6.2/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-22 19:01:07.337368 jeffutils-0.6.2/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.2/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    25602 2024-05-22 19:00:52.000000 jeffutils-0.6.2/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-22 19:01:07.337368 jeffutils-0.6.2/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-22 19:01:07.000000 jeffutils-0.6.2/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-22 19:01:07.000000 jeffutils-0.6.2/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-22 19:01:07.000000 jeffutils-0.6.2/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-22 19:01:07.000000 jeffutils-0.6.2/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 14:42:35.725003 jeffutils-0.6.3/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.3/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-24 14:42:35.725003 jeffutils-0.6.3/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.6.3/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.3/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-24 14:42:35.725003 jeffutils-0.6.3/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-24 14:42:32.000000 jeffutils-0.6.3/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 14:42:35.721003 jeffutils-0.6.3/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 14:42:35.721003 jeffutils-0.6.3/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.3/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    28978 2024-05-24 14:42:17.000000 jeffutils-0.6.3/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 14:42:35.725003 jeffutils-0.6.3/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-24 14:42:35.000000 jeffutils-0.6.3/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-24 14:42:35.000000 jeffutils-0.6.3/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-24 14:42:35.000000 jeffutils-0.6.3/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-24 14:42:35.000000 jeffutils-0.6.3/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.6.2/LICENSE.txt` & `jeffutils-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.2/setup.py` & `jeffutils-0.6.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.6.2',
+    version='0.6.3',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.6.2/src/jeffutils/utils.py` & `jeffutils-0.6.3/src/jeffutils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from collections import defaultdict
 import sqlite3 as sql
 import json
 import numpy as np
 import pandas as pd
 import io
 import os
+import sys
+import importlib
+import re
 import pstats
 import cProfile
 import traceback
 from IPython.display import display
 from copy import deepcopy
 import ast
 
@@ -585,14 +588,96 @@
             else:
                 pass
             
         # sleep for 1 minute, so that it only checks all of the threads
         # every minute
         time.sleep(60)
         
+def reimport(import_statement:str):
+    """ takes in any single import statement and imports/reimports the module
+    and handles associated aliases.
+    
+    Examples:
+    'import random' - imports 'random' in sys.modules
+    'import numpy as np' - imports 'numpy' in sys.modules and assigns the
+       alias 'np' in the globals() dictionary
+    'import numpy as np, pandas as pd' - imports both numpy and pandas
+       with their associated aliases
+    'from jeffutils.utils import pprint, stack_trace, log_print as lp' -
+       imports pprint, stack_trace and log_print as lp
+       
+    raises:
+    AttributeError: if the module or function is not found in sys.modules
+    """
+    
+    def import_one(module:str):
+        """ takes in a string like 'random' or 'numpy as np' and imports that
+        module with its alias if given
+        """
+        if 'as' in module:
+            module_name, alias = module.split(' as ')
+            if module_name in sys.modules:
+                importlib.reload(sys.modules[module_name])
+                module_obj = sys.modules[module_name]
+            else:
+                module_obj = importlib.import_module(module_name)
+            globals()[alias] = module_obj
+            
+        else:
+            if module in sys.modules:
+                importlib.reload(sys.modules[module])
+                module_obj = sys.modules[module]
+            else:
+                module_obj = importlib.import_module(module)
+            
+    def import_sub_func(module, func):
+        """ handles something like "from random import randint" where 'random'
+        is the module and 'randint' is the function
+        """
+        if module not in sys.modules:
+            raise AttributeError(f"Module {module} not found in sys.modules")
+        module_obj = sys.modules[module]
+        
+        if 'as' in func:
+            func_name, alias = func.split(' as ')
+            if func_name in dir(module_obj):
+                globals()[alias] = getattr(module_obj, func_name)
+            else:
+                raise AttributeError(f"Function {func_name} not found in module {module}")
+        
+        else:
+            if func in dir(module_obj):
+                globals()[func] = getattr(module_obj, func)
+            else:
+                raise AttributeError(f"Function {func} not found in module {module}")
+    
+    # remove whitespace at the start and end of the import statement
+    import_statement = import_statement.strip()
+    
+    # extract all of the modules names ('os', 'numpy as np', 'jeffutils.utils', 'stack_trace')
+    module_re = re.compile(r"(\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b\sas\s\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b|\b(?!(?:import|from|as))[a-zA-Z0-9._]+\b)")
+    module_names = module_re.findall(import_statement)
+    
+    # if a vanilla import statement, import each module
+    if import_statement.startswith("import"):
+        for module_name in module_names:
+            import_one(module_name)
+        
+    # if importing functions/sub-modules from a module
+    elif import_statement.startswith("from"):
+        
+        # import the base module
+        module = module_names[0]
+        import_one(module)
+        
+        # import each sub-function from the module
+        for func_name in module_names[1:]:
+            import_sub_func(module, func_name)
+    
+        
 ############################################################
 #                       SQL FUNCTIONS                      #
 ############################################################
 
 def get_sql_tables_info(db_path, verbose=True):
     """
     Retrieve and print all table names and their respective column names from a SQLite database.
```

