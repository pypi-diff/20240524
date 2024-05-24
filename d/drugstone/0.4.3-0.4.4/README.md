# Comparing `tmp/drugstone-0.4.3.tar.gz` & `tmp/drugstone-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drugstone-0.4.3.tar", last modified: Wed Feb  7 12:42:46 2024, max compression
+gzip compressed data, was "dist/drugstone-0.4.4.tar", last modified: Thu May 23 15:06:30 2024, max compression
```

## Comparing `drugstone-0.4.3.tar` & `drugstone-0.4.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.942423 drugstone-0.4.3/
--rw-r--r--   0 michi      (501) staff       (20)     1068 2023-09-29 07:32:46.000000 drugstone-0.4.3/LICENSE
--rw-r--r--   0 michi      (501) staff       (20)    10385 2024-02-07 12:42:46.942584 drugstone-0.4.3/PKG-INFO
--rw-r--r--   0 michi      (501) staff       (20)     9900 2024-02-07 12:42:26.000000 drugstone-0.4.3/README.md
--rw-r--r--   0 michi      (501) staff       (20)      103 2023-09-29 07:32:46.000000 drugstone-0.4.3/pyproject.toml
--rw-r--r--   0 michi      (501) staff       (20)      603 2024-02-07 12:42:46.943757 drugstone-0.4.3/setup.cfg
--rw-r--r--   0 michi      (501) staff       (20)      116 2023-09-29 07:32:46.000000 drugstone-0.4.3/setup.py
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.896061 drugstone-0.4.3/src/
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.913301 drugstone-0.4.3/src/drugstone/
--rw-r--r--   0 michi      (501) staff       (20)      929 2024-01-29 11:12:37.000000 drugstone-0.4.3/src/drugstone/__init__.py
--rw-r--r--   0 michi      (501) staff       (20)     2090 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/deep_search.py
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.923198 drugstone-0.4.3/src/drugstone/external_scripts/
--rw-r--r--   0 michi      (501) staff       (20)        0 2024-01-18 14:30:32.000000 drugstone-0.4.3/src/drugstone/external_scripts/__init__.py
--rw-r--r--   0 michi      (501) staff       (20)      805 2024-01-18 16:43:26.000000 drugstone-0.4.3/src/drugstone/external_scripts/build_network.py
--rw-r--r--   0 michi      (501) staff       (20)     1891 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/external_scripts/map_nodes_to_internal_ids.py
--rw-r--r--   0 michi      (501) staff       (20)      909 2024-01-29 11:10:41.000000 drugstone-0.4.3/src/drugstone/fetching.py
--rw-r--r--   0 michi      (501) staff       (20)      618 2024-01-29 11:07:09.000000 drugstone-0.4.3/src/drugstone/license.py
--rw-r--r--   0 michi      (501) staff       (20)     4144 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/new_task.py
--rw-r--r--   0 michi      (501) staff       (20)     2943 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/new_tasks.py
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.932247 drugstone-0.4.3/src/drugstone/scripts/
--rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.3/src/drugstone/scripts/__init__.py
--rw-r--r--   0 michi      (501) staff       (20)     1392 2024-01-22 07:40:32.000000 drugstone-0.4.3/src/drugstone/scripts/add_edges_to_genes.py
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.934190 drugstone-0.4.3/src/drugstone/scripts/constants/
--rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.3/src/drugstone/scripts/constants/__init__.py
--rw-r--r--   0 michi      (501) staff       (20)     2539 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/scripts/constants/task_parameter.py
--rw-r--r--   0 michi      (501) staff       (20)      687 2024-01-29 11:17:02.000000 drugstone-0.4.3/src/drugstone/scripts/constants/url.py
--rw-r--r--   0 michi      (501) staff       (20)      637 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/scripts/fetch_edges.py
--rw-r--r--   0 michi      (501) staff       (20)     1017 2023-09-29 07:32:46.000000 drugstone-0.4.3/src/drugstone/scripts/merge_results.py
--rw-r--r--   0 michi      (501) staff       (20)     4852 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/scripts/normalize_nodes.py
--rw-r--r--   0 michi      (501) staff       (20)     4941 2024-01-29 11:20:05.000000 drugstone-0.4.3/src/drugstone/scripts/normalize_task_parameter.py
--rw-r--r--   0 michi      (501) staff       (20)      383 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/scripts/request_task_info.py
--rw-r--r--   0 michi      (501) staff       (20)      479 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/scripts/request_task_result.py
--rw-r--r--   0 michi      (501) staff       (20)      582 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/scripts/start_task.py
--rw-r--r--   0 michi      (501) staff       (20)      396 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/scripts/task_id.py
--rw-r--r--   0 michi      (501) staff       (20)     1007 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/scripts/wait_for_task_to_finish.py
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.937697 drugstone-0.4.3/src/drugstone/task/
--rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.3/src/drugstone/task/__init__.py
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.939450 drugstone-0.4.3/src/drugstone/task/models/
--rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.3/src/drugstone/task/models/__init__.py
--rw-r--r--   0 michi      (501) staff       (20)      645 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/task/models/drug.py
--rw-r--r--   0 michi      (501) staff       (20)     1076 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/task/models/gene.py
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.942005 drugstone-0.4.3/src/drugstone/task/scripts/
--rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.3/src/drugstone/task/scripts/__init__.py
--rw-r--r--   0 michi      (501) staff       (20)      931 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/task/scripts/create_path.py
--rw-r--r--   0 michi      (501) staff       (20)     2713 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/task/scripts/download_network_graph.py
--rw-r--r--   0 michi      (501) staff       (20)      517 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/task/scripts/make_upsetplot.py
--rw-r--r--   0 michi      (501) staff       (20)     1660 2024-02-07 11:04:05.000000 drugstone-0.4.3/src/drugstone/task/task.py
--rw-r--r--   0 michi      (501) staff       (20)     5430 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/task/task_result.py
--rw-r--r--   0 michi      (501) staff       (20)     3076 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/task/tasks.py
--rw-r--r--   0 michi      (501) staff       (20)     2844 2024-01-29 11:12:16.000000 drugstone-0.4.3/src/drugstone/task/tasks_result.py
-drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-02-07 12:42:46.920555 drugstone-0.4.3/src/drugstone.egg-info/
--rw-r--r--   0 michi      (501) staff       (20)    10385 2024-02-07 12:42:46.000000 drugstone-0.4.3/src/drugstone.egg-info/PKG-INFO
--rw-r--r--   0 michi      (501) staff       (20)     1569 2024-02-07 12:42:46.000000 drugstone-0.4.3/src/drugstone.egg-info/SOURCES.txt
--rw-r--r--   0 michi      (501) staff       (20)        1 2024-02-07 12:42:46.000000 drugstone-0.4.3/src/drugstone.egg-info/dependency_links.txt
--rw-r--r--   0 michi      (501) staff       (20)       40 2024-02-07 12:42:46.000000 drugstone-0.4.3/src/drugstone.egg-info/requires.txt
--rw-r--r--   0 michi      (501) staff       (20)       10 2024-02-07 12:42:46.000000 drugstone-0.4.3/src/drugstone.egg-info/top_level.txt
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:30.309251 drugstone-0.4.4/
+-rw-r--r--   0 michi      (501) staff       (20)     1068 2023-09-29 07:32:46.000000 drugstone-0.4.4/LICENSE
+-rw-r--r--   0 michi      (501) staff       (20)    11778 2024-05-23 15:06:30.309918 drugstone-0.4.4/PKG-INFO
+-rw-r--r--   0 michi      (501) staff       (20)    11293 2024-05-23 15:05:35.000000 drugstone-0.4.4/README.md
+-rw-r--r--   0 michi      (501) staff       (20)      103 2023-09-29 07:32:46.000000 drugstone-0.4.4/pyproject.toml
+-rw-r--r--   0 michi      (501) staff       (20)      603 2024-05-23 15:06:30.314843 drugstone-0.4.4/setup.cfg
+-rw-r--r--   0 michi      (501) staff       (20)      116 2023-09-29 07:32:46.000000 drugstone-0.4.4/setup.py
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:28.926595 drugstone-0.4.4/src/
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:29.046504 drugstone-0.4.4/src/drugstone/
+-rw-r--r--   0 michi      (501) staff       (20)      929 2024-01-29 11:12:37.000000 drugstone-0.4.4/src/drugstone/__init__.py
+-rw-r--r--   0 michi      (501) staff       (20)     2090 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/deep_search.py
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:29.094669 drugstone-0.4.4/src/drugstone/external_scripts/
+-rw-r--r--   0 michi      (501) staff       (20)        0 2024-01-18 14:30:32.000000 drugstone-0.4.4/src/drugstone/external_scripts/__init__.py
+-rw-r--r--   0 michi      (501) staff       (20)      805 2024-01-18 16:43:26.000000 drugstone-0.4.4/src/drugstone/external_scripts/build_network.py
+-rw-r--r--   0 michi      (501) staff       (20)     1891 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/external_scripts/map_nodes_to_internal_ids.py
+-rw-r--r--   0 michi      (501) staff       (20)      909 2024-01-29 11:10:41.000000 drugstone-0.4.4/src/drugstone/fetching.py
+-rw-r--r--   0 michi      (501) staff       (20)      618 2024-01-29 11:07:09.000000 drugstone-0.4.4/src/drugstone/license.py
+-rw-r--r--   0 michi      (501) staff       (20)     6058 2024-05-23 12:42:31.000000 drugstone-0.4.4/src/drugstone/new_task.py
+-rw-r--r--   0 michi      (501) staff       (20)     2943 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/new_tasks.py
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:29.176364 drugstone-0.4.4/src/drugstone/scripts/
+-rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.4/src/drugstone/scripts/__init__.py
+-rw-r--r--   0 michi      (501) staff       (20)     1392 2024-01-22 07:40:32.000000 drugstone-0.4.4/src/drugstone/scripts/add_edges_to_genes.py
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:29.204428 drugstone-0.4.4/src/drugstone/scripts/constants/
+-rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.4/src/drugstone/scripts/constants/__init__.py
+-rw-r--r--   0 michi      (501) staff       (20)     2539 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/scripts/constants/task_parameter.py
+-rw-r--r--   0 michi      (501) staff       (20)      687 2024-01-29 11:17:02.000000 drugstone-0.4.4/src/drugstone/scripts/constants/url.py
+-rw-r--r--   0 michi      (501) staff       (20)      637 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/scripts/fetch_edges.py
+-rw-r--r--   0 michi      (501) staff       (20)     1017 2023-09-29 07:32:46.000000 drugstone-0.4.4/src/drugstone/scripts/merge_results.py
+-rw-r--r--   0 michi      (501) staff       (20)     4882 2024-02-08 14:43:52.000000 drugstone-0.4.4/src/drugstone/scripts/normalize_nodes.py
+-rw-r--r--   0 michi      (501) staff       (20)     4941 2024-01-29 11:20:05.000000 drugstone-0.4.4/src/drugstone/scripts/normalize_task_parameter.py
+-rw-r--r--   0 michi      (501) staff       (20)      666 2024-02-08 14:49:13.000000 drugstone-0.4.4/src/drugstone/scripts/request_task_info.py
+-rw-r--r--   0 michi      (501) staff       (20)      479 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/scripts/request_task_result.py
+-rw-r--r--   0 michi      (501) staff       (20)      582 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/scripts/start_task.py
+-rw-r--r--   0 michi      (501) staff       (20)      396 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/scripts/task_id.py
+-rw-r--r--   0 michi      (501) staff       (20)     1007 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/scripts/wait_for_task_to_finish.py
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:29.234685 drugstone-0.4.4/src/drugstone/task/
+-rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.4/src/drugstone/task/__init__.py
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:29.242045 drugstone-0.4.4/src/drugstone/task/models/
+-rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.4/src/drugstone/task/models/__init__.py
+-rw-r--r--   0 michi      (501) staff       (20)      645 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/task/models/drug.py
+-rw-r--r--   0 michi      (501) staff       (20)     1076 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/task/models/gene.py
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:30.307233 drugstone-0.4.4/src/drugstone/task/scripts/
+-rw-r--r--   0 michi      (501) staff       (20)        0 2023-09-29 07:32:46.000000 drugstone-0.4.4/src/drugstone/task/scripts/__init__.py
+-rw-r--r--   0 michi      (501) staff       (20)      931 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/task/scripts/create_path.py
+-rw-r--r--   0 michi      (501) staff       (20)     2713 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/task/scripts/download_network_graph.py
+-rw-r--r--   0 michi      (501) staff       (20)      517 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/task/scripts/make_upsetplot.py
+-rw-r--r--   0 michi      (501) staff       (20)     1660 2024-02-07 11:04:05.000000 drugstone-0.4.4/src/drugstone/task/task.py
+-rw-r--r--   0 michi      (501) staff       (20)     5430 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/task/task_result.py
+-rw-r--r--   0 michi      (501) staff       (20)     3076 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/task/tasks.py
+-rw-r--r--   0 michi      (501) staff       (20)     2844 2024-01-29 11:12:16.000000 drugstone-0.4.4/src/drugstone/task/tasks_result.py
+drwxr-xr-x   0 michi      (501) staff       (20)        0 2024-05-23 15:06:29.090434 drugstone-0.4.4/src/drugstone.egg-info/
+-rw-r--r--   0 michi      (501) staff       (20)    11778 2024-05-23 15:06:24.000000 drugstone-0.4.4/src/drugstone.egg-info/PKG-INFO
+-rw-r--r--   0 michi      (501) staff       (20)     1569 2024-05-23 15:06:25.000000 drugstone-0.4.4/src/drugstone.egg-info/SOURCES.txt
+-rw-r--r--   0 michi      (501) staff       (20)        1 2024-05-23 15:06:24.000000 drugstone-0.4.4/src/drugstone.egg-info/dependency_links.txt
+-rw-r--r--   0 michi      (501) staff       (20)       40 2024-05-23 15:06:24.000000 drugstone-0.4.4/src/drugstone.egg-info/requires.txt
+-rw-r--r--   0 michi      (501) staff       (20)       10 2024-05-23 15:06:24.000000 drugstone-0.4.4/src/drugstone.egg-info/top_level.txt
```

### Comparing `drugstone-0.4.3/LICENSE` & `drugstone-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/PKG-INFO` & `drugstone-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drugstone
-Version: 0.4.3
+Version: 0.4.4
 Summary: The python package for the https://drugst.one/ platform.
 Home-page: https://github.com/t-ugur/drugstone.git
 Author: Ugur Turhan, Michael Hartung
 Author-email: michael.hartung@uni-hamburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -191,14 +191,49 @@
 u = tasks.get_union()                  
 u.download_json()
 
 i = tasks.get_intersection()
 i.download_json()
 ````
 
