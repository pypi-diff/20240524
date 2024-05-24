# Comparing `tmp/scprel-1.2.tar.gz` & `tmp/scprel-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scprel-1.2.tar", last modified: Thu May 23 10:34:31 2024, max compression
+gzip compressed data, was "dist/scprel-1.3.tar", last modified: Fri May 24 13:02:48 2024, max compression
```

## Comparing `scprel-1.2.tar` & `scprel-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2024-05-23 10:34:31.000000 scprel-1.2/
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1084 2024-05-22 14:02:32.000000 scprel-1.2/LICENSE.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     2976 2024-05-23 10:34:31.000000 scprel-1.2/PKG-INFO
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1825 2023-11-16 12:49:34.000000 scprel-1.2/README.md
-drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2024-05-23 10:34:31.000000 scprel-1.2/scprel/
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       36 2023-11-15 13:33:12.000000 scprel-1.2/scprel/__init__.py
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)    12305 2024-05-23 10:30:15.000000 scprel-1.2/scprel/functions.py
-drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2024-05-23 10:34:31.000000 scprel-1.2/scprel.egg-info/
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     2976 2024-05-23 10:34:26.000000 scprel-1.2/scprel.egg-info/PKG-INFO
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)      218 2024-05-23 10:34:28.000000 scprel-1.2/scprel.egg-info/SOURCES.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        1 2024-05-23 10:34:26.000000 scprel-1.2/scprel.egg-info/dependency_links.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       81 2024-05-23 10:34:26.000000 scprel-1.2/scprel.egg-info/requires.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        7 2024-05-23 10:34:26.000000 scprel-1.2/scprel.egg-info/top_level.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       38 2024-05-23 10:34:31.000000 scprel-1.2/setup.cfg
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1737 2024-05-23 10:31:07.000000 scprel-1.2/setup.py
+drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2024-05-24 13:02:48.000000 scprel-1.3/
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1084 2024-05-22 14:02:32.000000 scprel-1.3/LICENSE.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     2976 2024-05-24 13:02:48.000000 scprel-1.3/PKG-INFO
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1825 2023-11-16 12:49:34.000000 scprel-1.3/README.md
+drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2024-05-24 13:02:48.000000 scprel-1.3/scprel/
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       36 2023-11-15 13:33:12.000000 scprel-1.3/scprel/__init__.py
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)    12307 2024-05-24 12:58:03.000000 scprel-1.3/scprel/functions.py
+drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2024-05-24 13:02:48.000000 scprel-1.3/scprel.egg-info/
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     2976 2024-05-24 13:02:46.000000 scprel-1.3/scprel.egg-info/PKG-INFO
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)      218 2024-05-24 13:02:47.000000 scprel-1.3/scprel.egg-info/SOURCES.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        1 2024-05-24 13:02:46.000000 scprel-1.3/scprel.egg-info/dependency_links.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       81 2024-05-24 13:02:46.000000 scprel-1.3/scprel.egg-info/requires.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        7 2024-05-24 13:02:46.000000 scprel-1.3/scprel.egg-info/top_level.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       38 2024-05-24 13:02:48.000000 scprel-1.3/setup.cfg
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1737 2024-05-24 13:01:17.000000 scprel-1.3/setup.py
```

### Comparing `scprel-1.2/LICENSE.txt` & `scprel-1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scprel-1.2/PKG-INFO` & `scprel-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scprel
-Version: 1.2
+Version: 1.3
 Summary: Single-cell data preprocessing for multiple samples.
 Home-page: https://pypi.org/project/scprel/
 Author: GPuzanov (Grigory Puzanov)
 Author-email: <grigorypuzanov@gmail.com>
 License: UNKNOWN
 Description: ## Scprel - Single-Cell Data Preprocessing in Python
```

### Comparing `scprel-1.2/README.md` & `scprel-1.3/README.md`

 * *Files identical despite different names*

### Comparing `scprel-1.2/scprel/functions.py` & `scprel-1.3/scprel/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                'Myocytes',  'Natural killer T cells', 'Neutrophils', 'NK cells', 'Nuocytes',
                 'Plasma cells','Plasmacytoid dendritic cells', 'Platelets',
                 'Red pulp macrophages', 'Reticulocytes',  'T cytotoxic cells',
                'T follicular helper cells', 'T helper cells', 'T memory cells',
                'T regulatory cells', 'Thymocytes', 'Transient cells',
                ]
         # Filter by canonical_marker and human
-        markers = markers[markers['human'].isin([True])]
+        markers = markers[markers['human'].isin(['True'])]
         #&(markers['canonical_marker']=='True')
           
         # Remove duplicated entries
         markers = markers[~markers.duplicated(['cell_type', 'genesymbol'])]
         print('Cell types annotation...')
         
         for i in samr:
```

### Comparing `scprel-1.2/scprel.egg-info/PKG-INFO` & `scprel-1.3/scprel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scprel
-Version: 1.2
+Version: 1.3
 Summary: Single-cell data preprocessing for multiple samples.
 Home-page: https://pypi.org/project/scprel/
 Author: GPuzanov (Grigory Puzanov)
 Author-email: <grigorypuzanov@gmail.com>
 License: UNKNOWN
 Description: ## Scprel - Single-Cell Data Preprocessing in Python
```

### Comparing `scprel-1.2/setup.py` & `scprel-1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 #import codecs
 
-VERSION = '1.2'
+VERSION = '1.3'
 DESCRIPTION = 'Single-cell data preprocessing for multiple samples.'
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 #with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
```

