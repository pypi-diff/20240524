# Comparing `tmp/jeffutils-0.6.3.tar.gz` & `tmp/jeffutils-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.6.3.tar", last modified: Fri May 24 14:42:35 2024, max compression
+gzip compressed data, was "jeffutils-0.6.4.tar", last modified: Fri May 24 16:00:05 2024, max compression
```

## Comparing `jeffutils-0.6.3.tar` & `jeffutils-0.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 14:42:35.725003 jeffutils-0.6.3/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.3/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-24 14:42:35.725003 jeffutils-0.6.3/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.6.3/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.3/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-24 14:42:35.725003 jeffutils-0.6.3/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-24 14:42:32.000000 jeffutils-0.6.3/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 14:42:35.721003 jeffutils-0.6.3/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 14:42:35.721003 jeffutils-0.6.3/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.3/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    28978 2024-05-24 14:42:17.000000 jeffutils-0.6.3/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 14:42:35.725003 jeffutils-0.6.3/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-24 14:42:35.000000 jeffutils-0.6.3/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-24 14:42:35.000000 jeffutils-0.6.3/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-24 14:42:35.000000 jeffutils-0.6.3/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-24 14:42:35.000000 jeffutils-0.6.3/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 16:00:05.691100 jeffutils-0.6.4/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.4/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-24 16:00:05.691100 jeffutils-0.6.4/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.6.4/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.4/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-24 16:00:05.691100 jeffutils-0.6.4/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-24 16:00:02.000000 jeffutils-0.6.4/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 16:00:05.691100 jeffutils-0.6.4/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 16:00:05.691100 jeffutils-0.6.4/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.4/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    29013 2024-05-24 15:59:42.000000 jeffutils-0.6.4/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-24 16:00:05.691100 jeffutils-0.6.4/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-24 16:00:05.000000 jeffutils-0.6.4/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-24 16:00:05.000000 jeffutils-0.6.4/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-24 16:00:05.000000 jeffutils-0.6.4/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-24 16:00:05.000000 jeffutils-0.6.4/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.6.3/LICENSE.txt` & `jeffutils-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.3/setup.py` & `jeffutils-0.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.6.3',
+    version='0.6.4',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.6.3/src/jeffutils/utils.py` & `jeffutils-0.6.4/src/jeffutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         if len(curr_line + curr) > LENGTH_LIM:
             string += curr_line + "\n    "
             curr_line = ""
         curr_line += curr
     
     return string + curr_line
 
-def log_func_vars(func_name, vars, globals, locals, header=True):
+def log_func_vars(func_name, vars, globals, locals, header=True, only_log=False):
     """
     Logs the information in a formatted way.
 
     Parameters:
     func_name (str): The title of the function that is making this log.
     vars (list): a list of strings that represent the variable names to log.
     globals (dict): The global variables dictionary, typically passed as globals().
@@ -164,15 +164,15 @@
     str: The formatted log string.
 
     Notes:
     - The function will default to logging the information unless the LOG_TOGGLE dictionary has the function name set to False.
     """
     info_dict = get_log_dict(vars, globals, locals)
     string = get_log_string(func_name, info_dict)
-    log_print(string, header=header)
+    log_print(string, header=header, only_log=only_log)
     
     return string
 
 def initialize_log_func_vars_func(LOG_TOGGLE):
     """ returns a function that will log the variables of a function
     with the LOG_TOGGLE dictionary set to LOG_TOGGLE
     """
```

