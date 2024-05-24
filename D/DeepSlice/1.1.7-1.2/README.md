# Comparing `tmp/DeepSlice-1.1.7.tar.gz` & `tmp/deepslice-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSlice-1.1.7.tar", last modified: Tue Jan 30 12:12:49 2024, max compression
+gzip compressed data, was "deepslice-1.2.tar", last modified: Fri May 24 15:36:32 2024, max compression
```

## Comparing `DeepSlice-1.1.7.tar` & `deepslice-1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice/coord_post_processing/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/coord_post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/coord_post_processing/angle_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/coord_post_processing/depth_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice/coord_post_processing/plane_alignment_functions/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/coord_post_processing/spacing_and_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/metadata/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice/metadata/volumes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/metadata/volumes/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice/metadata/weights/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/metadata/weights/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice/neural_network/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/neural_network/network_architecture.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/neural_network/neural_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice/read_and_write/
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/read_and_write/QuickNII_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/DeepSlice/read_and_write/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/DeepSlice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-01-30 12:12:49.000000 DeepSlice-1.1.7/DeepSlice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-30 12:12:49.000000 DeepSlice-1.1.7/DeepSlice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 12:12:49.000000 DeepSlice-1.1.7/DeepSlice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-30 12:12:49.000000 DeepSlice-1.1.7/DeepSlice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-30 12:12:49.000000 DeepSlice-1.1.7/DeepSlice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-01-30 12:12:49.621643 DeepSlice-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-30 12:12:49.625643 DeepSlice-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-01-30 12:12:37.000000 DeepSlice-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.093908 deepslice-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/coord_post_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/angle_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/depth_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/coord_post_processing/plane_alignment_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/spacing_and_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/metadata/volumes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/volumes/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/metadata/weights/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/weights/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.093908 deepslice-1.2/DeepSlice/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/neural_network/network_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/neural_network/neural_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.093908 deepslice-1.2/DeepSlice/read_and_write/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/read_and_write/QuickNII_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/read_and_write/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.093908 deepslice-1.2/DeepSlice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 15:36:25.000000 deepslice-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-24 15:36:32.093908 deepslice-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-24 15:36:25.000000 deepslice-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 15:36:32.093908 deepslice-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-24 15:36:25.000000 deepslice-1.2/setup.py
```

### Comparing `DeepSlice-1.1.7/DeepSlice/coord_post_processing/angle_methods.py` & `deepslice-1.2/DeepSlice/coord_post_processing/angle_methods.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/DeepSlice/coord_post_processing/depth_estimation.py` & `deepslice-1.2/DeepSlice/coord_post_processing/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py` & `deepslice-1.2/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/DeepSlice/coord_post_processing/spacing_and_indexing.py` & `deepslice-1.2/DeepSlice/coord_post_processing/spacing_and_indexing.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/DeepSlice/main.py` & `deepslice-1.2/DeepSlice/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,19 +73,19 @@
             ensemble = False
         if use_secondary_model and ensemble:
             print("WARNING: use_secondary_model is set but ensemble is also set. use_secondary_model will be ignored.")
             use_secondary_model = False
         if use_secondary_model:
             print("Using secondary model")
             predictions = neural_network.predictions_util(
-                self.model, image_generator, secondary_weights,None, ensemble
+                self.model, image_generator, secondary_weights,None, ensemble, self.species
             )
         else:
             predictions = neural_network.predictions_util(
-                self.model, image_generator, primary_weights, secondary_weights, ensemble
+                self.model, image_generator, primary_weights, secondary_weights, ensemble, self.species
             )
         predictions["width"] = width
         predictions["height"] = height
         if section_numbers:
             predictions["nr"] = spacing_and_indexing.number_sections(
                 predictions["Filenames"], legacy_section_numbers
             )
