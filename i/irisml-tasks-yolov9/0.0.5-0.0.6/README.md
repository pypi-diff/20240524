# Comparing `tmp/irisml_tasks_yolov9-0.0.5.tar.gz` & `tmp/irisml_tasks_yolov9-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml_tasks_yolov9-0.0.5.tar", last modified: Fri May 10 07:05:36 2024, max compression
+gzip compressed data, was "irisml_tasks_yolov9-0.0.6.tar", last modified: Fri May 24 21:03:57 2024, max compression
```

## Comparing `irisml_tasks_yolov9-0.0.5.tar` & `irisml_tasks_yolov9-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:05:36.714450 irisml_tasks_yolov9-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-10 07:05:36.714450 irisml_tasks_yolov9-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:05:36.706451 irisml_tasks_yolov9-0.0.5/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:05:36.710451 irisml_tasks_yolov9-0.0.5/irisml/tasks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:05:36.710451 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:05:36.710451 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/gelan.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/gelanc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/gelane.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/yolov9.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/yolov9c.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/yolov9e.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/irisml/tasks/load_yolov9_prediction_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:05:36.714450 irisml_tasks_yolov9-0.0.5/irisml_tasks_yolov9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-10 07:05:36.000000 irisml_tasks_yolov9-0.0.5/irisml_tasks_yolov9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 07:05:36.000000 irisml_tasks_yolov9-0.0.5/irisml_tasks_yolov9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:05:36.000000 irisml_tasks_yolov9-0.0.5/irisml_tasks_yolov9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 07:05:36.000000 irisml_tasks_yolov9-0.0.5/irisml_tasks_yolov9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 07:05:36.000000 irisml_tasks_yolov9-0.0.5/irisml_tasks_yolov9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:05:36.714450 irisml_tasks_yolov9-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:05:36.714450 irisml_tasks_yolov9-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/test/test_create_yolov9_detection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-10 07:03:28.000000 irisml_tasks_yolov9-0.0.5/test/test_load_yolov9_prediction_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:03:57.450328 irisml_tasks_yolov9-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-24 21:03:57.450328 irisml_tasks_yolov9-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:03:57.442328 irisml_tasks_yolov9-0.0.6/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:03:57.446328 irisml_tasks_yolov9-0.0.6/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:03:57.446328 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:03:57.450328 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/gelan.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/gelanc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/gelane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/yolov9.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/yolov9c.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/yolov9e.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/irisml/tasks/load_yolov9_prediction_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:03:57.450328 irisml_tasks_yolov9-0.0.6/irisml_tasks_yolov9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-24 21:03:57.000000 irisml_tasks_yolov9-0.0.6/irisml_tasks_yolov9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-24 21:03:57.000000 irisml_tasks_yolov9-0.0.6/irisml_tasks_yolov9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:03:57.000000 irisml_tasks_yolov9-0.0.6/irisml_tasks_yolov9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 21:03:57.000000 irisml_tasks_yolov9-0.0.6/irisml_tasks_yolov9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 21:03:57.000000 irisml_tasks_yolov9-0.0.6/irisml_tasks_yolov9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:03:57.450328 irisml_tasks_yolov9-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:03:57.450328 irisml_tasks_yolov9-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/test/test_create_yolov9_detection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-24 21:01:44.000000 irisml_tasks_yolov9-0.0.6/test/test_load_yolov9_prediction_results.py
```

### Comparing `irisml_tasks_yolov9-0.0.5/LICENSE` & `irisml_tasks_yolov9-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/PKG-INFO` & `irisml_tasks_yolov9-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-yolov9
-Version: 0.0.5
+Version: 0.0.6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: irisml
 Requires-Dist: pyyolov9<1
 
 # irisml-tasks-yolov9
```

### Comparing `irisml_tasks_yolov9-0.0.5/README.md` & `irisml_tasks_yolov9-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py` & `irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/gelan.yaml` & `irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/gelan.yaml`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/gelanc.yaml` & `irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/gelanc.yaml`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/gelane.yaml` & `irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/gelane.yaml`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/yolov9.yaml` & `irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/yolov9.yaml`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/yolov9c.yaml` & `irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/yolov9c.yaml`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml/tasks/create_yolov9_detection_model/resources/yolov9e.yaml` & `irisml_tasks_yolov9-0.0.6/irisml/tasks/create_yolov9_detection_model/resources/yolov9e.yaml`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml/tasks/load_yolov9_prediction_results.py` & `irisml_tasks_yolov9-0.0.6/irisml/tasks/load_yolov9_prediction_results.py`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/irisml_tasks_yolov9.egg-info/PKG-INFO` & `irisml_tasks_yolov9-0.0.6/irisml_tasks_yolov9.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-yolov9
-Version: 0.0.5
+Version: 0.0.6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: irisml
 Requires-Dist: pyyolov9<1
 
 # irisml-tasks-yolov9
```

### Comparing `irisml_tasks_yolov9-0.0.5/irisml_tasks_yolov9.egg-info/SOURCES.txt` & `irisml_tasks_yolov9-0.0.6/irisml_tasks_yolov9.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+irisml/tasks/create_yolov9_dataset.py
 irisml/tasks/load_yolov9_prediction_results.py
 irisml/tasks/create_yolov9_detection_model/__init__.py
 irisml/tasks/create_yolov9_detection_model/create_yolov9_detection_model.py
 irisml/tasks/create_yolov9_detection_model/resources/gelan.yaml
 irisml/tasks/create_yolov9_detection_model/resources/gelanc.yaml
 irisml/tasks/create_yolov9_detection_model/resources/gelane.yaml
 irisml/tasks/create_yolov9_detection_model/resources/yolov9.yaml
```

### Comparing `irisml_tasks_yolov9-0.0.5/test/test_create_yolov9_detection_model.py` & `irisml_tasks_yolov9-0.0.6/test/test_create_yolov9_detection_model.py`

 * *Files identical despite different names*

### Comparing `irisml_tasks_yolov9-0.0.5/test/test_load_yolov9_prediction_results.py` & `irisml_tasks_yolov9-0.0.6/test/test_load_yolov9_prediction_results.py`

 * *Files identical despite different names*

