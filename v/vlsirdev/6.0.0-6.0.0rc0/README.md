# Comparing `tmp/vlsirdev-6.0.0.tar.gz` & `tmp/vlsirdev-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlsirdev-6.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vlsirdev-6.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vlsirdev-6.0.0.tar` & `vlsirdev-6.0.0rc0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-lrwxr-xr-x   0        0        0        0 2024-05-24 16:40:53.627980 vlsirdev-6.0.0/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0      982 2024-05-24 17:12:12.303027 vlsirdev-6.0.0/pyproject.toml
--rw-r--r--   0        0        0      161 2024-05-24 16:40:20.434027 vlsirdev-6.0.0/readme.md
--rw-r--r--   0        0        0      209 2024-05-24 17:12:12.303235 vlsirdev-6.0.0/vlsirdev/__init__.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 vlsirdev-6.0.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2024-05-24 16:40:53.627980 vlsirdev-6.0.0rc0/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0      985 2024-05-24 16:53:53.677900 vlsirdev-6.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      161 2024-05-24 16:40:20.434027 vlsirdev-6.0.0rc0/readme.md
+-rw-r--r--   0        0        0      212 2024-05-24 16:40:25.407139 vlsirdev-6.0.0rc0/vlsirdev/__init__.py
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 vlsirdev-6.0.0rc0/PKG-INFO
```

### Comparing `vlsirdev-6.0.0/pyproject.toml` & `vlsirdev-6.0.0rc0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "vlsirdev"
 description = "VLSIR Development Dependencies"
-version = "6.0.0" # VLSIR_VERSION
+version = "6.0.0rc0" # VLSIR_VERSION
 dependencies = [ # <= This right here is the whole point of this package!
     "pytest==7.1",
     "coverage",
     "pytest-cov",
     "pre-commit==2.20",
     "black==22.6",
     "flit",
```

### Comparing `vlsirdev-6.0.0/PKG-INFO` & `vlsirdev-6.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlsirdev
-Version: 6.0.0
+Version: 6.0.0rc0
 Summary: VLSIR Development Dependencies
 Keywords: PDK,EDA,analog,circuit
 Author-email: Dan Fritchman <dan@fritch.mn>
 Maintainer-email: Dan Fritchman <dan@fritch.mn>
 Requires-Python: >=3.7, <3.13
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
```

