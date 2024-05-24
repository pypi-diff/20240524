# Comparing `tmp/aggregate_root-0.0.2.tar.gz` & `tmp/aggregate_root-0.0.3.tar.gz`

## Comparing `aggregate_root-0.0.2.tar` & `aggregate_root-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aggregate_root-0.0.2/src/aggregate_root/__init__.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 aggregate_root-0.0.2/src/aggregate_root/aggregate_root.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 aggregate_root-0.0.2/src/aggregate_root/domain_event.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aggregate_root-0.0.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 aggregate_root-0.0.2/LICENSE
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aggregate_root-0.0.2/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 aggregate_root-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 aggregate_root-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/src/aggregate_root/__init__.py
+-rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/src/aggregate_root/aggregate_root.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/src/aggregate_root/domain_event.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/tests/test_aggregate_root.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/tests/test_domain_event.py
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/tests/test_sample.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/LICENSE
+-rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 aggregate_root-0.0.3/PKG-INFO
```

### Comparing `aggregate_root-0.0.2/LICENSE` & `aggregate_root-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aggregate_root-0.0.2/pyproject.toml` & `aggregate_root-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aggregate-root"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jeremy Willemse", email="jeremy@willemse.co" },
 ]
 description = "A small Python library for defining domain-driven design aggregates and domain events."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -17,7 +17,15 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
 ]
 
 [project.urls]
 Homepage = "https://github.com/willemse-and-co/aggregate-root"
 Issues = "https://github.com/willemse-and-co/aggregate-root/issues"
+
+[tool.hatch.envs.default]
+dependencies = [
+  "pytest>=8.2.1"
+]
+
+[tool.hatch.envs.default.env-vars]
+PYTHONPATH = "src"
```

