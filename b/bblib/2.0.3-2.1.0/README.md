# Comparing `tmp/bblib-2.0.3.tar.gz` & `tmp/bblib-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-2.0.3.tar", max compression
+gzip compressed data, was "bblib-2.1.0.tar", max compression
```

## Comparing `bblib-2.0.3.tar` & `bblib-2.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-05-22 11:06:26.981155 bblib-2.0.3/LICENSE
--rw-r--r--   0        0        0     3917 2024-05-22 11:06:26.981155 bblib-2.0.3/README.md
--rw-r--r--   0        0        0        0 2024-05-22 11:06:26.981155 bblib-2.0.3/bblib/__init__.py
--rwxr-xr-x   0        0        0    37195 2024-05-22 11:06:26.981155 bblib-2.0.3/bblib/methods.py
--rwxr-xr-x   0        0        0     9961 2024-05-22 11:06:26.981155 bblib-2.0.3/bblib/models.py
--rwxr-xr-x   0        0        0    18198 2024-05-22 11:06:26.981155 bblib-2.0.3/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-05-22 11:06:39.665029 bblib-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 bblib-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-05-24 11:38:56.802416 bblib-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3914 2024-05-24 11:38:56.802416 bblib-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 11:38:56.802416 bblib-2.1.0/bblib/__init__.py
+-rwxr-xr-x   0        0        0    38761 2024-05-24 11:38:56.802416 bblib-2.1.0/bblib/methods.py
+-rwxr-xr-x   0        0        0    10130 2024-05-24 11:38:56.802416 bblib-2.1.0/bblib/models.py
+-rwxr-xr-x   0        0        0    18200 2024-05-24 11:38:56.802416 bblib-2.1.0/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-05-24 11:39:07.974398 bblib-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7445 1970-01-01 00:00:00.000000 bblib-2.1.0/PKG-INFO
```

### Comparing `bblib-2.0.3/LICENSE` & `bblib-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-2.0.3/README.md` & `bblib-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 beambusters library. Python library to refine the detector center of diffraction patterns.
 
 For more information, see: https://github.com/anananacr/beambusters
 
 ## Python version
 
-Python 3.10.5 
+Python 3.10
 
 ## Installation
 pip install bblib
 
 ## Usage
 
 To utilize the methods `CenterOfMass`,  `FriedelPairs`, `MinimizePeakFWHM`  and `CircleDetection` it is required to have two configuration dictionaries, one for PeakFinder8 and another one for this library itself. The following snippet shows the general structure for both (parameters not used in your case can be omitted):
```

### Comparing `bblib-2.0.3/bblib/methods.py` & `bblib-2.1.0/bblib/methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from skimage.transform import hough_circle, hough_circle_peaks
 from skimage.feature import canny
 import multiprocessing
 import pathlib
 from scipy.optimize import curve_fit
 from matplotlib.colors import LogNorm
 
+
 class CenteringMethod(ABC):
     @abstractmethod
     def __init__(self, **kwargs) -> None: ...
 
     @abstractmethod
     def _prep_for_centering(self, **kwargs) -> None: ...
 
@@ -51,19 +52,15 @@
         self.plots_info = plots_info
         if config["plots_flag"] and not plots_info:
             raise ValueError(
                 "From config you want to save plots, please indicate the information to save the plots."
             )
 
         if not config["plots_flag"] and not plots_info:
-            plots_info =  {
-	        "file_name": "",
-	        "folder_name": "",
-	        "root_path": ""
-            }
+            plots_info = {"file_name": "", "folder_name": "", "root_path": ""}
 
     def _prep_for_centering(self, data: np.ndarray) -> None:
         self.initial_detector_center = self.PF8Config.get_detector_center()
         pf8 = PF8(self.PF8Config)
         peak_list = pf8.get_peaks_pf8(data=data)
         peak_list_x_in_frame, peak_list_y_in_frame = pf8.peak_list_in_slab(peak_list)
         row_indexes = np.zeros(peak_list["num_peaks"], dtype=int)
@@ -113,26 +110,30 @@
     def _run_centering(self, **kwargs) -> tuple:
         center = center_of_mass(self.visual_data, self.mask_for_center_of_mass)
         if self.centering_converged(center):
             center[0] += self.config["offset"]["x"]
             center[1] += self.config["offset"]["y"]
 
         if self.config["plots_flag"]:
