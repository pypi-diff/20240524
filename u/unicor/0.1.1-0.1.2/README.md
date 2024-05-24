# Comparing `tmp/unicor-0.1.1.tar.gz` & `tmp/unicor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicor-0.1.1.tar", last modified: Fri May 24 13:54:46 2024, max compression
+gzip compressed data, was "unicor-0.1.2.tar", last modified: Fri May 24 14:05:55 2024, max compression
```

## Comparing `unicor-0.1.1.tar` & `unicor-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 13:54:46.121137 unicor-0.1.1/
--rw-rw-rw-   0        0        0     1083 2024-05-24 07:23:07.000000 unicor-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1213 2024-05-24 13:54:46.119142 unicor-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      628 2024-05-24 07:37:53.000000 unicor-0.1.1/README.md
--rw-rw-rw-   0        0        0      663 2024-05-24 13:49:51.000000 unicor-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-24 13:54:46.122135 unicor-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-24 13:54:46.060140 unicor-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-24 13:54:46.116135 unicor-0.1.1/src/UniCor.egg-info/
--rw-rw-rw-   0        0        0     1213 2024-05-24 13:54:46.000000 unicor-0.1.1/src/UniCor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-05-24 13:54:46.000000 unicor-0.1.1/src/UniCor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 13:54:46.000000 unicor-0.1.1/src/UniCor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-24 13:54:46.000000 unicor-0.1.1/src/UniCor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-24 13:54:46.099135 unicor-0.1.1/src/unicor/
--rw-rw-rw-   0        0        0        2 2024-05-24 13:49:23.000000 unicor-0.1.1/src/unicor/__init__.py
--rw-rw-rw-   0        0        0     2800 2024-05-24 12:20:03.000000 unicor-0.1.1/src/unicor/unicor_metric.py
--rw-rw-rw-   0        0        0    10655 2024-05-24 12:19:52.000000 unicor-0.1.1/src/unicor/unicorp.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:05:55.551684 unicor-0.1.2/
+-rw-rw-rw-   0        0        0     1083 2024-05-24 07:23:07.000000 unicor-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1213 2024-05-24 14:05:55.549687 unicor-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2024-05-24 07:37:53.000000 unicor-0.1.2/README.md
+-rw-rw-rw-   0        0        0      663 2024-05-24 14:05:25.000000 unicor-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 14:05:55.551684 unicor-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 14:05:55.450832 unicor-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 14:05:55.547685 unicor-0.1.2/src/UniCor.egg-info/
+-rw-rw-rw-   0        0        0     1213 2024-05-24 14:05:55.000000 unicor-0.1.2/src/UniCor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-05-24 14:05:55.000000 unicor-0.1.2/src/UniCor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 14:05:55.000000 unicor-0.1.2/src/UniCor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 14:05:55.000000 unicor-0.1.2/src/UniCor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 14:05:55.530702 unicor-0.1.2/src/unicor/
+-rw-rw-rw-   0        0        0       72 2024-05-24 14:05:05.000000 unicor-0.1.2/src/unicor/__init__.py
+-rw-rw-rw-   0        0        0     2800 2024-05-24 12:20:03.000000 unicor-0.1.2/src/unicor/unicor_metric.py
+-rw-rw-rw-   0        0        0    10655 2024-05-24 12:19:52.000000 unicor-0.1.2/src/unicor/unicorp.py
```

### Comparing `unicor-0.1.1/LICENSE` & `unicor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unicor-0.1.1/PKG-INFO` & `unicor-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Hierarchical Feature Selection through Propagation of Uniquely Correlated Entities
 Author-email: Sebastian Staab <sebastian.staab@uni-konstanz.de>
 Project-URL: Homepage, https://github.com/SebastianStaab/UniCor
 Project-URL: Issues, https://github.com/SebastianStaab/UniCor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unicor-0.1.1/README.md` & `unicor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `unicor-0.1.1/pyproject.toml` & `unicor-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unicor"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Sebastian Staab", email="sebastian.staab@uni-konstanz.de" },
 ]
 description = "Hierarchical Feature Selection through Propagation of Uniquely Correlated Entities"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `unicor-0.1.1/src/UniCor.egg-info/PKG-INFO` & `unicor-0.1.2/src/UniCor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Hierarchical Feature Selection through Propagation of Uniquely Correlated Entities
 Author-email: Sebastian Staab <sebastian.staab@uni-konstanz.de>
 Project-URL: Homepage, https://github.com/SebastianStaab/UniCor
 Project-URL: Issues, https://github.com/SebastianStaab/UniCor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unicor-0.1.1/src/unicor/unicor_metric.py` & `unicor-0.1.2/src/unicor/unicor_metric.py`

 * *Files identical despite different names*

### Comparing `unicor-0.1.1/src/unicor/unicorp.py` & `unicor-0.1.2/src/unicor/unicorp.py`

 * *Files identical despite different names*