+### Use your own network
+You can add custom nodes and edges to the network, which may be considered for the drug-target or the drug search. Also, it is possible to ONLY consider your provided PPI-network and exclude PPI-edges provdided by Drugst.One.
+Please note that this is an experimental feature and is still being tested.
+```python
+import drugstone
+
+seeds = [
+    "CFTR", "TGFB1"
+]
+
+parameters = {
+    "target": "drug",
+    "algorithm": "trustrank",
+    "pdiDataset": 'nedrex',     # drug nodes and edges will still be taken from Drugst.One
+    "custom_edges": [   # add here your edges for you custom PPI
+        {"from": "CFTR", "to": "SCNN1G"},
+        {"from": "CFTR", "to": "SCNN1B"},
+        {"from": "TGFB1", "to": "DCTN4"},
+        {"from": "SCNN1B", "to": "SCNN1A"},
+        {"from": "SCNN1B", "to": "CLCA4"},
+        {"from": "TNFRSF1A", "to": "FCGR2A"}
+    ],
+    "exclude_drugstone_ppi_edges": True, # this parameter removes all Drugst.One PPI edges (only if edges in 'custom_edges' are provided)
+    "identifier": "symbol",
+    "include_indirect_drugs": True,
+    "network_nodes": ["CFTR", "TGFB1", "SCNN1B",    # add here your nodes for you custom PPI
+                      "DCTN4", "SCNN1A", "SCNN1G",
+                      "CLCA4", "TNFRSF1A", "FCGR2A"]
+}
+task = drugstone.new_task(seeds, parameters)
+r = task.get_result()
+genes = r.get_genes()
+drugs = r.get_drugs()
+```
+
 
 ## Combine a drug-target search with a drug search
 This will perform a drug-target search for the seed genes 
 and then use the drug-target search results and the seed genes
 to perform a drug-search.
 Finally, a Task with the drug-search results will be returned. 
 ````python
