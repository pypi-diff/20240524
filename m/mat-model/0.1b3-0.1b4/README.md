# Comparing `tmp/mat_model-0.1b3.tar.gz` & `tmp/mat_model-0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat_model-0.1b3.tar", last modified: Thu May 23 19:25:51 2024, max compression
+gzip compressed data, was "mat_model-0.1b4.tar", last modified: Fri May 24 17:41:09 2024, max compression
```

## Comparing `mat_model-0.1b3.tar` & `mat_model-0.1b4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.354019 mat_model-0.1b3/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      106 2024-04-10 16:16:51.000000 mat_model-0.1b3/CHANGELOG.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b3/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_model-0.1b3/MANIFEST.in
--rw-------   0 tarlisportela   (501) staff       (20)    41157 2024-04-19 21:04:47.000000 mat_model-0.1b3/MAT-Tools.drawio
--rwx------   0 tarlisportela   (501) staff       (20)    35812 2024-05-23 19:24:59.000000 mat_model-0.1b3/MAT-model-Tutorial.ipynb
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-23 19:25:51.353787 mat_model-0.1b3/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b3/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      719 2024-04-10 16:09:56.000000 mat_model-0.1b3/Steps to Build.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.353068 mat_model-0.1b3/mat_model.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1098 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)      139 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/requires.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        9 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/top_level.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.347220 mat_model-0.1b3/matmodel/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b3/matmodel/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b3/matmodel/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_model-0.1b3/matmodel/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.349061 mat_model-0.1b3/matmodel/base/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5661 2024-05-23 19:14:12.000000 mat_model-0.1b3/matmodel/base/Aspect.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2429 2024-04-19 21:37:21.000000 mat_model-0.1b3/matmodel/base/Movelet.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     6959 2024-05-22 19:03:55.000000 mat_model-0.1b3/matmodel/base/MultipleAspectSequence.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       83 2024-04-19 21:39:58.000000 mat_model-0.1b3/matmodel/base/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4430 2024-04-19 15:20:13.000000 mat_model-0.1b3/matmodel/base/xSubtrajectory.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      937 2024-04-19 21:33:09.000000 mat_model-0.1b3/matmodel/base/xTrajectory.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.349897 mat_model-0.1b3/matmodel/comparator/
--rw-r--r--   0 tarlisportela   (501) staff       (20)       45 2024-05-23 16:51:19.000000 mat_model-0.1b3/matmodel/comparator/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    13289 2024-05-23 19:17:39.000000 mat_model-0.1b3/matmodel/comparator/distance.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-18 16:20:36.000000 mat_model-0.1b3/matmodel/comparator/helper.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.350279 mat_model-0.1b3/matmodel/descriptor/
--rw-r--r--   0 tarlisportela   (501) staff       (20)       25 2024-04-18 16:09:57.000000 mat_model-0.1b3/matmodel/descriptor/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4241 2024-05-23 16:55:01.000000 mat_model-0.1b3/matmodel/descriptor/descriptor.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.351018 mat_model-0.1b3/matmodel/evaluation/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      742 2024-04-19 21:36:51.000000 mat_model-0.1b3/matmodel/evaluation/Feature.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      193 2024-04-17 15:21:31.000000 mat_model-0.1b3/matmodel/evaluation/Quality.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       45 2024-04-19 21:37:58.000000 mat_model-0.1b3/matmodel/evaluation/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.351245 mat_model-0.1b3/matmodel/index/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-19 18:35:46.000000 mat_model-0.1b3/matmodel/index/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.351610 mat_model-0.1b3/matmodel/method/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      701 2024-04-29 14:35:26.000000 mat_model-0.1b3/matmodel/method/MethodWrapper.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      100 2024-04-28 16:21:33.000000 mat_model-0.1b3/matmodel/method/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.352305 mat_model-0.1b3/matmodel/method/classification/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      884 2024-04-29 14:32:53.000000 mat_model-0.1b3/matmodel/method/classification/HiperMovelets.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      567 2024-04-28 16:18:41.000000 mat_model-0.1b3/matmodel/method/classification/MasterMovelets.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      143 2024-05-18 05:05:30.000000 mat_model-0.1b3/matmodel/method/classification/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.352889 mat_model-0.1b3/matmodel/util/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-16 19:42:44.000000 mat_model-0.1b3/matmodel/util/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      271 2024-04-16 20:08:42.000000 mat_model-0.1b3/matmodel/util/filters.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3247 2024-04-19 21:58:05.000000 mat_model-0.1b3/matmodel/util/parsers.py
--rw-------   0 tarlisportela   (501) staff       (20)    89436 2024-05-23 19:20:38.000000 mat_model-0.1b3/matmodel.drawio
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2117 2024-05-23 19:25:47.000000 mat_model-0.1b3/pyproject.toml
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-05-23 19:25:51.354054 mat_model-0.1b3/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2209 2024-04-10 16:09:27.000000 mat_model-0.1b3/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.955905 mat_model-0.1b4/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      106 2024-04-10 16:16:51.000000 mat_model-0.1b4/CHANGELOG.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b4/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_model-0.1b4/MANIFEST.in
+-rw-------   0 tarlisportela   (501) staff       (20)    41157 2024-04-19 21:04:47.000000 mat_model-0.1b4/MAT-Tools.drawio
+-rwx------   0 tarlisportela   (501) staff       (20)    35070 2024-05-24 17:37:38.000000 mat_model-0.1b4/MAT-model-Tutorial.ipynb
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-24 17:41:09.955695 mat_model-0.1b4/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b4/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      719 2024-04-10 16:09:56.000000 mat_model-0.1b4/Steps to Build.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.954985 mat_model-0.1b4/mat_model.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-24 17:41:09.000000 mat_model-0.1b4/mat_model.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1098 2024-05-24 17:41:09.000000 mat_model-0.1b4/mat_model.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-05-24 17:41:09.000000 mat_model-0.1b4/mat_model.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      139 2024-05-24 17:41:09.000000 mat_model-0.1b4/mat_model.egg-info/requires.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        9 2024-05-24 17:41:09.000000 mat_model-0.1b4/mat_model.egg-info/top_level.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.951787 mat_model-0.1b4/matmodel/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b4/matmodel/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b4/matmodel/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_model-0.1b4/matmodel/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.952553 mat_model-0.1b4/matmodel/base/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5661 2024-05-23 19:14:12.000000 mat_model-0.1b4/matmodel/base/Aspect.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2429 2024-04-19 21:37:21.000000 mat_model-0.1b4/matmodel/base/Movelet.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     6959 2024-05-22 19:03:55.000000 mat_model-0.1b4/matmodel/base/MultipleAspectSequence.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       83 2024-04-19 21:39:58.000000 mat_model-0.1b4/matmodel/base/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4430 2024-04-19 15:20:13.000000 mat_model-0.1b4/matmodel/base/xSubtrajectory.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      937 2024-04-19 21:33:09.000000 mat_model-0.1b4/matmodel/base/xTrajectory.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.952957 mat_model-0.1b4/matmodel/comparator/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       45 2024-05-23 16:51:19.000000 mat_model-0.1b4/matmodel/comparator/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    13293 2024-05-24 17:36:51.000000 mat_model-0.1b4/matmodel/comparator/distance.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-18 16:20:36.000000 mat_model-0.1b4/matmodel/comparator/helper.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.953196 mat_model-0.1b4/matmodel/descriptor/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       25 2024-04-18 16:09:57.000000 mat_model-0.1b4/matmodel/descriptor/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4241 2024-05-23 16:55:01.000000 mat_model-0.1b4/matmodel/descriptor/descriptor.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.953626 mat_model-0.1b4/matmodel/evaluation/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      742 2024-04-19 21:36:51.000000 mat_model-0.1b4/matmodel/evaluation/Feature.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      193 2024-04-17 15:21:31.000000 mat_model-0.1b4/matmodel/evaluation/Quality.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       45 2024-04-19 21:37:58.000000 mat_model-0.1b4/matmodel/evaluation/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.953752 mat_model-0.1b4/matmodel/index/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-19 18:35:46.000000 mat_model-0.1b4/matmodel/index/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.954002 mat_model-0.1b4/matmodel/method/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      701 2024-04-29 14:35:26.000000 mat_model-0.1b4/matmodel/method/MethodWrapper.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      100 2024-04-28 16:21:33.000000 mat_model-0.1b4/matmodel/method/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.954405 mat_model-0.1b4/matmodel/method/classification/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      884 2024-04-29 14:32:53.000000 mat_model-0.1b4/matmodel/method/classification/HiperMovelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      567 2024-04-28 16:18:41.000000 mat_model-0.1b4/matmodel/method/classification/MasterMovelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      143 2024-05-18 05:05:30.000000 mat_model-0.1b4/matmodel/method/classification/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-24 17:41:09.954776 mat_model-0.1b4/matmodel/util/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-16 19:42:44.000000 mat_model-0.1b4/matmodel/util/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      271 2024-04-16 20:08:42.000000 mat_model-0.1b4/matmodel/util/filters.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3247 2024-04-19 21:58:05.000000 mat_model-0.1b4/matmodel/util/parsers.py
+-rw-------   0 tarlisportela   (501) staff       (20)    89436 2024-05-23 19:20:38.000000 mat_model-0.1b4/matmodel.drawio
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2117 2024-05-24 17:39:10.000000 mat_model-0.1b4/pyproject.toml
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-05-24 17:41:09.955938 mat_model-0.1b4/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2209 2024-04-10 16:09:27.000000 mat_model-0.1b4/setup.py
```

### Comparing `mat_model-0.1b3/LICENSE` & `mat_model-0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/MAT-Tools.drawio` & `mat_model-0.1b4/MAT-Tools.drawio`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/MAT-model-Tutorial.ipynb` & `mat_model-0.1b4/MAT-model-Tutorial.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904600518724695%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1, 'outputs': {0: {'text': {insert: [(0, 'Requirement already "*

 * *            'satisfied: mat-model in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages '*

 * *            "(0.1b3)\\n')], delete: [17, 16, 15, 14, 13, 12, 11, 10, 2, 1, 0]}}}}, 2: "*

 * *            "{'execution_count': 2, 'outputs': {1: {'text': {insert: [(2, '100 1055k  100 1055k    "*

 * *            "0     0  2283k      0 --:--:-- --:--:-- --:--:-- 2294k\\n')], delete: [2]}}, 2: "*

 * *            "{'data': {'appl […]*

```diff
@@ -12,52 +12,42 @@
                 "\n",
                 "Created on Apr, 2024\n",
                 "Copyright (C) 2023, License GPL Version 3 or superior (see LICENSE file)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 1,
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: mat-model in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (0.1b1)\n",
-                        "Collecting mat-model\n",
-                        "  Downloading mat_model-0.1b2-py3-none-any.whl.metadata (5.0 kB)\n",
+                        "Requirement already satisfied: mat-model in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (0.1b3)\n",
                         "Requirement already satisfied: glob2 in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (from mat-model) (0.7)\n",
                         "Requirement already satisfied: numpy in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (from mat-model) (1.22.4)\n",
                         "Requirement already satisfied: pandas in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (from mat-model) (2.2.2)\n",
                         "Requirement already satisfied: python-dateutil>=2.8.2 in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (from pandas->mat-model) (2.8.2)\n",
                         "Requirement already satisfied: pytz>=2020.1 in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (from pandas->mat-model) (2022.1)\n",
                         "Requirement already satisfied: tzdata>=2022.7 in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (from pandas->mat-model) (2024.1)\n",