```

### Comparing `DeepSlice-1.1.7/DeepSlice/metadata/config.json` & `deepslice-1.2/DeepSlice/metadata/config.json`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/DeepSlice/metadata/metadata_loader.py` & `deepslice-1.2/DeepSlice/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/DeepSlice/neural_network/neural_network.py` & `deepslice-1.2/DeepSlice/neural_network/neural_network.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pandas as pd
 import numpy as np
 import os
 from skimage.color import rgb2gray
 import warnings
 import imghdr
 import struct
+import h5py
 
 
 def gray_scale(img: np.ndarray) -> np.ndarray:
     """
     Convert the image to grayscale
 
     :param img: The image to convert
@@ -34,16 +35,15 @@
     :param weights: The weights for the network
     :type weights: list
     :param species: The species of the animal, this is necessary because of a previous error where the models are slightly different for different species
     :return: The initialised neural network
     :rtype: keras.models.Sequential
     """
     base_model = Xception(include_top=True, weights=xception_weights)
-    base_model._layers.pop()
-    base_model._layers.pop()
+    
     if species == "rat":
         inputs = Input(shape=(299, 299, 3))
         base_model_layer = base_model(inputs, training=True)
         dense1_layer = Dense(256, activation="relu")(base_model_layer)
         dense2_layer = Dense(256, activation="relu")(dense1_layer)
         output_layer = Dense(9, activation="linear")(dense2_layer)
         model = Model(inputs=inputs, outputs=output_layer)
@@ -51,19 +51,49 @@
         model = Sequential()
         model.add(base_model)
         model.add(Dense(256, activation="relu"))
         model.add(Dense(256, activation="relu"))
         model.add(Dense(9, activation="linear"))
 
     if weights != None:
-        model.load_weights(weights)
+        model = load_xception_weights(model, weights, species)
     return model
 
 
-
+def load_xception_weights(model, weights, species = "mouse"):
+    with h5py.File(weights, "r") as new:
+        # set weight of each layer manually
+        if species == "mouse":
+            xception_idx = 0
+            dense_idx = 1
+        elif species == "rat":
+            # RatModelInProgress.h5 has an "input_2" layer at index 0, so we need to adjust the indices<
+            xception_idx = 1
+            dense_idx = 2
+
+        model.layers[dense_idx].set_weights([new["dense"]["dense"]["kernel:0"], new["dense"]["dense"]["bias:0"]])
+        model.layers[dense_idx+1].set_weights([new["dense_1"]["dense_1"]["kernel:0"], new["dense_1"]["dense_1"]["bias:0"]])
+        model.layers[dense_idx+2].set_weights([new["dense_2"]["dense_2"]["kernel:0"], new["dense_2"]["dense_2"]["bias:0"]])
+
+        # Set the weights of the xception model 
+        weight_names = new["xception"].attrs["weight_names"].tolist()
+        weight_names_layers = [name.decode("utf-8").split("/")[0] for name in weight_names]
+
+        for i in range(len(model.layers[xception_idx].layers)):
+            name_of_layer = model.layers[xception_idx].layers[i].name
+            # if layer name is in the weight names, then we will set weights
+            if name_of_layer in weight_names_layers:
+                # Get name of weights in the layer
+                layer_weight_names = []
+                for weight in model.layers[xception_idx].layers[i].weights:
+                    layer_weight_names.append(weight.name.split("/")[1])
+                h5_group = new["xception"][name_of_layer]
+                weights_list = [np.array(h5_group[kk]) for kk in layer_weight_names]
+                model.layers[xception_idx].layers[i].set_weights(weights_list)
+    return model 
 
 def load_images_from_path(image_path: str) -> np.ndarray:
     """
     Load the images from the given path
     :param image_path: The path to the images
     :type image_path: str
     :return: an Image generator for the found images
@@ -137,42 +167,43 @@
 
 def predictions_util(
     model: Sequential,
     image_generator: ImageDataGenerator,
     primary_weights: str,
     secondary_weights: str,
     ensemble: bool = False,
+    species : str = "mouse"
 ):
     """
     Predict the image alignments
     
     :param model: The model to use for prediction
     :param image_generator: The image generator to use for prediction
     :type model: keras.models.Sequential
     :type image_generator: keras.preprocessing.image.ImageDataGenerator
     :return: The predicted alignments
     :rtype: list
     """
-    model.load_weights(primary_weights)
+    model = load_xception_weights(model, primary_weights, species)
     predictions = model.predict(
         image_generator,
         steps=image_generator.n // image_generator.batch_size,
         verbose=1,
     )
     predictions = predictions.astype(np.float64)
     if ensemble:
         image_generator.reset()
-        model.load_weights(secondary_weights)
+        model = load_xception_weights(model, secondary_weights, species)
         secondary_predictions = model.predict(
             image_generator,
             steps=image_generator.n // image_generator.batch_size,
             verbose=1,
         )
         predictions = np.mean([predictions, secondary_predictions], axis=0)
-        model.load_weights(primary_weights)
+        model = load_xception_weights(model, primary_weights, species)
     filenames = image_generator.filenames
     filenames = [os.path.basename(i) for i in filenames]
     predictions_df = pd.DataFrame(
         {
             "Filenames": filenames,
             "ox": predictions[:, 0],
             "oy": predictions[:, 1],
```

