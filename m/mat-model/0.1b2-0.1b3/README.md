# Comparing `tmp/mat_model-0.1b2.tar.gz` & `tmp/mat_model-0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat_model-0.1b2.tar", last modified: Thu May 23 15:19:45 2024, max compression
+gzip compressed data, was "mat_model-0.1b3.tar", last modified: Thu May 23 19:25:51 2024, max compression
```

## Comparing `mat_model-0.1b2.tar` & `mat_model-0.1b3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.226677 mat_model-0.1b2/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      106 2024-04-10 16:16:51.000000 mat_model-0.1b2/CHANGELOG.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b2/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_model-0.1b2/MANIFEST.in
--rw-------   0 tarlisportela   (501) staff       (20)    41157 2024-04-19 21:04:47.000000 mat_model-0.1b2/MAT-Tools.drawio
--rwx------   0 tarlisportela   (501) staff       (20)    26766 2024-05-23 14:21:15.000000 mat_model-0.1b2/MAT-model-Tutorial.ipynb
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-23 15:19:45.226279 mat_model-0.1b2/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b2/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)      719 2024-04-10 16:09:56.000000 mat_model-0.1b2/Steps to Build.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.225401 mat_model-0.1b2/mat_model.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1126 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)      139 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/requires.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        9 2024-05-23 15:19:45.000000 mat_model-0.1b2/mat_model.egg-info/top_level.txt
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.219472 mat_model-0.1b2/matmodel/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b2/matmodel/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b2/matmodel/README.md
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_model-0.1b2/matmodel/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.221025 mat_model-0.1b2/matmodel/base/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     5094 2024-05-23 15:02:02.000000 mat_model-0.1b2/matmodel/base/Aspect.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2429 2024-04-19 21:37:21.000000 mat_model-0.1b2/matmodel/base/Movelet.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     6959 2024-05-22 19:03:55.000000 mat_model-0.1b2/matmodel/base/MultipleAspectSequence.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       83 2024-04-19 21:39:58.000000 mat_model-0.1b2/matmodel/base/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4430 2024-04-19 15:20:13.000000 mat_model-0.1b2/matmodel/base/xSubtrajectory.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      937 2024-04-19 21:33:09.000000 mat_model-0.1b2/matmodel/base/xTrajectory.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.221519 mat_model-0.1b2/matmodel/descriptor/
--rw-r--r--   0 tarlisportela   (501) staff       (20)       25 2024-04-18 16:09:57.000000 mat_model-0.1b2/matmodel/descriptor/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-05-22 17:16:27.000000 mat_model-0.1b2/matmodel/descriptor/descriptor.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.222632 mat_model-0.1b2/matmodel/distance/
--rw-r--r--   0 tarlisportela   (501) staff       (20)       47 2024-04-18 16:21:07.000000 mat_model-0.1b2/matmodel/distance/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)    10303 2024-05-22 19:37:32.000000 mat_model-0.1b2/matmodel/distance/comparator.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-18 16:20:36.000000 mat_model-0.1b2/matmodel/distance/helper.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.223198 mat_model-0.1b2/matmodel/evaluation/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      742 2024-04-19 21:36:51.000000 mat_model-0.1b2/matmodel/evaluation/Feature.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      193 2024-04-17 15:21:31.000000 mat_model-0.1b2/matmodel/evaluation/Quality.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       45 2024-04-19 21:37:58.000000 mat_model-0.1b2/matmodel/evaluation/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.223425 mat_model-0.1b2/matmodel/index/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-19 18:35:46.000000 mat_model-0.1b2/matmodel/index/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.223773 mat_model-0.1b2/matmodel/method/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      701 2024-04-29 14:35:26.000000 mat_model-0.1b2/matmodel/method/MethodWrapper.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      100 2024-04-28 16:21:33.000000 mat_model-0.1b2/matmodel/method/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.224464 mat_model-0.1b2/matmodel/method/classification/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      884 2024-04-29 14:32:53.000000 mat_model-0.1b2/matmodel/method/classification/HiperMovelets.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      567 2024-04-28 16:18:41.000000 mat_model-0.1b2/matmodel/method/classification/MasterMovelets.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      143 2024-05-18 05:05:30.000000 mat_model-0.1b2/matmodel/method/classification/__init__.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 15:19:45.225084 mat_model-0.1b2/matmodel/util/
--rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-16 19:42:44.000000 mat_model-0.1b2/matmodel/util/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)      271 2024-04-16 20:08:42.000000 mat_model-0.1b2/matmodel/util/filters.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3247 2024-04-19 21:58:05.000000 mat_model-0.1b2/matmodel/util/parsers.py
--rw-------   0 tarlisportela   (501) staff       (20)    87313 2024-05-23 14:55:08.000000 mat_model-0.1b2/matmodel.drawio
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2117 2024-05-23 15:18:38.000000 mat_model-0.1b2/pyproject.toml
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-05-23 15:19:45.226776 mat_model-0.1b2/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2209 2024-04-10 16:09:27.000000 mat_model-0.1b2/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.354019 mat_model-0.1b3/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      106 2024-04-10 16:16:51.000000 mat_model-0.1b3/CHANGELOG.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b3/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      147 2023-12-15 20:28:19.000000 mat_model-0.1b3/MANIFEST.in
+-rw-------   0 tarlisportela   (501) staff       (20)    41157 2024-04-19 21:04:47.000000 mat_model-0.1b3/MAT-Tools.drawio
+-rwx------   0 tarlisportela   (501) staff       (20)    35812 2024-05-23 19:24:59.000000 mat_model-0.1b3/MAT-model-Tutorial.ipynb
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-23 19:25:51.353787 mat_model-0.1b3/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b3/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      719 2024-04-10 16:09:56.000000 mat_model-0.1b3/Steps to Build.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.353068 mat_model-0.1b3/mat_model.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5015 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1098 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      139 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/requires.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        9 2024-05-23 19:25:51.000000 mat_model-0.1b3/mat_model.egg-info/top_level.txt
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.347220 mat_model-0.1b3/matmodel/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35149 2024-04-10 16:14:23.000000 mat_model-0.1b3/matmodel/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2766 2024-04-10 16:16:34.000000 mat_model-0.1b3/matmodel/README.md
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2023-12-15 20:26:21.000000 mat_model-0.1b3/matmodel/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.349061 mat_model-0.1b3/matmodel/base/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     5661 2024-05-23 19:14:12.000000 mat_model-0.1b3/matmodel/base/Aspect.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2429 2024-04-19 21:37:21.000000 mat_model-0.1b3/matmodel/base/Movelet.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     6959 2024-05-22 19:03:55.000000 mat_model-0.1b3/matmodel/base/MultipleAspectSequence.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       83 2024-04-19 21:39:58.000000 mat_model-0.1b3/matmodel/base/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4430 2024-04-19 15:20:13.000000 mat_model-0.1b3/matmodel/base/xSubtrajectory.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      937 2024-04-19 21:33:09.000000 mat_model-0.1b3/matmodel/base/xTrajectory.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.349897 mat_model-0.1b3/matmodel/comparator/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       45 2024-05-23 16:51:19.000000 mat_model-0.1b3/matmodel/comparator/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    13289 2024-05-23 19:17:39.000000 mat_model-0.1b3/matmodel/comparator/distance.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-18 16:20:36.000000 mat_model-0.1b3/matmodel/comparator/helper.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.350279 mat_model-0.1b3/matmodel/descriptor/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       25 2024-04-18 16:09:57.000000 mat_model-0.1b3/matmodel/descriptor/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4241 2024-05-23 16:55:01.000000 mat_model-0.1b3/matmodel/descriptor/descriptor.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.351018 mat_model-0.1b3/matmodel/evaluation/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      742 2024-04-19 21:36:51.000000 mat_model-0.1b3/matmodel/evaluation/Feature.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      193 2024-04-17 15:21:31.000000 mat_model-0.1b3/matmodel/evaluation/Quality.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       45 2024-04-19 21:37:58.000000 mat_model-0.1b3/matmodel/evaluation/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.351245 mat_model-0.1b3/matmodel/index/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-19 18:35:46.000000 mat_model-0.1b3/matmodel/index/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.351610 mat_model-0.1b3/matmodel/method/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      701 2024-04-29 14:35:26.000000 mat_model-0.1b3/matmodel/method/MethodWrapper.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      100 2024-04-28 16:21:33.000000 mat_model-0.1b3/matmodel/method/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.352305 mat_model-0.1b3/matmodel/method/classification/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      884 2024-04-29 14:32:53.000000 mat_model-0.1b3/matmodel/method/classification/HiperMovelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      567 2024-04-28 16:18:41.000000 mat_model-0.1b3/matmodel/method/classification/MasterMovelets.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      143 2024-05-18 05:05:30.000000 mat_model-0.1b3/matmodel/method/classification/__init__.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-05-23 19:25:51.352889 mat_model-0.1b3/matmodel/util/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        0 2024-04-16 19:42:44.000000 mat_model-0.1b3/matmodel/util/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      271 2024-04-16 20:08:42.000000 mat_model-0.1b3/matmodel/util/filters.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3247 2024-04-19 21:58:05.000000 mat_model-0.1b3/matmodel/util/parsers.py
+-rw-------   0 tarlisportela   (501) staff       (20)    89436 2024-05-23 19:20:38.000000 mat_model-0.1b3/matmodel.drawio
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2117 2024-05-23 19:25:47.000000 mat_model-0.1b3/pyproject.toml
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-05-23 19:25:51.354054 mat_model-0.1b3/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2209 2024-04-10 16:09:27.000000 mat_model-0.1b3/setup.py
```

### Comparing `mat_model-0.1b2/LICENSE` & `mat_model-0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/MAT-Tools.drawio` & `mat_model-0.1b3/MAT-Tools.drawio`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/PKG-INFO` & `mat_model-0.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-model
-Version: 0.1b2
+Version: 0.1b3
 Summary: MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-model
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-model
```

