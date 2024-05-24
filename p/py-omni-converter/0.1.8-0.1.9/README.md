# Comparing `tmp/py-omni-converter-0.1.8.tar.gz` & `tmp/py-omni-converter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-omni-converter-0.1.8.tar", max compression
+gzip compressed data, was "py-omni-converter-0.1.9.tar", max compression
```

## Comparing `py-omni-converter-0.1.8.tar` & `py-omni-converter-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      888 2022-01-28 07:23:56.888218 py-omni-converter-0.1.8/omni_converter/__init__.py
--rw-r--r--   0        0        0        0 2021-01-20 01:35:20.000000 py-omni-converter-0.1.8/omni_converter/auto_data/__init__.py
--rw-r--r--   0        0        0     2960 2022-02-08 09:20:28.833845 py-omni-converter-0.1.8/omni_converter/auto_data/auto_v2.py
--rw-r--r--   0        0        0      117 2022-01-27 19:45:15.323554 py-omni-converter-0.1.8/omni_converter/auto_data/default_rules.py
--rw-r--r--   0        0        0      252 2021-12-12 05:33:52.203091 py-omni-converter-0.1.8/omni_converter/auto_data/format_resolution.py
--rw-r--r--   0        0        0        0 2022-01-28 07:51:48.578051 py-omni-converter-0.1.8/omni_converter/auto_data/solver.py
--rw-r--r--   0        0        0    46245 2022-01-28 07:25:51.947552 py-omni-converter-0.1.8/omni_converter/coconut/__coconut__.py
--rw-r--r--   0        0        0    36144 2022-01-27 17:51:28.449294 py-omni-converter-0.1.8/omni_converter/coconut/astar.py
--rw-r--r--   0        0        0    37461 2022-01-27 17:51:30.813249 py-omni-converter-0.1.8/omni_converter/coconut/auto_data.py
--rw-r--r--   0        0        0     5201 2022-01-27 17:48:20.843618 py-omni-converter-0.1.8/omni_converter/coconut/monad.py
--rw-r--r--   0        0        0        0 2021-12-12 03:23:52.107423 py-omni-converter-0.1.8/omni_converter/solver/__init__.py
--rw-r--r--   0        0        0     7770 2022-02-08 09:06:57.712059 py-omni-converter-0.1.8/omni_converter/solver/astar.py
--rw-r--r--   0        0        0      580 2021-12-12 04:13:53.279936 py-omni-converter-0.1.8/omni_converter/solver/heap_wrapper.py
--rw-r--r--   0        0        0     6446 2022-01-30 13:14:19.122774 py-omni-converter-0.1.8/omni_converter/solver/rules.py
--rw-r--r--   0        0        0     3149 2022-02-08 09:13:57.151822 py-omni-converter-0.1.8/omni_converter/util.py
--rw-r--r--   0        0        0      517 2022-02-08 09:25:42.167782 py-omni-converter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      734 2022-02-08 09:25:50.186160 py-omni-converter-0.1.8/setup.py
--rw-r--r--   0        0        0      554 2022-02-08 09:25:50.186352 py-omni-converter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      888 2022-01-28 07:23:56.888218 py-omni-converter-0.1.9/omni_converter/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-20 01:35:20.000000 py-omni-converter-0.1.9/omni_converter/auto_data/__init__.py
+-rw-r--r--   0        0        0     2960 2022-02-08 09:20:28.833845 py-omni-converter-0.1.9/omni_converter/auto_data/auto_v2.py
+-rw-r--r--   0        0        0      117 2022-01-27 19:45:15.323554 py-omni-converter-0.1.9/omni_converter/auto_data/default_rules.py
+-rw-r--r--   0        0        0      252 2021-12-12 05:33:52.203091 py-omni-converter-0.1.9/omni_converter/auto_data/format_resolution.py
+-rw-r--r--   0        0        0        0 2022-01-28 07:51:48.578051 py-omni-converter-0.1.9/omni_converter/auto_data/solver.py
+-rw-r--r--   0        0        0    46245 2022-01-28 07:25:51.947552 py-omni-converter-0.1.9/omni_converter/coconut/__coconut__.py
+-rw-r--r--   0        0        0    36144 2022-01-27 17:51:28.449294 py-omni-converter-0.1.9/omni_converter/coconut/astar.py
+-rw-r--r--   0        0        0    37461 2022-01-27 17:51:30.813249 py-omni-converter-0.1.9/omni_converter/coconut/auto_data.py
+-rw-r--r--   0        0        0     5201 2022-01-27 17:48:20.843618 py-omni-converter-0.1.9/omni_converter/coconut/monad.py
+-rw-r--r--   0        0        0        0 2021-12-12 03:23:52.107423 py-omni-converter-0.1.9/omni_converter/solver/__init__.py
+-rw-r--r--   0        0        0     7786 2022-02-09 07:41:05.065772 py-omni-converter-0.1.9/omni_converter/solver/astar.py
+-rw-r--r--   0        0        0      580 2021-12-12 04:13:53.279936 py-omni-converter-0.1.9/omni_converter/solver/heap_wrapper.py
+-rw-r--r--   0        0        0     6446 2022-01-30 13:14:19.122774 py-omni-converter-0.1.9/omni_converter/solver/rules.py
+-rw-r--r--   0        0        0     3149 2022-02-08 09:13:57.151822 py-omni-converter-0.1.9/omni_converter/util.py
+-rw-r--r--   0        0        0      517 2022-02-09 07:41:59.389310 py-omni-converter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      734 2022-02-09 07:42:02.969546 py-omni-converter-0.1.9/setup.py
+-rw-r--r--   0        0        0      554 2022-02-09 07:42:02.969697 py-omni-converter-0.1.9/PKG-INFO
```

### Comparing `py-omni-converter-0.1.8/omni_converter/__init__.py` & `py-omni-converter-0.1.9/omni_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/omni_converter/auto_data/auto_v2.py` & `py-omni-converter-0.1.9/omni_converter/auto_data/auto_v2.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/omni_converter/coconut/__coconut__.py` & `py-omni-converter-0.1.9/omni_converter/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/omni_converter/coconut/astar.py` & `py-omni-converter-0.1.9/omni_converter/coconut/astar.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/omni_converter/coconut/auto_data.py` & `py-omni-converter-0.1.9/omni_converter/coconut/auto_data.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/omni_converter/coconut/monad.py` & `py-omni-converter-0.1.9/omni_converter/coconut/monad.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/omni_converter/solver/astar.py` & `py-omni-converter-0.1.9/omni_converter/solver/astar.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     cache_path: str
 
     def __post_init__(self):
         self.solve_cache = DefaultShelveCache(
             self._get_edges, self.cache_path
         )
         logger.debug(f"using solver cache at {self.solve_cache.path}")
