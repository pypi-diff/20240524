# Comparing `tmp/data_prep_toolkit_kfp-0.1.1.tar.gz` & `tmp/data_prep_toolkit_kfp-0.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_prep_toolkit_kfp-0.1.1.tar", last modified: Fri May 24 10:13:47 2024, max compression
+gzip compressed data, was "data_prep_toolkit_kfp-0.1.1.dev0.tar", last modified: Tue May 21 09:16:55 2024, max compression
```

## Comparing `data_prep_toolkit_kfp-0.1.1.tar` & `data_prep_toolkit_kfp-0.1.1.dev0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.658657 data_prep_toolkit_kfp-0.1.1/
--rw-r--r--   0 boris      (501) staff       (20)     2117 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/Makefile
--rw-r--r--   0 boris      (501) staff       (20)     2697 2024-05-24 10:13:47.658121 data_prep_toolkit_kfp-0.1.1/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)     1890 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/README.md
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.634318 data_prep_toolkit_kfp-0.1.1/doc/
--rw-r--r--   0 boris      (501) staff       (20)      452 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/doc/kfp_support_library.md
--rw-r--r--   0 boris      (501) staff       (20)     1212 2024-05-24 10:12:19.000000 data_prep_toolkit_kfp-0.1.1/pyproject.toml
--rw-r--r--   0 boris      (501) staff       (20)       38 2024-05-24 10:13:47.658774 data_prep_toolkit_kfp-0.1.1/setup.cfg
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.630975 data_prep_toolkit_kfp-0.1.1/src/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.656232 data_prep_toolkit_kfp-0.1.1/src/data_prep_toolkit_kfp.egg-info/
--rw-r--r--   0 boris      (501) staff       (20)     2697 2024-05-24 10:13:47.000000 data_prep_toolkit_kfp-0.1.1/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
--rw-r--r--   0 boris      (501) staff       (20)     1397 2024-05-24 10:13:47.000000 data_prep_toolkit_kfp-0.1.1/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
--rw-r--r--   0 boris      (501) staff       (20)        1 2024-05-24 10:13:47.000000 data_prep_toolkit_kfp-0.1.1/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
--rw-r--r--   0 boris      (501) staff       (20)      168 2024-05-24 10:13:47.000000 data_prep_toolkit_kfp-0.1.1/src/data_prep_toolkit_kfp.egg-info/requires.txt
--rw-r--r--   0 boris      (501) staff       (20)       12 2024-05-24 10:13:47.000000 data_prep_toolkit_kfp-0.1.1/src/data_prep_toolkit_kfp.egg-info/top_level.txt
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.631638 data_prep_toolkit_kfp-0.1.1/src/kfp_support/
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.638867 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/
--rw-r--r--   0 boris      (501) staff       (20)      238 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/README.md
--rw-r--r--   0 boris      (501) staff       (20)       67 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)    27135 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/kuberay_apis.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.645850 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/
--rw-r--r--   0 boris      (501) staff       (20)     1326 2024-05-20 13:38:14.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)    17734 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/cluster.py
--rw-r--r--   0 boris      (501) staff       (20)     5390 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/environmentvariables.py
--rw-r--r--   0 boris      (501) staff       (20)     8063 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/headnode.py
--rw-r--r--   0 boris      (501) staff       (20)     6367 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/jobsubmission.py
--rw-r--r--   0 boris      (501) staff       (20)     7491 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/templates.py
--rw-r--r--   0 boris      (501) staff       (20)    14921 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/volumes.py
--rw-r--r--   0 boris      (501) staff       (20)     8441 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/workernode.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.646659 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/
--rw-r--r--   0 boris      (501) staff       (20)     2698 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/README.md
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.651023 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/
--rw-r--r--   0 boris      (501) staff       (20)      360 2024-05-20 13:38:14.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/__init__.py
--rw-r--r--   0 boris      (501) staff       (20)     4936 2024-05-20 13:38:14.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/components_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     3758 2024-05-20 13:38:14.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/kfp_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     6821 2024-05-20 13:38:14.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/pipeline_utils.py
--rw-r--r--   0 boris      (501) staff       (20)     2744 2024-05-24 10:01:52.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
--rw-r--r--   0 boris      (501) staff       (20)    22072 2024-05-22 07:01:10.000000 data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/remote_jobs_utils.py
-drwxr-xr-x   0 boris      (501) staff       (20)        0 2024-05-24 10:13:47.655351 data_prep_toolkit_kfp-0.1.1/test/
--rw-r--r--   0 boris      (501) staff       (20)    15224 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/test/api_params_test.py
--rw-r--r--   0 boris      (501) staff       (20)     2319 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/test/configmaps.py
--rw-r--r--   0 boris      (501) staff       (20)    10486 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/test/kuberay_api_test.py
--rw-r--r--   0 boris      (501) staff       (20)     1401 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/test/pipeline_utils_test.py
--rw-r--r--   0 boris      (501) staff       (20)     3232 2024-05-17 14:49:26.000000 data_prep_toolkit_kfp-0.1.1/test/ray_remote_jobs_test.py
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.318799 data_prep_toolkit_kfp-0.1.1.dev0/
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     2117 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/Makefile
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     2702 2024-05-21 09:16:55.318799 data_prep_toolkit_kfp-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     1890 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/README.md
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.309798 data_prep_toolkit_kfp-0.1.1.dev0/doc/
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)      452 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/doc/kfp_support_library.md
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     1216 2024-05-21 09:16:38.000000 data_prep_toolkit_kfp-0.1.1.dev0/pyproject.toml
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)       38 2024-05-21 09:16:55.318799 data_prep_toolkit_kfp-0.1.1.dev0/setup.cfg
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.307798 data_prep_toolkit_kfp-0.1.1.dev0/src/
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.315799 data_prep_toolkit_kfp-0.1.1.dev0/src/data_prep_toolkit_kfp.egg-info/
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     2702 2024-05-21 09:16:54.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/data_prep_toolkit_kfp.egg-info/PKG-INFO
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     1397 2024-05-21 09:16:55.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)        1 2024-05-21 09:16:54.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/data_prep_toolkit_kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)      168 2024-05-21 09:16:54.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/data_prep_toolkit_kfp.egg-info/requires.txt
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)       12 2024-05-21 09:16:54.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/data_prep_toolkit_kfp.egg-info/top_level.txt
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.308798 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.311798 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)      238 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/README.md
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)       67 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/__init__.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)    27135 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/kuberay_apis.py
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.313799 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     1326 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/__init__.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)    17734 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/cluster.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     5390 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/environmentvariables.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     8063 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/headnode.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     6367 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/jobsubmission.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     7491 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/templates.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)    14921 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/volumes.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     8441 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/workernode.py
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.313799 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     2698 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/README.md
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.314799 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)      360 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/__init__.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     4936 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/components_utils.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     3951 2024-05-21 09:09:27.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/kfp_utils.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     6821 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/pipeline_utils.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     3116 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)    21676 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/remote_jobs_utils.py
+drwxr-xr-x   0 nassarmo (217779328) domain users (10002)        0 2024-05-21 09:16:55.315799 data_prep_toolkit_kfp-0.1.1.dev0/test/
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)    15224 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/test/api_params_test.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     2319 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/test/configmaps.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)    10486 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/test/kuberay_api_test.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     1401 2024-05-02 06:59:52.000000 data_prep_toolkit_kfp-0.1.1.dev0/test/pipeline_utils_test.py
+-rw-r--r--   0 nassarmo (217779328) domain users (10002)     3232 2024-05-21 08:55:56.000000 data_prep_toolkit_kfp-0.1.1.dev0/test/ray_remote_jobs_test.py
```

### Comparing `data_prep_toolkit_kfp-0.1.1/Makefile` & `data_prep_toolkit_kfp-0.1.1.dev0/Makefile`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/PKG-INFO` & `data_prep_toolkit_kfp-0.1.1.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.1.1
+Version: 0.1.1.dev0
 Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
-Requires-Dist: data-prep-toolkit==0.1.1
+Requires-Dist: data-prep-toolkit==0.1.0
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
```