### Comparing `mat_model-0.1b2/README.md` & `mat_model-0.1b3/README.md`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/Steps to Build.txt` & `mat_model-0.1b3/Steps to Build.txt`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/mat_model.egg-info/PKG-INFO` & `mat_model-0.1b3/mat_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat-model
-Version: 0.1b2
+Version: 0.1b3
 Summary: MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining
 Home-page: https://github.com/ttportela/mat-model
 Author: Tarlis Tortelli Portela
 Author-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 Maintainer-email: Tarlis Tortelli Portela <tarlis@tarlis.com.br>
 License: GPL Version 3 or superior (see LICENSE file)
 Project-URL: Homepage, https://github.com/ttportela/mat-model
```

### Comparing `mat_model-0.1b2/mat_model.egg-info/SOURCES.txt` & `mat_model-0.1b3/mat_model.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -18,20 +18,19 @@
 matmodel/__init__.py
 matmodel/base/Aspect.py
 matmodel/base/Movelet.py
 matmodel/base/MultipleAspectSequence.py
 matmodel/base/__init__.py
 matmodel/base/xSubtrajectory.py
 matmodel/base/xTrajectory.py
+matmodel/comparator/__init__.py
+matmodel/comparator/distance.py
+matmodel/comparator/helper.py
 matmodel/descriptor/__init__.py
 matmodel/descriptor/descriptor.py