-                        "Requirement already satisfied: six>=1.5 in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (from python-dateutil>=2.8.2->pandas->mat-model) (1.15.0)\n",
-                        "Downloading mat_model-0.1b2-py3-none-any.whl (43 kB)\n",
-                        "\u001b[2K   \u001b[90m\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u001b[0m \u001b[32m43.7/43.7 kB\u001b[0m \u001b[31m1.3 MB/s\u001b[0m eta \u001b[36m0:00:00\u001b[0m\n",
-                        "\u001b[?25hInstalling collected packages: mat-model\n",
-                        "  Attempting uninstall: mat-model\n",
-                        "    Found existing installation: mat-model 0.1b1\n",
-                        "    Uninstalling mat-model-0.1b1:\n",
-                        "      Successfully uninstalled mat-model-0.1b1\n",
-                        "Successfully installed mat-model-0.1b2\n"
+                        "Requirement already satisfied: six>=1.5 in /Users/tarlisportela/miniforge3/lib/python3.9/site-packages (from python-dateutil>=2.8.2->pandas->mat-model) (1.15.0)\n"
                     ]
                 }
             ],
             "source": [
                 "#!pip install mat-model\n",
                 "!pip install --upgrade mat-model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
@@ -67,21 +57,21 @@
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current\n",
                         "                                 Dload  Upload   Total   Spent    Left  Speed\n",
-                        "100 1055k  100 1055k    0     0  4087k      0 --:--:-- --:--:-- --:--:-- 4155k\n"
+                        "100 1055k  100 1055k    0     0  2283k      0 --:--:-- --:--:-- --:--:-- 2294k\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "1849777543e2491496fa9871c0b3af9c",
+                            "model_id": "cecaf661d9ed45c381cbe2f1a6873f81",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Spliting Data (class-balanced):   0%|          | 0/193 [00:00<?, ?it/s]"
                         ]
                     },