### Comparing `DeepSlice-1.1.7/DeepSlice/read_and_write/QuickNII_functions.py` & `deepslice-1.2/DeepSlice/read_and_write/QuickNII_functions.py`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/DeepSlice.egg-info/PKG-INFO` & `deepslice-1.2/DeepSlice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.7
+Version: 1.2
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.7.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scikit-image
-Requires-Dist: tensorflow==1.15.0
-Requires-Dist: h5py==2.10.0
+Requires-Dist: tensorflow<=2.15.0
+Requires-Dist: h5py
 Requires-Dist: typing
-Requires-Dist: pandas==1.3.5
+Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: protobuf==3.20
 Requires-Dist: lxml
 Requires-Dist: urllib3==1.26.6
 
 
 
@@ -57,24 +57,24 @@
 
 
 <a name='Installation'></a> 
 <h1> Installation </h1>
 <!-- This h2 must be bold  -->
 
 <h2 style="font-weight: bold; text-decoration: underline"> From PIP  </h2>
-This is the easy and recommended way to install DeepSlice. Make sure your env has Python 3.7 installed and then simply:
+This is the easy and recommended way to install DeepSlice, simply:
 
 ```bash
 pip install DeepSlice
 ```
 And you're ready to go! 🚀 Check out the PyPi package [here](https://pypi.org/project/DeepSlice/)
 
 <h2 style="font-weight: bold; text-decoration: underline"> From Source </h2>
 
-**First** To use DeepSlice you must have python3.7 installed. In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
+**First**  In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
 
 
 **Second** Once anaconda is installed, cd into your cloned DeepSlice directory, then cd into the 'conda_environments' directory, and use our premade environment files to setup your system. 
 ```
 cd DeepSlice/conda_environments
 ```
 * **CPU Installation** For most users we recommend using the DS-CPU.yaml installation file. this will install all the dependencies required to run DeepSlice on your CPU.