```

### Comparing `drugstone-0.4.3/README.md` & `drugstone-0.4.4/src/drugstone.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: drugstone
+Version: 0.4.4
+Summary: The python package for the https://drugst.one/ platform.
+Home-page: https://github.com/t-ugur/drugstone.git
+Author: Ugur Turhan, Michael Hartung
+Author-email: michael.hartung@uni-hamburg.de
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">
 <img src="https://drugst.one/assets/logo_black.png" width="300">
 </h1><br>
 
 This is the python package for the drugst.one platform. It offers tools for network-based drug repurposing and 
 is a programmatic interface to Drugst.one.
 
@@ -177,14 +191,49 @@
 u = tasks.get_union()                  
 u.download_json()
 
 i = tasks.get_intersection()
 i.download_json()
 ````
 
+### Use your own network
+You can add custom nodes and edges to the network, which may be considered for the drug-target or the drug search. Also, it is possible to ONLY consider your provided PPI-network and exclude PPI-edges provdided by Drugst.One.
+Please note that this is an experimental feature and is still being tested.
+```python
+import drugstone
+
+seeds = [
+    "CFTR", "TGFB1"
+]
+
+parameters = {
+    "target": "drug",
+    "algorithm": "trustrank",
+    "pdiDataset": 'nedrex',     # drug nodes and edges will still be taken from Drugst.One
+    "custom_edges": [   # add here your edges for you custom PPI
+        {"from": "CFTR", "to": "SCNN1G"},
+        {"from": "CFTR", "to": "SCNN1B"},
+        {"from": "TGFB1", "to": "DCTN4"},
+        {"from": "SCNN1B", "to": "SCNN1A"},
+        {"from": "SCNN1B", "to": "CLCA4"},
+        {"from": "TNFRSF1A", "to": "FCGR2A"}
+    ],
+    "exclude_drugstone_ppi_edges": True, # this parameter removes all Drugst.One PPI edges (only if edges in 'custom_edges' are provided)
+    "identifier": "symbol",
+    "include_indirect_drugs": True,
+    "network_nodes": ["CFTR", "TGFB1", "SCNN1B",    # add here your nodes for you custom PPI
+                      "DCTN4", "SCNN1A", "SCNN1G",
+                      "CLCA4", "TNFRSF1A", "FCGR2A"]
+}
+task = drugstone.new_task(seeds, parameters)
+r = task.get_result()
+genes = r.get_genes()
+drugs = r.get_drugs()
+```
+
 
 ## Combine a drug-target search with a drug search
 This will perform a drug-target search for the seed genes 
 and then use the drug-target search results and the seed genes
 to perform a drug-search.
 Finally, a Task with the drug-search results will be returned. 
 ````python
