# Comparing `tmp/pulumi_cloudinit-1.5.0a1715923547.tar.gz` & `tmp/pulumi_cloudinit-1.5.0a1716566662.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_cloudinit-1.5.0a1715923547.tar", last modified: Fri May 17 05:32:11 2024, max compression
+gzip compressed data, was "pulumi_cloudinit-1.5.0a1716566662.tar", last modified: Fri May 24 16:08:04 2024, max compression
```

## Comparing `pulumi_cloudinit-1.5.0a1715923547.tar` & `pulumi_cloudinit-1.5.0a1716566662.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:11.182071 pulumi_cloudinit-1.5.0a1715923547/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 05:32:11.182071 pulumi_cloudinit-1.5.0a1715923547/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:11.182071 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:11.182071 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 05:32:11.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 05:32:11.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:32:11.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 05:32:11.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 05:32:11.000000 pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 05:32:04.000000 pulumi_cloudinit-1.5.0a1715923547/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 05:32:11.182071 pulumi_cloudinit-1.5.0a1715923547/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:08:04.011182 pulumi_cloudinit-1.5.0a1716566662/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-24 16:08:04.011182 pulumi_cloudinit-1.5.0a1716566662/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:08:04.011182 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16889 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:08:04.011182 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-24 16:08:04.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-24 16:08:04.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:08:04.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 16:08:04.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 16:08:04.000000 pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-24 16:07:57.000000 pulumi_cloudinit-1.5.0a1716566662/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:08:04.011182 pulumi_cloudinit-1.5.0a1716566662/setup.cfg
```

### Comparing `pulumi_cloudinit-1.5.0a1715923547/PKG-INFO` & `pulumi_cloudinit-1.5.0a1716566662/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1715923547
+Version: 1.5.0a1716566662
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1715923547/README.md` & `pulumi_cloudinit-1.5.0a1716566662/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/__init__.py` & `pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/_inputs.py` & `pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/_utilities.py` & `pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/config.py` & `pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/get_config.py` & `pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/outputs.py` & `pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit/provider.py` & `pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pulumi_cloudinit.egg-info/PKG-INFO` & `pulumi_cloudinit-1.5.0a1716566662/pulumi_cloudinit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudinit
-Version: 1.5.0a1715923547
+Version: 1.5.0a1716566662
 Summary: A Pulumi package for creating and managing cloudinit cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudinit
 Keywords: pulumi,cloudinit
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudinit-1.5.0a1715923547/pyproject.toml` & `pulumi_cloudinit-1.5.0a1716566662/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_cloudinit"
   description = "A Pulumi package for creating and managing cloudinit cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "cloudinit"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.5.0a1715923547"
+  version = "1.5.0a1716566662"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-cloudinit"
 
 [build-system]
```

