# Comparing `tmp/bblib-2.1.0.tar.gz` & `tmp/bblib-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-2.1.0.tar", max compression
+gzip compressed data, was "bblib-2.1.1.tar", max compression
```

## Comparing `bblib-2.1.0.tar` & `bblib-2.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-05-24 11:38:56.802416 bblib-2.1.0/LICENSE
--rw-r--r--   0        0        0     3914 2024-05-24 11:38:56.802416 bblib-2.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-24 11:38:56.802416 bblib-2.1.0/bblib/__init__.py
--rwxr-xr-x   0        0        0    38761 2024-05-24 11:38:56.802416 bblib-2.1.0/bblib/methods.py
--rwxr-xr-x   0        0        0    10130 2024-05-24 11:38:56.802416 bblib-2.1.0/bblib/models.py
--rwxr-xr-x   0        0        0    18200 2024-05-24 11:38:56.802416 bblib-2.1.0/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-05-24 11:39:07.974398 bblib-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7445 1970-01-01 00:00:00.000000 bblib-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-05-24 12:39:08.517947 bblib-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3914 2024-05-24 12:39:08.517947 bblib-2.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 12:39:08.517947 bblib-2.1.1/bblib/__init__.py
+-rwxr-xr-x   0        0        0    38819 2024-05-24 12:39:08.517947 bblib-2.1.1/bblib/methods.py
+-rwxr-xr-x   0        0        0    10130 2024-05-24 12:39:08.517947 bblib-2.1.1/bblib/models.py
+-rwxr-xr-x   0        0        0    18200 2024-05-24 12:39:08.517947 bblib-2.1.1/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-05-24 12:39:22.829980 bblib-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7445 1970-01-01 00:00:00.000000 bblib-2.1.1/PKG-INFO
```

### Comparing `bblib-2.1.0/LICENSE` & `bblib-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-2.1.0/README.md` & `bblib-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bblib-2.1.0/bblib/methods.py` & `bblib-2.1.1/bblib/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
         data_visualize = geometry.DataVisualizer(
             pixel_maps=non_shifted_pixel_maps_for_visualization
         )
 
         with h5py.File(f"{self.PF8Config.bad_pixel_map_filename}", "r") as f:
             mask = np.array(f[f"{self.PF8Config.bad_pixel_map_hdf5_path}"])
 
-        if self.config["polarization"]["skip"]:
+        if not self.config["polarization"]["apply_polarization_correction"]:
             peak_list = pf8.get_peaks_pf8(data=data)
             if (
                 self.PF8Config.pf8_detector_info["nasics_x"]
                 * self.PF8Config.pf8_detector_info["nasics_y"]
                 > 1
             ):
                 self.visual_data = data_visualize.visualize_data(data=data * mask)
@@ -703,15 +703,15 @@
         data_visualize = geometry.DataVisualizer(
             pixel_maps=non_shifted_pixel_maps_for_visualization
         )
 
         with h5py.File(f"{self.PF8Config.bad_pixel_map_filename}", "r") as f:
             mask = np.array(f[f"{self.PF8Config.bad_pixel_map_hdf5_path}"])
 
-        if self.config["polarization"]["skip"]:
+        if not self.config["polarization"]["apply_polarization_correction"]:
             peak_list = pf8.get_peaks_pf8(data=data)
             if (
                 self.PF8Config.pf8_detector_info["nasics_x"]
                 * self.PF8Config.pf8_detector_info["nasics_y"]
                 > 1
             ):
                 self.visual_data = data_visualize.visualize_data(data=data * mask)
```

### Comparing `bblib-2.1.0/bblib/models.py` & `bblib-2.1.1/bblib/models.py`

 * *Files identical despite different names*

### Comparing `bblib-2.1.0/bblib/utils.py` & `bblib-2.1.1/bblib/utils.py`

 * *Files identical despite different names*

### Comparing `bblib-2.1.0/pyproject.toml` & `bblib-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "2.1.0"
+version = "2.1.1"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-2.1.0/PKG-INFO` & `bblib-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 2.1.0
+Version: 2.1.1
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