+            visual_img = self.visual_data * self.mask_for_center_of_mass
+            visual_img[np.where(visual_img<1)] = 1 # For better visualization of plots in logarithmic scale
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             if self.plots_info["value_auto"]:
-                ax1.imshow(
-                    self.visual_data * self.mask_for_center_of_mass,
+                pos = ax1.imshow(
+                    visual_img,
                     norm=LogNorm(),
                     cmap=self.plots_info["color_map"],
                     origin="lower",
                 )
-            else: 
-                ax1.imshow(
-                    self.visual_data * self.mask_for_center_of_mass,
-                    norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]),
+            else:
+                pos = ax1.imshow(
+                    visual_img,
+                    norm=LogNorm(
+                        self.plots_info["value_min"], self.plots_info["value_max"]
+                    ),
                     cmap=self.plots_info["color_map"],
                     origin="lower",
                 )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
@@ -142,23 +143,23 @@
             ax1.scatter(
                 center[0],
                 center[1],
                 color="r",
                 marker="o",
                 label=f"Refined detector center: ({center[0]}, {center[1]})",
             )
+            ax1.legend()
+            fig.colorbar(pos, ax=ax1, shrink=0.6)
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_of_mass/'
             )
             path.mkdir(parents=True, exist_ok=True)
-            ax1.legend()
             if not self.plots_info["axis_lim_auto"]:
                 ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
                 ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
-
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_of_mass/{self.plots_info["file_name"]}.png'
             )
             plt.close()
         return np.round(center, 0)
 
 
@@ -169,19 +170,15 @@
         self.plots_info = plots_info
         if config["plots_flag"] and not plots_info:
             raise ValueError(
                 "From config you want to save plots, please indicate the information to save the plots."
             )
 
         if not config["plots_flag"] and not plots_info:
-            plots_info =  {
-	        "file_name": "",
-	        "folder_name": "",
-	        "root_path": ""
-            }
+            plots_info = {"file_name": "", "folder_name": "", "root_path": ""}
 
     def _prep_for_centering(self, data: np.ndarray) -> None:
         self.initial_detector_center = self.PF8Config.get_detector_center()
         ## Find peaks
         pf8 = PF8(self.PF8Config)
         peak_list = pf8.get_peaks_pf8(data=data)
         peak_list_x_in_frame, peak_list_y_in_frame = pf8.peak_list_in_slab(peak_list)
@@ -236,15 +233,16 @@
             use_quantiles=True,
             low_threshold=self.config["canny"]["low_threshold"],
             high_threshold=self.config["canny"]["high_threshold"],
         )
 
         if self.config["plots_flag"]:
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
-            ax1.imshow(edges, origin="lower")
+            pos = ax1.imshow(edges, origin="lower", cmap=self.plots_info["color_map"])
+            fig.colorbar(pos, ax=ax1, shrink=0.6)
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/edges/'
             )
             path.mkdir(parents=True, exist_ok=True)
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/edges/{self.plots_info["file_name"]}.png'
             )
@@ -256,34 +254,38 @@
         hough_res = hough_circle(edges, hough_radii)
         # Select the most prominent 1 circle
         accums, xc, yc, radii = hough_circle_peaks(
             hough_res, hough_radii, total_num_peaks=1
         )
 
         if len(xc) > 0:
-            xc = xc[0]
-            yc = yc[0]
+            xc = xc[0] + self.config["offset"]["x"]
+            yc = yc[0] + self.config["offset"]["y"]
         else:
             xc = -1
             yc = -1
 
         center = [xc, yc]
         if self.config["plots_flag"]:
+            visual_img = self.visual_data * self.mask_for_circle_detection
+            visual_img[np.where(visual_img<1)] = 1 # For better visualization of plots in logarithmic scale
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             if self.plots_info["value_auto"]:
-                ax1.imshow(
-                    self.visual_data * self.mask_for_circle_detection,
+                pos = ax1.imshow(
+                    visual_img,
                     norm=LogNorm(),
                     origin="lower",
                     cmap=self.plots_info["color_map"],
                 )
             else:
-                ax1.imshow(
-                    self.visual_data * self.mask_for_circle_detection,
-                    norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]),
+                pos = ax1.imshow(
+                    visual_img,
+                    norm=LogNorm(
+                        self.plots_info["value_min"], self.plots_info["value_max"]
+                    ),
                     origin="lower",
                     cmap=self.plots_info["color_map"],
                 )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
