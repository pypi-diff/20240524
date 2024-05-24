# Comparing `tmp/logninja-0.1.3.tar.gz` & `tmp/logninja-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logninja-0.1.3.tar", last modified: Mon May 13 16:02:16 2024, max compression
+gzip compressed data, was "logninja-0.1.4.tar", last modified: Fri May 24 17:55:48 2024, max compression
```

## Comparing `logninja-0.1.3.tar` & `logninja-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 16:02:16.085021 logninja-0.1.3/
--rw-rw-rw-   0        0        0     1092 2024-05-11 18:30:54.000000 logninja-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      958 2024-05-13 16:02:16.082499 logninja-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       69 2024-05-11 22:42:33.000000 logninja-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 16:02:15.785781 logninja-0.1.3/logninja/
--rw-rw-rw-   0        0        0      716 2024-05-13 01:19:58.000000 logninja-0.1.3/logninja/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:02:16.022503 logninja-0.1.3/logninja/asgi/
--rw-rw-rw-   0        0        0        0 2024-05-11 22:58:24.000000 logninja-0.1.3/logninja/asgi/__init__.py
--rw-rw-rw-   0        0        0     3924 2024-05-13 01:26:33.000000 logninja-0.1.3/logninja/asgi/middleware.py
--rw-rw-rw-   0        0        0      139 2024-05-11 20:21:58.000000 logninja-0.1.3/logninja/console_formatter.py
--rw-rw-rw-   0        0        0      470 2024-05-11 23:30:27.000000 logninja-0.1.3/logninja/contextvars_filter.py
--rw-rw-rw-   0        0        0     1481 2024-05-13 01:25:36.000000 logninja-0.1.3/logninja/decorators.py
--rw-rw-rw-   0        0        0     1891 2024-05-13 01:20:22.000000 logninja-0.1.3/logninja/json_formatter.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:02:16.078505 logninja-0.1.3/logninja.egg-info/
--rw-rw-rw-   0        0        0      958 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      885 2024-05-13 15:54:33.000000 logninja-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 16:02:16.085021 logninja-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 16:02:16.066906 logninja-0.1.3/tests/
--rw-rw-rw-   0        0        0     1263 2024-05-12 21:17:02.000000 logninja-0.1.3/tests/test_json_formatter.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:55:48.512800 logninja-0.1.4/
+-rw-rw-rw-   0        0        0     1092 2024-05-11 18:30:54.000000 logninja-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      958 2024-05-24 17:55:48.508252 logninja-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2024-05-11 22:42:33.000000 logninja-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 17:55:48.394847 logninja-0.1.4/logninja/
+-rw-rw-rw-   0        0        0      716 2024-05-13 01:19:58.000000 logninja-0.1.4/logninja/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:55:48.494632 logninja-0.1.4/logninja/asgi/
+-rw-rw-rw-   0        0        0        0 2024-05-11 22:58:24.000000 logninja-0.1.4/logninja/asgi/__init__.py
+-rw-rw-rw-   0        0        0     3924 2024-05-13 01:26:33.000000 logninja-0.1.4/logninja/asgi/middleware.py
+-rw-rw-rw-   0        0        0      139 2024-05-11 20:21:58.000000 logninja-0.1.4/logninja/console_formatter.py
+-rw-rw-rw-   0        0        0      470 2024-05-11 23:30:27.000000 logninja-0.1.4/logninja/contextvars_filter.py
+-rw-rw-rw-   0        0        0     1481 2024-05-15 21:53:06.000000 logninja-0.1.4/logninja/decorators.py
+-rw-rw-rw-   0        0        0     1823 2024-05-24 17:50:31.000000 logninja-0.1.4/logninja/json_formatter.py
+-rw-rw-rw-   0        0        0     5926 2024-05-24 17:48:37.000000 logninja-0.1.4/logninja/traceback.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:55:48.503985 logninja-0.1.4/logninja.egg-info/
+-rw-rw-rw-   0        0        0      958 2024-05-24 17:55:48.000000 logninja-0.1.4/logninja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-05-24 17:55:48.000000 logninja-0.1.4/logninja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 17:55:48.000000 logninja-0.1.4/logninja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-24 17:55:48.000000 logninja-0.1.4/logninja.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 17:55:48.000000 logninja-0.1.4/logninja.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      885 2024-05-24 17:52:38.000000 logninja-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 17:55:48.513842 logninja-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 17:55:48.498739 logninja-0.1.4/tests/
+-rw-rw-rw-   0        0        0     1263 2024-05-12 21:17:02.000000 logninja-0.1.4/tests/test_json_formatter.py
```

### Comparing `logninja-0.1.3/LICENSE` & `logninja-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logninja-0.1.3/PKG-INFO` & `logninja-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logninja
-Version: 0.1.3
+Version: 0.1.4
 Summary: A log configuration library for Python projects.
 Author-email: Pedro Cantidio <ppcantidio@gmail.com>
 Project-URL: homepage, https://github.com/ppcantidio/logninja.py
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logninja-0.1.3/logninja/__init__.py` & `logninja-0.1.4/logninja/__init__.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.3/logninja/asgi/middleware.py` & `logninja-0.1.4/logninja/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.3/logninja/decorators.py` & `logninja-0.1.4/logninja/decorators.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.3/logninja/json_formatter.py` & `logninja-0.1.4/logninja/json_formatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime as dt
 import json
 import logging
 
+from logninja.traceback import format_exception
+
 LOG_RECORD_BUILTIN_ATTRS = {
     "args",
     "asctime",
     "created",
     "exc_info",
     "exc_text",
     "filename",
@@ -49,18 +51,15 @@
         always_fields = {
             "message": record.getMessage(),
             "timestamp": dt.datetime.fromtimestamp(
                 record.created, tz=dt.timezone.utc
             ).isoformat(),
         }
         if record.exc_info is not None:
-            always_fields["exc_info"] = self.formatException(record.exc_info)
-
-        if record.stack_info is not None:
-            always_fields["stack_info"] = self.formatStack(record.stack_info)
+            always_fields["exc_info"] = format_exception(exc_info=record.exc_info)
 
         message = {
             key: (
                 msg_val
                 if (msg_val := always_fields.pop(val, None)) is not None
                 else getattr(record, val)
             )
```

### Comparing `logninja-0.1.3/logninja.egg-info/PKG-INFO` & `logninja-0.1.4/logninja.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logninja
-Version: 0.1.3
+Version: 0.1.4
 Summary: A log configuration library for Python projects.
 Author-email: Pedro Cantidio <ppcantidio@gmail.com>
 Project-URL: homepage, https://github.com/ppcantidio/logninja.py
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `logninja-0.1.3/pyproject.toml` & `logninja-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "logninja"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Pedro Cantidio", email = "ppcantidio@gmail.com" }]
 description = "A log configuration library for Python projects."
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `logninja-0.1.3/tests/test_json_formatter.py` & `logninja-0.1.4/tests/test_json_formatter.py`

 * *Files identical despite different names*