-
+        @memoize
         def memoized_solve(start, end):
             key = (start, end)
             edges = self.solve_cache[key]
             assert edges is not None
             edges = [self.solver.solve(start, end,silent=True).edges for start, end in edges]
             return Converter(list(chain(*edges)))
```

### Comparing `py-omni-converter-0.1.8/omni_converter/solver/heap_wrapper.py` & `py-omni-converter-0.1.9/omni_converter/solver/heap_wrapper.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/omni_converter/solver/rules.py` & `py-omni-converter-0.1.9/omni_converter/solver/rules.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/omni_converter/util.py` & `py-omni-converter-0.1.9/omni_converter/util.py`

 * *Files identical despite different names*

### Comparing `py-omni-converter-0.1.8/pyproject.toml` & `py-omni-converter-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-omni-converter"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Kento Masui <nameissoap@gmail.com>"]
 packages = [{include="omni_converter"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 cytoolz = "*"
```

### Comparing `py-omni-converter-0.1.8/setup.py` & `py-omni-converter-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cytoolz', 'loguru', 'lru-dict>=1.0.0,<2.0.0', 'pampy', 'tabulate', 'tqdm']
 
 setup_kwargs = {
     'name': 'py-omni-converter',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'Kento Masui',
     'author_email': 'nameissoap@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `py-omni-converter-0.1.8/PKG-INFO` & `py-omni-converter-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-omni-converter
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Kento Masui
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

