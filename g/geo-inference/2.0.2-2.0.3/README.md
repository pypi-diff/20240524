# Comparing `tmp/geo_inference-2.0.2.tar.gz` & `tmp/geo_inference-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_inference-2.0.2.tar", last modified: Wed May 15 12:58:46 2024, max compression
+gzip compressed data, was "geo_inference-2.0.3.tar", last modified: Fri May 24 16:32:21 2024, max compression
```

## Comparing `geo_inference-2.0.2.tar` & `geo_inference-2.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-15 12:58:46.766708 geo_inference-2.0.2/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1072 2023-08-23 18:27:00.000000 geo_inference-2.0.2/LICENSE
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       50 2023-11-28 18:37:26.000000 geo_inference-2.0.2/MANIFEST.in
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-05-15 12:58:46.766708 geo_inference-2.0.2/PKG-INFO
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     3505 2024-04-17 02:45:20.000000 geo_inference-2.0.2/README.md
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-15 12:58:46.758709 geo_inference-2.0.2/geo_inference/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      156 2024-05-15 12:50:53.000000 geo_inference-2.0.2/geo_inference/__init__.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-15 12:58:46.758709 geo_inference-2.0.2/geo_inference/config/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.2/geo_inference/config/__init__.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      767 2023-11-28 18:37:26.000000 geo_inference-2.0.2/geo_inference/config/log_config.yaml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      637 2024-03-12 16:11:07.000000 geo_inference-2.0.2/geo_inference/config/logging_config.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      457 2024-03-12 16:11:07.000000 geo_inference-2.0.2/geo_inference/config/sample.yaml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    16062 2024-04-12 23:47:20.000000 geo_inference-2.0.2/geo_inference/geo_blocks.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     5657 2024-05-14 16:59:04.000000 geo_inference-2.0.2/geo_inference/geo_inference.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-15 12:58:46.762709 geo_inference-2.0.2/geo_inference/utils/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.2/geo_inference/utils/__init__.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     3424 2024-04-06 04:23:36.000000 geo_inference-2.0.2/geo_inference/utils/geo.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    22881 2024-04-06 15:55:07.000000 geo_inference-2.0.2/geo_inference/utils/geo_transforms.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     9775 2024-04-11 03:07:16.000000 geo_inference-2.0.2/geo_inference/utils/helpers.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)    11870 2024-04-10 16:49:51.000000 geo_inference-2.0.2/geo_inference/utils/polygon.py
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-15 12:58:46.762709 geo_inference-2.0.2/geo_inference.egg-info/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-05-15 12:58:46.000000 geo_inference-2.0.2/geo_inference.egg-info/PKG-INFO
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      707 2024-05-15 12:58:46.000000 geo_inference-2.0.2/geo_inference.egg-info/SOURCES.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)        1 2024-05-15 12:58:46.000000 geo_inference-2.0.2/geo_inference.egg-info/dependency_links.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       67 2024-05-15 12:58:46.000000 geo_inference-2.0.2/geo_inference.egg-info/entry_points.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)      264 2024-05-15 12:58:46.000000 geo_inference-2.0.2/geo_inference.egg-info/requires.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       14 2024-05-15 12:58:46.000000 geo_inference-2.0.2/geo_inference.egg-info/top_level.txt
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1832 2024-05-15 12:50:53.000000 geo_inference-2.0.2/pyproject.toml
--rw-r--r--   0 valhassa (17081319) geousers  (1100)       38 2024-05-15 12:58:46.766708 geo_inference-2.0.2/setup.cfg
-drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-15 12:58:46.762709 geo_inference-2.0.2/tests/
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     6201 2024-04-10 18:14:44.000000 geo_inference-2.0.2/tests/test_geo_blocks.py
--rw-r--r--   0 valhassa (17081319) geousers  (1100)     1842 2024-04-11 03:12:23.000000 geo_inference-2.0.2/tests/test_geo_inference.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1072 2023-08-23 18:27:00.000000 geo_inference-2.0.3/LICENSE
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       50 2023-11-28 18:37:26.000000 geo_inference-2.0.3/MANIFEST.in
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-05-24 16:32:21.656823 geo_inference-2.0.3/PKG-INFO
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     3505 2024-04-17 02:45:20.000000 geo_inference-2.0.3/README.md
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/geo_inference/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      156 2024-05-24 16:32:10.000000 geo_inference-2.0.3/geo_inference/__init__.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/geo_inference/config/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.3/geo_inference/config/__init__.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      767 2023-11-28 18:37:26.000000 geo_inference-2.0.3/geo_inference/config/log_config.yaml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      637 2024-03-12 16:11:07.000000 geo_inference-2.0.3/geo_inference/config/logging_config.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      457 2024-03-12 16:11:07.000000 geo_inference-2.0.3/geo_inference/config/sample.yaml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    16178 2024-05-24 15:05:14.000000 geo_inference-2.0.3/geo_inference/geo_blocks.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     5657 2024-05-14 16:59:04.000000 geo_inference-2.0.3/geo_inference/geo_inference.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/geo_inference/utils/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        0 2023-11-28 18:37:26.000000 geo_inference-2.0.3/geo_inference/utils/__init__.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     3424 2024-04-06 04:23:36.000000 geo_inference-2.0.3/geo_inference/utils/geo.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    22881 2024-04-06 15:55:07.000000 geo_inference-2.0.3/geo_inference/utils/geo_transforms.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     9775 2024-04-11 03:07:16.000000 geo_inference-2.0.3/geo_inference/utils/helpers.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)    11870 2024-04-10 16:49:51.000000 geo_inference-2.0.3/geo_inference/utils/polygon.py
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/geo_inference.egg-info/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6209 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/PKG-INFO
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      707 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)        1 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       67 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/entry_points.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)      264 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/requires.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       14 2024-05-24 16:32:21.000000 geo_inference-2.0.3/geo_inference.egg-info/top_level.txt
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1832 2024-05-24 16:32:10.000000 geo_inference-2.0.3/pyproject.toml
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)       38 2024-05-24 16:32:21.656823 geo_inference-2.0.3/setup.cfg
+drwxr-xr-x   0 valhassa (17081319) geousers  (1100)        0 2024-05-24 16:32:21.656823 geo_inference-2.0.3/tests/
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     6201 2024-04-10 18:14:44.000000 geo_inference-2.0.3/tests/test_geo_blocks.py
+-rw-r--r--   0 valhassa (17081319) geousers  (1100)     1842 2024-04-11 03:12:23.000000 geo_inference-2.0.3/tests/test_geo_inference.py
```

### Comparing `geo_inference-2.0.2/LICENSE` & `geo_inference-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/PKG-INFO` & `geo_inference-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-inference
-Version: 2.0.2
+Version: 2.0.3
 Summary: Extract features from geospatial imagery using deep learning models
 Author-email: Victor Alhassan <victor.alhassan@nrcan-rncan.gc.ca>
 License: MIT License
         
         Copyright (c) 2023 Victor Alhassan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geo_inference-2.0.2/README.md` & `geo_inference-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/geo_inference/config/log_config.yaml` & `geo_inference-2.0.3/geo_inference/config/log_config.yaml`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/geo_inference/config/logging_config.py` & `geo_inference-2.0.3/geo_inference/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/geo_inference/geo_blocks.py` & `geo_inference-2.0.3/geo_inference/geo_blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,18 +349,20 @@
             windows (torch.Tensor): The windows used for inference.
             pixel_coords (list): The pixel coordinates of the patches.
 
         Returns:
             None
         """
         for output, window, (x, y, patch_width, patch_height) in zip(batch, windows, pixel_coords):
-            if self.classes == 1:
-                output = F.sigmoid(output) * window
-            else:
-                output = F.softmax(output, dim=0) * window
+            # It is best to have these functions scripted in the model
+            # if self.classes == 1:
+            #     output = F.sigmoid(output) * window
+            # else:
+            #     output = F.softmax(output, dim=0) * window
+            output = output * window
             self.image[:, y : y + patch_height, x : x + patch_width] += output.cpu().numpy()
             self.norm_mask[:, y : y + patch_height, x : x + patch_width] += window.cpu().numpy()
     
     @torch.no_grad()
     def merge_on_gpu(self,):
         """
         Merge the patches on GPU.
```

