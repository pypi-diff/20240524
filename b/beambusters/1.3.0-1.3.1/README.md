# Comparing `tmp/beambusters-1.3.0.tar.gz` & `tmp/beambusters-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beambusters-1.3.0.tar", max compression
+gzip compressed data, was "beambusters-1.3.1.tar", max compression
```

## Comparing `beambusters-1.3.0.tar` & `beambusters-1.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-24 11:50:44.096361 beambusters-1.3.0/LICENSE
--rw-r--r--   0        0        0      630 2024-05-24 11:50:44.096361 beambusters-1.3.0/README.md
--rwxr-xr-x   0        0        0        0 2024-05-24 11:50:44.096361 beambusters-1.3.0/beambusters/__init__.py
--rw-r--r--   0        0        0    11938 2024-05-24 11:50:44.096361 beambusters-1.3.0/beambusters/main.py
--rwxr-xr-x   0        0        0     3170 2024-05-24 11:50:44.096361 beambusters-1.3.0/beambusters/settings.py
--rwxr-xr-x   0        0        0     1394 2024-05-24 11:50:44.096361 beambusters-1.3.0/beambusters/utils.py
--rw-r--r--   0        0        0     2026 2024-05-24 11:50:53.620432 beambusters-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 12:43:24.896475 beambusters-1.3.1/LICENSE
+-rw-r--r--   0        0        0      630 2024-05-24 12:43:24.896475 beambusters-1.3.1/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-24 12:43:24.896475 beambusters-1.3.1/beambusters/__init__.py
+-rw-r--r--   0        0        0    12068 2024-05-24 12:43:24.896475 beambusters-1.3.1/beambusters/main.py
+-rwxr-xr-x   0        0        0     3562 2024-05-24 12:43:24.896475 beambusters-1.3.1/beambusters/settings.py
+-rwxr-xr-x   0        0        0     1394 2024-05-24 12:43:24.896475 beambusters-1.3.1/beambusters/utils.py
+-rw-r--r--   0        0        0     2027 2024-05-24 12:43:37.180607 beambusters-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3969 1970-01-01 00:00:00.000000 beambusters-1.3.1/PKG-INFO
```

### Comparing `beambusters-1.3.0/LICENSE` & `beambusters-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.0/README.md` & `beambusters-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.0/beambusters/main.py` & `beambusters-1.3.1/beambusters/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             plots_info["file_name"] = config["plots"]["file_name"] + f"_{frame_number}"
 
         with h5py.File(f"{file_name}", "r") as f:
             data = np.array(f[data_hdf5_path][frame_number], dtype=np.int32)
             if not initialized_arrays:
                 _data_shape = data.shape
 
-            if config["burst_mode"]["on"]:
+            if config["burst_mode"]["is_active"]:
                 storage_cell_hdf5_path=config["burst_mode"]["storage_cell_hdf5_path"]
                 debug_hdf5_path=config["burst_mode"]["debug_hdf5_path"]
                 
                 storage_cell_number_of_frame = int(
                     f[f"{storage_cell_hdf5_path}"][frame_number]
                 )
                 debug_from_raw_of_frame = np.array(f[f"{debug_hdf5_path}"][frame_number])
@@ -115,80 +115,80 @@
                 (number_of_frames, 2), dtype=np.int16
             )
             detector_center_from_friedel_pairs = np.zeros(
                 (number_of_frames, 2), dtype=np.float32
             )
             shift_x_mm = np.zeros((number_of_frames,), dtype=np.float32)
             shift_y_mm = np.zeros((number_of_frames,), dtype=np.float32)
-            if config["burst_mode"]["on"]:
+            if config["burst_mode"]["is_active"]:
                 storage_cell_number = np.zeros((number_of_frames,), dtype=np.int16)
                 debug_from_raw = np.zeros((number_of_frames, 2), dtype=np.int16)
             initialized_arrays = True
 
         raw_dataset[index, :, :] = data
 
-        if config["burst_mode"]["on"]:
+        if config["burst_mode"]["is_active"]:
             storage_cell_number[index] = storage_cell_number_of_frame
             debug_from_raw[index, :] = debug_from_raw_of_frame
 
         calibrated_data = data
 
         dataset[index, :, :] = calibrated_data
 
         ## Refine the detector center
         ## Set geometry in PF8
 
         PF8Config.set_geometry_from_file(config["geometry_file"])
 
-        if "center_of_mass" not in config["skip_methods"]:
+        if "center_of_mass" not in config["skip_centering_methods"]:
             center_of_mass_method = CenterOfMass(
                 config=config, PF8Config=PF8Config, plots_info=plots_info
             )
             detector_center_from_center_of_mass[index, :] = center_of_mass_method(
                 data=calibrated_data
             )
 