@@ -342,8 +391,8 @@
 parameters = {'identifier': 'symbol', 'ppiDataset': 'IID'}
 
 network = drugstone.build_network(genes, parameters)
 ```
 
 
 Copyright: 2024 - Institute for Computational Systems Biology 
-by Prof. Dr. Jan Baumbach.
+by Prof. Dr. Jan Baumbach.
```

### Comparing `drugstone-0.4.3/setup.cfg` & `drugstone-0.4.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drugstone
-version = 0.4.3
+version = 0.4.4
 author = Ugur Turhan, Michael Hartung
 author_email = michael.hartung@uni-hamburg.de
 description = The python package for the https://drugst.one/ platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/t-ugur/drugstone.git
 classifiers =
```

### Comparing `drugstone-0.4.3/src/drugstone/__init__.py` & `drugstone-0.4.4/src/drugstone/__init__.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/deep_search.py` & `drugstone-0.4.4/src/drugstone/deep_search.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/external_scripts/build_network.py` & `drugstone-0.4.4/src/drugstone/external_scripts/build_network.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/external_scripts/map_nodes_to_internal_ids.py` & `drugstone-0.4.4/src/drugstone/external_scripts/map_nodes_to_internal_ids.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/fetching.py` & `drugstone-0.4.4/src/drugstone/fetching.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/license.py` & `drugstone-0.4.4/src/drugstone/license.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/new_tasks.py` & `drugstone-0.4.4/src/drugstone/new_tasks.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/scripts/add_edges_to_genes.py` & `drugstone-0.4.4/src/drugstone/scripts/add_edges_to_genes.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/scripts/constants/task_parameter.py` & `drugstone-0.4.4/src/drugstone/scripts/constants/task_parameter.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/scripts/constants/url.py` & `drugstone-0.4.4/src/drugstone/scripts/constants/url.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/scripts/fetch_edges.py` & `drugstone-0.4.4/src/drugstone/scripts/fetch_edges.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/scripts/merge_results.py` & `drugstone-0.4.4/src/drugstone/scripts/merge_results.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/scripts/normalize_nodes.py` & `drugstone-0.4.4/src/drugstone/scripts/normalize_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
     # Adds to the genes if it's a seed or not.
     is_seed = results["nodeAttributes"]["isSeed"]
     for _, g_details in genes.items():
         g_details["is_seed"] = False if g_details[identifier][0] not in is_seed else is_seed[g_details[identifier][0]]
 
     # Add information if node is result node