@@ -322,15 +312,15 @@
                             "15269  29559   1070  \n",
                             "15270  29559   1070  \n",
                             "15271  29559   1070  \n",
                             "\n",
                             "[15272 rows x 10 columns]"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from matdata.dataset import *\n",
                 "ds = 'mat.FoursquareNYC'\n",
@@ -345,21 +335,21 @@
                 "#### Trajectory Objects\n",
                 "\n",
                 "Alternatively, you can convert the dataframe into Trajectory objects:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "3076951508764aaf9050f10047fd5b71",
+                            "model_id": "2aaef32031ef41ae997d1c5ad4133f3c",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Converting Trajectories:   0%|          | 0/694 [00:00<?, ?it/s]"
                         ]
                     },
@@ -371,15 +361,15 @@
                 "from matmodel.util.parsers import df2trajectory\n",
                 "\n",
                 "T = df2trajectory(df)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\ud835\ude1b\ud800\udd01135 \t\ud835\ude311\u27e8(40.690 -73.982), 145.0, Monday, NYCT Transit Survey Unit, Office, Professional & Other Places, -1.0, Clouds\u27e9\u21b4\n",
@@ -402,15 +392,15 @@
             "source": [
                 "traj = T[1]\n",
                 "traj.display()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "[1. space (space2d),\n",
                             " 2. time (numeric),\n",
@@ -418,26 +408,26 @@
                             " 4. poi (nominal),\n",
                             " 5. type (nominal),\n",
                             " 6. root_type (nominal),\n",
                             " 7. rating (numeric),\n",
                             " 8. weather (nominal)]"
                         ]
                     },
