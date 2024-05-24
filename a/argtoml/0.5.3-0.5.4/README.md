# Comparing `tmp/argtoml-0.5.3.tar.gz` & `tmp/argtoml-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argtoml-0.5.3.tar", last modified: Thu May 23 12:53:54 2024, max compression
+gzip compressed data, was "argtoml-0.5.4.tar", last modified: Thu May 23 13:14:11 2024, max compression
```

## Comparing `argtoml-0.5.3.tar` & `argtoml-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 12:53:54.518287 argtoml-0.5.3/
--rw-r--r--   0 jo3       (1000) jo3       (1000)     1069 2023-07-23 14:09:52.000000 argtoml-0.5.3/LICENSE
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-23 12:53:54.518287 argtoml-0.5.3/PKG-INFO
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3218 2024-01-02 10:21:38.000000 argtoml-0.5.3/README.md
-drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 12:53:54.518287 argtoml-0.5.3/argtoml/
--rw-r--r--   0 jo3       (1000) jo3       (1000)       57 2024-02-13 08:37:22.000000 argtoml-0.5.3/argtoml/__init__.py
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3240 2024-05-07 09:23:38.000000 argtoml-0.5.3/argtoml/__main__.py
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3121 2024-05-07 11:35:09.000000 argtoml-0.5.3/argtoml/locate.py
--rw-r--r--   0 jo3       (1000) jo3       (1000)    10953 2024-02-13 08:37:22.000000 argtoml-0.5.3/argtoml/main.py
--rw-r--r--   0 jo3       (1000) jo3       (1000)     5467 2024-05-23 12:52:06.000000 argtoml-0.5.3/argtoml/opt.py
-drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 12:53:54.518287 argtoml-0.5.3/argtoml.egg-info/
--rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-23 12:53:54.000000 argtoml-0.5.3/argtoml.egg-info/PKG-INFO
--rw-r--r--   0 jo3       (1000) jo3       (1000)      273 2024-05-23 12:53:54.000000 argtoml-0.5.3/argtoml.egg-info/SOURCES.txt
--rw-r--r--   0 jo3       (1000) jo3       (1000)        1 2024-05-23 12:53:54.000000 argtoml-0.5.3/argtoml.egg-info/dependency_links.txt
--rw-r--r--   0 jo3       (1000) jo3       (1000)        8 2024-05-23 12:53:54.000000 argtoml-0.5.3/argtoml.egg-info/top_level.txt
--rw-r--r--   0 jo3       (1000) jo3       (1000)      951 2024-05-23 12:53:20.000000 argtoml-0.5.3/pyproject.toml
--rw-r--r--   0 jo3       (1000) jo3       (1000)       38 2024-05-23 12:53:54.518287 argtoml-0.5.3/setup.cfg
--rw-r--r--   0 jo3       (1000) jo3       (1000)       61 2023-07-23 14:09:52.000000 argtoml-0.5.3/setup.py
-drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 12:53:54.518287 argtoml-0.5.3/tests/
--rw-r--r--   0 jo3       (1000) jo3       (1000)      218 2023-07-23 14:09:52.000000 argtoml-0.5.3/tests/test_main.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 13:14:11.986836 argtoml-0.5.4/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1069 2023-07-23 14:09:52.000000 argtoml-0.5.4/LICENSE
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-23 13:14:11.986836 argtoml-0.5.4/PKG-INFO
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3218 2024-01-02 10:21:38.000000 argtoml-0.5.4/README.md
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 13:14:11.983503 argtoml-0.5.4/argtoml/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       57 2024-02-13 08:37:22.000000 argtoml-0.5.4/argtoml/__init__.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3240 2024-05-07 09:23:38.000000 argtoml-0.5.4/argtoml/__main__.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3121 2024-05-07 11:35:09.000000 argtoml-0.5.4/argtoml/locate.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)    10953 2024-02-13 08:37:22.000000 argtoml-0.5.4/argtoml/main.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     5476 2024-05-23 13:13:04.000000 argtoml-0.5.4/argtoml/opt.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 13:14:11.986836 argtoml-0.5.4/argtoml.egg-info/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3731 2024-05-23 13:14:11.000000 argtoml-0.5.4/argtoml.egg-info/PKG-INFO
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      273 2024-05-23 13:14:11.000000 argtoml-0.5.4/argtoml.egg-info/SOURCES.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)        1 2024-05-23 13:14:11.000000 argtoml-0.5.4/argtoml.egg-info/dependency_links.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)        8 2024-05-23 13:14:11.000000 argtoml-0.5.4/argtoml.egg-info/top_level.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      951 2024-05-23 13:13:24.000000 argtoml-0.5.4/pyproject.toml
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       38 2024-05-23 13:14:11.986836 argtoml-0.5.4/setup.cfg
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       61 2023-07-23 14:09:52.000000 argtoml-0.5.4/setup.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-05-23 13:14:11.983503 argtoml-0.5.4/tests/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      218 2023-07-23 14:09:52.000000 argtoml-0.5.4/tests/test_main.py
```

### Comparing `argtoml-0.5.3/LICENSE` & `argtoml-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.3/PKG-INFO` & `argtoml-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.5.3
+Version: 0.5.4
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.5.3/README.md` & `argtoml-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.3/argtoml/__main__.py` & `argtoml-0.5.4/argtoml/__main__.py`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.3/argtoml/locate.py` & `argtoml-0.5.4/argtoml/locate.py`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.3/argtoml/main.py` & `argtoml-0.5.4/argtoml/main.py`

 * *Files identical despite different names*

### Comparing `argtoml-0.5.3/argtoml/opt.py` & `argtoml-0.5.4/argtoml/opt.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,19 +54,19 @@
     new = copy.deepcopy(old)
 
     for k, v in iter_opt(add):
         if type(v) is str and path is not None:
             v = string_to_path(v, path)
 
         if k in old:
-            # Check whether identical keys have values of the same type.
-            if type(old[k]) is not type(v):
+            # We treat Paths and strings as the same type.
+            if type(old[k]) is not type(v) and not (isinstance(v, Path) and type(old[k]) is str):
                 raise TypeError(
-                    f"{k} is originally {old[k]} of type {type(old[k])},"
-                    + f"but is to become {v} of type {type(v)}."
+                    f"{k} is originally '{old[k]}' of type {type(old[k])},"
+                    + f"but is to become '{v}' of type {type(v)}."
                 )
             old_v = old[k]
         else:
             old_v = {}
 
         if isinstance(v, get_args(Opt)):
             new[k] = merge_opts(old_v, v, path)  #type:ignore
@@ -130,18 +130,17 @@
     if len(keys) == 1:
         if value is not None:
             if isinstance(reference[key], Path) and type(value) is str:
                 value = string_to_path(value, Path('.'))
             elif type(reference[key]) is not type(value):
                 old_value = reference[key]
                 raise TypeError(
-                    f"{key} is originally {old_value} of type {type(old_value)},"
-                    + f" but is to become {value} of type {type(value)}."
+                    f"{key} is originally '{old_value}' of type {type(old_value)},"
+                    + f" but is to become '{value}' of type {type(value)}."
                 )
-            print(key, reference[key])
             del reference[key]
             opt[key] = value
         else:
             return opt[key]
     else:
         if key not in reference and value is not None:
             raise KeyError(f"{key} is being edited twice.")
```

### Comparing `argtoml-0.5.3/argtoml.egg-info/PKG-INFO` & `argtoml-0.5.4/argtoml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argtoml
-Version: 0.5.3
+Version: 0.5.4
 Summary: Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file.
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/argtoml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `argtoml-0.5.3/pyproject.toml` & `argtoml-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "argtoml"
-version = "0.5.3"
+version = "0.5.4"
 description = "Add the keys from a .toml file to your CLI as arguments. Their values default to the values in the .toml file."
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

