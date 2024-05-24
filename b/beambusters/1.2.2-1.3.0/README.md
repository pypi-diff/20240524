# Comparing `tmp/beambusters-1.2.2.tar.gz` & `tmp/beambusters-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beambusters-1.2.2.tar", max compression
+gzip compressed data, was "beambusters-1.3.0.tar", max compression
```

## Comparing `beambusters-1.2.2.tar` & `beambusters-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-23 09:53:31.817970 beambusters-1.2.2/LICENSE
--rw-r--r--   0        0        0      630 2024-05-23 09:53:31.817970 beambusters-1.2.2/README.md
--rwxr-xr-x   0        0        0        0 2024-05-23 09:53:31.817970 beambusters-1.2.2/beambusters/__init__.py
--rw-r--r--   0        0        0    11843 2024-05-23 09:53:31.817970 beambusters-1.2.2/beambusters/main.py
--rwxr-xr-x   0        0        0     3170 2024-05-23 09:53:31.817970 beambusters-1.2.2/beambusters/settings.py
--rwxr-xr-x   0        0        0      143 2024-05-23 09:53:31.817970 beambusters-1.2.2/beambusters/utils.py
--rw-r--r--   0        0        0     2026 2024-05-23 09:53:41.226044 beambusters-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 11:50:44.096361 beambusters-1.3.0/LICENSE
+-rw-r--r--   0        0        0      630 2024-05-24 11:50:44.096361 beambusters-1.3.0/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-24 11:50:44.096361 beambusters-1.3.0/beambusters/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-24 11:50:44.096361 beambusters-1.3.0/beambusters/main.py
+-rwxr-xr-x   0        0        0     3170 2024-05-24 11:50:44.096361 beambusters-1.3.0/beambusters/settings.py
+-rwxr-xr-x   0        0        0     1394 2024-05-24 11:50:44.096361 beambusters-1.3.0/beambusters/utils.py
+-rw-r--r--   0        0        0     2026 2024-05-24 11:50:53.620432 beambusters-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.3.0/PKG-INFO
```

### Comparing `beambusters-1.2.2/LICENSE` & `beambusters-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beambusters-1.2.2/README.md` & `beambusters-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `beambusters-1.2.2/beambusters/main.py` & `beambusters-1.3.0/beambusters/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typer
 from beambusters import settings
 import subprocess as sub
 import h5py
 import numpy as np
-from beambusters.utils import centering_converged
+from beambusters.utils import centering_converged, list_events
 import matplotlib.pyplot as plt
 import math
 import hdf5plugin
 import os
 import pathlib
 import sys
 from bblib.methods import CenterOfMass, FriedelPairs, MinimizePeakFWHM, CircleDetection
@@ -34,38 +34,36 @@
     config = settings.read(path_to_config)
     BeambustersParam = settings.parse(config)
     files = open(input, "r")
     paths = files.readlines()
     files.close()
 
     if len(paths[0][:-1].split(" //")) == 1:
-        # Not listed events. TODO test if CrystFEL not loaded sucessfully.
         list_name = input
         events_list_file = (
             f"{list_name.split('.')[0]}_events.lst{list_name.split('.lst')[-1]}"
         )
-        command = f"source /etc/profile.d/modules.sh; module load maxwell crystfel/0.11.0; list_events -i {list_name} -o {events_list_file} -g {config['geometry_file']}"
-        sub.call(command, shell=True)
+        list_events(list_name, events_list_file, config["geometry_file"])
         files = open(events_list_file, "r")
         paths = files.readlines()
         files.close()
 
     geometry_txt = open(config["geometry_file"], "r").readlines()
-    h5_path = [
+    data_hdf5_path = [
         x.split(" = ")[-1][:-1] for x in geometry_txt if x.split(" = ")[0] == "data"
     ][0]
 
     initialized_arrays = False
 
     ## Check plots info
 
     if config["plots"]["flag"]:
         config["plots_flag"] = True
         plots_info = settings.parse_plots_info(config=config)
-        number_of_frames = 50
+        number_of_frames = config["plots"]["maximum_number_of_frames"]
         starting_frame = config["starting_frame"]
     else:
         config["plots_flag"] = False
         plots_info = {"file_name": "", "folder_name": "", "root_path": ""}
         number_of_frames = len(paths)
         starting_frame = 0
 
@@ -83,23 +81,26 @@
         print(f"Event: //{frame_number}")
         frame_number = int(frame_number)
 
         if config["plots_flag"]:
             plots_info["file_name"] = config["plots"]["file_name"] + f"_{frame_number}"
 
         with h5py.File(f"{file_name}", "r") as f:
-            data = np.array(f[h5_path][frame_number], dtype=np.int32)
+            data = np.array(f[data_hdf5_path][frame_number], dtype=np.int32)
             if not initialized_arrays:
                 _data_shape = data.shape
 
-            if config["burst_mode"]:
+            if config["burst_mode"]["on"]:
+                storage_cell_hdf5_path=config["burst_mode"]["storage_cell_hdf5_path"]
+                debug_hdf5_path=config["burst_mode"]["debug_hdf5_path"]
+                
                 storage_cell_number_of_frame = int(
-                    f["/entry/data/storage_cell_number"][frame_number]
+                    f[f"{storage_cell_hdf5_path}"][frame_number]
                 )
-                debug_from_raw_of_frame = np.array(f["/entry/data/debug"][frame_number])
+                debug_from_raw_of_frame = np.array(f[f"{debug_hdf5_path}"][frame_number])
 
         if not initialized_arrays:
             raw_dataset = np.zeros((number_of_frames, *_data_shape), dtype=np.int32)
             dataset = np.zeros((number_of_frames, *_data_shape), dtype=np.int32)
             refined_detector_center = np.zeros((number_of_frames, 2), dtype=np.float32)
             refined_center_flag = np.zeros(number_of_frames, dtype=np.int16)
 
@@ -114,22 +115,22 @@
                 (number_of_frames, 2), dtype=np.int16
             )
             detector_center_from_friedel_pairs = np.zeros(
                 (number_of_frames, 2), dtype=np.float32
             )
             shift_x_mm = np.zeros((number_of_frames,), dtype=np.float32)
             shift_y_mm = np.zeros((number_of_frames,), dtype=np.float32)
-            if config["burst_mode"]:
+            if config["burst_mode"]["on"]:
                 storage_cell_number = np.zeros((number_of_frames,), dtype=np.int16)
                 debug_from_raw = np.zeros((number_of_frames, 2), dtype=np.int16)
             initialized_arrays = True
 
         raw_dataset[index, :, :] = data
 
-        if config["burst_mode"]:
+        if config["burst_mode"]["on"]:
             storage_cell_number[index] = storage_cell_number_of_frame
             debug_from_raw[index, :] = debug_from_raw_of_frame
 
         calibrated_data = data
 
         dataset[index, :, :] = calibrated_data
 
@@ -218,16 +219,17 @@
             for x in beam_position_shift_in_pixels
         ]
         shift_x_mm[index] = detector_shift_in_mm[0]
         shift_y_mm[index] = detector_shift_in_mm[1]
 
     ## Create output path
     file_label = os.path.basename(file_name).split("/")[-1][:-3]
-    root_directory, path_on_raw = os.path.dirname(file_name).split("/converted/")
-    output_path = config["output_path"] + "/centered/" + path_on_raw
+    converted_path=config["input_path"].split("/")[-1]
+    root_directory, path_in_raw = os.path.dirname(file_name).split(converted_path)
+    output_path = config["output_path"] + path_in_raw
     path = pathlib.Path(output_path)
     path.mkdir(parents=True, exist_ok=True)
 
     ## Get camera length from PF8 pixel maps
     clen = float(np.mean(PF8Config.pixel_maps["z"]))
 
     ## Write centered file
@@ -239,28 +241,28 @@
             grp_data.attrs["NX_class"] = "NXdata"
             if not config["compression"]["compress_data"]:
                 grp_data.create_dataset("data", data=dataset)
             else:
                 grp_data.create_dataset(
                     "data",
                     data=dataset,
-                    compression=config["compression"]["type"],
+                    compression=config["compression"]["filter"],
                     compression_opts=config["compression"]["opts"]
                 )
 
             grp_data.create_dataset("raw_file_id", data=raw_file_id)
-            if config["burst_mode"]:
+            if config["burst_mode"]["on"]:
                 grp_data.create_dataset("storage_cell_number", data=storage_cell_number)
                 grp_data.create_dataset("debug", data=debug_from_raw)
             grp_shots = entry.create_group("shots")
             grp_shots.attrs["NX_class"] = "NXdata"
             grp_shots.create_dataset("detector_shift_x_in_mm", data=shift_x_mm)
             grp_shots.create_dataset("detector_shift_y_in_mm", data=shift_y_mm)
             grp_shots.create_dataset("refined_center_flag", data=refined_center_flag)
-            grp_proc = f.create_group("pre_processing")
+            grp_proc = f.create_group("preprocessing")
             grp_proc.attrs["NX_class"] = "NXdata"
             for key, value in BeambustersParam.items():
                 grp_proc.create_dataset(key, data=value)
             grp_proc.create_dataset("raw_path", data=paths)
             grp_proc.create_dataset(
                 "refined_detector_center", data=refined_detector_center
             )
```