-matmodel/distance/Comparator.py
-matmodel/distance/__init__.py
-matmodel/distance/comparator.py
-matmodel/distance/helper.py
 matmodel/evaluation/Feature.py
 matmodel/evaluation/Quality.py
 matmodel/evaluation/__init__.py
 matmodel/index/__init__.py
 matmodel/method/MethodWrapper.py
 matmodel/method/__init__.py
 matmodel/method/classification/HiperMovelets.py
```

### Comparing `mat_model-0.1b2/matmodel/LICENSE` & `mat_model-0.1b3/matmodel/LICENSE`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/README.md` & `mat_model-0.1b3/matmodel/README.md`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/base/Aspect.py` & `mat_model-0.1b3/matmodel/base/Aspect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import datetime
+
 class Aspect():
     def __init__(self, value):
         self._value = value
 
     @property
     def value(self, units=None):
         return self._value
@@ -28,15 +30,15 @@
     def __init__(self, value):
         x, y = value.split(' ')
         Aspect.__init__(self, str((x,y)))
         x, y = float(x), float(y)
         self.x = x
         self.y = y
 
-    @Space2D.value.getter
+    @Aspect.value.getter
     def value(self):
         return (self.x, self.y)
     
     def __repr__(self):
         return "({:.3f} {:.3f})".format(self.x, self.y)
     
     def __eq__(self, other):
@@ -48,34 +50,33 @@
         Aspect.__init__(self, str((x,y,z)))
         
         x, y, z = float(x), float(y), float(z)
         self.x = x
         self.y = y
         self.z = z
 
-    @Space3D.value.getter
+    @Aspect.value.getter
     def value(self):
         return (self.x, self.y, self.z)
     
     def __repr__(self):
         return "({:.3f} {:.3f} {:.3f})".format(self.x, self.y, self.z)
     
     def __eq__(self, other):
         return self.x == other.x and self.y == other.y and self.z == other.z
 
 class DateTime(Aspect):
-    def __init__(self, start):     
-#            from datetime import datetime
-#            #Format like: "YYYY-MM-DD HH:MM:SS.ffffff"
-#            return DateTimeAspect( datetime.fromisoformat(v) )
-        
-        # TODO Converter datetime
+    def __init__(self, start, mask="%H:%M"): 
+        # Convert to datetime:
+        start = self.convert(start)
         Aspect.__init__(self, start)
+        
+        self.mask = mask
     
-    @DateTime.start.getter
+    @property
     def start(self):
         return self._value
     
     def day(self): #Just the day (1..30|31*)
         return self._value.day
     
     def month(self): #Just the month (1..12)
@@ -101,16 +102,15 @@
     
     def seconds(self):
         return self.minutes()*60 + self._value.second
     
     def microseconds(self):
         return self.seconds()*1000000 + self._value.microsecond
     
-    @DateTime.value.getter
-    def value(self, units=None): # TODO for interval?
+    def get(self, units=None): # TODO for interval?
         if units == None:
             return self._value
         elif units == 'D':
             return self.day()
         elif units == 'M':
             return self.month()
         elif units == 'Y':
@@ -124,42 +124,61 @@
         elif units == 's':
             return self.seconds()
         elif units == 'ms':
             return self.microseconds()
         else:
             raise Exception('[ERROR DateTime Aspect]: invalid \'units='+str(units)+'\' conversion.')
     
+    def convertMinToDate(self, minutes):
+        # reference date (can be any one)
+        reference_date = datetime.datetime(2024, 1, 1)
+
+        # Compute difference of time in minutes
+        time_diff = datetime.timedelta(minutes=minutes)
+
+        # Add diff to refence date
+        result_date = reference_date + time_diff
+
+        return result_date
+    
+    def convert(self, value, mask = None):
+        return datetime.datetime.strptime(value, mask) if mask else self.convertMinToDate(int(value))
+    
 class Interval(DateTime):