@@ -298,14 +300,15 @@
                 label=f"Refined detector center: ({center[0]}, {center[1]})",
             )
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_circle_detection/'
             )
             path.mkdir(parents=True, exist_ok=True)
             ax1.legend()
+            fig.colorbar(pos, ax=ax1, shrink=0.6)
             if not self.plots_info["axis_lim_auto"]:
                 ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
                 ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_circle_detection/{self.plots_info["file_name"]}.png'
             )
             plt.close()
@@ -320,20 +323,15 @@
         self.plot_fwhm_flag = False
         if config["plots_flag"] and not plots_info:
             raise ValueError(
                 "From config you want to save plots, please indicate the information to save the plots."
             )
 
         if not config["plots_flag"] and not plots_info:
-            plots_info =  {
-	        "file_name": "",
-	        "folder_name": "",
-	        "root_path": ""
-            }
-
+            plots_info = {"file_name": "", "folder_name": "", "root_path": ""}
 
     def _calculate_fwhm(self, coordinate: tuple) -> dict:
         center_to_radial_average = coordinate
         try:
             x_all, y_all = azimuthal_average(
                 self.visual_data,
                 center=center_to_radial_average,
@@ -394,16 +392,16 @@
                 x_fit,
                 y_fit,
                 "r--",
                 label=f"gaussian fit \n a:{round(popt[0],2)} \n x0:{round(popt[1],2)} \n sigma:{round(popt[2],2)} \n R² {round(r_squared, 4)}\n FWHM : {round(fwhm,3)}",
             )
 
             plt.title("Azimuthal integration")
-            #plt.xlim(0, 500)
-            #plt.ylim(0, 5)
+            # plt.xlim(0, 500)
+            # plt.ylim(0, 5)
             plt.legend()
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/radial_average/'
             )
             path.mkdir(parents=True, exist_ok=True)
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/radial_average/{self.plots_info["file_name"]}.png'
@@ -424,16 +422,18 @@
         ## Find peaks
         self.PF8Config.update_pixel_maps(
             initial_guess[0] - self.initial_detector_center[0],
             initial_guess[1] - self.initial_detector_center[1],
         )
         pf8 = PF8(self.PF8Config)
         # Assemble data and mask
-        data_visualize = geometry.DataVisualizer(pixel_maps=non_shifted_pixel_maps_for_visualization)
-        
+        data_visualize = geometry.DataVisualizer(
+            pixel_maps=non_shifted_pixel_maps_for_visualization
+        )
+
         with h5py.File(f"{self.PF8Config.bad_pixel_map_filename}", "r") as f:
             mask = np.array(f[f"{self.PF8Config.bad_pixel_map_hdf5_path}"])
 
         if self.config["polarization"]["skip"]:
             peak_list = pf8.get_peaks_pf8(data=data)
             if (
                 self.PF8Config.pf8_detector_info["nasics_x"]
@@ -534,40 +534,48 @@
     def _run_centering(self, **kwargs) -> tuple:
         if self.config["plots_flag"]:
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/fwhm_map/'
             )
             path.mkdir(parents=True, exist_ok=True)
 
-        center = get_fwhm_map_global_min(
+        xc, yc = get_fwhm_map_global_min(
             self.fwhm_summary,
             f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}',
             f'{self.plots_info["file_name"]}',
             self.pixel_step,
             self.config["plots_flag"],
         )
 
+        xc += self.config["offset"]["x"]
+        yc += self.config["offset"]["y"]
+        center = [xc, yc]
+
         if self.centering_converged(center):
             self.plot_fwhm_flag = True
             self._calculate_fwhm(center)
             self.plot_fwhm_flag = False
 
         if self.config["plots_flag"]:
+            visual_img = self.visual_data * self.mask_for_fwhm_min
+            visual_img[np.where(visual_img<1)] = 1 # For better visualization of plots in logarithmic scale
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             if self.plots_info["value_auto"]:
-                ax1.imshow(
-                    self.visual_data * self.mask_for_fwhm_min,
+                pos = ax1.imshow(
+                    visual_img,
                     norm=LogNorm(),
                     origin="lower",
                     cmap=self.plots_info["color_map"],
                 )
             else:
-                ax1.imshow(
-                    self.visual_data * self.mask_for_fwhm_min,
-                    norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]),
+                pos = ax1.imshow(
+                    visual_img,
+                    norm=LogNorm(
+                        self.plots_info["value_min"], self.plots_info["value_max"]
+                    ),
                     origin="lower",
                     cmap=self.plots_info["color_map"],
                 )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
