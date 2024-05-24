# Comparing `tmp/skale_contracts-1.0.1a7.tar.gz` & `tmp/skale_contracts-1.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale_contracts-1.0.1a7.tar", last modified: Wed May 22 17:20:45 2024, max compression
+gzip compressed data, was "skale_contracts-1.0.1a8.tar", last modified: Fri May 24 07:09:47 2024, max compression
```

## Comparing `skale_contracts-1.0.1a7.tar` & `skale_contracts-1.0.1a8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:45.648006 skale_contracts-1.0.1a7/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 17:20:45.648006 skale_contracts-1.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-22 17:20:45.648006 skale_contracts-1.0.1a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:45.644006 skale_contracts-1.0.1a7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:45.644006 skale_contracts-1.0.1a7/src/skale_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/project_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:45.648006 skale_contracts-1.0.1a7/src/skale_contracts/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/projects/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/projects/ima.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/projects/skale_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/projects/skale_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 17:20:38.000000 skale_contracts-1.0.1a7/src/skale_contracts/skale_contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:20:45.648006 skale_contracts-1.0.1a7/src/skale_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 17:20:45.000000 skale_contracts-1.0.1a7/src/skale_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 17:20:45.000000 skale_contracts-1.0.1a7/src/skale_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:20:45.000000 skale_contracts-1.0.1a7/src/skale_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 17:20:45.000000 skale_contracts-1.0.1a7/src/skale_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 17:20:45.000000 skale_contracts-1.0.1a7/src/skale_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 17:20:43.000000 skale_contracts-1.0.1a7/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:09:47.073514 skale_contracts-1.0.1a8/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-24 07:09:47.073514 skale_contracts-1.0.1a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-24 07:09:47.077514 skale_contracts-1.0.1a8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:09:47.069513 skale_contracts-1.0.1a8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:09:47.073514 skale_contracts-1.0.1a8/src/skale_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/project_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:09:47.073514 skale_contracts-1.0.1a8/src/skale_contracts/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/projects/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/projects/ima.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/projects/skale_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/projects/skale_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-24 07:09:39.000000 skale_contracts-1.0.1a8/src/skale_contracts/skale_contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:09:47.073514 skale_contracts-1.0.1a8/src/skale_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-24 07:09:47.000000 skale_contracts-1.0.1a8/src/skale_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-24 07:09:47.000000 skale_contracts-1.0.1a8/src/skale_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:09:47.000000 skale_contracts-1.0.1a8/src/skale_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 07:09:47.000000 skale_contracts-1.0.1a8/src/skale_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 07:09:47.000000 skale_contracts-1.0.1a8/src/skale_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 07:09:45.000000 skale_contracts-1.0.1a8/version.txt
```

### Comparing `skale_contracts-1.0.1a7/PKG-INFO` & `skale_contracts-1.0.1a8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 1.0.1a7
+Version: 1.0.1a8
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale_contracts-1.0.1a7/setup.cfg` & `skale_contracts-1.0.1a8/setup.cfg`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/instance.py` & `skale_contracts-1.0.1a8/src/skale_contracts/instance.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/metadata.py` & `skale_contracts-1.0.1a8/src/skale_contracts/metadata.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/network.py` & `skale_contracts-1.0.1a8/src/skale_contracts/network.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/project.py` & `skale_contracts-1.0.1a8/src/skale_contracts/project.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/project_factory.py` & `skale_contracts-1.0.1a8/src/skale_contracts/project_factory.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/projects/context.py` & `skale_contracts-1.0.1a8/src/skale_contracts/projects/context.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/projects/ima.py` & `skale_contracts-1.0.1a8/src/skale_contracts/projects/ima.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/projects/skale_allocator.py` & `skale_contracts-1.0.1a8/src/skale_contracts/projects/skale_allocator.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/projects/skale_manager.py` & `skale_contracts-1.0.1a8/src/skale_contracts/projects/skale_manager.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts/skale_contracts.py` & `skale_contracts-1.0.1a8/src/skale_contracts/skale_contracts.py`

 * *Files identical despite different names*

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts.egg-info/PKG-INFO` & `skale_contracts-1.0.1a8/src/skale_contracts.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale-contracts
-Version: 1.0.1a7
+Version: 1.0.1a8
 Summary: A tool for access to SKALE smart contracts
 Home-page: https://github.com/skalenetwork/skale-contracts
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `skale_contracts-1.0.1a7/src/skale_contracts.egg-info/SOURCES.txt` & `skale_contracts-1.0.1a8/src/skale_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