-    def __init__(self, start, end):
-        DateTime.__init__(self, start)
-        # TODO Converter datetime
+    def __init__(self, start, end, mask="%H:%M"):
+        DateTime.__init__(self, start, mask)
+        # Convert to datetime
+        end = self.convert(end)
         self.end = end
+        
+    def __repr__(self):
+        return '[{} 𛲔𛲔 {}]'.format(self.start, self.end)
 
 class Rank(Aspect):
     def __init__(self, descriptor):
         Aspect.__init__(self, descriptor)
         self.rank_values = [] # ->RankValue
         
-    @Rank.descriptor.getter
+    @property
     def descriptor(self):
         return self._value
     
     def add(self, aspect, proportion):
         self.rank_values.append(RankValue(aspect, proportion))
     
 class RankValue:
     def __init__(self, value, proportion):
         self.value = value
         self.proportion = proportion
 
 # ------------------------------------------------------------------------------------------------------------
 def instantiateAspect(k,v):
     try:
-        if k.dtype == 'nominal':
-            return Categorical( str(v) )
+        if k.dtype == 'nominal' or k.dtype == 'categorical':
+            return Categoric( str(v) )
         elif k.dtype == 'numeric':
             return Numeric( v )
         elif k.dtype == 'time' or k.dtype == 'datetime':
             return DateTime( v )
         elif k.dtype == 'space2d':
             x, y = v.split(' ')
             return Space2D( v )
@@ -168,10 +187,11 @@
             return Space3D( v )
         elif k.dtype == 'rank':
             return Rank( v )
 #        elif k.dtype == 'boolean':
 #            return Aspect( bool(v) )
         else:
             return Aspect( v )
-    except:
+    except Exception as e:
+        print(e)
         raise Exception("[ERROR Aspect.py]: Failed to load value " + str(v) \
-                        + " as type " + str(k['type']) + ' attr#' + str(k['order']))
+                        + " as type " + k.dtype + ' attr#' + str(k.order))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mat_model-0.1b2/matmodel/base/Movelet.py` & `mat_model-0.1b3/matmodel/base/Movelet.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/base/MultipleAspectSequence.py` & `mat_model-0.1b3/matmodel/base/MultipleAspectSequence.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/base/xSubtrajectory.py` & `mat_model-0.1b3/matmodel/base/xSubtrajectory.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/base/xTrajectory.py` & `mat_model-0.1b3/matmodel/base/xTrajectory.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/descriptor/descriptor.py` & `mat_model-0.1b3/matmodel/descriptor/descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from matmodel.distance import Comparator
+from matmodel.comparator import Comparator
 
 class DataDescriptor:
     def __init__(self, idDesc=None, labelDesc=None, attributes=[]):
         self.idDesc = idDesc
         self.labelDesc = labelDesc
         
         self.attributes = attributes
```

### Comparing `mat_model-0.1b2/matmodel/distance/comparator.py` & `mat_model-0.1b3/matmodel/comparator/distance.py`

 * *Files 23% similar despite different names*

```diff
@@ -102,15 +102,73 @@
         asp2 (Aspect<numeric>) - value 2 to compare
         
         Return:
         distance - distance difference value, abs(asp1 - asp2).
         '''
         return abs(asp1._value - asp2._value)
 
-class DateDistance(Comparator): 
+class TimeDistance(Comparator):    
+    '''Calculates the closest time distance.
+    Only works for time in hours, minutes, seconds, and microseconds. Ex.: difference between 22h and 2h is 3h.
+
+    Properties:
+    units='ms'      - Unit measure to get distance: h (hours), m (minutes), s (seconds), ms (microseconds)
+    max_value=None  - Maximum possible value for distance (Ex.: hours = 24)
+    '''
+    
+    def __init__(self, max_value=None, units='m'): 
+        # Works for time in hours, minutes or seconds. Ex.: difference between 22h and 2h is 3h.
+        self.units = units
+        if units == 'h':
+            max_value = 23
+        elif units == 'm':
+            max_value = 24*60-1
+        elif units == 's':
+            max_value = 24*60*60-1
+        elif units == 'ms':
+            max_value = 24*60*60*1000-1
+        
+        Comparator.__init__(self, max_value)
+        
+    
+    def distance(self, asp1, asp2):
+        '''Calculates the closest time distance.
+        
+        Arguments:
+        asp1 (Aspect<numeric>, DateTime Aspect) - value 1 to compare
+        asp2 (Aspect<numeric>, DateTime Aspect) - value 2 to compare
+        
+        Return:
+        distance - distance difference in the informed units.
+        '''
+        
+        v1 = asp1.get(self.units)
+        v2 = asp2.get(self.units)
+        
+        v1, v2 = max(v1, v2), min(v1, v2)
+        
+        return min( ((self.max_value - v1) + v2 +1), (v1 - v2) )
+    
+    def abs_distance(self, asp1, asp2):
+        '''Calculates the simple time distance.
+        
+        Arguments:
+        asp1 (Aspect<numeric>, DateTime Aspect) - value 1 to compare
+        asp2 (Aspect<numeric>, DateTime Aspect) - value 2 to compare
+        
+        Return:
+        distance - distance difference in the informed units.
+        '''
+        
+        v1 = asp1.get(self.units)
+        v2 = asp2.get(self.units)
+        
+        return abs(v1 - v2)
+
+class DatetimeDistance(Comparator): 
     '''Calculates the date distance in one of the following units:
     D - days
     M - months
     Y - years
     w - weeks
     h - hours
     m - minutes