@@ -589,14 +597,15 @@
                 label=f"Refined detector center: ({center[0]}, {center[1]})",
             )
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_fwhm_minimization/'
             )
             path.mkdir(parents=True, exist_ok=True)
             ax1.legend()
+            fig.colorbar(pos, ax=ax1, shrink=0.6)
             if not self.plots_info["axis_lim_auto"]:
                 ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
                 ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_fwhm_minimization/{self.plots_info["file_name"]}.png'
             )
             plt.close()
@@ -609,29 +618,27 @@
         self.config = config
         self.PF8Config = PF8Config
         self.plots_info = plots_info
         if config["plots_flag"] and not plots_info:
             raise ValueError(
                 "From config you want to save plots, please indicate the information to save the plots."
             )
-        
+
         if not config["plots_flag"] and not plots_info:
-            plots_info =  {
-	        "file_name": "",
-	        "folder_name": "",
-	        "root_path": ""
-            }
+            plots_info = {"file_name": "", "folder_name": "", "root_path": ""}
 
     def _select_closest_peaks(self, peaks_list: list, inverted_peaks: list) -> list:
         pairs_list = []
         for i in peaks_list:
             radius = 0.1
             found_peak = False
             while not found_peak and radius <= self.config["search_radius"]:
-                found_peak = self._find_a_peak_in_the_surrounding(i, inverted_peaks, radius)
+                found_peak = self._find_a_peak_in_the_surrounding(
+                    i, inverted_peaks, radius
+                )
                 radius += 0.1
             if found_peak:
                 pairs_list.append((i, found_peak))
         pairs_list = self._check_paired_reflections(pairs_list)
         return pairs_list
 
     def _find_a_peak_in_the_surrounding(
@@ -655,22 +662,28 @@
         cut_peaks_list.sort(key=lambda x: x[1])
 
         if cut_peaks_list == []:
             return False
         else:
             return cut_peaks_list[0][0]
 
-    def _check_paired_reflections(self, pairs_list:list)-> list:
+    def _check_paired_reflections(self, pairs_list: list) -> list:
         ## check if the reversed peak is also on the list
         filtered_pairs = []
-        
+
         for original_peak, inverted_peak in pairs_list:
-            inverted_peak_inverted_twice = (-1*inverted_peak[0],-1*inverted_peak[1])
-            original_peak_inverted_twice = (-1*original_peak[0],-1*original_peak[1])
-            inverted_pair=(inverted_peak_inverted_twice,original_peak_inverted_twice)
+            inverted_peak_inverted_twice = (
+                -1 * inverted_peak[0],
+                -1 * inverted_peak[1],
+            )
+            original_peak_inverted_twice = (
+                -1 * original_peak[0],
+                -1 * original_peak[1],
+            )
+            inverted_pair = (inverted_peak_inverted_twice, original_peak_inverted_twice)
             if inverted_pair in pairs_list:
                 filtered_pairs.append((original_peak, inverted_peak))
 
         return filtered_pairs
 
     def _prep_for_centering(self, data: np.ndarray, initial_guess: tuple) -> None:
 
@@ -683,15 +696,17 @@
             initial_guess[0] - self.initial_detector_center[0],
             initial_guess[1] - self.initial_detector_center[1],
         )
 
         pf8 = PF8(self.PF8Config)
 
         # Assemble data and mask
-        data_visualize = geometry.DataVisualizer(pixel_maps=non_shifted_pixel_maps_for_visualization)
+        data_visualize = geometry.DataVisualizer(
+            pixel_maps=non_shifted_pixel_maps_for_visualization
+        )
 
         with h5py.File(f"{self.PF8Config.bad_pixel_map_filename}", "r") as f:
             mask = np.array(f[f"{self.PF8Config.bad_pixel_map_hdf5_path}"])
 
         if self.config["polarization"]["skip"]:
             peak_list = pf8.get_peaks_pf8(data=data)
             if (
@@ -747,66 +762,89 @@
                     self.PF8Config.ss_in_rows,
                 )
 
         peak_list_in_slab = pf8.peak_list_in_slab(peak_list)
         self.peak_list_x_in_frame, self.peak_list_y_in_frame = peak_list_in_slab
 
     def _run_centering(self, **kwargs) -> tuple:
-       
+
         peak_list_x_in_frame = self.peak_list_x_in_frame.copy()
         peak_list_y_in_frame = self.peak_list_y_in_frame.copy()
 
         peaks = list(zip(peak_list_x_in_frame, peak_list_y_in_frame))
         inverted_peaks_x = [-1 * k for k in peak_list_x_in_frame]
         inverted_peaks_y = [-1 * k for k in peak_list_y_in_frame]
         inverted_peaks = list(zip(inverted_peaks_x, inverted_peaks_y))
         pairs_list = self._select_closest_peaks(peaks, inverted_peaks)
 
         ## Calculcate the beam center shift
-        
+
         self.peaks_list_original = [x for x, y in pairs_list]
         self.peaks_list_inverted = [y for x, y in pairs_list]
 
-        if len(pairs_list)>0:
-            print(f"--------------  Friedel pairs search --------------\nNumber of Friedel Pairs in frame: {len(pairs_list)/2}")
+        if len(pairs_list) > 0:
+            print(
+                f"--------------  Friedel pairs search --------------\nNumber of Friedel Pairs in frame: {len(pairs_list)/2}"
+            )
             print(f"Pairs list for analysis:")
             print(pairs_list)
 
             friedel_coordinates_in_x = [x for x, y in self.peaks_list_original]
             friedel_coordinates_in_y = [y for x, y in self.peaks_list_original]
-            
+
             print(f"Friedel pairs position before center correction in pixels:")
             print(self.peaks_list_original)
-            
-            shift_x = sum(friedel_coordinates_in_x)/len(friedel_coordinates_in_x)
-            shift_y = sum(friedel_coordinates_in_y)/len(friedel_coordinates_in_y)
+
+            shift_x = self.config["offset"]["x"] + (
+                sum(friedel_coordinates_in_x) / len(friedel_coordinates_in_x)
+            )
+            shift_y = self.config["offset"]["y"] + (
+                sum(friedel_coordinates_in_y) / len(friedel_coordinates_in_y)
+            )
             print("Center shift in x", shift_x)
             print("Center shift in y", shift_y)
-            center = [self.initial_guess[0]+shift_x, self.initial_guess[1]+shift_y]
+            center = [
+                np.round(self.initial_guess[0] + shift_x, 1),
+                np.round(self.initial_guess[1] + shift_y, 1),
+            ]
 
             print(f"Friedel pairs position after center correction in pixels:")
-            pairs_list_after_correction=[(x[0]-shift_x, x[1]-shift_y) for x in self.peaks_list_original]
+            pairs_list_after_correction = [
+                (np.round(x[0] - shift_x, 1), np.round(x[1] - shift_y, 1))
+                for x in self.peaks_list_original
+            ]
             print(pairs_list_after_correction)
             print(f"All reflections after center correction in pixels:")
-            peaks_list_after_correction=[(x[0]-shift_x, x[1]-shift_y) for x in peaks]
+            peaks_list_after_correction = [
+                (np.round(x[0] - shift_x, 1), np.round(x[1] - shift_y, 1))
+                for x in peaks
+            ]
             print(peaks_list_after_correction)
 
         else:
             center = [-1, -1]
 
         if self.config["plots_flag"] and self.centering_converged(center):
 
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             if self.plots_info["value_auto"]:
                 pos = ax1.imshow(
-                    self.visual_data, norm=LogNorm(), cmap=self.plots_info["color_map"], origin="lower"
+                    self.visual_data,
+                    norm=LogNorm(),
+                    cmap=self.plots_info["color_map"],
+                    origin="lower",
                 )
             else:
                 pos = ax1.imshow(
-                    self.visual_data, norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]), cmap=self.plots_info["color_map"], origin="lower"
+                    self.visual_data,
+                    norm=LogNorm(
+                        self.plots_info["value_min"], self.plots_info["value_max"]
+                    ),
+                    cmap=self.plots_info["color_map"],
+                    origin="lower",
                 )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="b",
                 marker="o",
                 s=25,
@@ -825,73 +863,83 @@
                 center[0],
                 center[1],
                 color="r",
                 marker="o",
                 s=25,
                 label=f"Refined detector center:({np.round(center[0],1)}, {np.round(center[1],1)})",
             )
