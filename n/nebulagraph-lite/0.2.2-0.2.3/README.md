# Comparing `tmp/nebulagraph_lite-0.2.2.tar.gz` & `tmp/nebulagraph_lite-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nebulagraph_lite-0.2.2.tar", last modified: Wed Mar  6 04:45:48 2024, max compression
+gzip compressed data, was "nebulagraph_lite-0.2.3.tar", last modified: Thu May 23 12:13:52 2024, max compression
```

## Comparing `nebulagraph_lite-0.2.2.tar` & `nebulagraph_lite-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-03-06 04:45:31.530148 nebulagraph_lite-0.2.2/LICENSE
--rw-r--r--   0        0        0     7190 2024-03-06 04:45:31.530148 nebulagraph_lite-0.2.2/README.md
--rw-r--r--   0        0        0      859 2024-03-06 04:45:48.970340 nebulagraph_lite-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      129 2024-03-06 04:45:31.538148 nebulagraph_lite-0.2.2/src/nebulagraph_lite/__init__.py
--rw-r--r--   0        0        0     4446 2024-03-06 04:45:31.538148 nebulagraph_lite-0.2.2/src/nebulagraph_lite/cli.py
--rw-r--r--   0        0        0    27930 2024-03-06 04:45:31.538148 nebulagraph_lite-0.2.2/src/nebulagraph_lite/nebulagraph.py
--rw-r--r--   0        0        0     3625 2024-03-06 04:45:31.538148 nebulagraph_lite-0.2.2/src/nebulagraph_lite/utils.py
--rw-r--r--   0        0        0        0 2024-03-06 04:45:31.538148 nebulagraph_lite-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     4687 2024-03-06 04:45:31.538148 nebulagraph_lite-0.2.2/tests/e2e/jupyter/jupyter_test.ipynb
--rw-r--r--   0        0        0     3877 2024-03-06 04:45:31.538148 nebulagraph_lite-0.2.2/tests/e2e/jupyter/modelscope_test.ipynb
--rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 nebulagraph_lite-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7200 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/README.md
+-rw-r--r--   0        0        0      859 2024-05-23 12:13:52.144414 nebulagraph_lite-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      129 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/src/nebulagraph_lite/__init__.py
+-rw-r--r--   0        0        0     4446 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/src/nebulagraph_lite/cli.py
+-rw-r--r--   0        0        0    27930 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/src/nebulagraph_lite/nebulagraph.py
+-rw-r--r--   0        0        0     3625 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/src/nebulagraph_lite/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     4687 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/tests/e2e/jupyter/jupyter_test.ipynb
+-rw-r--r--   0        0        0     3877 2024-05-23 12:13:33.612196 nebulagraph_lite-0.2.3/tests/e2e/jupyter/modelscope_test.ipynb
+-rw-r--r--   0        0        0     7535 1970-01-01 00:00:00.000000 nebulagraph_lite-0.2.3/PKG-INFO
```

### Comparing `nebulagraph_lite-0.2.2/LICENSE` & `nebulagraph_lite-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.2/README.md` & `nebulagraph_lite-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: nebulagraph-lite
+Version: 0.2.3
+Summary: Plug and play NebulaGraph with pip install.
+Author-Email: Wey Gu <weyl.gu@gmail.com>
+License: Apache 2.0
+Requires-Python: >=3.8
+Requires-Dist: udocker==1.3.13
+Requires-Dist: psutil>=5.9.6
+Requires-Dist: nebula3-python>=3.8.0
+Description-Content-Type: text/markdown
+
 <div>
   <img src="https://github.com/nebula-contrib/nebulagraph-lite/assets/1651790/97b5dccb-bca1-4141-b426-03bcb3761a10" alt="NebulaGraph-Lite-logo" height="100" style="float:left;">
   <h1 style="margin-left:110px;">NebulaGraph Lite</h1>
 </div>
 
 Try NebulaGraph with `pip install`, on Linux/ WSL2 or even [Google Colab](https://colab.research.google.com/github/nebula-contrib/nebulagraph-lite/blob/main/examples/NebulaGraph_Lite.ipynb) or [ModelScope Notebook](https://modelscope.cn/my/mynotebook/preset), in container, rootless.
 
@@ -72,18 +84,18 @@
 
 Go with 👉 [![Open in ModelScope](https://img.shields.io/badge/ModelScope-Notebook-blue?logo=jupyter)](https://github.com/nebula-contrib/nebulagraph-lite/blob/main/examples/NebulaGraph_Lite.ipynb)
 
 </details>
 
 ## What's next
 
-Play with `nebula3-python` or [ipython-ngql](https://github.com/nebula-contrib/ipython-ngql) and walk through the [Documentation](https://docs.nebula-graph.io/)!
+Play with `nebula3-python` or [jupyter-nebulagraph](https://jupyter-nebulagraph.readthedocs.io) and walk through the [Documentation](https://docs.nebula-graph.io/)!
 
 ```bash
-pip3 install ipython-ngql
+pip3 install jupyter-nebulagraph
 %load_ext ngql
 ```
 
 And we could access it like:
 
 ```python
 %ngql --address 127.0.0.1 --port 9669 --user root --password nebula
```

### Comparing `nebulagraph_lite-0.2.2/pyproject.toml` & `nebulagraph_lite-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 description = "Plug and play NebulaGraph with pip install."
 authors = [
     { name = "Wey Gu", email = "weyl.gu@gmail.com" },
 ]
 dependencies = [
     "udocker==1.3.13",
     "psutil>=5.9.6",
-    "nebula3-python>=3.5.0",
+    "nebula3-python>=3.8.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "0.2.2"
+version = "0.2.3"
 
 [project.license]
 text = "Apache 2.0"
 
 [project.scripts]
 nebulagraph = "nebulagraph_lite.cli:main"
```

### Comparing `nebulagraph_lite-0.2.2/src/nebulagraph_lite/cli.py` & `nebulagraph_lite-0.2.3/src/nebulagraph_lite/cli.py`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.2/src/nebulagraph_lite/nebulagraph.py` & `nebulagraph_lite-0.2.3/src/nebulagraph_lite/nebulagraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 BASKETBALLPLAYER_DATASET_URL_ALT = "https://www.modelscope.cn/api/v1/models/sdfsdfoph1ofdsaofdf/nebulagraph-lite/repo?Revision=master&FilePath=releases/3.6.0/basketballplayer.ngql"
 
 # CN Docker-Registry Mirror
 CN_DOCKER_REGISTRY_MIRROR = "docker.m.daocloud.io"
 
 # ModelScope Model ID
 MODELSCOPE_MODEL_ID = "sdfsdfoph1ofdsaofdf/nebulagraph-lite"
-MODELSCOPE_MODEL_FILE_PATH = "releases/3.6.0/nebulagraph_lite.tar.gz"
+MODELSCOPE_MODEL_FILE_PATH = "releases/3.8.0/nebulagraph_lite.tar.gz"
 MODELSCOPE_MODEL_VERSION = "master"
 
 # udocker tarball
 UDOCKER_TARBALL_URL = ""
 # udocker tool version
 UDOCKER_VERSION = "1.2.11"
 UDOCKER_TARBALL_FILENAME = f"udocker-englib-{UDOCKER_VERSION}.tar.gz"
```

### Comparing `nebulagraph_lite-0.2.2/src/nebulagraph_lite/utils.py` & `nebulagraph_lite-0.2.3/src/nebulagraph_lite/utils.py`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.2/tests/e2e/jupyter/jupyter_test.ipynb` & `nebulagraph_lite-0.2.3/tests/e2e/jupyter/jupyter_test.ipynb`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.2/tests/e2e/jupyter/modelscope_test.ipynb` & `nebulagraph_lite-0.2.3/tests/e2e/jupyter/modelscope_test.ipynb`

 * *Files identical despite different names*

### Comparing `nebulagraph_lite-0.2.2/PKG-INFO` & `nebulagraph_lite-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: nebulagraph-lite
-Version: 0.2.2
-Summary: Plug and play NebulaGraph with pip install.
-Author-Email: Wey Gu <weyl.gu@gmail.com>
-License: Apache 2.0
-Requires-Python: >=3.8
-Requires-Dist: udocker==1.3.13
-Requires-Dist: psutil>=5.9.6
-Requires-Dist: nebula3-python>=3.5.0
-Description-Content-Type: text/markdown
-
 <div>
   <img src="https://github.com/nebula-contrib/nebulagraph-lite/assets/1651790/97b5dccb-bca1-4141-b426-03bcb3761a10" alt="NebulaGraph-Lite-logo" height="100" style="float:left;">
   <h1 style="margin-left:110px;">NebulaGraph Lite</h1>
 </div>
 
 Try NebulaGraph with `pip install`, on Linux/ WSL2 or even [Google Colab](https://colab.research.google.com/github/nebula-contrib/nebulagraph-lite/blob/main/examples/NebulaGraph_Lite.ipynb) or [ModelScope Notebook](https://modelscope.cn/my/mynotebook/preset), in container, rootless.
 
@@ -84,18 +72,18 @@
 
 Go with 👉 [![Open in ModelScope](https://img.shields.io/badge/ModelScope-Notebook-blue?logo=jupyter)](https://github.com/nebula-contrib/nebulagraph-lite/blob/main/examples/NebulaGraph_Lite.ipynb)
 
 </details>
 
 ## What's next
 
-Play with `nebula3-python` or [ipython-ngql](https://github.com/nebula-contrib/ipython-ngql) and walk through the [Documentation](https://docs.nebula-graph.io/)!
+Play with `nebula3-python` or [jupyter-nebulagraph](https://jupyter-nebulagraph.readthedocs.io) and walk through the [Documentation](https://docs.nebula-graph.io/)!
 
 ```bash
-pip3 install ipython-ngql
+pip3 install jupyter-nebulagraph
 %load_ext ngql
 ```
 
 And we could access it like:
 
 ```python
 %ngql --address 127.0.0.1 --port 9669 --user root --password nebula
```

