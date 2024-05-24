# Comparing `tmp/dockerblade-0.6.0.tar.gz` & `tmp/dockerblade-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerblade-0.6.0.tar", max compression
+gzip compressed data, was "dockerblade-0.6.1.tar", max compression
```

## Comparing `dockerblade-0.6.0.tar` & `dockerblade-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11358 2024-05-20 19:44:50.243460 dockerblade-0.6.0/LICENSE
--rw-r--r--   0        0        0     2280 2024-05-20 19:44:50.244164 dockerblade-0.6.0/README.rst
--rw-r--r--   0        0        0     3795 2024-05-20 22:53:49.710027 dockerblade-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      287 2024-05-20 22:53:49.710304 dockerblade-0.6.0/src/dockerblade/__init__.py
--rw-r--r--   0        0        0     4262 2024-05-20 22:53:49.710610 dockerblade-0.6.0/src/dockerblade/container.py
--rw-r--r--   0        0        0     5266 2024-05-20 22:53:49.710920 dockerblade-0.6.0/src/dockerblade/daemon.py
--rw-r--r--   0        0        0     3958 2024-05-20 22:53:49.711144 dockerblade-0.6.0/src/dockerblade/exceptions.py
--rw-r--r--   0        0        0    23316 2024-05-20 22:53:49.711402 dockerblade-0.6.0/src/dockerblade/files.py
--rw-r--r--   0        0        0     5138 2024-05-20 22:53:49.711735 dockerblade-0.6.0/src/dockerblade/popen.py
--rw-r--r--   0        0        0        0 2024-05-20 19:44:50.246808 dockerblade-0.6.0/src/dockerblade/py.typed
--rw-r--r--   0        0        0    13600 2024-05-20 22:53:49.712000 dockerblade-0.6.0/src/dockerblade/shell.py
--rw-r--r--   0        0        0     1851 2024-05-20 22:53:49.712212 dockerblade-0.6.0/src/dockerblade/stopwatch.py
--rw-r--r--   0        0        0      362 2024-05-20 22:53:49.712482 dockerblade-0.6.0/src/dockerblade/util.py
--rw-r--r--   0        0        0       22 2024-05-20 22:53:49.712736 dockerblade-0.6.0/src/dockerblade/version.py
--rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 dockerblade-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-20 19:44:50.243460 dockerblade-0.6.1/LICENSE
+-rw-r--r--   0        0        0     2280 2024-05-20 19:44:50.244164 dockerblade-0.6.1/README.rst
+-rw-r--r--   0        0        0     3795 2024-05-24 01:56:31.362730 dockerblade-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      287 2024-05-20 22:53:49.710304 dockerblade-0.6.1/src/dockerblade/__init__.py
+-rw-r--r--   0        0        0     4262 2024-05-20 22:53:49.710610 dockerblade-0.6.1/src/dockerblade/container.py
+-rw-r--r--   0        0        0     5266 2024-05-20 22:53:49.710920 dockerblade-0.6.1/src/dockerblade/daemon.py
+-rw-r--r--   0        0        0     3958 2024-05-20 22:53:49.711144 dockerblade-0.6.1/src/dockerblade/exceptions.py
+-rw-r--r--   0        0        0    23678 2024-05-24 01:54:52.469945 dockerblade-0.6.1/src/dockerblade/files.py
+-rw-r--r--   0        0        0     5138 2024-05-20 22:53:49.711735 dockerblade-0.6.1/src/dockerblade/popen.py
+-rw-r--r--   0        0        0        0 2024-05-20 19:44:50.246808 dockerblade-0.6.1/src/dockerblade/py.typed
+-rw-r--r--   0        0        0    13600 2024-05-20 22:53:49.712000 dockerblade-0.6.1/src/dockerblade/shell.py
+-rw-r--r--   0        0        0     1851 2024-05-20 22:53:49.712212 dockerblade-0.6.1/src/dockerblade/stopwatch.py
+-rw-r--r--   0        0        0      362 2024-05-20 22:53:49.712482 dockerblade-0.6.1/src/dockerblade/util.py
+-rw-r--r--   0        0        0       22 2024-05-24 01:54:13.809826 dockerblade-0.6.1/src/dockerblade/version.py
+-rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 dockerblade-0.6.1/PKG-INFO
```

### Comparing `dockerblade-0.6.0/LICENSE` & `dockerblade-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerblade-0.6.0/README.rst` & `dockerblade-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `dockerblade-0.6.0/pyproject.toml` & `dockerblade-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dockerblade"
-version = "0.6.0"
+version = "0.6.1"
 description = "Interact with Docker containers via Python-like APIs"
 authors = ["Chris Timperley <ctimperley@cmu.edu>"]
 license = "Apache-2.0"
 repository = "https://github.com/ChrisTimperley/dockerblade"
 readme = "README.rst"
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `dockerblade-0.6.0/src/dockerblade/container.py` & `dockerblade-0.6.1/src/dockerblade/container.py`

 * *Files identical despite different names*

### Comparing `dockerblade-0.6.0/src/dockerblade/daemon.py` & `dockerblade-0.6.1/src/dockerblade/daemon.py`

 * *Files identical despite different names*

### Comparing `dockerblade-0.6.0/src/dockerblade/exceptions.py` & `dockerblade-0.6.1/src/dockerblade/exceptions.py`

 * *Files identical despite different names*

### Comparing `dockerblade-0.6.0/src/dockerblade/files.py` & `dockerblade-0.6.1/src/dockerblade/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import contextlib
 import os
 import subprocess
 import tempfile
 import typing
 from collections.abc import Iterator
 from pathlib import Path