-        if "circle_detection" not in config["skip_methods"]:
+        if "circle_detection" not in config["skip_centering_methods"]:
             circle_detection_method = CircleDetection(
                 config=config, PF8Config=PF8Config, plots_info=plots_info
             )
             detector_center_from_circle_detection[index, :] = circle_detection_method(
                 data=calibrated_data
             )
 
         ## Define the initial_guess
 
-        if config["force_center"]["mode"]:
+        if config["force_center"]["state"]:
             initial_guess = [config["force_center"]["x"], config["force_center"]["y"]]
-        elif config["method"] == "center_of_mass":
+        elif config["centering_method_for_initial_guess"] == "center_of_mass":
             initial_guess = detector_center_from_center_of_mass[index]
-        elif config["method"] == "circle_detection":
+        elif config["centering_method_for_initial_guess"] == "circle_detection":
             initial_guess = detector_center_from_circle_detection[index]
         else:
             initial_guess = PF8Config.detector_center_from_geom
 
         initial_guess_center[index, :] = initial_guess
 
         distance = math.sqrt(
-            (initial_guess[0] - config["force_center"]["x"]) ** 2
-            + (initial_guess[1] - config["force_center"]["y"]) ** 2
+            (initial_guess[0] - config["reference_center"]["x"]) ** 2
+            + (initial_guess[1] - config["reference_center"]["y"]) ** 2
         )
 
         if distance < config["outlier_distance"]:
             ## Ready for detector center refinement
             PF8Config.update_pixel_maps(
                 initial_guess[0] - PF8Config.detector_center_from_geom[0],
                 initial_guess[1] - PF8Config.detector_center_from_geom[1],
             )
 
             pf8 = PF8(PF8Config)
             peak_list = pf8.get_peaks_pf8(data=calibrated_data)
             PF8Config.set_geometry_from_file(config["geometry_file"])
 
-            if "friedel_pairs" not in config["skip_methods"]:
+            if "friedel_pairs" not in config["skip_centering_methods"]:
                 PF8Config.set_geometry_from_file(config["geometry_file"])
                 friedel_pairs_method = FriedelPairs(
                     config=config, PF8Config=PF8Config, plots_info=plots_info
                 )
                 detector_center_from_friedel_pairs[index, :] = friedel_pairs_method(
                     data=calibrated_data, initial_guess=initial_guess
                 )
@@ -235,26 +235,26 @@
     ## Write centered file
     if not test_only:
         with h5py.File(f"{output_path}/{file_label}.h5", "w") as f:
             entry = f.create_group("entry")
             entry.attrs["NX_class"] = "NXentry"
             grp_data = entry.create_group("data")
             grp_data.attrs["NX_class"] = "NXdata"
-            if not config["compression"]["compress_data"]:
+            if not config["compression"]["compress_output_data"]:
                 grp_data.create_dataset("data", data=dataset)
             else:
                 grp_data.create_dataset(
                     "data",
                     data=dataset,
                     compression=config["compression"]["filter"],
                     compression_opts=config["compression"]["opts"]
                 )
 
             grp_data.create_dataset("raw_file_id", data=raw_file_id)
-            if config["burst_mode"]["on"]:
+            if config["burst_mode"]["is_active"]:
                 grp_data.create_dataset("storage_cell_number", data=storage_cell_number)
                 grp_data.create_dataset("debug", data=debug_from_raw)
             grp_shots = entry.create_group("shots")
             grp_shots.attrs["NX_class"] = "NXdata"
             grp_shots.create_dataset("detector_shift_x_in_mm", data=shift_x_mm)
             grp_shots.create_dataset("detector_shift_y_in_mm", data=shift_y_mm)
             grp_shots.create_dataset("refined_center_flag", data=refined_center_flag)
```

### Comparing `beambusters-1.3.0/beambusters/utils.py` & `beambusters-1.3.1/beambusters/utils.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.0/pyproject.toml` & `beambusters-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beambusters"
-version = "1.3.0"
+version = "1.3.1"
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
-bblib = "2.1.0"
+bblib = "^2.1.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `beambusters-1.3.0/PKG-INFO` & `beambusters-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: beambusters
-Version: 1.3.0
+Version: 1.3.1
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
-Requires-Dist: bblib (==2.1.0)
+Requires-Dist: bblib (>=2.1.1,<3.0.0)
 Requires-Dist: black (==24.1.1)
 Requires-Dist: build (==1.0.3)
 Requires-Dist: cachecontrol (==0.14.0)
 Requires-Dist: certifi (==2024.2.2)
 Requires-Dist: cffi (==1.16.0)
 Requires-Dist: charset-normalizer (==3.3.2)
 Requires-Dist: cleo (==2.1.0)
```

