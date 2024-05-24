# Comparing `tmp/types-python-crontab-3.0.0.20240417.tar.gz` & `tmp/types-python-crontab-3.1.0.20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-crontab-3.0.0.20240417.tar", last modified: Wed Apr 17 02:16:58 2024, max compression
+gzip compressed data, was "types-python-crontab-3.1.0.20240524.tar", last modified: Fri May 24 02:22:35 2024, max compression
```

## Comparing `types-python-crontab-3.0.0.20240417.tar` & `types-python-crontab-3.1.0.20240524.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.733122 types-python-crontab-3.0.0.20240417/
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/cronlog-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/cronlog-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/cronlog-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/cronlog-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/crontab-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontab-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontab-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontab-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/crontabs-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontabs-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontabs-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontabs-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:16:58.733122 types-python-crontab-3.0.0.20240417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:35.046668 types-python-crontab-3.1.0.20240524/
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-24 02:22:35.046668 types-python-crontab-3.1.0.20240524/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:35.042668 types-python-crontab-3.1.0.20240524/cronlog-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/cronlog-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/cronlog-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/cronlog-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:35.046668 types-python-crontab-3.1.0.20240524/crontab-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/crontab-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/crontab-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/crontab-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:35.046668 types-python-crontab-3.1.0.20240524/crontabs-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/crontabs-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/crontabs-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/crontabs-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 02:22:35.046668 types-python-crontab-3.1.0.20240524/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-24 02:22:34.000000 types-python-crontab-3.1.0.20240524/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:22:35.046668 types-python-crontab-3.1.0.20240524/types_python_crontab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-24 02:22:35.000000 types-python-crontab-3.1.0.20240524/types_python_crontab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-24 02:22:35.000000 types-python-crontab-3.1.0.20240524/types_python_crontab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:22:35.000000 types-python-crontab-3.1.0.20240524/types_python_crontab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 02:22:35.000000 types-python-crontab-3.1.0.20240524/types_python_crontab.egg-info/top_level.txt
```

### Comparing `types-python-crontab-3.0.0.20240417/CHANGELOG.md` & `types-python-crontab-3.1.0.20240524/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.1.0.20240524 (2024-05-24)
+
+Bump python-crontab to 3.1.* (#12008)
+
 ## 3.0.0.20240417 (2024-04-17)
 
 Remove remaining bare `Incomplete`s (#11768)
 
 Enable Y065
 
 ## 3.0.0.20240106 (2024-01-06)
```

### Comparing `types-python-crontab-3.0.0.20240417/PKG-INFO` & `types-python-crontab-3.1.0.20240524/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-crontab
-Version: 3.0.0.20240417
+Version: 3.1.0.20240524
 Summary: Typing stubs for python-crontab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`.
 
 This version of `types-python-crontab` aims to provide accurate annotations
-for `python-crontab==3.0.*`.
+for `python-crontab==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `ac6c61ba04c3d3abf476570de04a9afe7447890b` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
```

### Comparing `types-python-crontab-3.0.0.20240417/cronlog-stubs/__init__.pyi` & `types-python-crontab-3.1.0.20240524/cronlog-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-3.0.0.20240417/crontab-stubs/__init__.pyi` & `types-python-crontab-3.1.0.20240524/crontab-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -255,14 +255,15 @@
     @property
     def also(self) -> Also: ...
     def clear(self) -> None: ...
     def get_range(self, *vrange: int | str | CronValue) -> list[int | CronRange]: ...
     def __iter__(self) -> Iterator[int]: ...
     def __len__(self) -> int: ...
     def parse_value(self, val: str, sunday: int | None = ...) -> int | CronValue: ...
+    def test_value(self, value: str, sunday: int | None = None) -> str: ...
 
 def get_cronvalue(value: int, enums: list[str]) -> int | CronValue: ...
 
 class CronValue:
     text: str
     value: int
     def __init__(self, value: str, enums: list[str]) -> None: ...
```

### Comparing `types-python-crontab-3.0.0.20240417/crontabs-stubs/__init__.pyi` & `types-python-crontab-3.1.0.20240524/crontabs-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-3.0.0.20240417/setup.py` & `types-python-crontab-3.1.0.20240524/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`.
 
 This version of `types-python-crontab` aims to provide accurate annotations
-for `python-crontab==3.0.*`.
+for `python-crontab==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `ac6c61ba04c3d3abf476570de04a9afe7447890b` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.20240417",
+      version="3.1.0.20240524",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md",
```

### Comparing `types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/PKG-INFO` & `types-python-crontab-3.1.0.20240524/types_python_crontab.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-crontab
-Version: 3.0.0.20240417
+Version: 3.1.0.20240524
 Summary: Typing stubs for python-crontab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-crontab`.
 
 This version of `types-python-crontab` aims to provide accurate annotations
-for `python-crontab==3.0.*`.
+for `python-crontab==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `ac6c61ba04c3d3abf476570de04a9afe7447890b` and was tested
+with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
```