@@ -126,80 +184,98 @@
     '''
     
     def __init__(self, max_value=None, units=None):
         Comparator.__init__(self, max_value)
         self.units = units
     
     def distance(self, asp1, asp2):
-        dt1 = max(asp1._value - asp2._value)
-        dt2 = min(asp1._value - asp2._value)
+        dt1 = max(asp1._value, asp2._value)
+        dt2 = min(asp1._value, asp2._value)
 #        delta = abs(asp1._value - asp2._value)
         if self.units == None or self.units == 's':
             return (dt1 - dt2).total_seconds()
-        if units == 'D':
+        if self.units == 'D':
             return (dt1 - dt2).days
-        elif units == 'M': # This is a workaround datetime.timedelta:
+        elif self.units == 'M': # This is a workaround datetime.timedelta:
             from dateutil.relativedelta import relativedelta
             delta = relativedelta(dt1, dt2)
             return delta.years*12 + delta.months
-        elif units == 'Y':
+        elif self.units == 'Y':
             return dt1.year - dt2.year
-        elif units == 'w':
+        elif self.units == 'w':
             return (dt1 - dt2).days // 7
-        elif units == 'h':
+        elif self.units == 'h':
             return (dt1 - dt2).total_seconds() // 3600
-        elif units == 'm':
+        elif self.units == 'm':
             return (dt1 - dt2).total_seconds() // 60
-        elif units == 'weekday':
+        elif self.units == 'weekday':
             return dt1.weekday() - dt2.weekday()
-        elif units == '=weekday':
+        elif self.units == '=weekday':
             return dt1.weekday() == dt2.weekday()
-        elif units == 'isweekday':
+        elif self.units == 'isweekday':
             return 0 if dt1.isweekday() == dt2.isweekday() else 1
         else:               
             return (dt1 - dt2).total_seconds()
+    
+class InintervalDistance(DatetimeDistance): # TimeDistance.distance calculate difference in minutes (if units == 'm')        
+    def __init__(self, max_value=None, units='m'):
+        DateDistance.__init__(self, max_value, units)  
+        
+    def distance(self, asp1, asp2):
+        from matmodel.base import Interval
+        
+        # in case one aspect is an Interval return 0 if match, else return 1
+        if isinstance(asp1, Interval) or isinstance(asp2, Interval):
+            return 0 if self.match(asp1, asp2) else 1
+        else:
+            return super().distance(asp1, asp2) # Gets the time difference
+    
+    def match(self, asp1, asp2, match_threshold=0): #Check if the dates or intervals match (can use with 'DateTime' or 'Interval' instances, or mixed)
+        from matmodel.base import DateTime, Interval
+        
+        if not (isinstance(asp1, DateTime) and isinstance(asp2, DateTime)):
+            raise TypeError("Aspects must be 'DateTime' or 'Interval' instances.")
 
-class TimeDistance(Comparator):    
-    '''Calculates the closest time distance.
-    Only works for time in hours, minutes, seconds, and microseconds. Ex.: difference between 22h and 2h is 3h.
+        # For 2 intervals:
+        if isinstance(asp1, Interval) and isinstance(asp2, Interval):
+            return self.converge(asp1, asp2)
+        
+        # For 1 date and 1 interval:
+        # If asp1 or asp2 represents a point in time (just DateTime.start),
+        elif isinstance(asp1, Interval) or isinstance(asp2, Interval):
+            return self.match_date_interval(asp1, asp2)
 
-    Properties:
-    units='ms'      - Unit measure to get distance: h (hours), m (minutes), s (seconds), ms (microseconds)
-    max_value=None  - Maximum possible value for distance (Ex.: hours = 24)
-    '''
-    
-    def __init__(self, max_value=None, units='m'): 
-        # Works for time in hours, minutes or seconds. Ex.: difference between 22h and 2h is 3h.
-        self.units = units
-        if max_value:
-            self.max_value = max_value
-        elif units == 'h':
-            self.max_value = 23
-        elif units == 'm':
-            self.max_value = 24*60-1
-        elif units == 's':
-            self.max_value = 24*60*60-1
-        elif units == 'ms':
-            self.max_value = 24*60*60*1000-1
+        # If both asp1 and asp2 represents a point in time, we use the distance to see a match:
+        # (match_th is a threshold for matching, default 0)
+        else:
+            return self.match_dates(asp1, asp2, match_threshold)
     
-    def distance(self, asp1, asp2):
-        '''Calculates the closest time distance.
+    def match_dates(self, asp1, asp2, match_threshold=0):
+        return False if int(self.distance(asp1, asp2)) > match_threshold else True
         
-        Arguments:
-        asp1 (Aspect<numeric>, DateTimeAspect) - value 1 to compare
-        asp2 (Aspect<numeric>, DateTimeAspect) - value 2 to compare
+    def match_date_interval(self, asp1, asp2):
+        from matmodel.base import Interval
         
