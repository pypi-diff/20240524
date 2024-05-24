# Comparing `tmp/pyhectiqlab-3.0.7.tar.gz` & `tmp/pyhectiqlab-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhectiqlab-3.0.7.tar", last modified: Thu May 16 18:07:05 2024, max compression
+gzip compressed data, was "pyhectiqlab-3.0.8.tar", last modified: Fri May 24 15:19:08 2024, max compression
```

## Comparing `pyhectiqlab-3.0.7.tar` & `pyhectiqlab-3.0.8.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.054126 pyhectiqlab-3.0.7/pyhectiqlab/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.054126 pyhectiqlab-3.0.7/pyhectiqlab/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/pyhectiqlab/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    24784 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/pyhectiqlab/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:07:05.062126 pyhectiqlab-3.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.607113 pyhectiqlab-3.0.8/pyhectiqlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.607113 pyhectiqlab-3.0.8/pyhectiqlab/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.607113 pyhectiqlab-3.0.8/pyhectiqlab/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/functional/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25208 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/pyhectiqlab/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyhectiqlab/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 15:19:08.000000 pyhectiqlab-3.0.8/pyhectiqlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:19:08.611113 pyhectiqlab-3.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-24 15:18:51.000000 pyhectiqlab-3.0.8/tests/test_run.py
```

### Comparing `pyhectiqlab-3.0.7/PKG-INFO` & `pyhectiqlab-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.7
+Version: 3.0.8
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/__init__.py` & `pyhectiqlab-3.0.8/pyhectiqlab/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-__version__ = "3.0.7"
+__version__ = "3.0.8"
 
 from pyhectiqlab.settings import getenv
 
 API_URL = getenv("HECTIQLAB_API_URL", "https://api.lab.hectiq.ai")
 
 from pyhectiqlab.config import Config
 from pyhectiqlab.dataset import Dataset
 from pyhectiqlab.model import Model
 from pyhectiqlab.run import Run
 from pyhectiqlab import functional
 
+from pyhectiqlab.logging import setup_logging
+setup_logging()
 
 def debug_mode():
     from pyhectiqlab.client import Client
-
     Client.online(False)
 
