# Comparing `tmp/pulumi_archive-0.1.0a1715922700.tar.gz` & `tmp/pulumi_archive-0.1.0a1716504266.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_archive-0.1.0a1715922700.tar", last modified: Fri May 17 05:15:53 2024, max compression
+gzip compressed data, was "pulumi_archive-0.1.0a1716504266.tar", last modified: Thu May 23 23:02:26 2024, max compression
```

## Comparing `pulumi_archive-0.1.0a1715922700.tar` & `pulumi_archive-0.1.0a1716504266.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:15:53.601922 pulumi_archive-0.1.0a1715922700/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-17 05:15:53.601922 pulumi_archive-0.1.0a1715922700/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:15:53.597922 pulumi_archive-0.1.0a1715922700/pulumi_archive/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    40277 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    17891 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:15:53.601922 pulumi_archive-0.1.0a1715922700/pulumi_archive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-17 05:15:53.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-17 05:15:53.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:15:53.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 05:15:53.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 05:15:53.000000 pulumi_archive-0.1.0a1715922700/pulumi_archive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 05:15:44.000000 pulumi_archive-0.1.0a1715922700/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 05:15:53.601922 pulumi_archive-0.1.0a1715922700/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:02:26.538718 pulumi_archive-0.1.0a1716504266/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-23 23:02:26.538718 pulumi_archive-0.1.0a1716504266/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:02:26.538718 pulumi_archive-0.1.0a1716504266/pulumi_archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40277 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17891 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:02:26.538718 pulumi_archive-0.1.0a1716504266/pulumi_archive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-23 23:02:26.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 23:02:26.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:02:26.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 23:02:26.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 23:02:26.000000 pulumi_archive-0.1.0a1716504266/pulumi_archive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-23 23:02:19.000000 pulumi_archive-0.1.0a1716504266/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 23:02:26.538718 pulumi_archive-0.1.0a1716504266/setup.cfg
```

### Comparing `pulumi_archive-0.1.0a1715922700/PKG-INFO` & `pulumi_archive-0.1.0a1716504266/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_archive
-Version: 0.1.0a1715922700
+Version: 0.1.0a1716504266
 Summary: A Pulumi package for creating and managing Archive cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-archive
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_archive-0.1.0a1715922700/README.md` & `pulumi_archive-0.1.0a1716504266/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.1.0a1715922700/pulumi_archive/__init__.py` & `pulumi_archive-0.1.0a1716504266/pulumi_archive/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.1.0a1715922700/pulumi_archive/_inputs.py` & `pulumi_archive-0.1.0a1716504266/pulumi_archive/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.1.0a1715922700/pulumi_archive/_utilities.py` & `pulumi_archive-0.1.0a1716504266/pulumi_archive/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.1.0a1715922700/pulumi_archive/file.py` & `pulumi_archive-0.1.0a1716504266/pulumi_archive/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.1.0a1715922700/pulumi_archive/get_file.py` & `pulumi_archive-0.1.0a1716504266/pulumi_archive/get_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.1.0a1715922700/pulumi_archive/outputs.py` & `pulumi_archive-0.1.0a1716504266/pulumi_archive/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.1.0a1715922700/pulumi_archive/provider.py` & `pulumi_archive-0.1.0a1716504266/pulumi_archive/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_archive-0.1.0a1715922700/pulumi_archive.egg-info/PKG-INFO` & `pulumi_archive-0.1.0a1716504266/pulumi_archive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_archive
-Version: 0.1.0a1715922700
+Version: 0.1.0a1716504266
 Summary: A Pulumi package for creating and managing Archive cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-archive
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_archive-0.1.0a1715922700/pyproject.toml` & `pulumi_archive-0.1.0a1716504266/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_archive"
   description = "A Pulumi package for creating and managing Archive cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.0a1715922700"
+  version = "0.1.0a1716504266"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com/"
     Repository = "https://github.com/pulumi/pulumi-archive"
 
 [build-system]
```

