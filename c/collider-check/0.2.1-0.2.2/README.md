# Comparing `tmp/collider_check-0.2.1.tar.gz` & `tmp/collider_check-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collider_check-0.2.1.tar", last modified: Fri May 24 07:46:56 2024, max compression
+gzip compressed data, was "collider_check-0.2.2.tar", last modified: Fri May 24 10:23:09 2024, max compression
```

## Comparing `collider_check-0.2.1.tar` & `collider_check-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1072 2024-04-23 15:24:05.000000 collider_check-0.2.1/LICENSE
--rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-05-24 07:46:56.247410 collider_check-0.2.1/PKG-INFO
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      798 2024-04-23 15:24:05.000000 collider_check-0.2.1/README.md
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      913 2024-05-24 07:43:45.000000 collider_check-0.2.1/pyproject.toml
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       38 2024-05-24 07:46:56.247410 collider_check-0.2.1/setup.cfg
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/src/
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/src/collider_check/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1027 2024-05-24 07:44:25.000000 collider_check-0.2.1/src/collider_check/__init__.py
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)    27427 2024-05-24 07:43:16.000000 collider_check-0.2.1/src/collider_check/collider_check.py
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/src/collider_check.egg-info/
--rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/PKG-INFO
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      329 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/SOURCES.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)        1 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/dependency_links.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       64 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/requires.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       15 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/top_level.txt
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/tests/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     6763 2024-04-23 15:24:05.000000 collider_check-0.2.1/tests/test_check.py
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 10:23:09.403074 collider_check-0.2.2/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1072 2024-04-23 15:24:05.000000 collider_check-0.2.2/LICENSE
+-rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-05-24 10:23:09.403074 collider_check-0.2.2/PKG-INFO
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      798 2024-04-23 15:24:05.000000 collider_check-0.2.2/README.md
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      913 2024-05-24 10:23:01.000000 collider_check-0.2.2/pyproject.toml
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       38 2024-05-24 10:23:09.403074 collider_check-0.2.2/setup.cfg
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 10:23:09.403074 collider_check-0.2.2/src/
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 10:23:09.403074 collider_check-0.2.2/src/collider_check/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1027 2024-05-24 10:22:56.000000 collider_check-0.2.2/src/collider_check/__init__.py
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)    27744 2024-05-24 10:22:29.000000 collider_check-0.2.2/src/collider_check/collider_check.py
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 10:23:09.403074 collider_check-0.2.2/src/collider_check.egg-info/
+-rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-05-24 10:23:09.000000 collider_check-0.2.2/src/collider_check.egg-info/PKG-INFO
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      329 2024-05-24 10:23:09.000000 collider_check-0.2.2/src/collider_check.egg-info/SOURCES.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)        1 2024-05-24 10:23:09.000000 collider_check-0.2.2/src/collider_check.egg-info/dependency_links.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       64 2024-05-24 10:23:09.000000 collider_check-0.2.2/src/collider_check.egg-info/requires.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       15 2024-05-24 10:23:09.000000 collider_check-0.2.2/src/collider_check.egg-info/top_level.txt
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 10:23:09.403074 collider_check-0.2.2/tests/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     6763 2024-04-23 15:24:05.000000 collider_check-0.2.2/tests/test_check.py
```

### Comparing `collider_check-0.2.1/LICENSE` & `collider_check-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `collider_check-0.2.1/PKG-INFO` & `collider_check-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collider-check
-Version: 0.2.1
+Version: 0.2.2
 Summary: A small package that provides functions to check the observables in a collider, using a collider built with Xsuite.
 Author-email: Colas Droin <colas.noe.droin@cern.ch>
 License: MIT License
         
         Copyright (c) [2023] [Colas Droin]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `collider_check-0.2.1/README.md` & `collider_check-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `collider_check-0.2.1/pyproject.toml` & `collider_check-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = false
 
 [project]
 name = "collider-check"
-version = "0.2.1"
+version = "0.2.2"
 description = "A small package that provides functions to check the observables in a collider, using a collider built with Xsuite."
 readme = "README.md"
 authors = [{ name = "Colas Droin", email = "colas.noe.droin@cern.ch" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `collider_check-0.2.1/src/collider_check/__init__.py` & `collider_check-0.2.2/src/collider_check/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Package version
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 import xtrack as xt
 
 # Import ColliderCheck class in the namespace
 from .collider_check import ColliderCheck