+    print('results', results)
     for node in results['targetNodes']:
         try:
             # node is drug
             label = drugstone_drug_id_to_label[node]
             drugs[label]['isResult'] = True
         except KeyError:
             # node is gene
```

### Comparing `drugstone-0.4.3/src/drugstone/scripts/normalize_task_parameter.py` & `drugstone-0.4.4/src/drugstone/scripts/normalize_task_parameter.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/scripts/start_task.py` & `drugstone-0.4.4/src/drugstone/scripts/start_task.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/scripts/wait_for_task_to_finish.py` & `drugstone-0.4.4/src/drugstone/scripts/wait_for_task_to_finish.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/models/drug.py` & `drugstone-0.4.4/src/drugstone/task/models/drug.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/models/gene.py` & `drugstone-0.4.4/src/drugstone/task/models/gene.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/scripts/create_path.py` & `drugstone-0.4.4/src/drugstone/task/scripts/create_path.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/scripts/download_network_graph.py` & `drugstone-0.4.4/src/drugstone/task/scripts/download_network_graph.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/scripts/make_upsetplot.py` & `drugstone-0.4.4/src/drugstone/task/scripts/make_upsetplot.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/task.py` & `drugstone-0.4.4/src/drugstone/task/task.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/task_result.py` & `drugstone-0.4.4/src/drugstone/task/task_result.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/tasks.py` & `drugstone-0.4.4/src/drugstone/task/tasks.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone/task/tasks_result.py` & `drugstone-0.4.4/src/drugstone/task/tasks_result.py`

 * *Files identical despite different names*

### Comparing `drugstone-0.4.3/src/drugstone.egg-info/PKG-INFO` & `drugstone-0.4.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: drugstone
-Version: 0.4.3
-Summary: The python package for the https://drugst.one/ platform.
-Home-page: https://github.com/t-ugur/drugstone.git
-Author: Ugur Turhan, Michael Hartung
-Author-email: michael.hartung@uni-hamburg.de
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
 <img src="https://drugst.one/assets/logo_black.png" width="300">
 </h1><br>
 
 This is the python package for the drugst.one platform. It offers tools for network-based drug repurposing and 
 is a programmatic interface to Drugst.one.
 