-                    "execution_count": 4,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "traj.attributes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "[1. space (space2d),\n",
                             " 2. time (numeric),\n",
@@ -445,26 +435,26 @@
                             " 4. poi (nominal),\n",
                             " 5. type (nominal),\n",
                             " 6. root_type (nominal),\n",
                             " 7. rating (numeric),\n",
                             " 8. weather (nominal)]"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "traj.attributes_desc.attributes # same as traj.attributes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "9. tid (numeric)\n",
@@ -476,242 +466,242 @@
                 "# Special desctriptors for trajectory:\n",
                 "print(traj.attributes_desc.idDesc)\n",
                 "print(traj.attributes_desc.labelDesc)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "\ud835\ude311\u27e8(40.690 -73.982), 145.0, Monday, NYCT Transit Survey Unit, Office, Professional & Other Places, -1.0, Clouds\u27e9"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "traj.points[0]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(Monday, NYCT Transit Survey Unit)"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Values\n",
                 "traj.points[0].aspects[2], traj.points[0].aspects[3]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "('poi', NYCT Transit Survey Unit)"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# name attr, and value\n",
                 "traj.attributes[3].text, traj.points[0].aspects[3]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(True, False, matmodel.base.Aspect.Space2D, matmodel.base.Aspect.Categoric)"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a = traj.points[0].aspects[0]\n",
                 "b = traj.points[0].aspects[2]\n",
                 "from matmodel.base import Space2D\n",
                 "\n",
                 "isinstance(a, Space2D), isinstance(b, Space2D), type(a), type(b)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "((40.6900872257332, -73.9817776229191), tuple, 'Monday', str)"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "a.value, type(a.value), b.value, type(b.value)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "1 -- space -- space2d\n",
-                        "Comparator 1: <matmodel.comparator.distance.EuclideanDistance object at 0x10779ca30>\n",
-                        "Comparator 8: <matmodel.comparator.distance.EqualsDistance object at 0x153137ca0>\n"
+                        "Comparator 1: <matmodel.comparator.distance.EuclideanDistance object at 0x14baa80d0>\n",
+                        "Comparator 8: <matmodel.comparator.distance.EqualsDistance object at 0x14baa85b0>\n"
                     ]
                 }
             ],
             "source": [
                 "a1 = traj.attributes[0]\n",
                 "a8 = traj.attributes[7]\n",
                 "print(a1.order, a1.text, a1.dtype, sep=' -- ')\n",
                 "\n",
                 "print('Comparator 1:', a1.comparator)\n",
                 "print('Comparator 8:', a8.comparator)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 45,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "1. space (space2d) <matmodel.comparator.distance.EuclideanDistance object at 0x16929a6a0>\n",
-                        "2. time (time) <matmodel.comparator.distance.TimeDistance object at 0x16929a5b0>\n",
-                        "3. day (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a610>\n",
-                        "4. poi (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a430>\n",
-                        "5. type (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a400>\n",
-                        "6. root_type (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a1c0>\n",
-                        "7. rating (numeric) <matmodel.comparator.distance.AbsoluteDistance object at 0x16929a310>\n",
-                        "8. weather (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a2e0>\n"
+                        "1. space (space2d) <matmodel.comparator.distance.EuclideanDistance object at 0x14baa80d0>\n",
+                        "2. time (numeric) <matmodel.comparator.distance.AbsoluteDistance object at 0x14baa8100>\n",
+                        "3. day (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x14baa81f0>\n",
+                        "4. poi (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x14baa82b0>\n",
+                        "5. type (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x14baa8370>\n",
+                        "6. root_type (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x14baa8430>\n",
+                        "7. rating (numeric) <matmodel.comparator.distance.AbsoluteDistance object at 0x14baa8490>\n",
+                        "8. weather (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x14baa85b0>\n"
                     ]
                 }
             ],
             "source": [
                 "for attr in traj.attributes:\n",
                 "    print(attr, attr.comparator)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 31,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0.02068644437005193"
                         ]
                     },