```

### Comparing `collider_check-0.2.1/src/collider_check/collider_check.py` & `collider_check-0.2.2/src/collider_check/collider_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         configuration file."""
 
         # Store the collider
         self.collider = collider
 
         # Store the filling scheme path
         self.path_filling_scheme = path_filling_scheme
-        
+
         # Check the type of particles and store
         if type_particles in ["proton", "lead"]:
             self.type_particles = type_particles
         else:
-            raise ValueError("type_particles must be either 'proton' or 'lead'.") 
-        
+            raise ValueError("type_particles must be either 'proton' or 'lead'.")
+
         # Record cross-section correspondinlgy
         if self.type_particles == "proton":
             self.cross_section = 81e-27
         elif self.type_particles == "lead":
             self.cross_section = 281e-24
 
         # Define the configuration through a property since it might not be there
@@ -99,19 +99,21 @@
 
     @property
     def nemitt_y(self):
         if self.configuration is not None:
             return self.configuration["config_collider"]["config_beambeam"]["nemitt_y"]
         print("Warning: no configuration provided. Using default value of 2.2e-6 for nemitt_y.")
         return 2.2e-6
-    
+
     @property
     def n_lr_per_side(self):
         if self.configuration is not None:
-            return self.configuration["config_collider"]["config_beambeam"]["num_long_range_encounters_per_side"]['ip1']
+            return self.configuration["config_collider"]["config_beambeam"][
+                "num_long_range_encounters_per_side"
+            ]["ip1"]
         print("Warning: no configuration provided. Using default value of 1 for n_lr_per_side.")
         return 16
 
     def _check_configuration(self):
         if self.configuration is None:
             raise ValueError(
                 "No configuration has been provided when instantiating the ColliderCheck object."
@@ -120,15 +122,14 @@
     def _load_configuration_luminosity(self):
         self.num_particles_per_bunch = float(
             self.configuration["config_collider"]["config_beambeam"]["num_particles_per_bunch"]
         )
         self.sigma_z = self.configuration["config_collider"]["config_beambeam"]["sigma_z"]
 
     def _load_filling_scheme_arrays(self):
-
         if self.path_filling_scheme is None:
             # Get the filling scheme path (should already be an absolute path)
             self.path_filling_scheme = self.configuration["config_collider"]["config_beambeam"][
                 "mask_with_filling_pattern"
             ]["pattern_fname"]
 
             # Check if filling scheme file exists, and replace it by local if not
@@ -137,24 +138,22 @@
                     package_path = str(files("collider_dashboard"))
                 except NameError as e:
                     raise ValueError(
                         "collider_dashboard not installed... Filling scheme file could not be"
                         " loaded from the path in the configuration or locally."
                     ) from e
                 if os.path.isfile(
-                    f"{package_path}/data/"
-                    + self.path_filling_scheme.split("/")[-1]
+                    f"{package_path}/data/" + self.path_filling_scheme.split("/")[-1]
                 ):
                     print(
                         "Filling scheme file could not be loaded from the path in the"
                         " configuration. Loading it locally."
                     )
                     self.path_filling_scheme = (
-                        f"{package_path}/data/"
-                        + self.path_filling_scheme.split("/")[-1]
+                        f"{package_path}/data/" + self.path_filling_scheme.split("/")[-1]
                     )
                 else:
                     raise ValueError(
                         "Filling scheme file could not be loaded from the path in the configuration"
                         " or locally."
                     )
 
@@ -302,14 +301,19 @@
             beam_weak: survey_weak[ip][["X", "Y", "Z"], my_filter_string],
         }
         twiss_filtered = {
             beam_strong: twiss_strong[:, my_filter_string],
             beam_weak: twiss_weak[:, my_filter_string],
         }
         s = survey_filtered[beam_strong]["Z"]
+        # Compute if the beambeam element is on or off (list of 1 and 0)
+        l_scale_strength = [
+            self.collider["lhcb1"].element_refs[name_el].scale_strength._value
+            for name_el in twiss_filtered[beam_strong].name
+        ]
         d_x_weak_strong_in_meter = (
             twiss_filtered[beam_weak]["x"]
             - twiss_filtered[beam_strong]["x"]
             + survey_filtered[beam_weak]["X"]
             - survey_filtered[beam_strong]["X"]
         )
         d_y_weak_strong_in_meter = (
@@ -323,28 +327,29 @@
             s,
             my_filter_string,
             beam_strong,
             twiss_filtered,
             survey_filtered,
             d_x_weak_strong_in_meter,
             d_y_weak_strong_in_meter,
+            l_scale_strength,
         )
 
     def _compute_emittances_separation(self):
         if self.type_particles == "proton":
             # gamma relativistic of a proton
             gamma_rel = self.energy / (
                 constants.physical_constants["proton mass energy equivalent in MeV"][0] / 1000
             )
         elif self.type_particles == "lead":
             # gamma relativistic of a lead ion (value needs to be double-checked)
             gamma_rel = self.energy / (193084.751 / 1000)
         else:
             raise ValueError("type_particles must be either 'proton' or 'lead'.")
-        
+
         # beta relativistic of a proton at 7 TeV
         beta_rel = np.sqrt(1 - 1 / gamma_rel**2)
 
         emittance_strong_x = self.nemitt_x / gamma_rel / beta_rel
         emittance_strong_y = self.nemitt_y / gamma_rel / beta_rel
 
         emittance_weak_x = self.nemitt_x / gamma_rel / beta_rel
@@ -414,14 +419,15 @@
             s,
             my_filter_string,
             beam_strong,
             twiss_filtered,
             survey_filtered,
             d_x_weak_strong_in_meter,
             d_y_weak_strong_in_meter,
+            l_scale_strength,
         ) = self._compute_ip_specific_separation(ip=ip, beam_weak=beam_weak)
 
         # Get emittances
         (
             gamma_rel,
             beta_rel,
             emittance_weak_x,
@@ -471,14 +477,15 @@
             "gamma_rel": gamma_rel,
             "beta_rel": beta_rel,
             "energy": self.energy,
             "my_filter_string": my_filter_string,
             "beam_weak": beam_weak,
             "beam_strong": beam_strong,
             "ip": ip,
+            "l_scale_strength": l_scale_strength,
         }
 
     def return_dic_position_all_ips(self):
         """This function computes all the variables needed to compute the position of the beam in
         all IRs. The variables are stored and returne in a dictionnary. The extreme positions are:
         IP1 : mqy.4l1.b1 to mqy.4r1.b1
         IP2 : mqy.b5l2.b1 to mqy.b4r2.b1
```

### Comparing `collider_check-0.2.1/src/collider_check.egg-info/PKG-INFO` & `collider_check-0.2.2/src/collider_check.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collider-check
-Version: 0.2.1
+Version: 0.2.2
 Summary: A small package that provides functions to check the observables in a collider, using a collider built with Xsuite.
 Author-email: Colas Droin <colas.noe.droin@cern.ch>
 License: MIT License
         
         Copyright (c) [2023] [Colas Droin]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `collider_check-0.2.1/tests/test_check.py` & `collider_check-0.2.2/tests/test_check.py`

 * *Files identical despite different names*

