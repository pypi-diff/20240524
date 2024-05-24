# Comparing `tmp/pumaz-1.6.1.tar.gz` & `tmp/pumaz-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pumaz-1.6.1.tar", last modified: Mon Apr 22 13:38:38 2024, max compression
+gzip compressed data, was "pumaz-1.6.3.tar", last modified: Fri May 24 18:29:06 2024, max compression
```

## Comparing `pumaz-1.6.1.tar` & `pumaz-1.6.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:38:38.497245 pumaz-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    13321 2024-04-22 13:38:38.497245 pumaz-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-04-22 13:38:32.000000 pumaz-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:38:38.497245 pumaz-1.6.1/pumaz/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16931 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    45401 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/pumaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-22 13:38:32.000000 pumaz-1.6.1/pumaz/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:38:38.497245 pumaz-1.6.1/pumaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13321 2024-04-22 13:38:38.000000 pumaz-1.6.1/pumaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-22 13:38:38.000000 pumaz-1.6.1/pumaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:38:38.000000 pumaz-1.6.1/pumaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 13:38:38.000000 pumaz-1.6.1/pumaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-22 13:38:38.000000 pumaz-1.6.1/pumaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 13:38:38.000000 pumaz-1.6.1/pumaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:38:38.497245 pumaz-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-22 13:38:32.000000 pumaz-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:29:06.560712 pumaz-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    13265 2024-05-24 18:29:06.560712 pumaz-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-24 18:29:02.000000 pumaz-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:29:06.560712 pumaz-1.6.3/pumaz/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16931 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44926 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/pumaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-24 18:29:02.000000 pumaz-1.6.3/pumaz/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:29:06.560712 pumaz-1.6.3/pumaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13265 2024-05-24 18:29:06.000000 pumaz-1.6.3/pumaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-24 18:29:06.000000 pumaz-1.6.3/pumaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:29:06.000000 pumaz-1.6.3/pumaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 18:29:06.000000 pumaz-1.6.3/pumaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-24 18:29:06.000000 pumaz-1.6.3/pumaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 18:29:06.000000 pumaz-1.6.3/pumaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:29:06.560712 pumaz-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-24 18:29:02.000000 pumaz-1.6.3/setup.py
```

### Comparing `pumaz-1.6.1/PKG-INFO` & `pumaz-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 1.6.1
+Version: 1.6.3
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at, Sebastian.Gutschmayer@meduniwien.ac.at, Manuel.pires@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Classifier: Development Status :: 4 - Beta
@@ -225,15 +225,15 @@
 Well, in the world of mathematics and science, 'Z' often represents the unknown, the variable that's yet to be discovered, or the final destination in a series. We at QIMP believe in always pushing boundaries, venturing into uncharted territories, and staying on the cutting edge of technology. The 'Z' embodies this philosophy. It represents our constant quest to uncover what lies beyond the known, to explore the undiscovered, and to bring you the future of medical imaging.
 
 Each time you see a 'Z' in one of our package names, be reminded of the spirit of exploration and discovery that drives our work. With QIMP, you're not just installing a package; you're joining us on a journey to the frontiers of medical image processing. Here's to exploring the 'Z' dimension together! 🚀
  
 
 ## Contributors ✨
 
-Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+Thanks goes to these wonderful people  ✨:
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
```

### Comparing `pumaz-1.6.1/README.md` & `pumaz-1.6.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 Well, in the world of mathematics and science, 'Z' often represents the unknown, the variable that's yet to be discovered, or the final destination in a series. We at QIMP believe in always pushing boundaries, venturing into uncharted territories, and staying on the cutting edge of technology. The 'Z' embodies this philosophy. It represents our constant quest to uncover what lies beyond the known, to explore the undiscovered, and to bring you the future of medical imaging.
 
 Each time you see a 'Z' in one of our package names, be reminded of the spirit of exploration and discovery that drives our work. With QIMP, you're not just installing a package; you're joining us on a journey to the frontiers of medical image processing. Here's to exploring the 'Z' dimension together! 🚀
  
 
 ## Contributors ✨
 
-Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+Thanks goes to these wonderful people  ✨:
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
```

### Comparing `pumaz-1.6.1/pumaz/constants.py` & `pumaz-1.6.3/pumaz/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 MOOSE_PREFIX_PUMA_CPU = 'Clin_CT_PUMA4_'
 MOOSE_LABEL_INDEX = {
     1: "legs",
     2: "body",
     3: "head",
     4: "arms"
 }
-MOOSE_FILLER_LABEL = 18
+MOOSE_FILLER_LABEL = 24
 
 # FOLDER NAMES
 
 PUMA_WORKING_FOLDER = 'PUMAZ-v1' + '-' + datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
 TRANSFORMS_FOLDER = 'transforms'
 ALIGNED_MASK_FOLDER = 'aligned_MASK'
 ALIGNED_CT_FOLDER = 'aligned_CT'