-                    "execution_count": 31,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Dist\u00e2ncia espacial:\n",
                 "a1.comparator.distance(traj.points[0].aspects[0], traj.points[1].aspects[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 32,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0"
                         ]
                     },
-                    "execution_count": 32,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Calcular a distancia do p1 com p2, no atributo Weather (S\u00e3o iguais)\n",
                 "a8.comparator.distance(traj.points[0].aspects[7], traj.points[1].aspects[7])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 33,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "1"
                         ]
                     },
-                    "execution_count": 33,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Calcular a distancia do p1 com p6, no atributo 1 (S\u00e3o diferentes)\n",
                 "a8.comparator.distance(traj.points[0].aspects[7], traj.points[5].aspects[7])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 34,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(4, 100)"
                         ]
                     },
-                    "execution_count": 34,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Exemplos de valores de dist\u00e2ncia:\n",
                 "d1 = 2\n",
@@ -720,24 +710,24 @@
                 "# isso era uma fun\u00e7\u00e3o que o Andres usava para aumentar a diferen\u00e7a proporcionalmente quanto maior fosse a distancia,\n",
                 "# vai at\u00e9 o max_value do comparador (se for setado)\n",
                 "a1.comparator.enhance(d1), a1.comparator.enhance(d2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 35,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(0.25, 0.75)"
                         ]
                     },
