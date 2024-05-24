# Comparing `tmp/viirs-tools-0.1.1.tar.gz` & `tmp/viirs-tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viirs-tools-0.1.1.tar", last modified: Sun Apr 28 20:00:43 2024, max compression
+gzip compressed data, was "viirs-tools-1.0.0.tar", last modified: Fri May 24 07:21:54 2024, max compression
```

## Comparing `viirs-tools-0.1.1.tar` & `viirs-tools-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-28 20:00:43.788798 viirs-tools-0.1.1/
--rw-r--r--   0 andmin    (1000) users      (984)    11358 2024-04-12 22:48:16.000000 viirs-tools-0.1.1/LICENSE
--rw-r--r--   0 andmin    (1000) users      (984)    17191 2024-04-28 20:00:43.788798 viirs-tools-0.1.1/PKG-INFO
--rw-r--r--   0 andmin    (1000) users      (984)     3591 2024-04-16 16:53:39.000000 viirs-tools-0.1.1/README.md
--rw-r--r--   0 andmin    (1000) users      (984)       38 2024-04-28 20:00:43.788798 viirs-tools-0.1.1/setup.cfg
--rw-r--r--   0 andmin    (1000) users      (984)      939 2024-04-28 17:06:20.000000 viirs-tools-0.1.1/setup.py
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-28 20:00:43.786798 viirs-tools-0.1.1/viirs_tools/
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-28 20:00:43.787798 viirs-tools-0.1.1/viirs_tools/Assimilator/
--rw-r--r--   0 andmin    (1000) users      (984)     4351 2024-04-19 22:01:45.000000 viirs-tools-0.1.1/viirs_tools/Assimilator/Assimilator.py
--rw-r--r--   0 andmin    (1000) users      (984)     2400 2024-04-12 18:17:28.000000 viirs-tools-0.1.1/viirs_tools/Assimilator/Reading.py
--rw-r--r--   0 andmin    (1000) users      (984)     1958 2024-04-12 18:23:24.000000 viirs-tools-0.1.1/viirs_tools/Assimilator/ReadingHelpers.py
--rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-12 18:13:42.000000 viirs-tools-0.1.1/viirs_tools/Assimilator/__init__.py
--rw-r--r--   0 andmin    (1000) users      (984)     8664 2024-04-28 17:05:50.000000 viirs-tools-0.1.1/viirs_tools/CloudMask.py
--rw-r--r--   0 andmin    (1000) users      (984)     3683 2024-04-12 21:14:32.000000 viirs-tools-0.1.1/viirs_tools/NightMask.py
--rw-r--r--   0 andmin    (1000) users      (984)     3159 2024-04-28 16:41:06.000000 viirs-tools-0.1.1/viirs_tools/Utils.py
--rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-11 15:10:43.000000 viirs-tools-0.1.1/viirs_tools/__init__.py
-drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-04-28 20:00:43.787798 viirs-tools-0.1.1/viirs_tools.egg-info/
--rw-r--r--   0 andmin    (1000) users      (984)    17191 2024-04-28 20:00:42.000000 viirs-tools-0.1.1/viirs_tools.egg-info/PKG-INFO
--rw-r--r--   0 andmin    (1000) users      (984)      447 2024-04-28 20:00:43.000000 viirs-tools-0.1.1/viirs_tools.egg-info/SOURCES.txt
--rw-r--r--   0 andmin    (1000) users      (984)        1 2024-04-28 20:00:43.000000 viirs-tools-0.1.1/viirs_tools.egg-info/dependency_links.txt
--rw-r--r--   0 andmin    (1000) users      (984)       30 2024-04-28 20:00:43.000000 viirs-tools-0.1.1/viirs_tools.egg-info/requires.txt
--rw-r--r--   0 andmin    (1000) users      (984)       12 2024-04-28 20:00:43.000000 viirs-tools-0.1.1/viirs_tools.egg-info/top_level.txt
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-05-24 07:21:54.310414 viirs-tools-1.0.0/
+-rw-r--r--   0 andmin    (1000) users      (984)    11358 2024-04-12 22:48:16.000000 viirs-tools-1.0.0/LICENSE
+-rw-r--r--   0 andmin    (1000) users      (984)    18049 2024-05-24 07:21:54.309414 viirs-tools-1.0.0/PKG-INFO
+-rw-r--r--   0 andmin    (1000) users      (984)     4449 2024-05-24 07:08:56.000000 viirs-tools-1.0.0/README.md
+-rw-r--r--   0 andmin    (1000) users      (984)       38 2024-05-24 07:21:54.311415 viirs-tools-1.0.0/setup.cfg
+-rw-r--r--   0 andmin    (1000) users      (984)      939 2024-05-19 18:18:46.000000 viirs-tools-1.0.0/setup.py
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-05-24 07:21:54.301410 viirs-tools-1.0.0/viirs_tools/
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-05-24 07:21:54.306412 viirs-tools-1.0.0/viirs_tools/Assimilator/
+-rw-r--r--   0 andmin    (1000) users      (984)     4351 2024-04-19 22:01:45.000000 viirs-tools-1.0.0/viirs_tools/Assimilator/Assimilator.py
+-rw-r--r--   0 andmin    (1000) users      (984)     2400 2024-04-12 18:17:28.000000 viirs-tools-1.0.0/viirs_tools/Assimilator/Reading.py
+-rw-r--r--   0 andmin    (1000) users      (984)     1958 2024-04-12 18:23:24.000000 viirs-tools-1.0.0/viirs_tools/Assimilator/ReadingHelpers.py
+-rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-12 18:13:42.000000 viirs-tools-1.0.0/viirs_tools/Assimilator/__init__.py
+-rw-r--r--   0 andmin    (1000) users      (984)     8016 2024-05-17 15:20:13.000000 viirs-tools-1.0.0/viirs_tools/CloudMask.py
+-rw-r--r--   0 andmin    (1000) users      (984)     5786 2024-05-19 23:03:59.000000 viirs-tools-1.0.0/viirs_tools/Fires.py
+-rw-r--r--   0 andmin    (1000) users      (984)     8613 2024-05-17 20:12:54.000000 viirs-tools-1.0.0/viirs_tools/LST.py
+-rw-r--r--   0 andmin    (1000) users      (984)     3668 2024-05-14 11:45:07.000000 viirs-tools-1.0.0/viirs_tools/NightMask.py
+-rw-r--r--   0 andmin    (1000) users      (984)     4574 2024-05-17 15:35:22.000000 viirs-tools-1.0.0/viirs_tools/Utils.py
+-rw-r--r--   0 andmin    (1000) users      (984)     2651 2024-05-17 15:10:41.000000 viirs-tools-1.0.0/viirs_tools/Water.py
+-rw-r--r--   0 andmin    (1000) users      (984)        0 2024-04-11 15:10:43.000000 viirs-tools-1.0.0/viirs_tools/__init__.py
+drwxr-xr-x   0 andmin    (1000) users      (984)        0 2024-05-24 07:21:54.307413 viirs-tools-1.0.0/viirs_tools.egg-info/
+-rw-r--r--   0 andmin    (1000) users      (984)    18049 2024-05-24 07:21:53.000000 viirs-tools-1.0.0/viirs_tools.egg-info/PKG-INFO
+-rw-r--r--   0 andmin    (1000) users      (984)      508 2024-05-24 07:21:54.000000 viirs-tools-1.0.0/viirs_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 andmin    (1000) users      (984)        1 2024-05-24 07:21:53.000000 viirs-tools-1.0.0/viirs_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 andmin    (1000) users      (984)       30 2024-05-24 07:21:53.000000 viirs-tools-1.0.0/viirs_tools.egg-info/requires.txt
+-rw-r--r--   0 andmin    (1000) users      (984)       12 2024-05-24 07:21:53.000000 viirs-tools-1.0.0/viirs_tools.egg-info/top_level.txt
```

### Comparing `viirs-tools-0.1.1/LICENSE` & `viirs-tools-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.1.1/PKG-INFO` & `viirs-tools-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viirs-tools
-Version: 0.1.1
+Version: 1.0.0
 Summary: Python library for processing VIIRS data
 Home-page: https://github.com/Veon2479/viirs-tools
 Author: Andrey Shuliak
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -245,32 +245,49 @@
 
 ## Usage
 
 The `viirs-tools` library provides the following core modules and their main functions:
 
 1. **CloudMask**:
    + `rsnpp_day_img`: Day reflectance/thermal I-bands cloud test. [^1]