-        Return:
-        distance - distance difference in the informed units.
-        '''
-        v1 = asp1.value(self.units)
-        v2 = asp2.value(self.units)
-        v1 = max(v1, v2)
-        v2 = min(v1, v2)
-        return min( ((self.max_value - v1) + v2 +1), (v1 - v2) )
+        if isinstance(asp2, Interval): #  asp1 is the DateTime, asp2 is the Interval
+            D = asp1
+            I = asp2
+        else:
+            D = asp2
+            I = asp1
+            
+        return True if D.start >= I.start and D.start <= I.end else False
+    
+    def converge(self, asp1, asp2):
+        if not (isinstance(asp1, Interval) and isinstance(asp2, Interval)):
+            raise TypeError("Aspects must be 'Interval' instances.")
+
+        if max(asp1.start, asp2.start) <= min(asp1.end, asp2.end):
+            return True
+        else:
+            return False
     
 class EuclideanDistance(Comparator):
     def __init__(self, max_value=None):
         Comparator.__init__(self, max_value)
 
     def distance(self, asp1, asp2):
         '''Calculates the Euclidean distance (works for points of 2D, 3D, and more).
```

### Comparing `mat_model-0.1b2/matmodel/evaluation/Feature.py` & `mat_model-0.1b3/matmodel/evaluation/Feature.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/method/MethodWrapper.py` & `mat_model-0.1b3/matmodel/method/MethodWrapper.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/method/classification/HiperMovelets.py` & `mat_model-0.1b3/matmodel/method/classification/HiperMovelets.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/method/classification/MasterMovelets.py` & `mat_model-0.1b3/matmodel/method/classification/MasterMovelets.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel/util/parsers.py` & `mat_model-0.1b3/matmodel/util/parsers.py`

 * *Files identical despite different names*

### Comparing `mat_model-0.1b2/matmodel.drawio` & `mat_model-0.1b3/matmodel.drawio`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-<mxfile host="app.diagrams.net" modified="2024-05-23T14:55:08.743Z" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36" etag="S5ZcHV_cwoiQNoxT-Row" version="24.4.0" type="device">
+<mxfile host="app.diagrams.net" modified="2024-05-23T19:20:38.019Z" agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36" etag="15x4_NI05WOczd87_IfR" version="24.4.0" type="device">
   <diagram id="C5RBs43oDa-KdzZeNtuy" name="Page-1">
-    <mxGraphModel dx="1831" dy="1753" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
+    <mxGraphModel dx="1831" dy="1816" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="827" pageHeight="1169" math="0" shadow="0">
       <root>
         <mxCell id="WIyWlLk6GJQsqaUBKTNV-0" />
         <mxCell id="WIyWlLk6GJQsqaUBKTNV-1" parent="WIyWlLk6GJQsqaUBKTNV-0" />
         <mxCell id="wUrawppS3UO5J027udKO-70" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-0" target="wUrawppS3UO5J027udKO-7" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
               <mxPoint x="310" y="-120" />
@@ -174,15 +174,15 @@
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-51" value="- trajectory" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-50" vertex="1" connectable="0">
           <mxGeometry x="-0.3143" y="1" relative="1" as="geometry">
             <mxPoint x="-5" y="-10" as="offset" />
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-55" value="Comparator" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#d80073;fontColor=#ffffff;strokeColor=#A50040;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1775" y="77" width="220" height="162" as="geometry" />
+          <mxGeometry x="1975" y="57" width="220" height="162" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-56" value="#&amp;nbsp;MAX_VALUE: float" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-55" vertex="1">
           <mxGeometry y="26" width="220" height="24" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-57" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-55" vertex="1">
           <mxGeometry y="50" width="220" height="8" as="geometry" />
         </mxCell>
@@ -194,167 +194,170 @@
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-59" value="+&amp;nbsp;normalize&lt;span style=&quot;background-color: initial;&quot;&gt;(distance, maxValue): float&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-55" vertex="1">
           <mxGeometry y="110" width="220" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-60" value="+&amp;nbsp;enhance&lt;span style=&quot;background-color: initial;&quot;&gt;(distance): float&lt;/span&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-55" vertex="1">
           <mxGeometry y="136" width="220" height="26" as="geometry" />
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-61" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;shadow=0;strokeWidth=1;endFill=1;dashed=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-58" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
+        <mxCell id="lsfipmTJbNCapsntxlYZ-61" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=open;shadow=0;strokeWidth=1;endFill=1;dashed=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-55" target="lsfipmTJbNCapsntxlYZ-19" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1885" y="120" />
+              <mxPoint x="1370" y="110" />
+              <mxPoint x="1370" y="110" />
             </Array>
+            <mxPoint x="1775" y="116" as="sourcePoint" />
+            <mxPoint x="1163" y="100" as="targetPoint" />
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-63" value="(asp1, asp2)" style="edgeLabel;html=1;align=center;verticalAlign=middle;resizable=0;points=[];" parent="lsfipmTJbNCapsntxlYZ-61" vertex="1" connectable="0">
           <mxGeometry x="-0.2297" y="-3" relative="1" as="geometry">
-            <mxPoint x="127" y="-7" as="offset" />
+            <mxPoint x="277" y="-7" as="offset" />
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-93" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-65" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1586" y="260" />
-              <mxPoint x="1885" y="260" />
+              <mxPoint x="1786" y="260" />
+              <mxPoint x="2085" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-65" value="NumericDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1521" y="290" width="130" height="60" as="geometry" />
+          <mxGeometry x="1721" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-67" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-65" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-70" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-65" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-94" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-81" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1727" y="260" />
-              <mxPoint x="1885" y="260" />
+              <mxPoint x="1927" y="260" />
+              <mxPoint x="2085" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-81" value="EuclideanDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1662" y="290" width="130" height="60" as="geometry" />
+          <mxGeometry x="1862" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-82" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-81" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-83" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-81" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-95" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-84" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1866" y="260" />
-              <mxPoint x="1885" y="260" />
+              <mxPoint x="2066" y="260" />
+              <mxPoint x="2085" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-84" value="ManhattanDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1801" y="290" width="130" height="60" as="geometry" />
+          <mxGeometry x="2001" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-85" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-84" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-86" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-84" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-96" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-87" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="2004" y="260" />
-              <mxPoint x="1885" y="260" />
+              <mxPoint x="2204" y="260" />
+              <mxPoint x="2085" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-87" value="EqualsDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1939" y="290" width="130" height="60" as="geometry" />
+          <mxGeometry x="2139" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-88" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-87" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-89" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-87" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-97" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-90" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="2144" y="260" />
-              <mxPoint x="1885" y="260" />
+              <mxPoint x="2344" y="260" />
+              <mxPoint x="2085" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-90" value="DateDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="2079" y="290" width="130" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-90" value="TimeDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="2279" y="290" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-91" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-90" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-92" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-90" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-104" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;exitDx=0;exitDy=0;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-101" target="lsfipmTJbNCapsntxlYZ-55" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="2276" y="260" />
-              <mxPoint x="1885" y="260" />
+              <mxPoint x="2476" y="260" />
+              <mxPoint x="2085" y="260" />
             </Array>
           </mxGeometry>
         </mxCell>
-        <mxCell id="lsfipmTJbNCapsntxlYZ-101" value="TimeDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="2221" y="290" width="110" height="60" as="geometry" />
+        <mxCell id="lsfipmTJbNCapsntxlYZ-101" value="DatetimeDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
+          <mxGeometry x="2421" y="290" width="110" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-102" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-101" vertex="1">
           <mxGeometry y="26" width="110" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-103" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-101" vertex="1">
           <mxGeometry y="34" width="110" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-117" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-114" target="lsfipmTJbNCapsntxlYZ-87" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="1933" y="380" />
-              <mxPoint x="2004" y="380" />
+              <mxPoint x="2133" y="380" />
+              <mxPoint x="2204" y="380" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-114" value="LcsDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1868" y="398" width="130" height="60" as="geometry" />
+          <mxGeometry x="2068" y="398" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-115" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-114" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-116" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-114" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-121" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-118" target="lsfipmTJbNCapsntxlYZ-87" edge="1">
           <mxGeometry relative="1" as="geometry">
             <Array as="points">
-              <mxPoint x="2073" y="380" />
-              <mxPoint x="2004" y="380" />
+              <mxPoint x="2273" y="380" />
+              <mxPoint x="2204" y="380" />
             </Array>
           </mxGeometry>
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-118" value="CaselessDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="2008" y="398" width="130" height="60" as="geometry" />
+          <mxGeometry x="2208" y="398" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-119" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-118" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-120" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-118" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-125" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;endArrow=block;endSize=10;endFill=0;shadow=0;strokeWidth=1;" parent="WIyWlLk6GJQsqaUBKTNV-1" source="lsfipmTJbNCapsntxlYZ-122" target="lsfipmTJbNCapsntxlYZ-65" edge="1">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-122" value="AbsoluteDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" parent="WIyWlLk6GJQsqaUBKTNV-1" vertex="1">
-          <mxGeometry x="1521" y="390" width="130" height="60" as="geometry" />
+          <mxGeometry x="1721" y="390" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-123" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" parent="lsfipmTJbNCapsntxlYZ-122" vertex="1">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="lsfipmTJbNCapsntxlYZ-124" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" parent="lsfipmTJbNCapsntxlYZ-122" vertex="1">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
@@ -705,18 +708,23 @@
         <mxCell id="CCnf-G1CkggKAS8I-f5b-2" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-0">
           <mxGeometry y="50" width="140" height="8" as="geometry" />
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-3" value="+&amp;nbsp;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-0">
           <mxGeometry y="58" width="140" height="26" as="geometry" />
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-30" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="CCnf-G1CkggKAS8I-f5b-13" target="lsfipmTJbNCapsntxlYZ-19">
-          <mxGeometry relative="1" as="geometry" />
+          <mxGeometry relative="1" as="geometry">
+            <Array as="points">
+              <mxPoint x="1600" y="210" />
+              <mxPoint x="1083" y="210" />
+            </Array>
+          </mxGeometry>
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-13" value="Numeric" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;strokeColor=#82b366;fontColor=default;fillColor=#d5e8d4;" vertex="1" parent="WIyWlLk6GJQsqaUBKTNV-1">
-          <mxGeometry x="1470" y="140" width="160" height="84" as="geometry" />
+          <mxGeometry x="1520" y="237" width="160" height="84" as="geometry" />
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-14" value="&lt;span style=&quot;font-weight: normal;&quot;&gt;&lt;i&gt;-&amp;nbsp;value&lt;span style=&quot;background-color: initial;&quot;&gt;: float&lt;/span&gt;&lt;/i&gt;&lt;/span&gt;" style="text;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;fontStyle=1;fontColor=default;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-13">
           <mxGeometry y="26" width="160" height="24" as="geometry" />
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-15" value="" style="line;strokeWidth=1;align=center;verticalAlign=top;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;fillColor=#d5e8d4;strokeColor=#82b366;fontFamily=Helvetica;fontSize=12;fontColor=default;fontStyle=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-13">
           <mxGeometry y="50" width="160" height="8" as="geometry" />
         </mxCell>
@@ -743,19 +751,31 @@
         <mxCell id="CCnf-G1CkggKAS8I-f5b-20" value="+&amp;nbsp;" style="text;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;fontFamily=Helvetica;fontSize=12;fontStyle=1;fontColor=default;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-17">
           <mxGeometry y="58" width="160" height="26" as="geometry" />
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-24" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="CCnf-G1CkggKAS8I-f5b-21" target="lsfipmTJbNCapsntxlYZ-114">
           <mxGeometry relative="1" as="geometry" />
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-21" value="Editl&lt;span style=&quot;background-color: initial;&quot;&gt;csDistance&lt;/span&gt;" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" vertex="1" parent="WIyWlLk6GJQsqaUBKTNV-1">
-          <mxGeometry x="1868" y="495" width="130" height="60" as="geometry" />
+          <mxGeometry x="2068" y="495" width="130" height="60" as="geometry" />
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-22" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-21">
           <mxGeometry y="26" width="130" height="8" as="geometry" />
         </mxCell>
         <mxCell id="CCnf-G1CkggKAS8I-f5b-23" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-21">
           <mxGeometry y="34" width="130" height="26" as="geometry" />
         </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-36" style="edgeStyle=orthogonalEdgeStyle;rounded=0;orthogonalLoop=1;jettySize=auto;html=1;shadow=0;strokeColor=default;strokeWidth=1;align=center;verticalAlign=middle;fontFamily=Helvetica;fontSize=11;fontColor=default;labelBackgroundColor=default;endArrow=block;endFill=0;endSize=10;" edge="1" parent="WIyWlLk6GJQsqaUBKTNV-1" source="CCnf-G1CkggKAS8I-f5b-32" target="lsfipmTJbNCapsntxlYZ-101">
+          <mxGeometry relative="1" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-32" value="IntervalDistance" style="swimlane;fontStyle=1;align=center;verticalAlign=top;childLayout=stackLayout;horizontal=1;startSize=26;horizontalStack=0;resizeParent=1;resizeParentMax=0;resizeLast=0;collapsible=1;marginBottom=0;whiteSpace=wrap;html=1;fillColor=#e1d5e7;strokeColor=#9673a6;" vertex="1" parent="WIyWlLk6GJQsqaUBKTNV-1">
+          <mxGeometry x="2421" y="398" width="110" height="60" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-33" value="" style="line;strokeWidth=1;fillColor=none;align=left;verticalAlign=middle;spacingTop=-1;spacingLeft=3;spacingRight=3;rotatable=0;labelPosition=right;points=[];portConstraint=eastwest;strokeColor=inherit;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-32">
+          <mxGeometry y="26" width="110" height="8" as="geometry" />
+        </mxCell>
+        <mxCell id="CCnf-G1CkggKAS8I-f5b-34" value="&lt;i&gt;overriden methods&lt;/i&gt;" style="text;strokeColor=none;fillColor=none;align=left;verticalAlign=top;spacingLeft=4;spacingRight=4;overflow=hidden;rotatable=0;points=[[0,0.5],[1,0.5]];portConstraint=eastwest;whiteSpace=wrap;html=1;" vertex="1" parent="CCnf-G1CkggKAS8I-f5b-32">
+          <mxGeometry y="34" width="110" height="26" as="geometry" />
+        </mxCell>
       </root>
     </mxGraphModel>
   </diagram>
 </mxfile>
```

### Comparing `mat_model-0.1b2/pyproject.toml` & `mat_model-0.1b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 [project]
 name = "mat-model"
-version = "0.1b2"
+version = "0.1b3"
 description = "MAT-model: Model Classes for Multiple Aspect Trajectory Data Mining"
 authors = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
 maintainers = [
     {name = "Tarlis Tortelli Portela", email = "tarlis@tarlis.com.br"},
  ]
```

### Comparing `mat_model-0.1b2/setup.py` & `mat_model-0.1b3/setup.py`

 * *Files identical despite different names*