-
 __all__ = [
     "API_URL",
     "Artifact",
     "Dataset",
     "Model",
     "Run",
     "Config",
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/artifact.py` & `pyhectiqlab-3.0.8/pyhectiqlab/artifact.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/auth.py` & `pyhectiqlab-3.0.8/pyhectiqlab/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pyhectiqlab import API_URL
 from pathlib import Path
 from typing import Optional, Union
 
 
 def load_credentials(name: Optional[str] = None) -> Union[None, str]:
-    path = os.getenv("pyhectiqlab_CREDENTIALS_FILE", os.path.join(Path.home(), ".hectiq-lab", "credentials.toml"))
+    path = os.getenv("HECTIQLAB_CREDENTIALS", os.path.join(Path.home(), ".hectiq-lab", "credentials.toml"))
     if not os.path.exists(path):
         return None
     with open(path, "r") as path:
         data = toml.load(path)
     # If key_name is provided, we return the value of the key_name
     if name is not None:
         return data[name]
@@ -23,15 +23,15 @@
     return None
 
 
 def is_authenticated(name: Optional[str] = None) -> bool:
     """Checks if local is authenticated to the Hectiq Lab.
     If API key is None, the api_key is taken from:
      - the api_key located in the file `~/.hectiq-lab/credentials.toml`
-     (or the pyhectiqlab_CREDENTIALS_FILE).
+     (or the HECTIQLAB_CREDENTIALS).
 
     Args:
         name (Optional[str], optional): Name of the API key. If None, the first available key is used.
             Default: None.
 
     Returns:
         bool: True if the user is authenticated, False otherwise.
@@ -65,28 +65,28 @@
 
     @property
     def user(self):
         return self.data.get("user")
 
     @property
     def api_key(self):
-        return self.data.get("value")
+        return os.getenv("HECTIQLAB_API_KEY") or self.data.get("value")
 
     @property
     def auth_header(self):
         return {"X-API-Key": self.api_key} if self.api_key else {}
 
     @property
     def auth_token_header(self):
         return {"Authentification": f"Bearer {self.access_token}"} if self.access_token is not None else {}
 
     def refresh_token(self):
         response = httpx.post(f"{API_URL}/app/auth/auth-api-key", headers=self.auth_header)
         if response.status_code != 200:
-            logging.error(f"User could not be authenticated. Continuing in offline mode.")
+            logging.error("User could not be authenticated. Continuing in offline mode.")
             return
         self.access_token = response.cookies["access_token"]
 
     def auth_flow(self, request: httpx.Request):
         request.headers.update(self.auth_token_header)
         response = yield request
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/block.py` & `pyhectiqlab-3.0.8/pyhectiqlab/block.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/cli/__init__.py` & `pyhectiqlab-3.0.8/pyhectiqlab/cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,24 @@
 import click
 from .auth import auth_group
 from clisync import CliSync
 
 
 def main():
     import pyhectiqlab
-    import pyhectiqlab.const as const
     from pyhectiqlab import Run, Model, Dataset
     from pyhectiqlab.project import Project
     from pyhectiqlab.artifact import Artifact
     from pyhectiqlab.tag import Tag
     from pyhectiqlab.versions import PackageVersion
 
     # enable block and project creation for the cli
     pyhectiqlab.const.DISABLE_BLOCK_CREATION = pyhectiqlab.const.DISABLE_PROJECT_CREATION = False
 
     group = CliSync(module=pyhectiqlab, classes=[Run, Model, Dataset, Artifact, Tag, Project, PackageVersion])
-    cli = click.CommandCollection(sources=[auth_group, group])
+    cli = click.CommandCollection(sources=[auth_group, group], help="👋 Hectiq Lab CLI. Documentation at https://docs.hectiq.ai.")
     # Standalone mode is False so that the errors can be caught by the runs
     cli(standalone_mode=False)
     sys.exit()
 
-
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/cli/auth.py` & `pyhectiqlab-3.0.8/pyhectiqlab/cli/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+import os
 import click
 
 
 @click.group()
 def auth_group():
     pass
 
+@auth_group.command("info", help="Display information about your package.")
+def display_info():
+    import pyhectiqlab
+    click.secho("pyhectiqlab", bold=True)
+    click.echo(f" → Version: {pyhectiqlab.__version__}")
+    click.echo(f" → Directory path: {os.path.dirname(pyhectiqlab.__file__)}")
 
 @auth_group.command("authenticate", help="Authenticate to the Hectiq Lab.")
 def authenticate():
     """Authenticate to the Hectiq Console."""
     import httpx
     import os
     import toml
@@ -64,15 +71,7 @@
         data = {}
         data[name] = api_key
         toml.dump(data, f)
         f.write("\n")
 
         click.echo(f"A new API key has been added to {credentials_path}.")
     click.secho("You are now logged in.", fg="green")
-
-
-@auth_group.command("show-secret-key", help="Show the secret key.")
-def show_key():
-    from pyhectiqlab.auth import load_credentials
-
-    data = load_credentials()
-    click.echo(f"Your secret key is: {data['value']}")
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/client.py` & `pyhectiqlab-3.0.8/pyhectiqlab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import tqdm
 
 logger = logging.getLogger()
 
 ResponseType = Union[dict[str, Any], bytes, Type[None]]
 
 
+
 class Client:
     """
     Client singleton for making sync and async requests in the Hectiq Lab API. This client
     can be used in a context manager, or as a singleton. For performing async requests, the object
     must be instanciated.
 
     Example:
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/dataset.py` & `pyhectiqlab-3.0.8/pyhectiqlab/dataset.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/decorators.py` & `pyhectiqlab-3.0.8/pyhectiqlab/decorators.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/logging.py` & `pyhectiqlab-3.0.8/pyhectiqlab/logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,73 @@
 import logging
 from typing import Optional
+import os
 
 STEP_HANDLER_NAME = "hectiq-lab-step-handler"
 
+hectiqlab_logger: logging.Logger = logging.getLogger("hectiqlab")
+httpx_logger: logging.Logger = logging.getLogger("httpx")
+
+def setup_logging() -> None:
+    env = os.environ.get("HECTIQLAB_LOG_LEVEL", "warning").lower()
+    logging.basicConfig(
+        format="[%(asctime)s - %(name)s:%(lineno)d - %(levelname)s] %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+    )
+    if env == "info":
+        hectiqlab_logger.setLevel(logging.INFO)
+        httpx_logger.setLevel(logging.INFO)
+    elif env == "warning":
+        hectiqlab_logger.setLevel(logging.WARNING)
+        httpx_logger.setLevel(logging.WARNING)
+    else:
+        hectiqlab_logger.setLevel(logging.DEBUG)
+        httpx_logger.setLevel(logging.DEBUG)
 
 def stream_log(
     on_dump: callable,
     logger_name: Optional[str] = None,
     log_level: Optional[int] = logging.INFO,
     capacity: Optional[int] = 1000,
-):
+) -> None:
+    """
+    Stream logs to a memory handler.
+
+    Args:
+        on_dump (callable): The function to call when the buffer is flushed. Should take a list of strings as argument.
+        logger_name (str): The logger name. If None, the root logger is used.
+        log_level (int): The log level.
+        capacity (int): The buffer capacity.
+    """
     handler = MemoryHandler(name=STEP_HANDLER_NAME, capacity=capacity, target=on_dump)  # Flush every 5000 lines
     formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
     handler.setFormatter(formatter)
     root = logging.getLogger(logger_name)
     root.addHandler(handler)
     root.setLevel(log_level)
     handler.setLevel(log_level)
 
-
-def get_handler(logger_name: Optional[str] = None, name: Optional[str] = None):
+def get_handler(logger_name: Optional[str] = None) -> Optional[logging.Handler]:
     """
     Get a handler by name from the logger.
+
+    Args:
+        logger_name (str): The logger name. If None, the root logger is used.
+
+    Returns:
+        logging.Handler: The handler with the given name or None if not found.
     """
     logger = logging.getLogger(logger_name)
     for handler in logger.handlers:
         if not hasattr(handler, "name"):
             continue
         if handler.name == STEP_HANDLER_NAME:
             return handler
     return None
 
-
 class MemoryHandler(logging.StreamHandler):
     """
     A handler class which buffers logging records in memory, periodically
     flushing them to a target handler. Flushing occurs whenever the buffer
     is full, or when an event of a certain severity or greater is seen.
 
     Almost a copy of the standard library MemoryHandler, except that it
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/metrics.py` & `pyhectiqlab-3.0.8/pyhectiqlab/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/model.py` & `pyhectiqlab-3.0.8/pyhectiqlab/model.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/project.py` & `pyhectiqlab-3.0.8/pyhectiqlab/project.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/run.py` & `pyhectiqlab-3.0.8/pyhectiqlab/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,17 +171,18 @@
             category=category,
             config=config or {},
             tags=tags or [],
         )
 
         run = Run._client.post("/app/runs", json=data, wait_response=True)
         if run is None:
-            logging.error(f"Run failed to create.")
+            logging.error("Run failed to create.")
             return False
         Run.setup(**run)
+        Run._update(run_id=Run.id, status="initiated", package_versions=PackageVersion.all(repos=Run._repos))
         return run
 
     @staticmethod
     @functional_alias("retrieve_run")
     @no_git_diff()
     @clisync.include()
     def retrieve(
@@ -239,15 +240,15 @@
 
         run_id = run_id or Run.id
         if not run_id:
             logging.error("No run to retrieve. ")
             return
         run_id = Run._client.get(f"/app/runs/{run_id}", params=dict(fields=fields), wait_response=True)
         if not run_id:
-            logging.error(f"Run not found.")
+            logging.error(f"Run {run_id} not found. Verify the run ID and make sure you have access to it.")
             return
         if setup_with_result:
             Run.setup(**run_id)
         return run_id
 
     @staticmethod
     @online_method
@@ -257,15 +258,15 @@
         """Retrieve a config from a run.
         If the run does not have a config, an empty config is returned.
 
         Args:
             run (str, optional): Run ID. If None, the current run is used. Default: None.
             project (str, optional): Project name. If None, the current project is used. Default: None.
         """
-        run = run or Run.id
+        run = run_id or Run.id
         run = Run.retrieve_by_id(run=run, fields=["config"], setup_with_result=False)
         if run is None:
             return {}
 
         return run.get("config", {})
 
     @staticmethod
@@ -404,15 +405,15 @@
 
         basename, name_ext = os.path.splitext(name)
         if name_ext != "":
             extension = name_ext.strip(".")
         else:
             extension = (extension or "png").strip(".")
 
-        slug_name = slugify(basename)
+        slug_name = slugify.slugify(basename)
         fname = os.path.join(Run.tmp_artifacts, slug_name + "." + extension)
         figure.savefig(fname, dpi=dpi, format=extension, bbox_inches="tight", **kwargs)
 
         return Run.add_artifact(
             fname, name=name, step=step, wait_response=wait_response, run_id=run_id, project=project
         )
 
@@ -456,16 +457,21 @@
         """Push the metrics to the server.
         Do not use this method directly. Use the `add_metric` method instead.
         values is a list of tuples (step, value, timestamp).
         """
         run_id = run_id or Run.id
         if key is None or run_id is None or values is None:
             return
-
-        Run._client.post("/app/metrics", json=dict(name=key, values=values, run=run_id), wait_response=False)
+        data = dict(name=key, values=values, run=run_id)
+        # for value in values:
+        #     if len(value) != 3 or any(filter(lambda x: x is None, value)):
+        #         logging.error(f"Invalid metric value: {value}")
+        #         return
+        # print(data)
+        Run._client.post("/app/metrics", json=data, wait_response=False)
 
     @staticmethod
     @online_method
     @functional_alias("start_step")
     def start(
         name: str,
         run_id: Optional[str] = None,
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/settings/__init__.py` & `pyhectiqlab-3.0.8/pyhectiqlab/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/step.py` & `pyhectiqlab-3.0.8/pyhectiqlab/step.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/tag.py` & `pyhectiqlab-3.0.8/pyhectiqlab/tag.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/utils.py` & `pyhectiqlab-3.0.8/pyhectiqlab/utils.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab/versions.py` & `pyhectiqlab-3.0.8/pyhectiqlab/versions.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 import inspect
 import types
 import sys
 from pyhectiqlab.project import Project
 from pyhectiqlab.decorators import functional_alias
 from pyhectiqlab import settings
 
+import logging
+logger = logging.getLogger()
+
+from pyhectiqlab.logging import hectiqlab_logger
+
 try:
     from git import Repo
 except ImportError:
     pass
 
 try:
     import importlib.metadata as importlib_metadata
@@ -27,27 +32,39 @@
 
     @staticmethod
     @functional_alias("get_package_version")
     @clisync.include()
     def all(repos: Optional[List[str]] = None) -> dict:
         """Get all packages and system information."""
         packages = {}
-        packages["python"] = PackageVersion.python_version()
-        packages["system"] = PackageVersion.sysinfo()
-        packages["packages"] = PackageVersion.imported_modules_versions()
-
-        repos = repos or []
-        default_repos = settings.getenv("HECTIQ_LAB_REPOS", None)
-        if default_repos:
-            repos = default_repos.split(",") + repos
-
-        if repos:
-            packages["repos"] = {}
-            for repo in repos:
-                packages["repos"][repo] = PackageVersion.repo(repo)
+        try:
+            packages["python"] = PackageVersion.python_version()
+        except Exception as e:
+            logger.error(f"An error occurred while getting Python version: {e}")
+        try:
+            packages["system"] = PackageVersion.sysinfo()
+        except Exception as e:
+            logger.error(f"An error occurred while getting system information: {e}")
+        try:
+            packages["packages"] = PackageVersion.imported_modules_versions()
+        except Exception as e:
+            logger.error(f"An error occurred while getting package versions: {e}")
+        try:
+            repos = repos or []
+            default_repos = settings.getenv("HECTIQ_LAB_REPOS", None)
+            if default_repos:
+                repos = default_repos.split(",") + repos
+
+            if repos:
+                packages["repos"] = {}
+                for repo in repos:
+                    packages["repos"][repo] = PackageVersion.repo(repo)
+        except Exception as e:
+            logger.error(f"An error occurred while getting git repository information: {e}")
+        hectiqlab_logger.debug(f"Package versions: {packages}")
         return packages
 
     @staticmethod
     def python_version():
         """Get Python version."""
         return {"Python implementation": platform.python_implementation(), "Python version": platform.python_version()}
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab.egg-info/PKG-INFO` & `pyhectiqlab-3.0.8/pyhectiqlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.7
+Version: 3.0.8
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.7/pyhectiqlab.egg-info/SOURCES.txt` & `pyhectiqlab-3.0.8/pyhectiqlab.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,11 @@
 pyhectiqlab/functional/project.py
 pyhectiqlab/functional/run.py
 pyhectiqlab/functional/step.py
 pyhectiqlab/functional/tag.py
 pyhectiqlab/functional/utils.py
 pyhectiqlab/settings/__init__.py
 tests/test_dataset.py
+tests/test_metrics.py
 tests/test_model.py
 tests/test_project.py
 tests/test_run.py
```

### Comparing `pyhectiqlab-3.0.7/pyproject.toml` & `pyhectiqlab-3.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 maintainers = [
   {name = "Edward Laurence", email = "edwardl@hectiq.ai"},
   {name = "Charles Murphy", email = "cmurphy@hectiq.ai"},
 ]
 name = "pyhectiqlab"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "3.0.7"
+version = "3.0.8"
 
 [project.urls]
 Repository = "https://github.com/HectiqAI/hectiq-lab-revision.git"
 
 [project.entry-points.console_scripts]
 hectiq-lab = "pyhectiqlab.cli:main"
```

### Comparing `pyhectiqlab-3.0.7/tests/test_dataset.py` & `pyhectiqlab-3.0.8/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/tests/test_model.py` & `pyhectiqlab-3.0.8/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/tests/test_project.py` & `pyhectiqlab-3.0.8/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.7/tests/test_run.py` & `pyhectiqlab-3.0.8/tests/test_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
 from pyhectiqlab import Run
 from mock_client import mock_client
+from utils import random_uuid
 
 
 @pytest.fixture
 def config():
     return {"param": "test", "x": 1}
 
 
@@ -55,14 +56,21 @@
     import os
 
     with mock_client(Run) as r:
         run = r(rank=1, project="hectiq-ai/test")
         path = os.path.join(os.path.dirname(__file__), "dummy/artifact.txt")
         res = run.add_artifact(path, name="content.txt", wait_response=True)
 
+def test_run_add_figure():
+    run = Run(title=random_uuid(), project="hectiq-ai/test")
+    import matplotlib.pyplot as plt
+    plt.style.use("dark_background")
+    plt.figure(figsize=(3, 3))
+    plt.plot([1, 2, 3, 4], [1, 4, 9, 16])
+    run.add_figure(plt, name="test-figure", wait_response=True)
 
 def test_run_set_status():
     run = Run(rank=1, project="hectiq-ai/test")
     run.set_status("test status")
 
 
 def test_run_add_tag():
```