```

### Comparing `pumaz-1.6.1/pumaz/display.py` & `pumaz-1.6.3/pumaz/display.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.6.1/pumaz/download.py` & `pumaz-1.6.3/pumaz/download.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.6.1/pumaz/file_utilities.py` & `pumaz-1.6.3/pumaz/file_utilities.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.6.1/pumaz/image_conversion.py` & `pumaz-1.6.3/pumaz/image_conversion.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.6.1/pumaz/image_processing.py` & `pumaz-1.6.3/pumaz/image_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,31 +355,23 @@
     Returns:
     - None
     """
     # Load the masks
     multilabel_mask = sitk.ReadImage(multilabel_mask_path, sitk.sitkUInt8)
     body_mask = sitk.ReadImage(body_mask_path, sitk.sitkUInt8)
 
-    # Remove the filler label from the multilabel mask
-    multilabel_no_filler = sitk.BinaryThreshold(multilabel_mask, lowerThreshold=0,
-                                                upperThreshold=MOOSE_FILLER_LABEL - 1,
-                                                insideValue=1, outsideValue=0)
-
-    # Convert no filler mask back to the original values where filler label was removed
-    multilabel_no_filler = multilabel_no_filler * multilabel_mask
-
-    # Subtract the no filler binary mask from the binary body mask
+    # Subtract the binary PUMA mask from the binary body mask
     binary_body_mask = body_mask > 0
-    remaining_mask = binary_body_mask - (multilabel_no_filler > 0)
+    remaining_mask = binary_body_mask - (multilabel_mask > 0)
 
     # Scale the remaining mask with the filler label intensity
     scaled_remaining_mask = remaining_mask * MOOSE_FILLER_LABEL
 
     # Combine the multilabel mask with no filler label and the scaled remaining mask
-    final_mask = sitk.Add(multilabel_no_filler, scaled_remaining_mask)
+    final_mask = sitk.Add(multilabel_mask, scaled_remaining_mask)
 
     # Write the resulting mask to the output path
     sitk.WriteImage(final_mask, output_path)
```

### Comparing `pumaz-1.6.1/pumaz/input_validation.py` & `pumaz-1.6.3/pumaz/input_validation.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.6.1/pumaz/pumaz.py` & `pumaz-1.6.3/pumaz/pumaz.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,16 @@
     image_conversion.standardize_to_nifti(subject_folder)
     logging.info(" Standardization complete.")
 
     # --------------------------------------
     # CHECKING FOR PUMA COMPLIANT SUBJECTS
     # --------------------------------------
 
-    tracer_dirs = [os.path.join(subject_folder, d) for d in os.listdir(subject_folder) if
-                   os.path.isdir(os.path.join(subject_folder, d))]
+    tracer_dirs = [os.path.join(subject_folder, d) for d in os.listdir(subject_folder)
+                   if os.path.isdir(os.path.join(subject_folder, d)) and not d.startswith('PUMAZ-v1')]
     puma_compliant_subject_folders = input_validation.select_puma_compliant_subject_folders(tracer_dirs)
 
     num_subject_folders = len(puma_compliant_subject_folders)
     if num_subject_folders < 1:
         print(
             f'{constants.ANSI_RED} {emoji.emojize(":cross_mark:")} No puma compliant tracer directories found to continue!{constants.ANSI_RESET} {emoji.emojize(":light_bulb:")} See: https://github.com/Keyn34/PUMA#directory-structure-and-naming-conventions-for-puma-%EF%B8%8F')
         return
```

### Comparing `pumaz-1.6.1/pumaz/resources.py` & `pumaz-1.6.3/pumaz/resources.py`

 * *Files identical despite different names*

### Comparing `pumaz-1.6.1/pumaz.egg-info/PKG-INFO` & `pumaz-1.6.3/pumaz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pumaz
-Version: 1.6.1
+Version: 1.6.3
 Summary: PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and reproducibility of PET image studies.
 Home-page: https://github.com/QIMP-Team/PUMA
 Author: Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at, Sebastian.Gutschmayer@meduniwien.ac.at, Manuel.pires@meduniwien.ac.at
 License: GPLv3
 Keywords: PET tracer alignment,diffeomorphic imaging,image processing,multiplexed tracers
 Classifier: Development Status :: 4 - Beta
@@ -225,15 +225,15 @@
 Well, in the world of mathematics and science, 'Z' often represents the unknown, the variable that's yet to be discovered, or the final destination in a series. We at QIMP believe in always pushing boundaries, venturing into uncharted territories, and staying on the cutting edge of technology. The 'Z' embodies this philosophy. It represents our constant quest to uncover what lies beyond the known, to explore the undiscovered, and to bring you the future of medical imaging.
 
 Each time you see a 'Z' in one of our package names, be reminded of the spirit of exploration and discovery that drives our work. With QIMP, you're not just installing a package; you're joining us on a journey to the frontiers of medical image processing. Here's to exploring the 'Z' dimension together! 🚀
  
 
 ## Contributors ✨
 
-Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+Thanks goes to these wonderful people  ✨:
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
     <tr>
```

### Comparing `pumaz-1.6.1/setup.py` & `pumaz-1.6.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='pumaz',
-    version='1.6.1',
+    version='1.6.3',
     author='Lalith Kumar Shiyam Sundar, Sebastian Gutschmayer, Manuel Pires',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at, Sebastian.Gutschmayer@meduniwien.ac.at, '
                  'Manuel.pires@meduniwien.ac.at',
     description='PUMA (PET Universal Multi-tracer Aligner) is a robust and efficient tool for aligning images from '
                 'different PET tracers. It leverages advanced diffeomorphic imaging techniques to offer high-precision '
                 'alignment for multiplexed tracer images. PUMA aims to significantly enhance the accuracy and '
                 'reproducibility of PET image studies.',
```