-            
+
             plt.title("Center refinement: autocorrelation of Friedel pairs")
-            fig.colorbar(pos, shrink=0.6)
+            fig.colorbar(pos, ax=ax1, shrink=0.6)
             ax1.legend()
             if not self.plots_info["axis_lim_auto"]:
                 ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
                 ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
 
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/centered_friedel/'
             )
             path.mkdir(parents=True, exist_ok=True)
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/centered_friedel/{self.plots_info["file_name"]}.png'
             )
             plt.close("all")
-            
+
             original_peaks_x = [
                 np.round(k + self.initial_guess[0]) for k in peak_list_x_in_frame
             ]
             original_peaks_y = [
                 np.round(k + self.initial_guess[1]) for k in peak_list_y_in_frame
             ]
 
             inverted_non_shifted_peaks_x = [
                 np.round(k[0] + self.initial_guess[0]) for k in self.peaks_list_inverted
             ]
             inverted_non_shifted_peaks_y = [
                 np.round(k[1] + self.initial_guess[1]) for k in self.peaks_list_inverted
             ]
             inverted_shifted_peaks_x = [
-                np.round(k[0] + self.initial_guess[0] + shift_x) for k in self.peaks_list_inverted
+                np.round(k[0] + self.initial_guess[0] + shift_x)
+                for k in self.peaks_list_inverted
             ]
             inverted_shifted_peaks_y = [
-                np.round(k[1] + self.initial_guess[1] + shift_y) for k in self.peaks_list_inverted
+                np.round(k[1] + self.initial_guess[1] + shift_y)
+                for k in self.peaks_list_inverted
             ]
 
             ## Check pairs alignement
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
             if self.plots_info["value_auto"]:
                 pos = ax1.imshow(
-                    self.visual_data, norm=LogNorm(), cmap=self.plots_info["color_map"], origin="lower"
+                    self.visual_data,
+                    norm=LogNorm(),
+                    cmap=self.plots_info["color_map"],
+                    origin="lower",
                 )
             else:
                 pos = ax1.imshow(
-                    self.visual_data, norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]), cmap=self.plots_info["color_map"], origin="lower"
+                    self.visual_data,
+                    norm=LogNorm(
+                        self.plots_info["value_min"], self.plots_info["value_max"]
+                    ),
+                    cmap=self.plots_info["color_map"],
+                    origin="lower",
                 )
-                
+
             ax1.scatter(
                 original_peaks_x,
                 original_peaks_y,
                 facecolor="none",
                 s=80,
                 marker="s",
                 edgecolor="red",
                 linewidth=1.5,
                 label="original peaks",
             )
-            
+
             ax1.scatter(
                 inverted_non_shifted_peaks_x,
                 inverted_non_shifted_peaks_y,
                 s=80,
                 facecolor="none",
                 marker="s",
                 edgecolor="tab:orange",
@@ -906,21 +954,21 @@
                 s=120,
                 marker="D",
                 linewidth=1.8,
                 alpha=0.8,
                 edgecolor="blue",
                 label="shift of inverted peaks",
             )
-            
+
             if not self.plots_info["axis_lim_auto"]:
                 ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
                 ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
-            
+
             plt.title("Bragg peaks alignement")
-            fig.colorbar(pos, shrink=0.6)
+            fig.colorbar(pos, ax=ax1, shrink=0.6)
             ax1.legend()
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/peaks/'
             )
             path.mkdir(parents=True, exist_ok=True)
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/peaks/{self.plots_info["file_name"]}.png'
```

### Comparing `bblib-2.0.3/bblib/models.py` & `bblib-2.1.0/bblib/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class PF8Info:
     max_num_peaks: np.int32 = 200
     adc_threshold: np.int32 = 0
     minimum_snr: np.float32 = 5
     min_pixel_count: np.int16 = 2
     max_pixel_count: np.int16 = 2000
     local_bg_radius: np.int16 = 3
-    min_res: np.int16 = 0 
+    min_res: np.int16 = 0
     max_res: np.int16 = 1200
     pf8_detector_info: TypeDetectorLayoutInformation = None
     bad_pixel_map_filename: str = None
     bad_pixel_map_hdf5_path: str = None
     pixel_maps: TypePixelMaps = None
     pixel_resolution: float = None
     _shifted_pixel_maps: bool = False