-                    "execution_count": 35,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Exemplos de valores de dist\u00e2ncia:\n",
                 "d1 = 25\n",
@@ -746,15 +736,15 @@
                 "# Se tiver valores de dist\u00e2ncia que quiser normalizar de 0 a 1, d\u00e1 pra atribuir o maior valor de dist\u00e2ncia poss\u00edvel:\n",
                 "a1.comparator.max_value = 100\n",
                 "a1.comparator.normalize(d1), a1.comparator.normalize(d2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 36,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Help on method distance in module matmodel.comparator.distance:\n",
@@ -774,15 +764,15 @@
             ],
             "source": [
                 "help(a1.comparator.distance)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 41,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Monday Monday 0\n",
@@ -803,21 +793,21 @@
                 "a1.comparator = EditlcsDistance()\n",
                 "print(traj.points[0].aspects[2], traj.points[2].aspects[2], a1.comparator.distance(traj.points[0].aspects[2], traj.points[2].aspects[2]))\n",
                 "print(traj.points[0].aspects[2], traj.points[5].aspects[2], a1.comparator.distance(traj.points[0].aspects[2], traj.points[5].aspects[2]))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "461fbfbf574a47a68abde50c69582206",
+                            "model_id": "369bc8e5d1ce44d5bf94a01c9c461113",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Converting Trajectories:   0%|          | 0/694 [00:00<?, ?it/s]"
                         ]
                     },
@@ -830,29 +820,29 @@
                 "from matmodel.util.parsers import df2trajectory\n",
                 "T = df2trajectory(df, attributes_desc='../datasets/mat/FoursquareNYC/FoursquareNYC.json')\n",
                 "traj = T[73]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 44,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "1. space (space2d) <matmodel.comparator.distance.EuclideanDistance object at 0x16929a6a0>\n",
-                        "2. time (time) <matmodel.comparator.distance.TimeDistance object at 0x16929a5b0>\n",
-                        "3. day (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a610>\n",
-                        "4. poi (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a430>\n",
-                        "5. type (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a400>\n",
-                        "6. root_type (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a1c0>\n",
-                        "7. rating (numeric) <matmodel.comparator.distance.AbsoluteDistance object at 0x16929a310>\n",
-                        "8. weather (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x16929a2e0>\n"
+                        "1. space (space2d) <matmodel.comparator.distance.EuclideanDistance object at 0x107ebfc40>\n",
+                        "2. time (time) <matmodel.comparator.distance.TimeDistance object at 0x107e37550>\n",
+                        "3. day (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x14d4ee340>\n",
+                        "4. poi (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x14c96fcd0>\n",
+                        "5. type (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x107f31340>\n",
+                        "6. root_type (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x107f31c70>\n",
+                        "7. rating (numeric) <matmodel.comparator.distance.AbsoluteDistance object at 0x107f31c40>\n",
+                        "8. weather (nominal) <matmodel.comparator.distance.EqualsDistance object at 0x107f31e20>\n"
                     ]
                 }
             ],
             "source": [
                 "for attr in traj.attributes:\n",
                 "    print(attr, attr.comparator)"
             ]
