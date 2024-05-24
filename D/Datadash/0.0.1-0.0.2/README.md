# Comparing `tmp/datadash-0.0.1.tar.gz` & `tmp/datadash-0.0.2.tar.gz`

## Comparing `datadash-0.0.1.tar` & `datadash-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datadash-0.0.1/src/datadash/__init__.py
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 datadash-0.0.1/src/datadash/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 datadash-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 datadash-0.0.1/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 datadash-0.0.1/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 datadash-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 datadash-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 datadash-0.0.2/src/datadash/__init__.py
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 datadash-0.0.2/src/datadash/__main__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 datadash-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 datadash-0.0.2/LICENSE
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 datadash-0.0.2/README.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 datadash-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 datadash-0.0.2/PKG-INFO
```

### Comparing `datadash-0.0.1/src/datadash/main.py` & `datadash-0.0.2/src/datadash/__main__.py`

 * *Files identical despite different names*

### Comparing `datadash-0.0.1/.gitignore` & `datadash-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `datadash-0.0.1/LICENSE` & `datadash-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datadash-0.0.1/pyproject.toml` & `datadash-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Datadash"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Taking a quick look at data."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `datadash-0.0.1/PKG-INFO` & `datadash-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Datadash
-Version: 0.0.1
+Version: 0.0.2
 Summary: Taking a quick look at data.
 Project-URL: Homepage, https://github.com/galenseilis/datadash
 Project-URL: Issues, https://github.com/galenseilis/datadash/issues
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