### Comparing `geo_inference-2.0.2/geo_inference/geo_inference.py` & `geo_inference-2.0.3/geo_inference/geo_inference.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/geo_inference/utils/geo.py` & `geo_inference-2.0.3/geo_inference/utils/geo.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/geo_inference/utils/geo_transforms.py` & `geo_inference-2.0.3/geo_inference/utils/geo_transforms.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/geo_inference/utils/helpers.py` & `geo_inference-2.0.3/geo_inference/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/geo_inference/utils/polygon.py` & `geo_inference-2.0.3/geo_inference/utils/polygon.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/geo_inference.egg-info/PKG-INFO` & `geo_inference-2.0.3/geo_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-inference
-Version: 2.0.2
+Version: 2.0.3
 Summary: Extract features from geospatial imagery using deep learning models
 Author-email: Victor Alhassan <victor.alhassan@nrcan-rncan.gc.ca>
 License: MIT License
         
         Copyright (c) 2023 Victor Alhassan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `geo_inference-2.0.2/geo_inference.egg-info/SOURCES.txt` & `geo_inference-2.0.3/geo_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/pyproject.toml` & `geo_inference-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geo-inference"
-version = "2.0.2"
+version = "2.0.3"
 description = "Extract features from geospatial imagery using deep learning models"
 readme = "README.md"
 authors = [{ name = "Victor Alhassan", email = "victor.alhassan@nrcan-rncan.gc.ca" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
@@ -47,15 +47,15 @@
 [project.scripts]
 geo_inference = "geo_inference.geo_inference:main"
 
 [tool.setuptools.packages.find]
 include = ["geo_inference*"]
 
 [tool.bumpver]
-current_version = "2.0.2"
+current_version = "2.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `geo_inference-2.0.2/tests/test_geo_blocks.py` & `geo_inference-2.0.3/tests/test_geo_blocks.py`

 * *Files identical despite different names*

### Comparing `geo_inference-2.0.2/tests/test_geo_inference.py` & `geo_inference-2.0.3/tests/test_geo_inference.py`

 * *Files identical despite different names*