@@ -862,29 +852,29 @@
             "metadata": {},
             "source": [
                 "---"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(2024-01-01 01:00:00,\n",
                             " 2024-01-01 02:30:00,\n",
                             " 2024-01-01 23:50:00,\n",
                             " [2024-01-01 01:10:00 \ud82f\udc94\ud82f\udc94 2024-01-01 02:00:00],\n",
                             " [2024-01-01 01:30:00 \ud82f\udc94\ud82f\udc94 2024-01-01 03:00:00],\n",
                             " [2024-01-01 23:00:00 \ud82f\udc94\ud82f\udc94 2024-01-01 23:50:00])"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from matmodel.base import DateTime, Interval\n",
                 "\n",
@@ -897,61 +887,61 @@
                 "i3 = Interval('1380', '1430') # v3 == end\n",
                 "\n",
                 "v1, v2, v3, i1, i2, i3"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 25,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(datetime.datetime, 60, 150, 1430)"
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 25,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "type(v1.value), v1.get('m'), v2.get('m'), v3.get('m')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 26,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(1439, None, None)"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 26,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from matmodel.comparator import *\n",
                 "\n",
                 "tD = TimeDistance() # Esse compara sempre em rela\u00e7\u00e3o ao hor\u00e1rio do dia (s\u00f3 considera o tempo)\n",
-                "dD = DateDistance(units='m') # esse comprara sempre da maior para o menor\n",
+                "dD = DatetimeDistance(units='m') # esse comprara sempre da maior para o menor\n",
                 "iD = InintervalDistance(units='m') # Esse compara datas e intervalos\n",
                 "\n",
                 "tD.max_value, iD.max_value, dD.max_value"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 27,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "90 90\n",
```

### Comparing `mat_model-0.1b3/PKG-INFO` & `mat_model-0.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-model
-Version: 0.1b3
+Version: 0.1b4
 Summary: MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-model
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-model
```

### Comparing `mat_model-0.1b3/README.md` & `mat_model-0.1b4/README.md`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/Steps to Build.txt` & `mat_model-0.1b4/Steps to Build.txt`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/mat_model.egg-info/PKG-INFO` & `mat_model-0.1b4/mat_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-model
-Version: 0.1b3
+Version: 0.1b4
 Summary: MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-model
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-model
```

### Comparing `mat_model-0.1b3/mat_model.egg-info/SOURCES.txt` & `mat_model-0.1b4/mat_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/LICENSE` & `mat_model-0.1b4/matmodel/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/README.md` & `mat_model-0.1b4/matmodel/README.md`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/base/Aspect.py` & `mat_model-0.1b4/matmodel/base/Aspect.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/base/Movelet.py` & `mat_model-0.1b4/matmodel/base/Movelet.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/base/MultipleAspectSequence.py` & `mat_model-0.1b4/matmodel/base/MultipleAspectSequence.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/base/xSubtrajectory.py` & `mat_model-0.1b4/matmodel/base/xSubtrajectory.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/base/xTrajectory.py` & `mat_model-0.1b4/matmodel/base/xTrajectory.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/comparator/distance.py` & `mat_model-0.1b4/matmodel/comparator/distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         elif self.units == 'isweekday':
             return 0 if dt1.isweekday() == dt2.isweekday() else 1
         else:               
             return (dt1 - dt2).total_seconds()
     
 class InintervalDistance(DatetimeDistance): # TimeDistance.distance calculate difference in minutes (if units == 'm')        
     def __init__(self, max_value=None, units='m'):
-        DateDistance.__init__(self, max_value, units)  
+        DatetimeDistance.__init__(self, max_value, units)  
         
     def distance(self, asp1, asp2):
         from matmodel.base import Interval
         
         # in case one aspect is an Interval return 0 if match, else return 1
         if isinstance(asp1, Interval) or isinstance(asp2, Interval):
             return 0 if self.match(asp1, asp2) else 1
```

### Comparing `mat_model-0.1b3/matmodel/descriptor/descriptor.py` & `mat_model-0.1b4/matmodel/descriptor/descriptor.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/evaluation/Feature.py` & `mat_model-0.1b4/matmodel/evaluation/Feature.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/method/MethodWrapper.py` & `mat_model-0.1b4/matmodel/method/MethodWrapper.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/method/classification/HiperMovelets.py` & `mat_model-0.1b4/matmodel/method/classification/HiperMovelets.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/method/classification/MasterMovelets.py` & `mat_model-0.1b4/matmodel/method/classification/MasterMovelets.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel/util/parsers.py` & `mat_model-0.1b4/matmodel/util/parsers.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/matmodel.drawio` & `mat_model-0.1b4/matmodel.drawio`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b3/pyproject.toml` & `mat_model-0.1b4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 [project]
 name = "mat-model"
-version = "0.1b3"
+version = "0.1b4"
 description = "MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
```

### Comparing `mat_model-0.1b3/setup.py` & `mat_model-0.1b4/setup.py`

 * *Files identical despite different names*

