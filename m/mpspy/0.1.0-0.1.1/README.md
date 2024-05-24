# Comparing `tmp/mpspy-0.1.0.tar.gz` & `tmp/mpspy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpspy-0.1.0.tar", max compression
+gzip compressed data, was "mpspy-0.1.1.tar", max compression
```

## Comparing `mpspy-0.1.0.tar` & `mpspy-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-05-24 13:37:53.275509 mpspy-0.1.0/LICENSE
--rw-r--r--   0        0        0      423 2024-05-24 13:37:53.275509 mpspy-0.1.0/README.md
--rw-r--r--   0        0        0      129 2024-05-24 13:37:53.275509 mpspy-0.1.0/mpspy/__init__.py
--rw-r--r--   0        0        0       52 2024-05-24 13:37:53.278843 mpspy-0.1.0/mpspy/log.py
--rw-r--r--   0        0        0    11757 2024-05-24 13:37:53.282176 mpspy-0.1.0/mpspy/reader.py
--rw-r--r--   0        0        0      387 2024-05-24 13:37:53.278843 mpspy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mpspy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 13:59:42.927204 mpspy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      423 2024-05-24 13:59:42.927204 mpspy-0.1.1/README.md
+-rw-r--r--   0        0        0      129 2024-05-24 13:59:42.927204 mpspy-0.1.1/mpspy/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-24 13:59:42.927204 mpspy-0.1.1/mpspy/log.py
+-rw-r--r--   0        0        0    11757 2024-05-24 13:59:42.927204 mpspy-0.1.1/mpspy/reader.py
+-rw-r--r--   0        0        0      387 2024-05-24 13:59:42.927204 mpspy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mpspy-0.1.1/PKG-INFO
```

### Comparing `mpspy-0.1.0/LICENSE` & `mpspy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mpspy-0.1.0/mpspy/reader.py` & `mpspy-0.1.1/mpspy/reader.py`

 * *Files identical despite different names*

### Comparing `mpspy-0.1.0/PKG-INFO` & `mpspy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpspy
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
```

