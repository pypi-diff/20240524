# Comparing `tmp/Multiclass_interface-1.1.tar.gz` & `tmp/multiclass_interface-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Multiclass_interface-1.1.tar", last modified: Thu Mar 21 09:52:48 2024, max compression
+gzip compressed data, was "multiclass_interface-1.2.tar", last modified: Fri May 24 06:00:47 2024, max compression
```

## Comparing `Multiclass_interface-1.1.tar` & `multiclass_interface-1.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 09:52:48.925370 Multiclass_interface-1.1/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-18 14:23:06.000000 Multiclass_interface-1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2228 2024-03-19 07:05:00.000000 Multiclass_interface-1.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-03-19 07:05:00.000000 Multiclass_interface-1.1/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 09:52:48.925370 Multiclass_interface-1.1/Multiclass_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1578 2024-03-21 09:52:48.000000 Multiclass_interface-1.1/Multiclass_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      697 2024-03-21 09:52:48.000000 Multiclass_interface-1.1/Multiclass_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 09:52:48.000000 Multiclass_interface-1.1/Multiclass_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-21 09:52:48.000000 Multiclass_interface-1.1/Multiclass_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-21 09:52:48.000000 Multiclass_interface-1.1/Multiclass_interface.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1578 2024-03-21 09:52:48.925370 Multiclass_interface-1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-19 07:07:38.000000 Multiclass_interface-1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 09:52:48.921370 Multiclass_interface-1.1/multiclass_interface/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-18 12:26:49.000000 Multiclass_interface-1.1/multiclass_interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5993 2024-03-18 12:33:01.000000 Multiclass_interface-1.1/multiclass_interface/mpi_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-18 19:36:25.000000 Multiclass_interface-1.1/multiclass_interface/multi_object_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8169 2024-03-21 09:39:37.000000 Multiclass_interface-1.1/multiclass_interface/multiprocess_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 09:52:48.925370 Multiclass_interface-1.1/multiclass_interface/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-21 09:51:14.000000 Multiclass_interface-1.1/multiclass_interface/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 19:36:25.000000 Multiclass_interface-1.1/multiclass_interface/tests/my_test_cls.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2024-03-18 14:23:06.000000 Multiclass_interface-1.1/multiclass_interface/tests/test_mpi.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-18 19:36:25.000000 Multiclass_interface-1.1/multiclass_interface/tests/test_multiclass_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-21 09:39:37.000000 Multiclass_interface-1.1/multiclass_interface/tests/test_multiprocessinterface.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-03-21 09:52:48.000000 Multiclass_interface-1.1/multiclass_interface/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-19 07:05:00.000000 Multiclass_interface-1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-21 09:52:48.925370 Multiclass_interface-1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:00:47.800943 multiclass_interface-1.2/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-18 14:23:06.000000 multiclass_interface-1.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-24 05:52:15.000000 multiclass_interface-1.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-03-19 07:05:00.000000 multiclass_interface-1.2/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:00:47.800943 multiclass_interface-1.2/Multiclass_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-24 06:00:47.800943 multiclass_interface-1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-19 07:07:38.000000 multiclass_interface-1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:00:47.800943 multiclass_interface-1.2/multiclass_interface/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-18 12:26:49.000000 multiclass_interface-1.2/multiclass_interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5716 2024-05-24 04:55:16.000000 multiclass_interface-1.2/multiclass_interface/mpi_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-18 19:36:25.000000 multiclass_interface-1.2/multiclass_interface/multi_object_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8169 2024-03-21 09:39:37.000000 multiclass_interface-1.2/multiclass_interface/multiprocess_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:00:47.800943 multiclass_interface-1.2/multiclass_interface/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 05:58:40.000000 multiclass_interface-1.2/multiclass_interface/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 19:36:25.000000 multiclass_interface-1.2/multiclass_interface/tests/my_test_cls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-24 05:09:43.000000 multiclass_interface-1.2/multiclass_interface/tests/test_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-18 19:36:25.000000 multiclass_interface-1.2/multiclass_interface/tests/test_multiclass_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-21 09:39:37.000000 multiclass_interface-1.2/multiclass_interface/tests/test_multiprocessinterface.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-24 06:00:47.000000 multiclass_interface-1.2/multiclass_interface/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-19 07:05:00.000000 multiclass_interface-1.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     5238 2024-05-24 05:43:55.000000 multiclass_interface-1.2/sequence_diagrams.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 06:00:47.800943 multiclass_interface-1.2/setup.cfg
```

### Comparing `Multiclass_interface-1.1/.gitlab-ci.yml` & `multiclass_interface-1.2/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 test_ubuntu:  # name the job what we like
   image: continuumio/anaconda3
   stage:  # build, test, deploy defined by default [2]
     test
   script:
   - pip install -e .[test]
   - pytest --cov-report term-missing:skip-covered --cov=multiclass_interface multiclass_interface/tests
-  - pytest --cov-report term-missing:skip-covered --cov=multiclass_interface multiclass_interface/tests
   coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
   tags:  # only runners with this tag can do the job [3]
   - ci-ubuntu
   rules:
     - if: $CI_COMMIT_BRANCH == "main"
     - if: $CI_PIPELINE_SOURCE == "merge_request_event"
