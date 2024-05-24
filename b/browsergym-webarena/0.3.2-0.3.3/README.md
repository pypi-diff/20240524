# Comparing `tmp/browsergym_webarena-0.3.2.tar.gz` & `tmp/browsergym_webarena-0.3.3.tar.gz`

## Comparing `browsergym_webarena-0.3.2.tar` & `browsergym_webarena-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/requirements.txt
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/src/browsergym/webarena/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/src/browsergym/webarena/config.py
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/src/browsergym/webarena/instance.py
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/src/browsergym/webarena/task.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/tests/test_env_general.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/tests/test_instance.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/tests/utils.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/.gitignore
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/README.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/requirements.txt
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/src/browsergym/webarena/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/src/browsergym/webarena/config.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/src/browsergym/webarena/instance.py
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/src/browsergym/webarena/task.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/tests/test_env_general.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/tests/test_instance.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/tests/utils.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/.gitignore
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/README.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 browsergym_webarena-0.3.3/PKG-INFO
```

### Comparing `browsergym_webarena-0.3.2/src/browsergym/webarena/instance.py` & `browsergym_webarena-0.3.3/src/browsergym/webarena/instance.py`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.3.2/src/browsergym/webarena/task.py` & `browsergym_webarena-0.3.3/src/browsergym/webarena/task.py`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.3.2/tests/test_env_general.py` & `browsergym_webarena-0.3.3/tests/test_env_general.py`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.3.2/tests/test_instance.py` & `browsergym_webarena-0.3.3/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.3.2/tests/utils.py` & `browsergym_webarena-0.3.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.3.2/README.md` & `browsergym_webarena-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.3.2/pyproject.toml` & `browsergym_webarena-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_webarena-0.3.2/PKG-INFO` & `browsergym_webarena-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: browsergym-webarena
-Version: 0.3.2
+Version: 0.3.3
 Summary: WebArena benchmark for BrowserGym
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Maxime Gasse, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
-Requires-Dist: browsergym-core==0.3.2
+Requires-Dist: browsergym-core==0.3.3
 Requires-Dist: libwebarena==0.0.3
 Description-Content-Type: text/markdown
 
 # WebArena benchmark for BrowserGym
 
 This package provides `browsergym.webarena`, which is an unofficial port of the [WebArena](https://webarena.dev/) benchmark for BrowserGym.
```

