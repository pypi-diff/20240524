# Comparing `tmp/byu_pytest_utils-0.7.8.tar.gz` & `tmp/byu_pytest_utils-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byu_pytest_utils-0.7.8.tar", max compression
+gzip compressed data, was "byu_pytest_utils-0.7.9.tar", max compression
```

## Comparing `byu_pytest_utils-0.7.8.tar` & `byu_pytest_utils-0.7.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1257 2023-12-22 21:30:47.715487 byu_pytest_utils-0.7.8/byu_pytest_utils/__init__.py
--rw-r--r--   0        0        0     2418 2024-01-02 20:36:07.184667 byu_pytest_utils-0.7.8/byu_pytest_utils/cpp_utils.py
--rw-r--r--   0        0        0     1168 2023-06-16 19:58:44.971739 byu_pytest_utils-0.7.8/byu_pytest_utils/decorators.py
--rw-r--r--   0        0        0    16963 2024-01-02 21:01:41.646152 byu_pytest_utils-0.7.8/byu_pytest_utils/dialog.py
--rw-r--r--   0        0        0     3114 2023-12-27 02:27:30.963706 byu_pytest_utils-0.7.8/byu_pytest_utils/edit_dist.py
--rw-r--r--   0        0        0     3708 2023-06-23 18:33:47.968688 byu_pytest_utils-0.7.8/byu_pytest_utils/pytest_plugin.py
--rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.7.8/byu_pytest_utils/utils.py
--rw-r--r--   0        0        0      562 2024-01-02 20:55:20.054216 byu_pytest_utils-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1257 2023-12-22 21:30:47.715487 byu_pytest_utils-0.7.9/byu_pytest_utils/__init__.py
+-rw-r--r--   0        0        0     2418 2024-01-02 20:36:07.184667 byu_pytest_utils-0.7.9/byu_pytest_utils/cpp_utils.py
+-rw-r--r--   0        0        0     1168 2023-06-16 19:58:44.971739 byu_pytest_utils-0.7.9/byu_pytest_utils/decorators.py
+-rw-r--r--   0        0        0    17179 2024-01-11 17:02:11.962506 byu_pytest_utils-0.7.9/byu_pytest_utils/dialog.py
+-rw-r--r--   0        0        0     3114 2023-12-27 02:27:30.963706 byu_pytest_utils-0.7.9/byu_pytest_utils/edit_dist.py
+-rw-r--r--   0        0        0     3708 2023-06-23 18:33:47.968688 byu_pytest_utils-0.7.9/byu_pytest_utils/pytest_plugin.py
+-rw-r--r--   0        0        0     3474 2023-04-21 21:39:00.608118 byu_pytest_utils-0.7.9/byu_pytest_utils/utils.py
+-rw-r--r--   0        0        0      562 2024-01-11 17:02:27.153786 byu_pytest_utils-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 byu_pytest_utils-0.7.9/PKG-INFO
```

### Comparing `byu_pytest_utils-0.7.8/byu_pytest_utils/__init__.py` & `byu_pytest_utils-0.7.9/byu_pytest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.8/byu_pytest_utils/cpp_utils.py` & `byu_pytest_utils-0.7.9/byu_pytest_utils/cpp_utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.8/byu_pytest_utils/decorators.py` & `byu_pytest_utils-0.7.9/byu_pytest_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.8/byu_pytest_utils/dialog.py` & `byu_pytest_utils-0.7.9/byu_pytest_utils/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,17 +281,20 @@
         response = await _read_stream(proc.stdout, read_timeout)
 
         output.append(response)
         print(output[-1], end='')
 
     proc.stdin.close()
 
-    code = await proc.wait()
-    if code != 0:
-        error = f'the program returned a non-zero exit code: {code}'
+    try:
+        code = await asyncio.wait_for(proc.wait(), 60)  # give the program a minute to finish
+        if code != 0:
+            error = f'the program returned a non-zero exit code: {code}'
+    except TimeoutError:
+        error = 'the program failed to finish in the expected amount of time; do you have an infinite loop?'
 
     return ''.join(output), error
 
 def _run_exec(executable, *args, inputs=None, read_timeout=1):
     args = [executable, *(str(a) for a in args)]
 
     output, error = asyncio.run(_run_exec_with_io(
```

### Comparing `byu_pytest_utils-0.7.8/byu_pytest_utils/edit_dist.py` & `byu_pytest_utils-0.7.9/byu_pytest_utils/edit_dist.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.8/byu_pytest_utils/pytest_plugin.py` & `byu_pytest_utils-0.7.9/byu_pytest_utils/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.8/byu_pytest_utils/utils.py` & `byu_pytest_utils-0.7.9/byu_pytest_utils/utils.py`

 * *Files identical despite different names*

### Comparing `byu_pytest_utils-0.7.8/pyproject.toml` & `byu_pytest_utils-0.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "byu_pytest_utils"
-version = "0.7.8"
+version = "0.7.9"
 description = "A few utilities for pytest to help with integration into gradescope"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Daniel Zappala <daniel.zappala@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Framework :: Pytest"
 ]
```

### Comparing `byu_pytest_utils-0.7.8/PKG-INFO` & `byu_pytest_utils-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byu-pytest-utils
-Version: 0.7.8
+Version: 0.7.9
 Summary: A few utilities for pytest to help with integration into gradescope
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
```