-   + `thermal_img`: Night thermal I-bands cloud test. [^2]
-   + `day_night_img`: Day/night cloud mask based on the previous 2
-
+   + `fire_day_img`, `fire_night_img`: Day and night I-bands cloud tests used in the [^2].
 
 2. **NightMask**:
    + `naive`: Day/night mask, based on the difference between presence of reflectance and thermal data, for both I- and M-bands
 
-3. **Utils**:
+3. **Water**:
+   + `water_bodies_day`: Day reflectance tests for water bodies from [^2]
+
+4. **LST**:
+   + `mono_window_i05`, `mono_window_m16`, `mono_window_m15`: LST retrieval for I05 band, based on the LANDSAT-8 alg [^3]
+
+5. **Fires**:
+   + `active_fires`: Active fire detection from [^2]
+
+6. **Utils**:
    - Just some helpful functions
 
-4. **Assimilator** submodule:
+7. **Assimilator** submodule:
 	1. **Assimilator**:
 		- `assimilate`: Retrieving data from NASA archives using [cmrfetch](https://github.com/bmflynn/cmrfetch), with support for handy data collection process management
 	2. **Reading**
 		- `read_npp_viaes_l1`: Reading [VIIRS/NPP Imagery Resolution 6-Min L1 Swath SDR 375m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/NPP_VIAES_L1#product-information) product files
 		- `read_npp_vmaes_l1`: Reading [VIIRS/NPP Moderate Resolution 6-Min L1 Swath SDR and GEO 750m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/NPP_VMAES_L1) product files
 		- `read_npp_cldmsk_l2`: Reading [VIIRS/SNPP Cloud Mask 6-Min Swath 750m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/CLDMSK_L2_VIIRS_SNPP#product-information) product files
 	3. **ReadingHelpers**
 		- Contains some helper functions for reading files that aren't supported by `SatPy` module (some examples of using them in the previous module)
 
 
+## Demo
+You can find demo Qt6 app in the `viirs-demo` folder. Note that it requires additional packages to be installed installed - `rasterio`,  `matplotlib`,  `PyQt6` and `TensorFlow`. Run `viirs-demo.py` to start it. Data for this demo can be found in the `demo-data` folder.
+
+
+## Additional tools
+In the `scripts` folder you can find useful tools for local satellite data analysis, such `assimilate.py` script. It was used for gathering data in the `demo-data` folder.
+
+
 ## References
 [^1]: M.Piper, T.Bahr (2015). A RAPID CLOUD MASK ALGORITHM FOR SUOMI NPP VIIRS IMAGERY EDRS.
 
 [^2]: W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014). The New VIIRS 375 m active fire detection data product: Algorithm description and initial assessment.
+
+[^3]: U.Avdan, G.Jovanovska (2016). Algorithm for Automated Mapping of Land Surface Temperature Using LANDSAT 8 Satellite Data
```

### Comparing `viirs-tools-0.1.1/README.md` & `viirs-tools-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -25,32 +25,49 @@
 
 ## Usage
 
 The `viirs-tools` library provides the following core modules and their main functions:
 
 1. **CloudMask**:
    + `rsnpp_day_img`: Day reflectance/thermal I-bands cloud test. [^1]
-   + `thermal_img`: Night thermal I-bands cloud test. [^2]
-   + `day_night_img`: Day/night cloud mask based on the previous 2
-
+   + `fire_day_img`, `fire_night_img`: Day and night I-bands cloud tests used in the [^2].
 
 2. **NightMask**:
    + `naive`: Day/night mask, based on the difference between presence of reflectance and thermal data, for both I- and M-bands
 
-3. **Utils**:
+3. **Water**:
+   + `water_bodies_day`: Day reflectance tests for water bodies from [^2]
+
+4. **LST**:
+   + `mono_window_i05`, `mono_window_m16`, `mono_window_m15`: LST retrieval for I05 band, based on the LANDSAT-8 alg [^3]
+
+5. **Fires**:
+   + `active_fires`: Active fire detection from [^2]
+
+6. **Utils**:
    - Just some helpful functions
 
-4. **Assimilator** submodule:
+7. **Assimilator** submodule:
 	1. **Assimilator**:
 		- `assimilate`: Retrieving data from NASA archives using [cmrfetch](https://github.com/bmflynn/cmrfetch), with support for handy data collection process management
 	2. **Reading**
 		- `read_npp_viaes_l1`: Reading [VIIRS/NPP Imagery Resolution 6-Min L1 Swath SDR 375m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/NPP_VIAES_L1#product-information) product files
 		- `read_npp_vmaes_l1`: Reading [VIIRS/NPP Moderate Resolution 6-Min L1 Swath SDR and GEO 750m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/NPP_VMAES_L1) product files
 		- `read_npp_cldmsk_l2`: Reading [VIIRS/SNPP Cloud Mask 6-Min Swath 750m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/CLDMSK_L2_VIIRS_SNPP#product-information) product files
 	3. **ReadingHelpers**
 		- Contains some helper functions for reading files that aren't supported by `SatPy` module (some examples of using them in the previous module)
 
 
+## Demo
+You can find demo Qt6 app in the `viirs-demo` folder. Note that it requires additional packages to be installed installed - `rasterio`,  `matplotlib`,  `PyQt6` and `TensorFlow`. Run `viirs-demo.py` to start it. Data for this demo can be found in the `demo-data` folder.
+
+
+## Additional tools
+In the `scripts` folder you can find useful tools for local satellite data analysis, such `assimilate.py` script. It was used for gathering data in the `demo-data` folder.
+
+
 ## References
 [^1]: M.Piper, T.Bahr (2015). A RAPID CLOUD MASK ALGORITHM FOR SUOMI NPP VIIRS IMAGERY EDRS.
 
 [^2]: W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014). The New VIIRS 375 m active fire detection data product: Algorithm description and initial assessment.
+
+[^3]: U.Avdan, G.Jovanovska (2016). Algorithm for Automated Mapping of Land Surface Temperature Using LANDSAT 8 Satellite Data
```

### Comparing `viirs-tools-0.1.1/setup.py` & `viirs-tools-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     name='viirs-tools',
     description='Python library for processing VIIRS data',
     long_description_content_type='text/markdown',
     long_description=long_description,
     url='https://github.com/Veon2479/viirs-tools',
     license=license_text,
     author='Andrey Shuliak',
-    version='0.1.1',
+    version='1.0.0',
     packages=find_packages(),
     install_requires=[
         'xarray',
     ],
     extras_require={
         'assimilator': ['netcdf4']
     },
```

### Comparing `viirs-tools-0.1.1/viirs_tools/Assimilator/Assimilator.py` & `viirs-tools-1.0.0/viirs_tools/Assimilator/Assimilator.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.1.1/viirs_tools/Assimilator/Reading.py` & `viirs-tools-1.0.0/viirs_tools/Assimilator/Reading.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.1.1/viirs_tools/Assimilator/ReadingHelpers.py` & `viirs-tools-1.0.0/viirs_tools/Assimilator/ReadingHelpers.py`

 * *Files identical despite different names*

### Comparing `viirs-tools-0.1.1/viirs_tools/CloudMask.py` & `viirs-tools-1.0.0/viirs_tools/CloudMask.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import xarray as xr
-import math
+from math import nan
 
 from . import Utils
 
 
 # Internal functions:
 
 
-def _rsnpp_day_img(ri1, ri2, ri3, bi4, bi5, nmask):
+def _rsnpp_day_img(ri1, ri2, ri3, bi4, bi5):
     """
         Day reflectance/thermal I-bands cloud test
         Based on the M.Piper, T.Bahr (2015).
         A RAPID CLOUD MASK ALGORITHM FOR SUOMI NPP VIIRS IMAGERY EDRS
     Args:
-        ri1 (list|np.ndarray|xr.Dataset): I01 in reflectance calibration
-        ri2 (list|np.ndarray|xr.Dataset): I02 in reflectance calibration
-        ri3 (list|np.ndarray|xr.Dataset): I03 in reflectance calibration
-        bi4 (list|np.ndarray|xr.Dataset): I04 in BT calibration
-        bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
-        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
+        ri1 (np.ndarray|xr.Dataset): I01 in reflectance calibration
+        ri2 (np.ndarray|xr.Dataset): I02 in reflectance calibration
+        ri3 (np.ndarray|xr.Dataset): I03 in reflectance calibration
+        bi4 (np.ndarray|xr.Dataset): I04 in BT calibration
+        bi5 (np.ndarray|xr.Dataset): I05 in BT calibration
     Returns:
-        (list|np.ndarray|xr.Dataset): integer cloud mask,
+        (np.ndarray|xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
 
     t1 = xr.where(ri1 > 8, True, False)
 
     ndsi = (ri1 - ri3) / (ri1 + ri3)
@@ -42,32 +41,31 @@
 
     cm = xr.where(t1 & t2, 0, 1)
     cm = xr.where(cm & t3, 0, 1)
     cm = xr.where(cm & t4, 0, 1)
     cm = xr.where(cm & t5, 0, 1)
     cm = xr.where(cm & t6, 0, 1)
 
-    cm = xr.where(nmask == 0, cm, math.nan)
-
+    nanmask = Utils.nan_mask(ri1)
+    cm = xr.where(nanmask, nan, cm)
     return cm
 
 
-def _fire_day_img(ri1, ri2, bi5, nmask):
+def _fire_day_img(ri1, ri2, bi5):
     """
         Day reflectance & termal I-bands cloud test
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
-        ri1 (list|np.ndarray|xr.Dataset): I01 in reflectance calibration
-        ri2 (list|np.ndarray|xr.Dataset): I02 in reflectance calibration
-        bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
-        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
+        ri1 (np.ndarray|xr.Dataset): I01 in reflectance calibration
+        ri2 (np.ndarray|xr.Dataset): I02 in reflectance calibration
+        bi5 (np.ndarray|xr.Dataset): I05 in BT calibration
     Returns:
-        (list|np.ndarray|xr.Dataset): integer cloud mask,
+        (np.ndarray|xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     cm = xr.where(bi5 < 265, 0, 1)
 
     sum_ri = ri1 + ri2
 
@@ -76,195 +74,185 @@
 
     t3 = xr.where(sum_ri > 70, 0, 1)
     t3 = xr.where(bi5 < 285, t2, 1)
 
     cm = xr.where(t2 == 0, 0, cm)
     cm = xr.where(t3 == 0, 0, cm)
 
-    cm = xr.where(nmask == 0, cm, math.nan)
+    cm = xr.where(ri1 is nan, nan, cm)
     return cm
 
 
-def _fire_night_img(bi4, bi5, nmask):
+def _fire_night_img(bi4, bi5, nmask=None):
     """
         Night termal I-bands cloud test
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
-        bi4 (list|np.ndarray|xr.Dataset): I04 in BT calibration
-        bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
-        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
+        bi4 (np.ndarray|xr.Dataset): I04 in BT calibration
+        bi5 (np.ndarray|xr.Dataset): I05 in BT calibration
+        nmask (np.ndarray|xr.Dataset, optional): Day/night mask (1 is night)
     Returns:
-        (list|np.ndarray|xr.Dataset): integer cloud mask,
+        (np.ndarray|xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     cm = xr.where(bi4 < 265, 0, 1)
     cm = xr.where(bi5 < 295, cm, 0)
-    cm = xr.where(Utils.not_nan_mask(bi4), cm, math.nan)
-
-    cm = xr.where(nmask == 1, cm, math.nan)
+    cm = xr.where(Utils.not_nan_mask(bi4), cm, nan)
 
+    if nmask is not None:
+        cm = xr.where(nmask == 1, cm, nan)
+    else:
+        cm = xr.where(bi4 is nan, nan, cm)
     return cm
 
 
 # Public wrappers:
 
 
-def rsnpp_day_img(ri1, ri2, ri3, bi4, bi5, nmask):
+def rsnpp_day_img(ri1, ri2, ri3, bi4, bi5):
     """
         Day reflectance/thermal I-bands cloud test
         Based on the M.Piper, T.Bahr (2015).
         A RAPID CLOUD MASK ALGORITHM FOR SUOMI NPP VIIRS IMAGERY EDRS
     Args:
-        ri1 (list|np.ndarray|xr.Dataset): I01 in reflectance calibration
-        ri2 (list|np.ndarray|xr.Dataset): I02 in reflectance calibration
-        ri3 (list|np.ndarray|xr.Dataset): I03 in reflectance calibration
-        bi4 (list|np.ndarray|xr.Dataset): I04 in BT calibration
-        bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
-        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
+        ri1 (np.ndarray|xr.Dataset): I01 in reflectance calibration
+        ri2 (np.ndarray|xr.Dataset): I02 in reflectance calibration
+        ri3 (np.ndarray|xr.Dataset): I03 in reflectance calibration
+        bi4 (np.ndarray|xr.Dataset): I04 in BT calibration
+        bi5 (np.ndarray|xr.Dataset): I05 in BT calibration
     Returns:
-        (list|np.ndarray|xr.Dataset): integer cloud mask,
+        (np.ndarray|xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     Utils._check_data(ri1)
     Utils._check_data(ri2)
     Utils._check_data(ri3)
     Utils._check_data(bi4)
     Utils._check_data(bi5)
-    Utils._check_data(nmask)
 
     return _rsnpp_day_img(
         ri1, ri2, ri3,
-        bi4, bi5,
-        nmask
+        bi4, bi5
     )
 
 
-def fire_day_img(ri1, ri2, bi5, nmask):
+def fire_day_img(ri1, ri2, bi5):
     """
         Day reflectance & termal I-bands cloud test
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
-        ri1 (list|np.ndarray|xr.Dataset): I01 in reflectance calibration
-        ri2 (list|np.ndarray|xr.Dataset): I02 in reflectance calibration
-        bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
-        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
+        ri1 (np.ndarray|xr.Dataset): I01 in reflectance calibration
+        ri2 (np.ndarray|xr.Dataset): I02 in reflectance calibration
+        bi5 (np.ndarray|xr.Dataset): I05 in BT calibration
     Returns:
-        (list|np.ndarray|xr.Dataset): integer cloud mask,
+        (np.ndarray|xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     Utils._check_data(ri1)
     Utils._check_data(ri2)
     Utils._check_data(bi5)
-    return _fire_day_img(ri1, ri2, bi5, nmask)
+    return _fire_day_img(ri1, ri2, bi5)
 
 
-def fire_night_img(bi4, bi5, nmask):
+def fire_night_img(bi4, bi5, nmask=None):
     """
         Night termal I-bands cloud test
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
-        bi4 (list|np.ndarray|xr.Dataset): I04 in BT calibration
-        bi5 (list|np.ndarray|xr.Dataset): I05 in BT calibration
-        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
+        bi4 (np.ndarray|xr.Dataset): I04 in BT calibration
+        bi5 (np.ndarray|xr.Dataset): I05 in BT calibration
+        nmask (np.ndarray|xr.Dataset, optional): Day/night mask (1 is night)
     Returns:
-        (list|np.ndarray|xr.Dataset): integer cloud mask,
+        (np.ndarray|xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     Utils._check_data(bi4)
     Utils._check_data(bi5)
-    return _fire_night_img(bi4, bi5, nmask)
+    return _fire_night_img(bi4, bi5, nmask=nmask)
 
 
 # Public xr.Dataset wrappers:
 
 
-def rsnpp_day_img_ds(ds, nmask):
+def rsnpp_day_img_ds(ds):
     """
         Wrapper for day reflectance/thermal I-bands cloud test
             for xr.Dataset objects
         Based on the M.Piper, T.Bahr (2015).
         A RAPID CLOUD MASK ALGORITHM FOR SUOMI NPP VIIRS IMAGERY EDRS
     Args:
         ds (xr.Dataset): dataset with I01-I05 bands data
-        nmask (xr.Dataset): Day/night mask (1 is night)
     Returns:
         (xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     if not isinstance(ds, xr.Dataset):
         raise ValueError(
             "Incorrect input data format"
         )
-    if not isinstance(nmask, xr.DataArray):
-        raise ValueError(
-            "Incorrect input data format"
-        )
     return rsnpp_day_img(
         ds['I01'],
         ds['I02'],
         ds['I03'],
         ds['I04'],
-        ds['I05'],
-        nmask
+        ds['I05']
     )
 
 
-def fire_day_img_ds(ds, nmask):
+def fire_day_img_ds(ds):
     """
         Wrapper for Day reflectance & termal I-bands cloud test for xr.Dataset
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
         ds (xr.Dataset): dataset with I01, I02, I05 bands data
-        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
     Returns:
         (xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     if not isinstance(ds, xr.Dataset):
         raise ValueError(
             "Incorrect input data format"
         )
     return fire_day_img(
         ds['I01'],
         ds['I02'],
-        ds['I05'],
-        nmask
+        ds['I05']
     )
 
 
-def fire_night_img_ds(ds, nmask):
+def fire_night_img_ds(ds, nmask=None):
     """
         Wrapper for Night termal I-bands cloud test for xr.Dataset
         Based on the W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014).
         The New VIIRS 375 m active fire detection data product:
             Algorithm description and initial assessment
     Args:
         ds (xr.Dataset): dataset with I04, I05 bands data
-        nmask (list|np.ndarray|xr.Dataset): Day/night mask (1 is night)
+        nmask (np.ndarray|xr.Dataset, optional): Day/night mask (1 is night)
     Returns:
         (xr.Dataset): integer cloud mask,
             0 is cloud, 1 is clear pixel
             Can contain NaN values
     """
     if not isinstance(ds, xr.Dataset):
         raise ValueError(
             "Incorrect input data format"
         )
     return fire_night_img(
         ds['I04'],
         ds['I05'],
-        nmask
+        nmask=nmask
     )
```

### Comparing `viirs-tools-0.1.1/viirs_tools/NightMask.py` & `viirs-tools-1.0.0/viirs_tools/NightMask.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 def naive(refband, btband):
     """
         Get night mask from any reflectance and brightness bands
         Day/Night state here meets the condition SZA < 90 deg
         Assumed that data was loaded in the reflectance or
             brightness-temperature, not radiance calibration
     Args:
-        refband (list|np.ndarray|xr.DataArray):
+        refband (np.ndarray|xr.DataArray):
             any reflectance data
-        btband (list|np.ndarray|xr.DataArray):
+        btband (np.ndarray|xr.DataArray):
             any brightness-temperature data
     Returns:
-        (list|np.ndarray|xr.DataArray): integer mask,
+        (np.ndarray|xr.DataArray): integer mask,
             1 means night state, 0 means day state,
             Can contain NaN values in case of missing data in BT band
     """
     bmask = Utils.not_nan_mask(btband)
     rmask = Utils.nan_mask(refband)
     return xr.where(bmask, rmask, math.nan).astype(float)
```

### Comparing `viirs-tools-0.1.1/viirs_tools/Utils.py` & `viirs-tools-1.0.0/viirs_tools/Utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import xarray as xr
 import numpy as np
-import math
+from math import nan
 
 # Internal functions:
 
 
 def _check_data(data):
     """
         Check object for being of appropriate type
         Currently supported types:
-            * list
             * np.ndarray
             * xr.DataArray
     Args:
         data (any): object to be tested
     """
-    if not isinstance(data, (list, np.ndarray, xr.DataArray)):
+    if not isinstance(data, (np.ndarray, xr.DataArray)):
         raise ValueError(
-            "Input data is not array (built-in, np or xr) object"
+            "Input data is not array (numpy or xarray) object"
         )
 
 
 def _get_da(ds, name):
     """
         Helper function for preserving datasets attributes
         that are crucial for later operations
@@ -45,77 +44,127 @@
 
 def max_values(data):
     """
         Single function for finding
         max values per time slice
         for various data forms
     Args:
-        data (list|np.ndarray|xr.DataArray):
+        data (np.ndarray|xr.DataArray):
             slice or set of slices for searching for max values
     Returns
         (xr.DataArray|dtype of data vales):
             max value for given slice or xr.Datarray of such values
             with time dimension
     """
-    if isinstance(data, (list, np.ndarray)):
+    if isinstance(data, np.ndarray):
         return np.nanmax(data)
-    else:
+    elif isinstance(data, xr.DataArray):
         dims = list(data.dims)
         data_max = None
         if 'time' in dims:
             dims.pop(dims.index('time'))
             data_max = data.max(dim=dims)
         else:
             data_max = data.max(dim=dims).item()
+    else:
+        raise ValueError(
+            "Input data is not array (numpy or xarray) object"
+        )
+    return data_max
+
+
+def median_values(data):
+    """
+        Single function for finding
+        median values per time slice
+        for various data forms
+    Args:
+        data (np.ndarray|xr.DataArray):
+            slice or set of slices for searching for max values
+    Returns
+        (xr.DataArray|dtype of data vales):
+            median value for given slice or xr.Datarray of such values
+            with time dimension
+    """
+    if isinstance(data, np.ndarray):
+        return np.nanmedian(data)
+    elif isinstance(data, xr.DataArray):
+        dims = list(data.dims)
+        data_max = None
+        if 'time' in dims:
+            dims.pop(dims.index('time'))
+            data_max = data.median(dim=dims)
+        else:
+            data_max = data.median(dim=dims).item()
+    else:
+        raise ValueError(
+            "Input data is not array (numpy or xarray) object"
+        )
     return data_max
 
 
 def nan_mask(data):
     """
         Performs type-independent Nan-checking
     Args:
-        data(list|np.ndarray|xr.DataArray|xr.Dataset):
+        data(np.ndarray|xr.DataArray|xr.Dataset):
             object to be tested
     """
-    if isinstance(data, (list, np.ndarray)):
+    if isinstance(data, np.ndarray):
         return np.isnan(data)
     elif isinstance(data, (xr.DataArray, xr.Dataset)):
         return data.isnull()
     else:
         raise ValueError(
-            "Input data is not array (built-in, np or xr) object"
+            "Input data is not array (numpy or xarray) object"
         )
 
 
 def not_nan_mask(data):
     """
         Performs type-independent not-Nan-checking
     Args:
-        data(list|np.ndarray|xr.DataArray|xr.Dataset):
+        data(np.ndarray|xr.DataArray|xr.Dataset):
             object to be tested
     """
-    if isinstance(data, (list, np.ndarray)):
+    if isinstance(data, np.ndarray):
         return np.logical_not(np.isnan(data))
     elif isinstance(data, (xr.DataArray, xr.Dataset)):
         return data.notnull()
     else:
         raise ValueError(
             "Input data is not array (built-in, np or xr) object"
         )
 
 
-def merge_masks(day_cm, night_cm, nm):
+def merge_day_night(day, night, nm):
     """
-        Merge day and night cloud masks
+        Merge day and night composits
     Args:
-        day_cm(list|np.ndarray|xr.DataArray):
-            day cloud mask
-        night_cm(list|np.ndarray|xr.DataArray):
-            night cloud mask
-        nm(list|np.ndarray|xr.DataArray):
+        day_cm(np.ndarray|xr.DataArray):
+            day composit
+        night_cm(np.ndarray|xr.DataArray):
+            night composit
+        nm(np.ndarray|xr.DataArray):
             binary night mask
     Returns:
-        (list|np.ndarray|xr.DataArray):
-            merged cloud mask
+        (np.ndarray|xr.DataArray):
+            merged composit
     """
-    mask = xr.where(nm == 0, day_cm, night_cm)
+    mask = xr.where(nm == 0, day, night)
     return mask
+
+
+def ndvi(NIR, R):
+    """
+        Get NDVI index from reflectance bands
+        Most common use is (I2, I1) or (M7, M5) as (NIR, R)
+    Args:
+        NIR(np.ndarray|xr.DataArray): near-infrared reflectance band
+        R(np.ndarray|xr.DataArray): red reflectance band
+    Returns:
+        (np.ndarray|xr.DataArray): NDVI index for each pixel,
+            can contain NaN values
+    """
+    i = (NIR - R) / (NIR + R)
+    mask = nan_mask(NIR)
+    return xr.where(mask, nan, i)
```

### Comparing `viirs-tools-0.1.1/viirs_tools.egg-info/PKG-INFO` & `viirs-tools-1.0.0/viirs_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viirs-tools
-Version: 0.1.1
+Version: 1.0.0
 Summary: Python library for processing VIIRS data
 Home-page: https://github.com/Veon2479/viirs-tools
 Author: Andrey Shuliak
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -245,32 +245,49 @@
 
 ## Usage
 
 The `viirs-tools` library provides the following core modules and their main functions:
 
 1. **CloudMask**:
    + `rsnpp_day_img`: Day reflectance/thermal I-bands cloud test. [^1]
-   + `thermal_img`: Night thermal I-bands cloud test. [^2]
-   + `day_night_img`: Day/night cloud mask based on the previous 2
-
+   + `fire_day_img`, `fire_night_img`: Day and night I-bands cloud tests used in the [^2].
 
 2. **NightMask**:
    + `naive`: Day/night mask, based on the difference between presence of reflectance and thermal data, for both I- and M-bands
 
-3. **Utils**:
+3. **Water**:
+   + `water_bodies_day`: Day reflectance tests for water bodies from [^2]
+
+4. **LST**:
+   + `mono_window_i05`, `mono_window_m16`, `mono_window_m15`: LST retrieval for I05 band, based on the LANDSAT-8 alg [^3]
+
+5. **Fires**:
+   + `active_fires`: Active fire detection from [^2]
+
+6. **Utils**:
    - Just some helpful functions
 
-4. **Assimilator** submodule:
+7. **Assimilator** submodule:
 	1. **Assimilator**:
 		- `assimilate`: Retrieving data from NASA archives using [cmrfetch](https://github.com/bmflynn/cmrfetch), with support for handy data collection process management
 	2. **Reading**
 		- `read_npp_viaes_l1`: Reading [VIIRS/NPP Imagery Resolution 6-Min L1 Swath SDR 375m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/NPP_VIAES_L1#product-information) product files
 		- `read_npp_vmaes_l1`: Reading [VIIRS/NPP Moderate Resolution 6-Min L1 Swath SDR and GEO 750m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/NPP_VMAES_L1) product files
 		- `read_npp_cldmsk_l2`: Reading [VIIRS/SNPP Cloud Mask 6-Min Swath 750m](https://ladsweb.modaps.eosdis.nasa.gov/missions-and-measurements/products/CLDMSK_L2_VIIRS_SNPP#product-information) product files
 	3. **ReadingHelpers**
 		- Contains some helper functions for reading files that aren't supported by `SatPy` module (some examples of using them in the previous module)
 
 
+## Demo
+You can find demo Qt6 app in the `viirs-demo` folder. Note that it requires additional packages to be installed installed - `rasterio`,  `matplotlib`,  `PyQt6` and `TensorFlow`. Run `viirs-demo.py` to start it. Data for this demo can be found in the `demo-data` folder.
+
+
+## Additional tools
+In the `scripts` folder you can find useful tools for local satellite data analysis, such `assimilate.py` script. It was used for gathering data in the `demo-data` folder.
+
+
 ## References
 [^1]: M.Piper, T.Bahr (2015). A RAPID CLOUD MASK ALGORITHM FOR SUOMI NPP VIIRS IMAGERY EDRS.
 
 [^2]: W.Schroeder, P.Oliva, L.Giglio, I.A.Csiszar (2014). The New VIIRS 375 m active fire detection data product: Algorithm description and initial assessment.
+
+[^3]: U.Avdan, G.Jovanovska (2016). Algorithm for Automated Mapping of Land Surface Temperature Using LANDSAT 8 Satellite Data
```