### Comparing `data_prep_toolkit_kfp-0.1.1/README.md` & `data_prep_toolkit_kfp-0.1.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/pyproject.toml` & `data_prep_toolkit_kfp-0.1.1.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "data_prep_toolkit_kfp"
-version = "0.1.1"
+version = "0.1.1-dev"
 requires-python = ">=3.10"
 description = "Data Preparation Kit Library. KFP support"
 license = {text = "Apache-2.0"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     { name = "Boris Lublinsky", email = "blublinsky@ibm.com" },
     { name = "Alexey Roytman", email = "roytman@il.ibm.com" },
     { name = "Mohammad Nassar", email = "Mohammad.Nassar@ibm.com" },
     { name = "Revital Eres", email = "eres@il.ibm.com" },
 ]
 dependencies = [
     "kfp==1.8.22",
     "requests",
-    "data-prep-toolkit==0.1.1",
+    "data-prep-toolkit==0.1.0",
 ]
 
 [build-system]
 requires = ["setuptools>=68.0.0", "wheel", "setuptools_scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
```

### Comparing `data_prep_toolkit_kfp-0.1.1/src/data_prep_toolkit_kfp.egg-info/PKG-INFO` & `data_prep_toolkit_kfp-0.1.1.dev0/src/data_prep_toolkit_kfp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data_prep_toolkit_kfp
-Version: 0.1.1
+Version: 0.1.1.dev0
 Summary: Data Preparation Kit Library. KFP support
 Author-email: Boris Lublinsky <blublinsky@ibm.com>, Alexey Roytman <roytman@il.ibm.com>, Mohammad Nassar <Mohammad.Nassar@ibm.com>, Revital Eres <eres@il.ibm.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kfp==1.8.22
 Requires-Dist: requests
-Requires-Dist: data-prep-toolkit==0.1.1
+Requires-Dist: data-prep-toolkit==0.1.0
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: pytest>=7.3.2; extra == "dev"
 Requires-Dist: pytest-dotenv>=0.5.2; extra == "dev"
 Requires-Dist: pytest-env>=1.0.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
```

### Comparing `data_prep_toolkit_kfp-0.1.1/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt` & `data_prep_toolkit_kfp-0.1.1.dev0/src/data_prep_toolkit_kfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/kuberay_apis.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/kuberay_apis.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/__init__.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/__init__.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/cluster.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/cluster.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/environmentvariables.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/environmentvariables.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/headnode.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/headnode.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/jobsubmission.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/jobsubmission.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/templates.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/templates.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/volumes.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/volumes.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/api_server_client/params/workernode.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/api_server_client/params/workernode.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/README.md` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/README.md`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/components_utils.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/components_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/kfp_utils.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/kfp_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,18 +85,23 @@
             return f"{ray_name[:9]}-{run_id[:5]}"
         return ray_name[:15]
 
     @staticmethod
     def dict_to_req(d: dict[str, Any], executor: str = "transformer_launcher.py") -> str:
         res = f"python {executor} "
         for key, value in d.items():
-            if isinstance(value, str):
-                res += f'--{key}="{value}" '
+            if isinstance(value, bool):
+                if value:
+                    res += f"--{key} "
+            elif isinstance(value, str):
+                if value != "":
+                    res += f'--{key}="{value}" '
             else:
                 res += f"--{key}={value} "
+        logger.info(f"request to execute: {res}")
         return res
 
     # Load a string that represents a json to python dictionary
     @staticmethod
     def load_from_json(js: str) -> dict[str, Any]:
         try:
             return json.loads(js)
```

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/pipeline_utils.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/pipelines_tests_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import sys
 
 from data_processing.utils import get_logger, str2bool
 
 from . import PipelinesUtils
 
 
 logger = get_logger(__name__)
@@ -36,14 +35,28 @@
         # Execution failed
         logger.warning(f"Pipeline {pipeline_name} failed with error {error} and status {status}")
         return None
     logger.info(f"Pipeline {pipeline_name} successfully completed")
     return pipeline_name
 
 
+def run_sanity_test(
+    pipeline_package_path: str = "", endpoint: str = "http://localhost:8080/kfp", overwrite: bool = True
+):
+    """
+    Run sanity test: automatic upload and run a pipeline.
+
+    :param pipeline_package_path: Local path to the pipeline package.
+    :param endpoint: endpoint to kfp service
+    """
+    pipeline_run = run_test(pipeline_package_path, endpoint=endpoint, overwrite=overwrite)
+    if pipeline_run is not None:
+        logger.info(f"{pipeline_run} run successfully launched")
+
+
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser(description="Run sanity test")
     parser.add_argument("-c", "--command", type=str, choices=["upload", "sanity-test"])
     parser.add_argument("-e", "--endpoint", type=str, default="http://localhost:8080/kfp")
     parser.add_argument("-p", "--pipeline_package_path", type=str, default="")
@@ -51,25 +64,21 @@
 
     args = parser.parse_args()
     match args.command:
         case "upload":
             file_name = os.path.basename(args.pipeline_package_path)
             pipeline_name = os.path.splitext(file_name)[0]
             utils = PipelinesUtils(host=args.endpoint)
-            pipeline = utils.upload_pipeline(
+            utils.upload_pipeline(
                 pipeline_package_path=args.pipeline_package_path,
                 pipeline_name=pipeline_name,
                 overwrite=str2bool(args.overwrite),
             )
-            if pipeline is None:
-                sys.exit(1)
         case "sanity-test":
-            run = run_test(
+            run_sanity_test(
                 endpoint=args.endpoint,
                 pipeline_package_path=args.pipeline_package_path,
                 overwrite=str2bool(args.overwrite),
             )
-            if run is None:
-                sys.exit(1)
         case _:
             logger.warning("Unsupported command")
             exit(1)
```

### Comparing `data_prep_toolkit_kfp-0.1.1/src/kfp_support/workflow_support/utils/remote_jobs_utils.py` & `data_prep_toolkit_kfp-0.1.1.dev0/src/kfp_support/workflow_support/utils/remote_jobs_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ################################################################################
 
 import re
 import sys
 import time
 from typing import Any
 
-from data_processing.data_access import DataAccess, DataAccessFactory
+from data_processing.data_access import DataAccess
 from data_processing.utils import ParamsUtils, get_logger
 from kfp_support.api_server_client import KubeRayAPIs
 from kfp_support.api_server_client.params import (
     DEFAULT_HEAD_START_PARAMS,
     DEFAULT_WORKER_START_PARAMS,
     Cluster,
     ClusterSpec,
@@ -408,63 +408,61 @@
 
 
 def _execute_remote_job(
     name: str,
     ns: str,
     script: str,
     params: dict[str, Any],
-    data_access_params: dict[str, Any],
     additional_params: dict[str, Any],
+    d_access: DataAccess,
     remote_jobs: RayRemoteJobs,
 ) -> None:
     """
     Execute remote job on Ray cluster
     :param name: cluster name
     :param ns: execution/cluster namespace
+    :param d_access: data access class
     :param additional_params: additional parameters for the job
-    :param data_access_params: data access parameters
     :param params: job execution parameters (specific for a specific transform,
                         generated by the transform workflow)
     :param script: script to run (has to be present in the image)
     :param remote_jobs: remote jobs execution support class
     :return:
     """
 
     status, error, submission = remote_jobs.submit_job(name=name, namespace=ns, request=params, executor=script)
     if status != 200:
         logger.error(f"Failed to submit job - status: {status}, error: {error}")
         exit(1)
 
     logger.info(f"submitted job successfully, submission id {submission}")
-    # create data access
-    data_factory = DataAccessFactory()
-    data_factory.apply_input_params(args=data_access_params)
-    data_access = data_factory.create_data_access()
     # print execution log
     remote_jobs.follow_execution(
         name=name,
         namespace=ns,
         submission_id=submission,
-        data_access=data_access,
+        data_access=d_access,
         print_timeout=additional_params.get("wait_print_tmout", 120),
         job_ready_timeout=additional_params.get("wait_job_ready_tmout", 600),
     )
 
 
 def execute_ray_jobs(
     name: str,  # name of Ray cluster
+    d_access: DataAccess,  # data access
     additional_params: dict[str, Any],
     e_params: dict[str, Any],
     exec_script_name: str,
     server_url: str,
 ) -> None:
     """
     Execute Ray jobs on a cluster periodically printing execution log. Completes when all Ray job complete.
     All of the jobs will be executed, although some of the jobs may fail.
     :param name: cluster name
+    :param d_access: data access class
     :param additional_params: additional parameters for the job
     :param e_params: job execution parameters (specific for a specific transform,
                         generated by the transform workflow)
     :param exec_script_name: script to run (has to be present in the image)
     :param server_url: API server url
     :return: None
     """
@@ -480,43 +478,42 @@
         wait_interval=additional_params.get("wait_interval", 2),
     )
     # find config parameter
     config = ParamsUtils.get_config_parameter(e_params)
     if config is None:
         exit(1)
     # get config value
-    config_value = KFPUtils.load_from_json(e_params[config].replace("'", '"'))
-    s3_creds = KFPUtils.load_from_json(e_params["data_s3_cred"].replace("'", '"'))
+    config_value = e_params[config]
     if type(config_value) is not list:
         # single request
         return _execute_remote_job(
             name=name,
             ns=ns,
             script=exec_script_name,
-            data_access_params={config: config_value, "data_s3_cred": s3_creds},
             params=e_params,
             additional_params=additional_params,
+            d_access=d_access,
             remote_jobs=remote_jobs,
         )
     # remove config key from the dictionary
     launch_params = dict(e_params)
     del launch_params[config]
     # Loop through all configuration
     n_launches = 0
     for conf in config_value:
         # populate individual config and launch
-        launch_params[config] = ParamsUtils.convert_to_ast(d=conf)
+        launch_params[config] = conf
         try:
             _execute_remote_job(
                 name=name,
                 ns=ns,
                 script=exec_script_name,
-                data_access_params={config: conf, "data_s3_cred": s3_creds},
                 params=launch_params,
                 additional_params=additional_params,
+                d_access=d_access,
                 remote_jobs=remote_jobs,
             )
             n_launches += 1
         except SystemExit:
             logger.warning(f"Failed to execute job for configuration {conf}")
             continue
```

### Comparing `data_prep_toolkit_kfp-0.1.1/test/api_params_test.py` & `data_prep_toolkit_kfp-0.1.1.dev0/test/api_params_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/test/configmaps.py` & `data_prep_toolkit_kfp-0.1.1.dev0/test/configmaps.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/test/kuberay_api_test.py` & `data_prep_toolkit_kfp-0.1.1.dev0/test/kuberay_api_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/test/pipeline_utils_test.py` & `data_prep_toolkit_kfp-0.1.1.dev0/test/pipeline_utils_test.py`

 * *Files identical despite different names*

### Comparing `data_prep_toolkit_kfp-0.1.1/test/ray_remote_jobs_test.py` & `data_prep_toolkit_kfp-0.1.1.dev0/test/ray_remote_jobs_test.py`

 * *Files identical despite different names*