```

#### html2text {}

```diff
@@ -1,64 +1,61 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.7 Summary: A package to
-align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
-DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.7.tar.gz Author: DeepSlice Team Author-email:
-harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
-histology,brain,atlas,alignment Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
-Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
-Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: numpy Requires-Dist: scikit-learn Requires-Dist: scikit-
-image Requires-Dist: tensorflow==1.15.0 Requires-Dist: h5py==2.10.0 Requires-
-Dist: typing Requires-Dist: pandas==1.3.5 Requires-Dist: requests Requires-
-Dist: protobuf==3.20 Requires-Dist: lxml Requires-Dist: urllib3==1.26.6 [![DOI]
-(https://zenodo.org/badge/274122364.svg)](https://zenodo.org/badge/latestdoi/
-274122364) ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
-DeepSlice is a python library which automatically aligns mouse histology with
-the allen brain atlas common coordinate framework (and now rat brain histology
-to the Waxholm rat brain atlas, though this is in beta). The alignments are
-viewable, and refinable, using the [QuickNII](https://www.nitrc.org/projects/
-quicknii "QuickNII") software package. DeepSlice requires no preprocessing and
-works on any stain, however we have found it performs best on brightfield
-images. At present one limitation is that it only works on Coronally cut
-sections, we will release an update in the future for sagittal and horizontally
-cut histology. ![Alt](docs/images/process.PNG) DeepSlice automates the process
-of identifying exactly where in the brain a section lies, it can accomodate
-non-orthogonal cutting planes and will produce an image specific annotation for
-each section in your brain. ## Workflow DeepSlice is fully integrated with the
-_Q_U_I_N_T_ _w_o_r_k_f_l_o_w_. Quint helps you register, segment and quantify brain wide
-datasets!   ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use
-DeepSlice but don't need your own personal installation, check out [**DeepSlice
-Flask**](https://www.DeepSlice.com.au), a fully functional web application
-which will allow you to upload your dataset and download the aligned results.
-The web interface was developed by [Michael Pegios](https://github.com/
-ThermoDev/). ## [Installation: How to install DeepSlice](#installation) ##
-[Usage: How to align using DeepSlice](#basic-usage) ## [For a jupyter notebook
-example check out](examples/example_notebooks/DeepSlice_example.ipynb) **Happy
-Aligning :)**
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.2 Summary: A package to align
+histology to 3D brain atlases Home-page: https://github.com/PolarBean/DeepSlice
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/
+1.2.tar.gz Author: DeepSlice Team Author-email: harry.carey@medisin.uio.no
+License: GPL-3.0 Keywords: histology,brain,atlas,alignment Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Science/Research Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: scikit-learn
+Requires-Dist: scikit-image Requires-Dist: tensorflow<=2.15.0 Requires-Dist:
+h5py Requires-Dist: typing Requires-Dist: pandas Requires-Dist: requests
+Requires-Dist: protobuf==3.20 Requires-Dist: lxml Requires-Dist:
+urllib3==1.26.6 [![DOI](https://zenodo.org/badge/274122364.svg)](https://
+zenodo.org/badge/latestdoi/274122364) ![Alt](docs/images/
+DeepSlice_github_banner.png "DeepSlice Banner") DeepSlice is a python library
+which automatically aligns mouse histology with the allen brain atlas common
+coordinate framework (and now rat brain histology to the Waxholm rat brain
+atlas, though this is in beta). The alignments are viewable, and refinable,
+using the [QuickNII](https://www.nitrc.org/projects/quicknii "QuickNII")
+software package. DeepSlice requires no preprocessing and works on any stain,
+however we have found it performs best on brightfield images. At present one
+limitation is that it only works on Coronally cut sections, we will release an
+update in the future for sagittal and horizontally cut histology. ![Alt](docs/
+images/process.PNG) DeepSlice automates the process of identifying exactly
+where in the brain a section lies, it can accomodate non-orthogonal cutting
+planes and will produce an image specific annotation for each section in your
+brain. ## Workflow DeepSlice is fully integrated with the _Q_U_I_N_T_ _w_o_r_k_f_l_o_w_. Quint
+helps you register, segment and quantify brain wide datasets!  
+ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use DeepSlice but
+don't need your own personal installation, check out [**DeepSlice Flask**]
+(https://www.DeepSlice.com.au), a fully functional web application which will
+allow you to upload your dataset and download the aligned results. The web
+interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
+[Installation: How to install DeepSlice](#installation) ## [Usage: How to align
+using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
+(examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ************ IInnssttaallllaattiioonn ************
 ********** FFrroomm PPIIPP **********
-This is the easy and recommended way to install DeepSlice. Make sure your env
-has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
-you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
-project/DeepSlice/)
+This is the easy and recommended way to install DeepSlice, simply: ```bash pip
+install DeepSlice ``` And you're ready to go! ð Check out the PyPi package
+[here](https://pypi.org/project/DeepSlice/)
 ********** FFrroomm SSoouurrccee **********
-**First** To use DeepSlice you must have python3.7 installed. In order to
-easily install all the dependancies we recommend using [Anaconda](https://
-www.anaconda.com/products/individual "Anaconda Installation Files"). **Second**
-Once anaconda is installed, cd into your cloned DeepSlice directory, then cd
-into the 'conda_environments' directory, and use our premade environment files
-to setup your system. ``` cd DeepSlice/conda_environments ``` * **CPU
-Installation** For most users we recommend using the DS-CPU.yaml installation
-file. this will install all the dependencies required to run DeepSlice on your
-CPU. Do this with the command: conda env create -f DS-CPU.yml * **GPU
-Installation** If you wish to run DeepSlice on a huge number of images, and
-have access to an nvidia GPU then please use the DS-GPU.yaml installation file.
-conda env create -f DS-GPU.yml **Finished :)** You are now ready to run
+**First** In order to easily install all the dependancies we recommend using
+[Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation
+Files"). **Second** Once anaconda is installed, cd into your cloned DeepSlice
+directory, then cd into the 'conda_environments' directory, and use our premade
+environment files to setup your system. ``` cd DeepSlice/conda_environments ```
+* **CPU Installation** For most users we recommend using the DS-CPU.yaml
+installation file. this will install all the dependencies required to run
+DeepSlice on your CPU. Do this with the command: conda env create -f DS-CPU.yml
+* **GPU Installation** If you wish to run DeepSlice on a huge number of images,
+and have access to an nvidia GPU then please use the DS-GPU.yaml installation
+file. conda env create -f DS-GPU.yml **Finished :)** You are now ready to run
 DeepSlice. Just activate the environment using ```python conda activate DS-CPU
 ``` or ```python conda activate DS-GPU ``` If you run into any problems create
 a github issue and I will help you solve it.
 # Basic Usage ## On start After cloning our repo and navigating into the
 directory open an ipython session and import our package. ```python from
 DeepSlice import DSModel ``` Next, specify the species you would like to use
 and initiate the model. ```python species = 'mouse' #available species are
```

### Comparing `DeepSlice-1.1.7/DeepSlice.egg-info/SOURCES.txt` & `deepslice-1.2/DeepSlice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/LICENSE` & `deepslice-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSlice-1.1.7/PKG-INFO` & `deepslice-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.1.7
+Version: 1.2
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.7.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scikit-image
-Requires-Dist: tensorflow==1.15.0
-Requires-Dist: h5py==2.10.0
+Requires-Dist: tensorflow<=2.15.0
+Requires-Dist: h5py
 Requires-Dist: typing
-Requires-Dist: pandas==1.3.5
+Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: protobuf==3.20
 Requires-Dist: lxml
 Requires-Dist: urllib3==1.26.6
 
 
 
@@ -57,24 +57,24 @@
 
 
 <a name='Installation'></a> 
 <h1> Installation </h1>
 <!-- This h2 must be bold  -->
 
 <h2 style="font-weight: bold; text-decoration: underline"> From PIP  </h2>
-This is the easy and recommended way to install DeepSlice. Make sure your env has Python 3.7 installed and then simply:
+This is the easy and recommended way to install DeepSlice, simply:
 
 ```bash
 pip install DeepSlice
 ```
 And you're ready to go! 🚀 Check out the PyPi package [here](https://pypi.org/project/DeepSlice/)
 
 <h2 style="font-weight: bold; text-decoration: underline"> From Source </h2>
 
-**First** To use DeepSlice you must have python3.7 installed. In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
+**First**  In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
 
 
 **Second** Once anaconda is installed, cd into your cloned DeepSlice directory, then cd into the 'conda_environments' directory, and use our premade environment files to setup your system. 
 ```
 cd DeepSlice/conda_environments
 ```
 * **CPU Installation** For most users we recommend using the DS-CPU.yaml installation file. this will install all the dependencies required to run DeepSlice on your CPU.
```

#### html2text {}

```diff
@@ -1,64 +1,61 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.1.7 Summary: A package to
-align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
-DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
-tags/1.1.7.tar.gz Author: DeepSlice Team Author-email:
-harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
-histology,brain,atlas,alignment Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
-Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
-Language :: Python :: 3.7 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: numpy Requires-Dist: scikit-learn Requires-Dist: scikit-
-image Requires-Dist: tensorflow==1.15.0 Requires-Dist: h5py==2.10.0 Requires-
-Dist: typing Requires-Dist: pandas==1.3.5 Requires-Dist: requests Requires-
-Dist: protobuf==3.20 Requires-Dist: lxml Requires-Dist: urllib3==1.26.6 [![DOI]
-(https://zenodo.org/badge/274122364.svg)](https://zenodo.org/badge/latestdoi/
-274122364) ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
-DeepSlice is a python library which automatically aligns mouse histology with
-the allen brain atlas common coordinate framework (and now rat brain histology
-to the Waxholm rat brain atlas, though this is in beta). The alignments are
-viewable, and refinable, using the [QuickNII](https://www.nitrc.org/projects/
-quicknii "QuickNII") software package. DeepSlice requires no preprocessing and
-works on any stain, however we have found it performs best on brightfield
-images. At present one limitation is that it only works on Coronally cut
-sections, we will release an update in the future for sagittal and horizontally
-cut histology. ![Alt](docs/images/process.PNG) DeepSlice automates the process
-of identifying exactly where in the brain a section lies, it can accomodate
-non-orthogonal cutting planes and will produce an image specific annotation for
-each section in your brain. ## Workflow DeepSlice is fully integrated with the
-_Q_U_I_N_T_ _w_o_r_k_f_l_o_w_. Quint helps you register, segment and quantify brain wide
-datasets!   ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use
-DeepSlice but don't need your own personal installation, check out [**DeepSlice
-Flask**](https://www.DeepSlice.com.au), a fully functional web application
-which will allow you to upload your dataset and download the aligned results.
-The web interface was developed by [Michael Pegios](https://github.com/
-ThermoDev/). ## [Installation: How to install DeepSlice](#installation) ##
-[Usage: How to align using DeepSlice](#basic-usage) ## [For a jupyter notebook
-example check out](examples/example_notebooks/DeepSlice_example.ipynb) **Happy
-Aligning :)**
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.2 Summary: A package to align
+histology to 3D brain atlases Home-page: https://github.com/PolarBean/DeepSlice
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/
+1.2.tar.gz Author: DeepSlice Team Author-email: harry.carey@medisin.uio.no
+License: GPL-3.0 Keywords: histology,brain,atlas,alignment Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Science/Research Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: scikit-learn
+Requires-Dist: scikit-image Requires-Dist: tensorflow<=2.15.0 Requires-Dist:
+h5py Requires-Dist: typing Requires-Dist: pandas Requires-Dist: requests
+Requires-Dist: protobuf==3.20 Requires-Dist: lxml Requires-Dist:
+urllib3==1.26.6 [![DOI](https://zenodo.org/badge/274122364.svg)](https://
+zenodo.org/badge/latestdoi/274122364) ![Alt](docs/images/
+DeepSlice_github_banner.png "DeepSlice Banner") DeepSlice is a python library
+which automatically aligns mouse histology with the allen brain atlas common
+coordinate framework (and now rat brain histology to the Waxholm rat brain
+atlas, though this is in beta). The alignments are viewable, and refinable,
+using the [QuickNII](https://www.nitrc.org/projects/quicknii "QuickNII")
+software package. DeepSlice requires no preprocessing and works on any stain,
+however we have found it performs best on brightfield images. At present one
+limitation is that it only works on Coronally cut sections, we will release an
+update in the future for sagittal and horizontally cut histology. ![Alt](docs/
+images/process.PNG) DeepSlice automates the process of identifying exactly
+where in the brain a section lies, it can accomodate non-orthogonal cutting
+planes and will produce an image specific annotation for each section in your
+brain. ## Workflow DeepSlice is fully integrated with the _Q_U_I_N_T_ _w_o_r_k_f_l_o_w_. Quint
+helps you register, segment and quantify brain wide datasets!  
+ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use DeepSlice but
+don't need your own personal installation, check out [**DeepSlice Flask**]
+(https://www.DeepSlice.com.au), a fully functional web application which will
+allow you to upload your dataset and download the aligned results. The web
+interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
+[Installation: How to install DeepSlice](#installation) ## [Usage: How to align
+using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
+(examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ************ IInnssttaallllaattiioonn ************
 ********** FFrroomm PPIIPP **********
-This is the easy and recommended way to install DeepSlice. Make sure your env
-has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
-you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
-project/DeepSlice/)
+This is the easy and recommended way to install DeepSlice, simply: ```bash pip
+install DeepSlice ``` And you're ready to go! ð Check out the PyPi package
+[here](https://pypi.org/project/DeepSlice/)
 ********** FFrroomm SSoouurrccee **********
-**First** To use DeepSlice you must have python3.7 installed. In order to
-easily install all the dependancies we recommend using [Anaconda](https://
-www.anaconda.com/products/individual "Anaconda Installation Files"). **Second**
-Once anaconda is installed, cd into your cloned DeepSlice directory, then cd
-into the 'conda_environments' directory, and use our premade environment files
-to setup your system. ``` cd DeepSlice/conda_environments ``` * **CPU
-Installation** For most users we recommend using the DS-CPU.yaml installation
-file. this will install all the dependencies required to run DeepSlice on your
-CPU. Do this with the command: conda env create -f DS-CPU.yml * **GPU
-Installation** If you wish to run DeepSlice on a huge number of images, and
-have access to an nvidia GPU then please use the DS-GPU.yaml installation file.
-conda env create -f DS-GPU.yml **Finished :)** You are now ready to run
+**First** In order to easily install all the dependancies we recommend using
+[Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation
+Files"). **Second** Once anaconda is installed, cd into your cloned DeepSlice
+directory, then cd into the 'conda_environments' directory, and use our premade
+environment files to setup your system. ``` cd DeepSlice/conda_environments ```
+* **CPU Installation** For most users we recommend using the DS-CPU.yaml
+installation file. this will install all the dependencies required to run
+DeepSlice on your CPU. Do this with the command: conda env create -f DS-CPU.yml
+* **GPU Installation** If you wish to run DeepSlice on a huge number of images,
+and have access to an nvidia GPU then please use the DS-GPU.yaml installation
+file. conda env create -f DS-GPU.yml **Finished :)** You are now ready to run
 DeepSlice. Just activate the environment using ```python conda activate DS-CPU
 ``` or ```python conda activate DS-GPU ``` If you run into any problems create
 a github issue and I will help you solve it.
 # Basic Usage ## On start After cloning our repo and navigating into the
 directory open an ipython session and import our package. ```python from
 DeepSlice import DSModel ``` Next, specify the species you would like to use
 and initiate the model. ```python species = 'mouse' #available species are
```

### Comparing `DeepSlice-1.1.7/README.md` & `deepslice-1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
 
 <a name='Installation'></a> 
 <h1> Installation </h1>
 <!-- This h2 must be bold  -->
 
 <h2 style="font-weight: bold; text-decoration: underline"> From PIP  </h2>
-This is the easy and recommended way to install DeepSlice. Make sure your env has Python 3.7 installed and then simply:
+This is the easy and recommended way to install DeepSlice, simply:
 
 ```bash
 pip install DeepSlice
 ```
 And you're ready to go! 🚀 Check out the PyPi package [here](https://pypi.org/project/DeepSlice/)
 
 <h2 style="font-weight: bold; text-decoration: underline"> From Source </h2>
 
-**First** To use DeepSlice you must have python3.7 installed. In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
+**First**  In order to easily install all the dependancies we recommend using [Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation Files"). 
 
 
 **Second** Once anaconda is installed, cd into your cloned DeepSlice directory, then cd into the 'conda_environments' directory, and use our premade environment files to setup your system. 
 ```
 cd DeepSlice/conda_environments
 ```
 * **CPU Installation** For most users we recommend using the DS-CPU.yaml installation file. this will install all the dependencies required to run DeepSlice on your CPU.
```

#### html2text {}

```diff
@@ -20,31 +20,29 @@
 to upload your dataset and download the aligned results. The web interface was
 developed by [Michael Pegios](https://github.com/ThermoDev/). ## [Installation:
 How to install DeepSlice](#installation) ## [Usage: How to align using
 DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
 (examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
 ************ IInnssttaallllaattiioonn ************
 ********** FFrroomm PPIIPP **********
-This is the easy and recommended way to install DeepSlice. Make sure your env
-has Python 3.7 installed and then simply: ```bash pip install DeepSlice ``` And
-you're ready to go! ð Check out the PyPi package [here](https://pypi.org/
-project/DeepSlice/)
+This is the easy and recommended way to install DeepSlice, simply: ```bash pip
+install DeepSlice ``` And you're ready to go! ð Check out the PyPi package
+[here](https://pypi.org/project/DeepSlice/)
 ********** FFrroomm SSoouurrccee **********
-**First** To use DeepSlice you must have python3.7 installed. In order to
-easily install all the dependancies we recommend using [Anaconda](https://
-www.anaconda.com/products/individual "Anaconda Installation Files"). **Second**
-Once anaconda is installed, cd into your cloned DeepSlice directory, then cd
-into the 'conda_environments' directory, and use our premade environment files
-to setup your system. ``` cd DeepSlice/conda_environments ``` * **CPU
-Installation** For most users we recommend using the DS-CPU.yaml installation
-file. this will install all the dependencies required to run DeepSlice on your
-CPU. Do this with the command: conda env create -f DS-CPU.yml * **GPU
-Installation** If you wish to run DeepSlice on a huge number of images, and
-have access to an nvidia GPU then please use the DS-GPU.yaml installation file.
-conda env create -f DS-GPU.yml **Finished :)** You are now ready to run
+**First** In order to easily install all the dependancies we recommend using
+[Anaconda](https://www.anaconda.com/products/individual "Anaconda Installation
+Files"). **Second** Once anaconda is installed, cd into your cloned DeepSlice
+directory, then cd into the 'conda_environments' directory, and use our premade
+environment files to setup your system. ``` cd DeepSlice/conda_environments ```
+* **CPU Installation** For most users we recommend using the DS-CPU.yaml
+installation file. this will install all the dependencies required to run
+DeepSlice on your CPU. Do this with the command: conda env create -f DS-CPU.yml
+* **GPU Installation** If you wish to run DeepSlice on a huge number of images,
+and have access to an nvidia GPU then please use the DS-GPU.yaml installation
+file. conda env create -f DS-GPU.yml **Finished :)** You are now ready to run
 DeepSlice. Just activate the environment using ```python conda activate DS-CPU
 ``` or ```python conda activate DS-GPU ``` If you run into any problems create
 a github issue and I will help you solve it.
 # Basic Usage ## On start After cloning our repo and navigating into the
 directory open an ipython session and import our package. ```python from
 DeepSlice import DSModel ``` Next, specify the species you would like to use
 and initiate the model. ```python species = 'mouse' #available species are
```

### Comparing `DeepSlice-1.1.7/setup.py` & `deepslice-1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='DeepSlice',
     packages=find_packages(),
-    version='1.1.7',
+    version='1.2',
     license='GPL-3.0',
     description='A package to align histology to 3D brain atlases',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepSlice Team',
     package_data={'DeepSlice': ['metadata/volumes/placeholder.txt', 'metadata/config.json','metadata/weights/*.txt']},
     include_package_data=True,
     author_email='harry.carey@medisin.uio.no',
     url='https://github.com/PolarBean/DeepSlice',
-    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.1.7.tar.gz',
+    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.tar.gz',
     keywords=['histology', 'brain', 'atlas', 'alignment'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scikit-image',
-        'tensorflow==1.15.0',
-        'h5py==2.10.0',
+        'tensorflow<=2.15.0',
+        'h5py',
         'typing',
-        'pandas==1.3.5',
+        'pandas',
         'requests',
         'protobuf==3.20',
         'lxml',
         'urllib3==1.26.6'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python',
     ],
 
 )
```