@@ -38,51 +38,59 @@
             ).reshape(self._data_shape)
             self.pixel_maps["y"] = (
                 self.pixel_maps["y"].flatten() - detector_shift_y
             ).reshape(self._data_shape)
             self.pixel_maps["radius"] = np.sqrt(
                 np.square(self.pixel_maps["x"]) + np.square(self.pixel_maps["y"])
             ).reshape(self._data_shape)
-            self.pixel_maps["phi"] = np.arctan2(self.pixel_maps["y"], self.pixel_maps["x"])
+            self.pixel_maps["phi"] = np.arctan2(
+                self.pixel_maps["y"], self.pixel_maps["x"]
+            )
         else:
             raise ValueError(
                 f"Pixel maps have been moved once before, to avoid errors reset the geometry before moving it again."
             )
 
     def set_geometry_from_file(self, geometry_filename: str = None):
         if geometry_filename:
             self.geometry_txt = open(geometry_filename, "r").readlines()
         else:
             if not self.geometry_txt:
-                raise ValueError("Please, specify the detector geometry in CrystFEL format.")
-        
-        # Passing bad pixel maps to PF8. 
-        # Warning! It will look for campus in the geom file either 'mask0_file' or 'mask_file'. 
-        # It doesn't look for multiple masks. 
+                raise ValueError(
+                    "Please, specify the detector geometry in CrystFEL format."
+                )
+
+        # Passing bad pixel maps to PF8.
+        # Warning! It will look for campus in the geom file either 'mask0_file' or 'mask_file'.
+        # It doesn't look for multiple masks.
         # It assumes bad pixels as zeros and good pixels as ones.
         try:
             self.bad_pixel_map_filename = [
                 x.split(" = ")[-1][:-1]
                 for x in self.geometry_txt
                 if x.split(" = ")[0] == "mask0_file"
             ][0]
         except IndexError:
             self.bad_pixel_map_filename = [
-               x.split(" = ")[-1][:-1]
+                x.split(" = ")[-1][:-1]
                 for x in self.geometry_txt
                 if x.split(" = ")[0] == "mask_file"
             ][0]
 
         try:
             self.bad_pixel_map_hdf5_path = [
-                x.split(" = ")[-1][:-1] for x in self.geometry_txt if x.split(" = ")[0] == "mask0_data"
+                x.split(" = ")[-1][:-1]
+                for x in self.geometry_txt
+                if x.split(" = ")[0] == "mask0_data"
             ][0]
         except IndexError:
             self.bad_pixel_map_hdf5_path = [
-                x.split(" = ")[-1][:-1] for x in self.geometry_txt if x.split(" = ")[0] == "mask"
+                x.split(" = ")[-1][:-1]
+                for x in self.geometry_txt
+                if x.split(" = ")[0] == "mask"
             ][0]
 
         geom = GeometryInformation(
             geometry_description=self.geometry_txt, geometry_format="crystfel"
         )
         self.pixel_resolution = 1 / geom.get_pixel_size()
         self.pixel_maps = geom.get_pixel_maps()
@@ -93,15 +101,17 @@
         self.detector_center_from_geom = self.get_detector_center()
 
         if (
             self.pf8_detector_info["nasics_x"] * self.pf8_detector_info["nasics_y"]
         ) == 1:
             ## Get single panel transformation matrix from the geometry file
             ### Warning! Check carefully if the visualized data after reorientation of the panel makes sense, e.g. if it is equal to the real experimental data geometry.
-            detector, _, _ = _read_crystfel_geometry_from_text(text_lines=self.geometry_txt)
+            detector, _, _ = _read_crystfel_geometry_from_text(
+                text_lines=self.geometry_txt
+            )
             detector_panels = dict(detector["panels"])
             panel_name = list(detector_panels.keys())[0]
             frame_dim_structure = [
                 x
                 for x in detector_panels[panel_name]["dim_structure"]
                 if x == "ss" or x == "fs"
             ]
@@ -152,15 +162,15 @@
         elif parameter == "bad_pixel_map_filename":
             return self.bad_pixel_map_filename
         elif parameter == "bad_pixel_map_hdf5_path":
             return self.bad_pixel_map_hdf5_path
 
     def get_detector_center(self) -> list:
         if not self._shifted_pixel_maps:
