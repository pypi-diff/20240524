# Comparing `tmp/python_texttools-0.0.1.tar.gz` & `tmp/python_texttools-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_texttools-0.0.1.tar", max compression
+gzip compressed data, was "python_texttools-0.0.1.1.tar", max compression
```

## Comparing `python_texttools-0.0.1.tar` & `python_texttools-0.0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_texttools-0.0.1/LICENSE
--rw-r--r--   0        0        0     1148 2024-05-22 10:03:11.553964 python_texttools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      199 2024-05-02 13:51:59.825054 python_texttools-0.0.1/readme.md
--rwxr-xr-x   0        0        0      197 2024-05-22 07:48:04.697979 python_texttools-0.0.1/texttools/__init__.py
--rwxr-xr-x   0        0        0      519 2024-05-22 06:48:18.392958 python_texttools-0.0.1/texttools/half_width.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_texttools-0.0.1/texttools/py.typed
--rwxr-xr-x   0        0        0     5204 2024-05-22 09:57:51.258564 python_texttools-0.0.1/texttools/text.py
--rwxr-xr-x   0        0        0    15696 2024-05-22 10:02:17.818133 python_texttools-0.0.1/texttools/text_find.py
--rw-r--r--   0        0        0     1327 1970-01-01 00:00:00.000000 python_texttools-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_texttools-0.0.1.1/LICENSE
+-rw-r--r--   0        0        0     1150 2024-05-24 17:02:20.951091 python_texttools-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-05-02 13:51:59.825054 python_texttools-0.0.1.1/readme.md
+-rwxr-xr-x   0        0        0      197 2024-05-22 07:48:04.697979 python_texttools-0.0.1.1/texttools/__init__.py
+-rwxr-xr-x   0        0        0      519 2024-05-22 06:48:18.392958 python_texttools-0.0.1.1/texttools/half_width.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_texttools-0.0.1.1/texttools/py.typed
+-rwxr-xr-x   0        0        0     5204 2024-05-22 09:57:51.258564 python_texttools-0.0.1.1/texttools/text.py
+-rwxr-xr-x   0        0        0    15696 2024-05-22 10:02:17.818133 python_texttools-0.0.1.1/texttools/text_find.py
+-rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 python_texttools-0.0.1.1/PKG-INFO
```

### Comparing `python_texttools-0.0.1/LICENSE` & `python_texttools-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_texttools-0.0.1/pyproject.toml` & `python_texttools-0.0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-texttools"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "Python texttools."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-texttools"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-texttools"
 keywords = ["http", "response"]
```

### Comparing `python_texttools-0.0.1/texttools/half_width.py` & `python_texttools-0.0.1.1/texttools/half_width.py`

 * *Files identical despite different names*

### Comparing `python_texttools-0.0.1/texttools/text.py` & `python_texttools-0.0.1.1/texttools/text.py`

 * *Files identical despite different names*

### Comparing `python_texttools-0.0.1/texttools/text_find.py` & `python_texttools-0.0.1.1/texttools/text_find.py`

 * *Files identical despite different names*

### Comparing `python_texttools-0.0.1/PKG-INFO` & `python_texttools-0.0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-texttools
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Python texttools.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-texttools
 License: MIT
 Keywords: http,response
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