```

### Comparing `Multiclass_interface-1.1/LICENSE` & `multiclass_interface-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Multiclass_interface-1.1/Multiclass_interface.egg-info/PKG-INFO` & `multiclass_interface-1.2/Multiclass_interface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multiclass_interface
-Version: 1.1
+Version: 1.2
 Summary: Multiclass interface
 Author-email: "Mads M. Pedersen" <mmpe@dtu.dk>
 Project-URL: Homepage, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface
 Project-URL: Bug Tracker, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Multiclass_interface-1.1/Multiclass_interface.egg-info/SOURCES.txt` & `multiclass_interface-1.2/Multiclass_interface.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .gitlab-ci.yml
 LICENSE
 README.md
 pyproject.toml
+sequence_diagrams.md
 Multiclass_interface.egg-info/PKG-INFO
 Multiclass_interface.egg-info/SOURCES.txt
 Multiclass_interface.egg-info/dependency_links.txt
 Multiclass_interface.egg-info/requires.txt
 Multiclass_interface.egg-info/top_level.txt
 multiclass_interface/__init__.py
 multiclass_interface/mpi_interface.py
```

### Comparing `Multiclass_interface-1.1/PKG-INFO` & `multiclass_interface-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multiclass_interface
-Version: 1.1
+Version: 1.2
 Summary: Multiclass interface
 Author-email: "Mads M. Pedersen" <mmpe@dtu.dk>
 Project-URL: Homepage, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface
 Project-URL: Bug Tracker, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Multiclass_interface-1.1/README.md` & `multiclass_interface-1.2/README.md`

 * *Files identical despite different names*

### Comparing `Multiclass_interface-1.1/multiclass_interface/mpi_interface.py` & `multiclass_interface-1.2/multiclass_interface/mpi_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import numpy as np
 import sys
-import os
-import subprocess
 import traceback
 import inspect
-from enum import Enum
 
-if 'SLURM_NTASKS' in os.environ:
-    mpi = int(os.environ['SLURM_NTASKS']) > 1
-elif any([k in os.environ for k in ['MPI_LOCALNRANKS', 'OMPI_COMM_WORLD_SIZE']]):
-    mpi = True
-else:
-    mpi = subprocess.run("python -c 'from mpi4py import MPI'", shell=True,
-                         check=False, stderr=subprocess.PIPE).returncode == 0
+comm = None
+size = 1
+rank = 0
+name = ""
+main = True
 
-if mpi:
+
+def activate_mpi():
+    global comm, size, rank, name, main
     from mpi4py import MPI
     comm = MPI.COMM_WORLD
     size = MPI.COMM_WORLD.Get_size()
     rank = MPI.COMM_WORLD.Get_rank()
     name = MPI.Get_processor_name()
-else:
-    size = 1
+    main = rank == 0
+
 
 MPIClassInterfaceAttributes = {
     'close',
     'use_rank',
     'cls',
     'work_loop',
     'object',
```

### Comparing `Multiclass_interface-1.1/multiclass_interface/multi_object_list.py` & `multiclass_interface-1.2/multiclass_interface/multi_object_list.py`

 * *Files identical despite different names*

### Comparing `Multiclass_interface-1.1/multiclass_interface/multiprocess_interface.py` & `multiclass_interface-1.2/multiclass_interface/multiprocess_interface.py`

 * *Files identical despite different names*

### Comparing `Multiclass_interface-1.1/multiclass_interface/tests/my_test_cls.py` & `multiclass_interface-1.2/multiclass_interface/tests/my_test_cls.py`

 * *Files identical despite different names*

### Comparing `Multiclass_interface-1.1/multiclass_interface/tests/test_mpi.py` & `multiclass_interface-1.2/multiclass_interface/tests/test_mpi.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,17 @@
     with ProcessClass(MyTest) as cls:
         myTest = cls(1)
         assert myTest.get_id() == 1
     print("done, test_mpi_ProcessClass")
 
 
 def mpitest_all():
+    mpi_interface.activate_mpi()
     mpi_interface.exit_mpi_on_close = False
-    from mpi4py import MPI
-    rank = MPI.COMM_WORLD.Get_rank()
+    rank = mpi_interface.rank
     from multiclass_interface.tests.test_multiprocessinterface import test_attribute, test_missing_attribute, test_execption, test_setattr, test_setattr_method
     mpi_interface.TERMINATE_ON_CLOSE = False
 
     def run(f, *args):
         try:
             if rank == 0:
                 print(f"Rank {rank} start {f.__name__}", flush=True)
```

### Comparing `Multiclass_interface-1.1/multiclass_interface/tests/test_multiclass_list.py` & `multiclass_interface-1.2/multiclass_interface/tests/test_multiclass_list.py`

 * *Files identical despite different names*

### Comparing `Multiclass_interface-1.1/multiclass_interface/tests/test_multiprocessinterface.py` & `multiclass_interface-1.2/multiclass_interface/tests/test_multiprocessinterface.py`

 * *Files identical despite different names*

### Comparing `Multiclass_interface-1.1/pyproject.toml` & `multiclass_interface-1.2/pyproject.toml`

 * *Files identical despite different names*