+from subprocess import DEVNULL
 from typing import Literal, overload
 
 import attr
 from loguru import logger
 
 from . import exceptions as exc
 from .util import quote_container, quote_host
@@ -70,15 +71,21 @@
                 path_container_escaped = f'"{path_container_escaped}"'
             if path_host_escaped[0] != '"':
                 path_host_escaped = f'"{path_host_escaped}"'
 
         cmd: str = (f"docker cp -L {path_host_escaped} "
                     f"{id_container}:{path_container_escaped}")
         try:
-            subprocess.check_call(cmd, shell=True)
+            subprocess.check_call(
+                cmd,
+                shell=True,
+                stdin=DEVNULL,
+                stdout=DEVNULL,
+                stderr=DEVNULL,
+            )
         except subprocess.CalledProcessError as error:
             path_container_parent: str = os.path.dirname(path_container)
             if not self.isdir(path_container_parent):
                 raise exc.ContainerFileNotFound(
                     path=path_container_parent,
                     container_id=id_container,
                 ) from error
@@ -125,15 +132,21 @@
             if path_host_escaped[0] != '"':
                 path_host_escaped = f'"{path_host_escaped}"'
 
         cmd: str = (f"docker cp -L "
                     f"{id_container}:{path_container_escaped} "
                     f"{path_host_escaped}")
         try:
-            subprocess.check_call(cmd, shell=True)
+            subprocess.check_call(
+                cmd,
+                shell=True,
+                stdin=DEVNULL,
+                stdout=DEVNULL,
+                stderr=DEVNULL,
+            )
         except subprocess.CalledProcessError as error:
             if not self.exists(path_container):
                 raise exc.ContainerFileNotFound(
                     path=path_container,
                     container_id=id_container,
                 ) from error
 
@@ -202,15 +215,18 @@
             an unexpected failure occurred.
         """
         escaped_directory = quote_container(directory)
         command = (f"test -e {escaped_directory} || exit 50 && "
                    f"test -d {escaped_directory} || exit 51 && "
                    f"rmdir {escaped_directory}")
         try:
-            self._shell.check_output(command, text=True)
+            self._shell.check_output(
+                command,
+                text=True,
+            )
         except exc.CalledProcessError as error:
             if error.returncode == EXIT_CODE_FILE_NOT_FOUND:
                 raise exc.ContainerFileNotFound(
                     path=directory,
                     container_id=self.container.id,
                 ) from error
             if error.returncode == EXIT_CODE_IS_NOT_A_DIRECTORY:
```

### Comparing `dockerblade-0.6.0/src/dockerblade/popen.py` & `dockerblade-0.6.1/src/dockerblade/popen.py`

 * *Files identical despite different names*

### Comparing `dockerblade-0.6.0/src/dockerblade/shell.py` & `dockerblade-0.6.1/src/dockerblade/shell.py`

 * *Files identical despite different names*

### Comparing `dockerblade-0.6.0/src/dockerblade/stopwatch.py` & `dockerblade-0.6.1/src/dockerblade/stopwatch.py`

 * *Files identical despite different names*

### Comparing `dockerblade-0.6.0/PKG-INFO` & `dockerblade-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerblade
-Version: 0.6.0
+Version: 0.6.1
 Summary: Interact with Docker containers via Python-like APIs
 Home-page: https://github.com/ChrisTimperley/dockerblade
 License: Apache-2.0
 Author: Chris Timperley
 Author-email: ctimperley@cmu.edu
 Requires-Python: >=3.11,<4
 Classifier: Intended Audience :: Developers
```