### Comparing `beambusters-1.2.2/beambusters/settings.py` & `beambusters-1.3.0/beambusters/settings.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.2.2/pyproject.toml` & `beambusters-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beambusters"
-version = "1.2.2"
+version = "1.3.0"
 description = ""
 authors = ["Ana Rodrigues <anananacr@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 beambusters = "beambusters.main:app"
 
@@ -88,13 +88,13 @@
 tomlkit = "0.12.3"
 trove-classifiers = "2024.2.23"
 typing-extensions = "4.10.0"
 tzdata = "2024.1"
 urllib3 = "2.2.1"
 virtualenv = "20.25.1"
 zipp = "3.17.0"
-bblib = "2.0.3"
+bblib = "2.1.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `beambusters-1.2.2/PKG-INFO` & `beambusters-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: beambusters
-Version: 1.2.2
+Version: 1.3.0
 Summary: 
 Author: Ana Rodrigues
 Author-email: anananacr@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: abstract (==2022.7.10)
 Requires-Dist: base32hex (==1.0.2)
-Requires-Dist: bblib (==2.0.3)
+Requires-Dist: bblib (==2.1.0)
 Requires-Dist: black (==24.1.1)
 Requires-Dist: build (==1.0.3)
 Requires-Dist: cachecontrol (==0.14.0)
 Requires-Dist: certifi (==2024.2.2)
 Requires-Dist: cffi (==1.16.0)
 Requires-Dist: charset-normalizer (==3.3.2)
 Requires-Dist: cleo (==2.1.0)
```