-            
+
             if (
                 self.pf8_detector_info["nasics_x"] * self.pf8_detector_info["nasics_y"]
                 > 1
             ):
                 # Multiple panels
                 # Get minimum array shape
                 y_minimum = (
@@ -188,15 +198,17 @@
                 _img_center_x = int(visual_img_shape[1] / 2)
                 _img_center_y = int(visual_img_shape[0] / 2)
             else:
                 # Single panel
                 _img_center_x = int(abs(np.min(self.pixel_maps["x"])))
                 _img_center_y = int(abs(np.min(self.pixel_maps["y"])))
         else:
-            print("Warning! The detector center was moved by a previous operation, the detector center is not the same as in the geometry file.")
+            print(
+                "Warning! The detector center was moved by a previous operation, the detector center is not the same as in the geometry file."
+            )
             _img_center_x = self.detector_center_from_geom[0] + self._detector_shift_x
             _img_center_y = self.detector_center_from_geom[1] + self._detector_shift_y
         return [_img_center_x, _img_center_y]
 
 
 class PF8:
     def __init__(self, info):
```

### Comparing `bblib-2.0.3/bblib/utils.py` & `bblib-2.1.0/bblib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
          coordinates of the diffraction center in x and y, such as the image center corresponds to data[yc, xc].
     """
 
     if mask is None:
         mask = np.ones_like(data)
     data = data * mask
     indexes = np.where(data > 0)
-    if np.sum(data[indexes])>1e-7:
+    if np.sum(data[indexes]) > 1e-7:
         xc = np.sum(data[indexes] * indexes[1]) / np.sum(data[indexes])
         yc = np.sum(data[indexes] * indexes[0]) / np.sum(data[indexes])
     else:
         xc = -1
         yc = -1
 
     if np.isnan(xc) or np.isnan(yc):
@@ -409,17 +409,17 @@
     ax1.set_ylabel("yc [px]")
     ax1.set_xlabel("xc [px]")
     ax1.set_title("Distance [px]")
 
     proj_x = np.sum(z, axis=0)
     # print('proj',len(proj_x))
     x = np.arange(x[0], x[-1] + pixel_step, pixel_step)
-    
+
     # print('x',len(x))
-    if len(proj_x)==len(x):
+    if len(proj_x) == len(x):
         index_x = np.unravel_index(np.argmin(proj_x, axis=None), proj_x.shape)
         xc = x[index_x]
         ax2.scatter(x, proj_x + pixel_step, color="b")
         ax2.scatter(xc, proj_x[index_x], color="r", label=f"xc: {np.round(xc,1)}")
         ax2.set_ylabel("Average distance [px]")
         ax2.set_xlabel("xc [px]")
         ax2.set_title("Distance projection in x")
@@ -427,15 +427,15 @@
     else:
         converged = 0
         xc = -1
         yc = -1
 
     proj_y = np.sum(z, axis=1)
     x = np.arange(y[0], y[-1] + pixel_step, pixel_step)
-    if len(proj_y)==len(x):
+    if len(proj_y) == len(x):
         index_y = np.unravel_index(np.argmin(proj_y, axis=None), proj_y.shape)
         yc = x[index_y]
         ax3.scatter(x, proj_y, color="b")
         ax3.scatter(yc, proj_y[index_y], color="r", label=f"yc: {np.round(yc,1)}")
         ax3.set_ylabel("Average Distance [px]")
         ax3.set_xlabel("yc [px]")
         ax3.set_title("Distance projection in y")
```

### Comparing `bblib-2.0.3/pyproject.toml` & `bblib-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "2.0.3"
+version = "2.1.0"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-2.0.3/PKG-INFO` & `bblib-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 2.0.3
+Version: 2.1.0
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -101,15 +101,15 @@
 
 beambusters library. Python library to refine the detector center of diffraction patterns.
 
 For more information, see: https://github.com/anananacr/beambusters
 
 ## Python version
 
-Python 3.10.5 
+Python 3.10
 
 ## Installation
 pip install bblib
 
 ## Usage
 
 To utilize the methods `CenterOfMass`,  `FriedelPairs`, `MinimizePeakFWHM`  and `CircleDetection` it is required to have two configuration dictionaries, one for PeakFinder8 and another one for this library itself. The following snippet shows the general structure for both (parameters not used in your case can be omitted):
```

