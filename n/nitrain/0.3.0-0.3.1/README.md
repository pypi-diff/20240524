# Comparing `tmp/nitrain-0.3.0.tar.gz` & `tmp/nitrain-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrain-0.3.0.tar", max compression
+gzip compressed data, was "nitrain-0.3.1.tar", max compression
```

## Comparing `nitrain-0.3.0.tar` & `nitrain-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0    34522 2024-04-24 12:16:09.356540 nitrain-0.3.0/LICENSE
--rw-r--r--   0        0        0    10779 2024-04-24 12:16:09.356540 nitrain-0.3.0/README.md
--rw-r--r--   0        0        0      187 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/__init__.py
--rw-r--r--   0        0        0      195 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/__init__.py
--rw-r--r--   0        0        0     5013 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/dataset.py
--rw-r--r--   0        0        0     3604 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/google_cloud_dataset.py
--rw-r--r--   0        0        0     3416 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/platform_dataset.py
--rw-r--r--   0        0        0     1264 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/datasets/utils.py
--rw-r--r--   0        0        0      125 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/explainers/__init__.py
--rw-r--r--   0        0        0     2307 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/explainers/occlusion_explainer.py
--rw-r--r--   0        0        0       27 2024-04-24 12:16:09.356540 nitrain-0.3.0/nitrain/loaders/__init__.py
--rw-r--r--   0        0        0      868 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/loaders/keras_loader.py
--rw-r--r--   0        0        0     4588 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/loaders/loader.py
--rw-r--r--   0        0        0      389 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/loaders/torch_loader.py
--rw-r--r--   0        0        0      145 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/models/__init__.py
--rw-r--r--   0        0        0     2293 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/models/fetch_architecture.py
--rw-r--r--   0        0        0      728 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/models/fetch_pretrained.py
--rw-r--r--   0        0        0      107 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/models/load.py
--rw-r--r--   0        0        0     6706 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/platform.py
--rw-r--r--   0        0        0      200 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/array_reader.py
--rw-r--r--   0        0        0     1986 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/column_reader.py
--rw-r--r--   0        0        0      915 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/compose_reader.py
--rw-r--r--   0        0        0      942 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/image_reader.py
--rw-r--r--   0        0        0     2143 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/pattern_reader.py
--rw-r--r--   0        0        0     4749 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/readers/utils.py
--rw-r--r--   0        0        0      375 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/__init__.py
--rw-r--r--   0        0        0     1134 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/base_sampler.py
--rw-r--r--   0        0        0     2828 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/block_sampler.py
--rw-r--r--   0        0        0     2615 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/patch_sampler.py
--rw-r--r--   0        0        0     1993 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/slice_patch_sampler.py
--rw-r--r--   0        0        0     2390 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/samplers/slice_sampler.py
--rw-r--r--   0        0        0      195 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/trainers/__init__.py
--rw-r--r--   0        0        0      419 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/trainers/google_cloud_trainer.py
--rw-r--r--   0        0        0     5825 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/trainers/platform_trainer.py
--rw-r--r--   0        0        0     3779 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/trainers/trainer.py
--rw-r--r--   0        0        0      276 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/__init__.py
--rw-r--r--   0        0        0      475 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/base_transform.py
--rw-r--r--   0        0        0     5591 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/intensity_transforms.py
--rw-r--r--   0        0        0     4642 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/spatial_transforms.py
--rw-r--r--   0        0        0     6597 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/structural_transforms.py
--rw-r--r--   0        0        0     1556 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/transforms/utility_transforms.py
--rw-r--r--   0        0        0      675 2024-04-24 12:16:09.360540 nitrain-0.3.0/nitrain/utils.py
--rw-r--r--   0        0        0      416 2024-04-24 12:16:09.360540 nitrain-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    11478 1970-01-01 00:00:00.000000 nitrain-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-05-24 17:05:11.966891 nitrain-0.3.1/LICENSE
+-rw-r--r--   0        0        0    10630 2024-05-24 17:05:11.966891 nitrain-0.3.1/README.md
+-rw-r--r--   0        0        0      336 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/datasets/__init__.py
+-rw-r--r--   0        0        0     5581 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/datasets/dataset.py
+-rw-r--r--   0        0        0     1896 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/datasets/google_cloud.py
+-rw-r--r--   0        0        0     6095 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/datasets/utils.py
+-rw-r--r--   0        0        0      115 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/explainers/__init__.py
+-rw-r--r--   0        0        0     1159 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/explainers/occlusion.py
+-rw-r--r--   0        0        0       27 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/loaders/__init__.py
+-rw-r--r--   0        0        0     6773 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/loaders/loader.py
+-rw-r--r--   0        0        0      122 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/models/__init__.py
+-rw-r--r--   0        0        0     2293 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/models/fetch_architecture.py
+-rw-r--r--   0        0        0      728 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/models/fetch_pretrained.py
+-rw-r--r--   0        0        0       32 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/predictors/__init__.py
+-rw-r--r--   0        0        0     2665 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/predictors/predictor.py
+-rw-r--r--   0        0        0      175 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/readers/__init__.py
+-rw-r--r--   0        0        0     4141 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/readers/column.py
+-rw-r--r--   0        0        0     1881 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/readers/compose.py
+-rw-r--r--   0        0        0     6057 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/readers/folder_name.py
+-rw-r--r--   0        0        0     4105 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/readers/image.py
+-rw-r--r--   0        0        0     1142 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/readers/memory.py
+-rw-r--r--   0        0        0     1405 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/readers/utils.py
+-rw-r--r--   0        0        0      335 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/samplers/__init__.py
+-rw-r--r--   0        0        0      934 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/samplers/base.py
+-rw-r--r--   0        0        0     2630 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/samplers/block.py
+-rw-r--r--   0        0        0     2369 2024-05-24 17:05:11.966891 nitrain-0.3.1/nitrain/samplers/patch.py
+-rw-r--r--   0        0        0     2322 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/samplers/slice.py
+-rw-r--r--   0        0        0     1816 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/samplers/slice_patch.py
+-rw-r--r--   0        0        0       28 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/trainers/__init__.py
+-rw-r--r--   0        0        0     3774 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/trainers/trainer.py
+-rw-r--r--   0        0        0      290 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/__init__.py
+-rw-r--r--   0        0        0      378 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/base.py
+-rw-r--r--   0        0        0     3953 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/image.py
+-rw-r--r--   0        0        0     4726 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/intensity.py
+-rw-r--r--   0        0        0     1267 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/labels.py
+-rw-r--r--   0        0        0     1875 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/math.py
+-rw-r--r--   0        0        0     1101 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/shape.py
+-rw-r--r--   0        0        0    10110 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/spatial.py
+-rw-r--r--   0        0        0     5522 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/spatial_random.py
+-rw-r--r--   0        0        0     1443 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/transforms/utility.py
+-rw-r--r--   0        0        0      358 2024-05-24 17:05:11.970891 nitrain-0.3.1/nitrain/utils.py
+-rw-r--r--   0        0        0      429 2024-05-24 17:05:11.970891 nitrain-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    11363 1970-01-01 00:00:00.000000 nitrain-0.3.1/PKG-INFO
```

### Comparing `nitrain-0.3.0/LICENSE` & `nitrain-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrain-0.3.0/README.md` & `nitrain-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,119 +1,124 @@
-# Nitrain - a framework for medical imaging AI
+# Nitrain: a medical imaging-native AI framework
 
 [![Coverage Status](https://coveralls.io/repos/github/nitrain/nitrain/badge.svg?branch=main)](https://coveralls.io/github/nitrain/nitrain?branch=main)
-[![Build](https://github.com/ncullen93/nitrain/actions/workflows/test.yml/badge.svg)](https://github.com/ncullen93/nitrain/actions/workflows/test.yml)
+[![Build](https://github.com/nitrain/nitrain/actions/workflows/test.yml/badge.svg)](https://github.com/nitrain/nitrain/actions/workflows/test.yml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nitrain)
 
-Nitrain (formerly <i>torchsample</i>) provides tools for sampling and augmenting medical images, training models on medical imaging datasets, and visualizing model results in a medical imaging context. It supports using pytorch, keras, and tensorflow.
+Nitrain (formerly <i>torchsample</i>) is a framework-agnostic library for sampling and augmenting medical images, training models on medical imaging datasets, and visualizing results in a medical imaging context.
 
-To learn how to use nitrain or to view complete examples of training medical imaging AI models using nitrain, visit [github.com/nitrain/tutorials](https://github.com/nitrain/tutorials) or view the rendered version at [nitrain.dev/docs](https://nitrain.dev/docs). If you want to learn more generally about medical imaging AI, check out the book [Becoming a medical imaging AI expert with Python](https://book.nitrain.dev).
+Full examples of training medical imaging AI models using nitrain can be found at the [tutorials](https://github.com/nitrain/tutorials) repo. If you are interested more generally in medical imaging AI, check out the book [Becoming a medical imaging AI expert with Python](https://book.nitrain.dev).
 
 <br />
 
 ## Quickstart
 
-Here is a canonical example of using nitrain to fit a brain-age model. If you want to learn a bit more about key components of nitrain then you can follow the overview tutorials just below the quickstart.
+Here is a canonical example of using nitrain to a semantic segmentation model. Notice how easy it is to map image files from a local folder and how straight-forward it is to sample batches of augmented, 2D slices from 3D images.
 
 ```python
 import nitrain as nt
-from nitrain.readers import PatternReader, ColumnReader
+from nitrain.readers import ImageReader, ColumnReader
 
 # create dataset from folder of images + participants file
-dataset = nt.Dataset(inputs=PatternReader('sub-*/anat/*_T1w.nii.gz'),
-                          outputs=ColumnReader('participants.tsv', 'age'),
-                          transforms={
-                              'inputs': [tx.Resize((64,64,64)), tx.NormalizeIntensity(0,1)],
-                          },
-                          base_dir='~/desktop/ds004711/')
+dataset = nt.Dataset(inputs=ImageReader('sub-*/anat/*_T1w.nii.gz'),
+                     outputs=ImageReader('sub-*/anat/*_aparc+aseg.nii.gz'),
+                     transforms={
+                         'inputs': tx.NormalizeIntensity(0,1),
+                         ('inputs', 'outputs'): tx.Resize((64,64,64))
+                     },
+                     base_dir='~/desktop/ds004711/')
 
 # create loader with random transforms
 loader = nt.Loader(dataset,
-                        images_per_batch=4,
-                        shuffle=True,
-                        sampler=nitrain.SliceSampler(batch_size = 32, axis = 2)
-                        transforms={
-                                'inputs': tx.RandomNoise(sd=0.2)
-                        })
+                   images_per_batch=4,
+                   sampler=nt.SliceSampler(batch_size = 32, axis = 2)
+                   transforms={
+                           'inputs': tx.RandomNoise(sd=0.2)
+                   })
 
 # create model from architecture
-arch_fn = nt.fetch_architecture('alexnet', dim=2)
+arch_fn = nt.fetch_architecture('unet', dim=2)
 model = arch_fn(input_image_size=(64,64,1),
-                number_of_outcomes=1,
-                mode='regression')
+                mode='segmentation')
 
 # create trainer and fit model
-trainer = nt.Trainer(model,
-                          loss='mse',
-                          optimizer='adam',
-                          lr=1e-3,
-                          callbacks=[utils.EarlyStopping(),
-                                     utils.ModelCheckpoints(freq=25)])
+trainer = nt.Trainer(model, task='segmentation')
 trainer.fit(loader, epochs=100)
 
 # upload trained model to platform
-nt.register_model(trainer.model, 'nick/t1-brain-age')
+nt.register_model(trainer.model, 'nick/t1-brain-segmentation')
 ```
 
-A more in-depth introduction can be found in the [tutorials](github.com/ncullen93/nitrain) and if you can also check out the [examples](github.com/ncullen93/nitrain) for self-contained notebooks showing how to perform common deep learning tasks.
+If you want to learn a bit more about key components of nitrain then you can follow the 10-minute overview tutorial further below. Also, a large variety of self-contained notebooks showing how to perform common medical imaging AI tasks is available in the [tutorials](https://www.github.com/nitrain/tutorials) repo.
 
 <br />
 
 ## Installation
 
 The latest release of nitrain can be installed from pypi:
 
 ```
 pip install nitrain
 ```
 
 Or you can install the latest development version directly from github:
 
 ```
-python -m pip install git+github.com/ncullen93/nitrain.git
+python -m pip install git+github.com/nitrain/nitrain.git
 ```
 
 ### Dependencies
 
-The nitrain package uses the `antspy` package to efficiently read and transform medical images. It relies on the `antspynet` package to create some architectures. Additionally, you can use keras (tf.keras or keras3), tensorflow, or pytorch as backend - with support for only importing the framework you are using.
+The [antspy](https://www.github.com/antsx/antspy) package is a key dependency that allows you to efficiently read, operate on, and visualize medical images. Additionally, you can use keras (tf.keras or keras3), tensorflow, pytorch, or jax as backend for creating your models.
 
 <br />
 
 ## Overview of nitrain
 
 The 10-minute overview presented below will take you through the key components of nitrain:
 
-- [Datasets and Loaders](#datasets-and-loaders)
-- [Samplers](#samplers)
-- [Transforms](#transforms)
+- [Datasets](#datasets)
+- [Loaders](#loaders)
 - [Architectures and pretrained models](#architectures-and-pretrained-models)
-- [Model trainers](#model-trainers)
+- [Model Trainers](#model-trainers)
 - [Explainers](#explainers)
 
 <br />
 
-### Datasets and Loaders
+### Datasets
 
 Datasets help you read in your images from wherever they are stored -- in a local folder, in memory, on a cloud service. You can flexibly specify the inputs and outputs using glob patterns, etc. Transforms can also be passed to your datasets as a sort of preprocessing pipeline that will be applied whenever the dataset is accessed.
 
 ```python
-from nitrain import datasets, transforms as tx
+import nitrain as nt
+from nitrain import transforms as tx
 
-dataset = datasets.FolderDataset(base_dir='~/datasets/ds004711',
-                                 x={'pattern': 'sub-*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
+dataset = datasets.FolderDataset(x={'pattern': 'sub-*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
                                  y={'file': 'participants.tsv', 'column': 'age'},
                                  x_transforms=[tx.Resample((64,64,64))])
 ```
 
 Although you will rarely need to do this, data can be read into memory by indexing the dataset:
 
 ```python
 x_raw, y_raw = dataset[:3]
 ```
 
+#### Readers
+
+Notice that we used a `FolderReader` to specify that we wanted to read images from a local folder.
+
+#### Fixed Transforms
+
+You also saw that we passed in transforms to our dataset using a dictionary. We call these "fixed transforms" because they will only be applied once to your images (when they are first loaded from file) and their result never changes.
+
+<br />
+
+### Loaders
+
 To prepare your images for batch generation during training, you pass the dataset into one the loaders. Here is where you can also pass in random transforms that will act as data augmentation. If you want to train on slices, patches, or blocks of images then you will additionally provide a sampler. The different samplers are explained later.
 
 ```python
 from nitrain import loaders, samplers
 
 loader = loaders.DatasetLoader(dataset,
                                images_per_batch=32,
@@ -122,17 +127,15 @@
 # loop through all images in batches for one epoch
 for x_batch, y_batch in loader:
         print(y_batch)
 ```
 
 The loader can be be used directly as a batch generator to fit models in tensorflow, keras, pytorch, or any other framework.
 
-<br />
-
-### Samplers
+#### Samplers
 
 Samplers allow you to keep the same dataset + loader workflow that batches entire images and applies transforms to them, but then expand on those transformed image batches to create special "sub-batches".
 
 For instance, samplers let you serve batches of 2D slices from 3D images, or 3D blocks from 3D images, and so forth. Samplers are essntial for common deep learning workflows in medical imaging where you often want to train a model on only parts of the image at once.
 
 ```python
 from nitrain import loaders, samplers, transforms as tx
@@ -140,17 +143,15 @@
                                images_per_batch=4,
                                x_transforms=[tx.RandomSmoothing(0, 1)],
                                sampler=samplers.SliceSampler(batch_size=24, axis=2))
 ```
 
 What happens is that we start with the ~190 images from the dataset, but 4 images will be read in from file at a time. Then, all possible 2D slices will be created from those 4 images and served in shuffled batches of 24 from the loader. Once all "sub-batches" (sets of 24 slices from the 4 images) have been served, the loader will move on to the next 4 images and serve slices from those images. One epoch is completed when all slices from all images have been served.
 
-<br />
-
-### Transforms
+#### Random Transforms
 
 The philosophy of nitrain is to be medical imaging-native. This means that all transforms are applied directly on images - specifically, `antsImage` types from the [ANTsPy](https://github.com/antsx/antspy) package - and only at the very end of batch generator are the images converted to arrays / tensors for model consumption.
 
 The nitrain package supports an extensive amount of medical imaging transforms:
 
 - Affine (Rotate, Translate, Shear, Zoom)
 - Flip, Pad, Crop, Slice
@@ -165,19 +166,19 @@
 
 my_tx = tx.CustomTransform(lambda x: x * 2)
 ```
 
 If you want to explore what a transform does, you can take a sample of it over any number of trials on the same image and then plot the results:
 
 ```python
-import ntimage as nt
+import ants
 import numpy as np
 from nitrain import transforms as tx
 
-img = nt.load(nt.example_data('r16'))
+img = ants.image_read(ants.get_data('r16'))
 
 my_tx = tx.RandomSmoothing(0, 2)
 imgs = my_tx.sample(img, n=12)
 
 nt.plot_grid(imgs, shape=(4,3))
 ```
```

### Comparing `nitrain-0.3.0/nitrain/models/fetch_architecture.py` & `nitrain-0.3.1/nitrain/models/fetch_architecture.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.3.0/nitrain/models/fetch_pretrained.py` & `nitrain-0.3.1/nitrain/models/fetch_pretrained.py`

 * *Files identical despite different names*

### Comparing `nitrain-0.3.0/nitrain/readers/compose_reader.py` & `nitrain-0.3.1/nitrain/readers/memory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 import glob
 import os
 from parse import parse
 from fnmatch import fnmatch
 
 import pandas as pd
 import numpy as np
+import ants
 
-class ComposeReader:
-    def __init__(self, readers, label=None):
-        self.readers = readers
+class MemoryReader:
+    def __init__(self, data, label=None):
+        """
+        Read from in-memory records.
+        
+        The records can be a numpy array, a list of images, a list of scalars, etc.
+        """
+        self.values = data
         self.label = label
-    
-    def map_values(self, base_dir=None, base_label=None):
-        for idx, reader in enumerate(self.readers):
-            reader.map_values(base_dir=base_dir, base_label=f'{base_label}-{idx}')
         
+        if ants.is_image(data[0]):
+            self.as_image = True
+        else:
+            self.as_image = False
+            
+    def select(self, idx):
+        new_reader = MemoryReader(self.values, self.label)
+        new_reader.values = self.values
+        new_reader.values = [new_reader.values[i] for i in idx]
+        return new_reader
+        
+    def map_values(self, base_dir=None, base_file=None, base_label=None):
         if self.label is None:
             if base_label is not None:
                 self.label = base_label
             else:
-                self.label = 'compose'
-        self.values = list(zip(*[reader.values for reader in self.readers]))
-
+                self.label = 'memory'
+        
     def __getitem__(self, idx):
-        values = {}
-        for reader in self.readers:
-            values.update(reader[idx])
-        return {self.label: values}
-    
-    def __len__(self):
-        return len(self.values)
+        return {self.label: self.values[idx]}
 
+    def __len__(self):
+        return len(self.values)
```

### Comparing `nitrain-0.3.0/nitrain/readers/pattern_reader.py` & `nitrain-0.3.1/nitrain/readers/image.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,105 @@
 import glob
 import os
 from parse import parse
 from fnmatch import fnmatch
+import glob
+from google.cloud import storage
+from google.oauth2 import service_account
 
 import pandas as pd
 import numpy as np
-import ntimage as nt
+import ants
 
-class PatternReader:
-    def __init__(self, pattern, exclude=None, label=None):
+class ImageReader:
+    def __init__(self, pattern, base_dir=None, exclude=None, label=None):
         """
-        >>> import ntimage as nt
-        >>> from nitrain.readers import PatternReader
-        >>> reader = PatternReader('volumes/*.nii')
+        >>> import ants
+        >>> from nitrain.readers import ImageReader
+        >>> reader = ImageReader('volumes/*.nii')
         >>> reader.map_values(base_dir='~/Desktop/kaggle-liver-ct/')
         >>> img = reader[1]
         """
-        self.pattern = pattern
+        self.pattern = os.path.expanduser(pattern)
+        
+        if base_dir:
+            base_dir = os.path.expanduser(base_dir)
+        self.base_dir = base_dir
         self.exclude = exclude
         self.label = label
     
-    def map_values(self, base_dir=None, base_label=None):
+    def select(self, idx):
+        new_reader = ImageReader(self.pattern, self.base_dir, self.exclude, self.label)
+        new_reader.values = self.values
+        new_reader.values = [new_reader.values[i] for i in idx]
+        return new_reader
+        
+    def map_gcs_values(self, bucket, credentials=None, base_dir=None, base_file=None, base_label=None):
+        if base_dir is None:
+            base_dir = self.base_dir
+        
         pattern = self.pattern
         exclude = self.exclude
         
-        pattern = os.path.expanduser(pattern)
         glob_pattern = pattern.replace('{id}','*')
         
         if base_dir is not None:
             if not base_dir.endswith('/'):
                 base_dir += '/'
-            base_dir = os.path.expanduser(base_dir)
             glob_pattern = os.path.join(base_dir, glob_pattern)
-        x = sorted(glob.glob(glob_pattern, recursive=True))
+        
+        # GCS
+        if isinstance(credentials, str):
+            credentials = service_account.Credentials.from_service_account_file(credentials)
+        storage_client = storage.Client(credentials=credentials)
+        bucket_client = storage_client.bucket(bucket)
+        
+        x = storage_client.list_blobs(bucket, match_glob=glob_pattern)
+        
+        x = list([blob.name.replace(base_dir, '') for blob in x])
+
+        if exclude:
+            x = [file for file in x if not fnmatch(file, exclude)]
+
+        if '{id}' in pattern:
+            ids = [parse(pattern.replace('*','{other}'), file).named['id'] for file in x]
+        else:
+            ids = None
+
+        if base_dir is not None:
+            x = [os.path.join(base_dir, file) for file in x]
+        
+        if len(x) == 0:
+            raise Exception(f'No filepaths found that match {glob_pattern}')
 
+        self.values = x
+        self.ids = ids
+        
+        if self.label is None:
+            if base_label is not None:
+                self.label = base_label
+            else:
+                self.label = 'pattern'
+                
+    def map_values(self, base_dir=None, base_label=None, **kwargs):
+        if base_dir is None:
+            base_dir = self.base_dir
+        
+        pattern = self.pattern
+        exclude = self.exclude
+        
+        glob_pattern = pattern.replace('{id}','*')
+        
+        if base_dir is not None:
+            if not base_dir.endswith('/'):
+                base_dir += '/'
+            glob_pattern = os.path.join(base_dir, glob_pattern)
+
+        x = sorted(glob.glob(glob_pattern, recursive=True))
+        
         if base_dir is not None:
             x = [os.path.relpath(xx, base_dir) for xx in x]
         
         if exclude:
             x = [file for file in x if not fnmatch(file, exclude)]
 
         if '{id}' in pattern:
@@ -57,13 +119,11 @@
         if self.label is None:
             if base_label is not None:
                 self.label = base_label
             else:
                 self.label = 'pattern'
                 
     def __getitem__(self, idx):
-        if not self.values:
-            raise Exception('You must call `map_values()` before indexing a reader.')
-        return {self.label: nt.load(self.values[idx])}
+        return {self.label: ants.image_read(self.values[idx])}
     
     def __len__(self):
         return len(self.values)
```

### Comparing `nitrain-0.3.0/nitrain/samplers/base_sampler.py` & `nitrain-0.3.1/nitrain/samplers/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 import numpy as np
 import random
 
+import ants
 
 class BaseSampler:
     """
     Standard sampler that just returns the batch with or without shuffling
     
     Examples
     --------
     
     """
     def __init__(self, batch_size, shuffle=False):
         self.batch_size = batch_size
         self.shuffle = shuffle
     
     def __call__(self, x, y):
-        self.x = x
-        self.y = y
+        self.x = rearrange_values(x)
+        self.y = rearrange_values(y)
         return self
 
     def __iter__(self):
         """
         Get a sampled batch
         """
         self.idx = 0
         return self
 
     def __next__(self):
         if self.idx < 1:
             self.idx += 1
             x = self.x
-            y = self.y
-                
-            if self.shuffle:
-                indices = random.sample(range(len(y)), len(y))
-                x = [x[i] for i in indices]
-                if 'NTImage' in str(type(y[0])):
-                    y = [y[i] for i in indices]
-                else:
-                    y = y[indices]
-            
+            y = self.y            
             return x, y
         else:
             raise StopIteration
-    
-    def __len__(self):
-        """
-        number of batches from the sampler
-        """
-        return 1
+        
+def rearrange_values(x):
+    if isinstance(x[0], list):
+        return [rearrange_values([x[i][j] for i in range(len(x))]) for j in range(len(x[0]))]
+    return x
```

### Comparing `nitrain-0.3.0/nitrain/samplers/block_sampler.py` & `nitrain-0.3.1/nitrain/samplers/block.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,23 +47,14 @@
             data_indices = slice(self.idx*self.batch_size, min((self.idx+1)*self.batch_size, len(self.x)))
             self.idx += 1
             x = self.x[data_indices]
             y = self.y[data_indices]
             return x, y
         else:
             raise StopIteration
-    
-    def __len__(self):
-        """
-        number of batches from the sampler
-        """
-        if not self.x:
-            return 0
-        return math.ceil(len(self.x) / self.batch_size)
-
 
 def create_patches(images, values, block_size, stride):
     cropped_images = []
     new_values = []
     for image, value in zip(images, values):
         # extract all blocks
         x_strides = np.arange(0, (image.shape[0]-block_size[0]+1), step=stride[0])
@@ -72,15 +63,15 @@
         
         grid = np.meshgrid(x_strides, y_strides, z_strides)
         x_indices = grid[0].flatten()
         y_indices = grid[1].flatten()
         z_indices = grid[2].flatten()
         
         for a, b, c in zip(x_indices, y_indices, z_indices):
-            cropped_image = image.crop_indices([a,b,c], 
-                                               [a+block_size[0], 
+            cropped_image = image.crop_indices((a,b,c),
+                                               (a+block_size[0],
                                                 b+block_size[1],
-                                                c+block_size[2]])
+                                                c+block_size[2]))
             cropped_images.append(cropped_image)
             new_values.append(value)
                 
     return cropped_images, np.array(new_values)
```

### Comparing `nitrain-0.3.0/nitrain/samplers/patch_sampler.py` & `nitrain-0.3.1/nitrain/samplers/patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,22 +48,14 @@
             data_indices = slice(self.idx*self.batch_size, min((self.idx+1)*self.batch_size, len(self.x)))
             self.idx += 1
             x = self.x[data_indices]
             y = self.y[data_indices]
             return x, y
         else:
             raise StopIteration
-    
-    def __len__(self):
-        """
-        number of batches from the sampler
-        """
-        if not self.x:
-            return 0
-        return math.ceil(len(self.x) / self.batch_size)
 
 
 def create_patches(images, values, patch_size, stride):
     cropped_images = []
     new_values = []
     for image, value in zip(images, values):
         # extract all patches
@@ -71,14 +63,13 @@
         y_strides = np.arange(0, (image.shape[1]-patch_size[1]+1), step=stride[1])
         
         grid = np.meshgrid(x_strides, y_strides)
         x_indices = grid[0].flatten()
         y_indices = grid[1].flatten()
         
         for a, b in zip(x_indices, y_indices):
-            cropped_image = image.crop_indices([a,b], 
-                                               [a+patch_size[0], 
-                                                b+patch_size[1]])
+            cropped_image = image.crop_indices((a,b),
+                                               (a+patch_size[0],b+patch_size[1]))
             cropped_images.append(cropped_image)
             new_values.append(value)
                 
     return cropped_images, np.array(new_values)
```

### Comparing `nitrain-0.3.0/nitrain/samplers/slice_patch_sampler.py` & `nitrain-0.3.1/nitrain/samplers/slice_patch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import random
 import math
 
-from .patch_sampler import create_patches
-from .slice_sampler import create_slices
+from .patch import create_patches
+from .slice import create_slices
 
 class SlicePatchSampler:
     """
     Sampler that returns 2D patches from 3D images.
     """
     def __init__(self, patch_size, stride, axis, batch_size, shuffle=False):
         
@@ -21,15 +21,16 @@
         self.stride = stride
         self.axis = axis
         self.batch_size = batch_size
         self.shuffle = shuffle
     
     def __call__(self, x, y):
         # create slices of all images
-        x, y = create_slices(x, y, self.axis)
+        x = create_slices(x, self.axis)
+        y = create_slices(y, self.axis)
         # then create patches from all those slices
         x, y = create_patches(x, y, self.patch_size, self.stride)
         
         self.x = x
         self.y = y
         self.n_batches = math.ceil(len(x) / self.batch_size)
                 
@@ -56,15 +57,7 @@
             data_indices = slice(self.idx*self.batch_size, min((self.idx+1)*self.batch_size, len(self.x)))
             self.idx += 1
             x = self.x[data_indices]
             y = self.y[data_indices]
             return x, y
         else:
             raise StopIteration
-    
-    def __len__(self):
-        """
-        number of batches from the sampler
-        """
-        if not self.x:
-            return 0
-        return math.ceil(len(self.x) / self.batch_size)
```

### Comparing `nitrain-0.3.0/nitrain/trainers/trainer.py` & `nitrain-0.3.1/nitrain/trainers/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             return self.model.summary()
     
     def save(self, path):
         if self.framework == 'keras':
             self.model.save(path)
     
     def __repr__(self):
-        s = 'LocalTrainer ({})\n'.format(self.task)
+        s = 'Trainer ({})\n'.format(self.task)
         s = s +\
             '     {:<10} : {}\n'.format('Framework', self.framework)+\
             '     {:<10} : {}\n'.format('Loss', self.loss)+\
             '     {:<10} : {}\n'.format('Optimizer', self.optimizer)
         return s
```

### Comparing `nitrain-0.3.0/PKG-INFO` & `nitrain-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,138 +1,144 @@
 Metadata-Version: 2.1
 Name: nitrain
-Version: 0.3.0
-Summary: Cloud-based framework for training and sharing medical imaging AI models
+Version: 0.3.1
+Summary: Train medical imaging AI models locally or in the cloud with any framework
 License: MIT
 Author: ncullen93
 Author-email: nicholas.cullen@med.lu.se
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nitrain-image (>=0.1.1,<0.2.0)
+Requires-Dist: antspyx (>=0.5.3,<0.6.0)
 Requires-Dist: parse (>=1.20.1,<2.0.0)
 Requires-Dist: pydot (>=2.0.0,<3.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
-# Nitrain - a framework for medical imaging AI
+# Nitrain: a medical imaging-native AI framework
 
 [![Coverage Status](https://coveralls.io/repos/github/nitrain/nitrain/badge.svg?branch=main)](https://coveralls.io/github/nitrain/nitrain?branch=main)
-[![Build](https://github.com/ncullen93/nitrain/actions/workflows/test.yml/badge.svg)](https://github.com/ncullen93/nitrain/actions/workflows/test.yml)
+[![Build](https://github.com/nitrain/nitrain/actions/workflows/test.yml/badge.svg)](https://github.com/nitrain/nitrain/actions/workflows/test.yml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/nitrain)
 
-Nitrain (formerly <i>torchsample</i>) provides tools for sampling and augmenting medical images, training models on medical imaging datasets, and visualizing model results in a medical imaging context. It supports using pytorch, keras, and tensorflow.
+Nitrain (formerly <i>torchsample</i>) is a framework-agnostic library for sampling and augmenting medical images, training models on medical imaging datasets, and visualizing results in a medical imaging context.
 
-To learn how to use nitrain or to view complete examples of training medical imaging AI models using nitrain, visit [github.com/nitrain/tutorials](https://github.com/nitrain/tutorials) or view the rendered version at [nitrain.dev/docs](https://nitrain.dev/docs). If you want to learn more generally about medical imaging AI, check out the book [Becoming a medical imaging AI expert with Python](https://book.nitrain.dev).
+Full examples of training medical imaging AI models using nitrain can be found at the [tutorials](https://github.com/nitrain/tutorials) repo. If you are interested more generally in medical imaging AI, check out the book [Becoming a medical imaging AI expert with Python](https://book.nitrain.dev).
 
 <br />
 
 ## Quickstart
 
-Here is a canonical example of using nitrain to fit a brain-age model. If you want to learn a bit more about key components of nitrain then you can follow the overview tutorials just below the quickstart.
+Here is a canonical example of using nitrain to a semantic segmentation model. Notice how easy it is to map image files from a local folder and how straight-forward it is to sample batches of augmented, 2D slices from 3D images.
 
 ```python
 import nitrain as nt
-from nitrain.readers import PatternReader, ColumnReader
+from nitrain.readers import ImageReader, ColumnReader
 
 # create dataset from folder of images + participants file
-dataset = nt.Dataset(inputs=PatternReader('sub-*/anat/*_T1w.nii.gz'),
-                          outputs=ColumnReader('participants.tsv', 'age'),
-                          transforms={
-                              'inputs': [tx.Resize((64,64,64)), tx.NormalizeIntensity(0,1)],
-                          },
-                          base_dir='~/desktop/ds004711/')
+dataset = nt.Dataset(inputs=ImageReader('sub-*/anat/*_T1w.nii.gz'),
+                     outputs=ImageReader('sub-*/anat/*_aparc+aseg.nii.gz'),
+                     transforms={
+                         'inputs': tx.NormalizeIntensity(0,1),
+                         ('inputs', 'outputs'): tx.Resize((64,64,64))
+                     },
+                     base_dir='~/desktop/ds004711/')
 
 # create loader with random transforms
 loader = nt.Loader(dataset,
-                        images_per_batch=4,
-                        shuffle=True,
-                        sampler=nitrain.SliceSampler(batch_size = 32, axis = 2)
-                        transforms={
-                                'inputs': tx.RandomNoise(sd=0.2)
-                        })
+                   images_per_batch=4,
+                   sampler=nt.SliceSampler(batch_size = 32, axis = 2)
+                   transforms={
+                           'inputs': tx.RandomNoise(sd=0.2)
+                   })
 
 # create model from architecture
-arch_fn = nt.fetch_architecture('alexnet', dim=2)
+arch_fn = nt.fetch_architecture('unet', dim=2)
 model = arch_fn(input_image_size=(64,64,1),
-                number_of_outcomes=1,
-                mode='regression')
+                mode='segmentation')
 
 # create trainer and fit model
-trainer = nt.Trainer(model,
-                          loss='mse',
-                          optimizer='adam',
-                          lr=1e-3,
-                          callbacks=[utils.EarlyStopping(),
-                                     utils.ModelCheckpoints(freq=25)])
+trainer = nt.Trainer(model, task='segmentation')
 trainer.fit(loader, epochs=100)
 
 # upload trained model to platform
-nt.register_model(trainer.model, 'nick/t1-brain-age')
+nt.register_model(trainer.model, 'nick/t1-brain-segmentation')
 ```
 
-A more in-depth introduction can be found in the [tutorials](github.com/ncullen93/nitrain) and if you can also check out the [examples](github.com/ncullen93/nitrain) for self-contained notebooks showing how to perform common deep learning tasks.
+If you want to learn a bit more about key components of nitrain then you can follow the 10-minute overview tutorial further below. Also, a large variety of self-contained notebooks showing how to perform common medical imaging AI tasks is available in the [tutorials](https://www.github.com/nitrain/tutorials) repo.
 
 <br />
 
 ## Installation
 
 The latest release of nitrain can be installed from pypi:
 
 ```
 pip install nitrain
 ```
 
 Or you can install the latest development version directly from github:
 
 ```
-python -m pip install git+github.com/ncullen93/nitrain.git
+python -m pip install git+github.com/nitrain/nitrain.git
 ```
 
 ### Dependencies
 
-The nitrain package uses the `antspy` package to efficiently read and transform medical images. It relies on the `antspynet` package to create some architectures. Additionally, you can use keras (tf.keras or keras3), tensorflow, or pytorch as backend - with support for only importing the framework you are using.
+The [antspy](https://www.github.com/antsx/antspy) package is a key dependency that allows you to efficiently read, operate on, and visualize medical images. Additionally, you can use keras (tf.keras or keras3), tensorflow, pytorch, or jax as backend for creating your models.
 
 <br />
 
 ## Overview of nitrain
 
 The 10-minute overview presented below will take you through the key components of nitrain:
 
-- [Datasets and Loaders](#datasets-and-loaders)
-- [Samplers](#samplers)
-- [Transforms](#transforms)
+- [Datasets](#datasets)
+- [Loaders](#loaders)
 - [Architectures and pretrained models](#architectures-and-pretrained-models)
-- [Model trainers](#model-trainers)
+- [Model Trainers](#model-trainers)
 - [Explainers](#explainers)
 
 <br />
 
-### Datasets and Loaders
+### Datasets
 
 Datasets help you read in your images from wherever they are stored -- in a local folder, in memory, on a cloud service. You can flexibly specify the inputs and outputs using glob patterns, etc. Transforms can also be passed to your datasets as a sort of preprocessing pipeline that will be applied whenever the dataset is accessed.
 
 ```python
-from nitrain import datasets, transforms as tx
+import nitrain as nt
+from nitrain import transforms as tx
 
-dataset = datasets.FolderDataset(base_dir='~/datasets/ds004711',
-                                 x={'pattern': 'sub-*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
+dataset = datasets.FolderDataset(x={'pattern': 'sub-*/anat/*_T1w.nii.gz', 'exclude': '**run-02*'},
                                  y={'file': 'participants.tsv', 'column': 'age'},
                                  x_transforms=[tx.Resample((64,64,64))])
 ```
 
 Although you will rarely need to do this, data can be read into memory by indexing the dataset:
 
 ```python
 x_raw, y_raw = dataset[:3]
 ```
 
+#### Readers
+
+Notice that we used a `FolderReader` to specify that we wanted to read images from a local folder.
+
+#### Fixed Transforms
+
+You also saw that we passed in transforms to our dataset using a dictionary. We call these "fixed transforms" because they will only be applied once to your images (when they are first loaded from file) and their result never changes.
+
+<br />
+
+### Loaders
+
 To prepare your images for batch generation during training, you pass the dataset into one the loaders. Here is where you can also pass in random transforms that will act as data augmentation. If you want to train on slices, patches, or blocks of images then you will additionally provide a sampler. The different samplers are explained later.
 
 ```python
 from nitrain import loaders, samplers
 
 loader = loaders.DatasetLoader(dataset,
                                images_per_batch=32,
@@ -141,17 +147,15 @@
 # loop through all images in batches for one epoch
 for x_batch, y_batch in loader:
         print(y_batch)
 ```
 
 The loader can be be used directly as a batch generator to fit models in tensorflow, keras, pytorch, or any other framework.
 
-<br />
-
-### Samplers
+#### Samplers
 
 Samplers allow you to keep the same dataset + loader workflow that batches entire images and applies transforms to them, but then expand on those transformed image batches to create special "sub-batches".
 
 For instance, samplers let you serve batches of 2D slices from 3D images, or 3D blocks from 3D images, and so forth. Samplers are essntial for common deep learning workflows in medical imaging where you often want to train a model on only parts of the image at once.
 
 ```python
 from nitrain import loaders, samplers, transforms as tx
@@ -159,17 +163,15 @@
                                images_per_batch=4,
                                x_transforms=[tx.RandomSmoothing(0, 1)],
                                sampler=samplers.SliceSampler(batch_size=24, axis=2))
 ```
 
 What happens is that we start with the ~190 images from the dataset, but 4 images will be read in from file at a time. Then, all possible 2D slices will be created from those 4 images and served in shuffled batches of 24 from the loader. Once all "sub-batches" (sets of 24 slices from the 4 images) have been served, the loader will move on to the next 4 images and serve slices from those images. One epoch is completed when all slices from all images have been served.
 
-<br />
-
-### Transforms
+#### Random Transforms
 
 The philosophy of nitrain is to be medical imaging-native. This means that all transforms are applied directly on images - specifically, `antsImage` types from the [ANTsPy](https://github.com/antsx/antspy) package - and only at the very end of batch generator are the images converted to arrays / tensors for model consumption.
 
 The nitrain package supports an extensive amount of medical imaging transforms:
 
 - Affine (Rotate, Translate, Shear, Zoom)
 - Flip, Pad, Crop, Slice
@@ -184,19 +186,19 @@
 
 my_tx = tx.CustomTransform(lambda x: x * 2)
 ```
 
 If you want to explore what a transform does, you can take a sample of it over any number of trials on the same image and then plot the results:
 
 ```python
-import ntimage as nt
+import ants
 import numpy as np
 from nitrain import transforms as tx
 
-img = nt.load(nt.example_data('r16'))
+img = ants.image_read(ants.get_data('r16'))
 
 my_tx = tx.RandomSmoothing(0, 2)
 imgs = my_tx.sample(img, n=12)
 
 nt.plot_grid(imgs, shape=(4,3))
 ```
```

