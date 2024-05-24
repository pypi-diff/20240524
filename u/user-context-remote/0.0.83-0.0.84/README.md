# Comparing `tmp/user_context_remote-0.0.83.tar.gz` & `tmp/user_context_remote-0.0.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_context_remote-0.0.83.tar", last modified: Thu May 23 00:35:31 2024, max compression
+gzip compressed data, was "user_context_remote-0.0.84.tar", last modified: Fri May 24 21:20:01 2024, max compression
```

## Comparing `user_context_remote-0.0.83.tar` & `user_context_remote-0.0.84.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:35:31.936182 user_context_remote-0.0.83/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-23 00:35:31.936182 user_context_remote-0.0.83/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-23 00:35:14.000000 user_context_remote-0.0.83/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 00:35:14.000000 user_context_remote-0.0.83/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 00:35:31.936182 user_context_remote-0.0.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-23 00:35:14.000000 user_context_remote-0.0.83/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:35:31.932182 user_context_remote-0.0.83/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:35:31.936182 user_context_remote-0.0.83/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 00:35:14.000000 user_context_remote-0.0.83/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-05-23 00:35:14.000000 user_context_remote-0.0.83/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:35:31.936182 user_context_remote-0.0.83/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-23 00:35:31.000000 user_context_remote-0.0.83/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-23 00:35:31.000000 user_context_remote-0.0.83/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:35:31.000000 user_context_remote-0.0.83/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 00:35:31.000000 user_context_remote-0.0.83/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 00:35:31.000000 user_context_remote-0.0.83/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-24 21:19:35.000000 user_context_remote-0.0.84/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 21:19:42.000000 user_context_remote-0.0.84/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-24 21:19:35.000000 user_context_remote-0.0.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:20:01.431029 user_context_remote-0.0.84/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:19:35.000000 user_context_remote-0.0.84/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-05-24 21:19:35.000000 user_context_remote-0.0.84/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:20:01.435029 user_context_remote-0.0.84/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 21:20:01.000000 user_context_remote-0.0.84/user_context_remote.egg-info/top_level.txt
```

### Comparing `user_context_remote-0.0.83/PKG-INFO` & `user_context_remote-0.0.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.83
+Version: 0.0.84
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `user_context_remote-0.0.83/README.md` & `user_context_remote-0.0.84/README.md`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.83/pyproject.toml` & `user_context_remote-0.0.84/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "user-context"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.59" # https://pypi.org/project/user-context i.e. https://pypi.org/project/storage-local/
+version = "0.0.60" # https://pypi.org/project/user-context i.e. https://pypi.org/project/storage-local/
 description = "user-context Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `user_context_remote-0.0.83/setup.py` & `user_context_remote-0.0.84/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.83',  # https://pypi.org/project/user-context-remote/
+    version='0.0.84',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.ai",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `user_context_remote-0.0.83/user_context_remote/src/user_context.py` & `user_context_remote-0.0.84/user_context_remote/src/user_context.py`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.83/user_context_remote.egg-info/PKG-INFO` & `user_context_remote-0.0.84/user_context_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.83
+Version: 0.0.84
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

