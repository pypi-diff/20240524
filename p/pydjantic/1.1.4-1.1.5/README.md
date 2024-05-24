# Comparing `tmp/pydjantic-1.1.4.tar.gz` & `tmp/pydjantic-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydjantic-1.1.4.tar", max compression
+gzip compressed data, was "pydjantic-1.1.5.tar", max compression
```

## Comparing `pydjantic-1.1.4.tar` & `pydjantic-1.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-01-01 16:42:00.891601 pydjantic-1.1.4/LICENSE
--rw-r--r--   0        0        0     5063 2024-01-01 16:42:00.891601 pydjantic-1.1.4/README.md
--rw-r--r--   0        0        0       97 2024-01-01 16:42:00.895601 pydjantic-1.1.4/pydjantic/__init__.py
--rw-r--r--   0        0        0        0 2024-01-01 16:42:00.895601 pydjantic-1.1.4/pydjantic/py.typed
--rw-r--r--   0        0        0     2227 2024-01-01 16:42:00.895601 pydjantic-1.1.4/pydjantic/pydjantic.py
--rw-r--r--   0        0        0     1006 2024-01-01 16:42:00.895601 pydjantic-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     6212 1970-01-01 00:00:00.000000 pydjantic-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-24 20:19:16.198737 pydjantic-1.1.5/LICENSE
+-rw-r--r--   0        0        0     5063 2024-05-24 20:19:16.202737 pydjantic-1.1.5/README.md
+-rw-r--r--   0        0        0       97 2024-05-24 20:19:16.202737 pydjantic-1.1.5/pydjantic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:19:16.202737 pydjantic-1.1.5/pydjantic/py.typed
+-rw-r--r--   0        0        0     2227 2024-05-24 20:19:16.202737 pydjantic-1.1.5/pydjantic/pydjantic.py
+-rw-r--r--   0        0        0     1006 2024-05-24 20:19:16.202737 pydjantic-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6212 1970-01-01 00:00:00.000000 pydjantic-1.1.5/PKG-INFO
```

### Comparing `pydjantic-1.1.4/LICENSE` & `pydjantic-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydjantic-1.1.4/README.md` & `pydjantic-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pydjantic-1.1.4/pydjantic/pydjantic.py` & `pydjantic-1.1.5/pydjantic/pydjantic.py`

 * *Files identical despite different names*

### Comparing `pydjantic-1.1.4/pyproject.toml` & `pydjantic-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydjantic"
-version = "1.1.4"
+version = "1.1.5"
 description = "Pydantic Settings for Django"
 authors = ["Vladimir Vyazovetskov <erhosen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErhoSen/pydjantic"
 repository = "https://github.com/ErhoSen/pydjantic"
 keywords = ["pydantic", "django", "PydanticSettings", "settings"]
```

### Comparing `pydjantic-1.1.4/PKG-INFO` & `pydjantic-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydjantic
-Version: 1.1.4
+Version: 1.1.5
 Summary: Pydantic Settings for Django
 Home-page: https://github.com/ErhoSen/pydjantic
 License: MIT
 Keywords: pydantic,django,PydanticSettings,settings
 Author: Vladimir Vyazovetskov
 Author-email: erhosen@gmail.com
 Requires-Python: >=3.8,<4.0
```