@@ -191,14 +177,49 @@
 u = tasks.get_union()                  
 u.download_json()
 
 i = tasks.get_intersection()
 i.download_json()
 ````
 
+### Use your own network
+You can add custom nodes and edges to the network, which may be considered for the drug-target or the drug search. Also, it is possible to ONLY consider your provided PPI-network and exclude PPI-edges provdided by Drugst.One.
+Please note that this is an experimental feature and is still being tested.
+```python
+import drugstone
+
+seeds = [
+    "CFTR", "TGFB1"
+]
+
+parameters = {
+    "target": "drug",
+    "algorithm": "trustrank",
+    "pdiDataset": 'nedrex',     # drug nodes and edges will still be taken from Drugst.One
+    "custom_edges": [   # add here your edges for you custom PPI
+        {"from": "CFTR", "to": "SCNN1G"},
+        {"from": "CFTR", "to": "SCNN1B"},
+        {"from": "TGFB1", "to": "DCTN4"},
+        {"from": "SCNN1B", "to": "SCNN1A"},
+        {"from": "SCNN1B", "to": "CLCA4"},
+        {"from": "TNFRSF1A", "to": "FCGR2A"}
+    ],
+    "exclude_drugstone_ppi_edges": True, # this parameter removes all Drugst.One PPI edges (only if edges in 'custom_edges' are provided)
+    "identifier": "symbol",
+    "include_indirect_drugs": True,
+    "network_nodes": ["CFTR", "TGFB1", "SCNN1B",    # add here your nodes for you custom PPI
+                      "DCTN4", "SCNN1A", "SCNN1G",
+                      "CLCA4", "TNFRSF1A", "FCGR2A"]
+}
+task = drugstone.new_task(seeds, parameters)
+r = task.get_result()
+genes = r.get_genes()
+drugs = r.get_drugs()
+```
+
 
 ## Combine a drug-target search with a drug search
 This will perform a drug-target search for the seed genes 
 and then use the drug-target search results and the seed genes
 to perform a drug-search.
 Finally, a Task with the drug-search results will be returned. 
 ````python
@@ -356,8 +377,8 @@
 parameters = {'identifier': 'symbol', 'ppiDataset': 'IID'}
 
 network = drugstone.build_network(genes, parameters)
 ```
 
 
 Copyright: 2024 - Institute for Computational Systems Biology 
-by Prof. Dr. Jan Baumbach.
+by Prof. Dr. Jan Baumbach.
```

### Comparing `drugstone-0.4.3/src/drugstone.egg-info/SOURCES.txt` & `drugstone-0.4.4/src/drugstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

