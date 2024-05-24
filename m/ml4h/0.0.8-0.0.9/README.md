# Comparing `tmp/ml4h-0.0.8.tar.gz` & `tmp/ml4h-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4h-0.0.8.tar", last modified: Fri Nov  3 20:45:23 2023, max compression
+gzip compressed data, was "ml4h-0.0.9.tar", last modified: Fri Nov  3 21:05:35 2023, max compression
```

## Comparing `ml4h-0.0.8.tar` & `ml4h-0.0.9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.593214 ml4h-0.0.8/
--rw-r--r--   0 sam        (503) staff       (20)     1633 2023-05-09 09:39:59.000000 ml4h-0.0.8/LICENSE.txt
--rw-r--r--   0 sam        (503) staff       (20)     4491 2023-05-09 09:39:59.000000 ml4h-0.0.8/NOTICE.txt
--rw-r--r--   0 sam        (503) staff       (20)     8048 2023-11-03 20:45:23.593069 ml4h-0.0.8/PKG-INFO
--rw-r--r--   0 sam        (503) staff       (20)     7783 2023-11-03 20:40:56.000000 ml4h-0.0.8/README.md
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.578775 ml4h-0.0.8/ml4h/
--rwxr-xr-x   0 sam        (503) staff       (20)     2361 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/DatabaseClient.py
--rwxr-xr-x   0 sam        (503) staff       (20)    23803 2023-11-03 20:40:52.000000 ml4h-0.0.8/ml4h/TensorMap.py
--rwxr-xr-x   0 sam        (503) staff       (20)       22 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/__init__.py
--rwxr-xr-x   0 sam        (503) staff       (20)    35600 2023-09-25 18:54:19.000000 ml4h-0.0.8/ml4h/arguments.py
--rw-r--r--   0 sam        (503) staff       (20)    17485 2023-11-03 20:40:52.000000 ml4h-0.0.8/ml4h/data_descriptions.py
--rwxr-xr-x   0 sam        (503) staff       (20)     9425 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/defines.py
--rwxr-xr-x   0 sam        (503) staff       (20)    65687 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/explorations.py
--rwxr-xr-x   0 sam        (503) staff       (20)     7604 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/hypertuning.py
--rwxr-xr-x   0 sam        (503) staff       (20)     1846 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/logger.py
--rwxr-xr-x   0 sam        (503) staff       (20)     6325 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/make_tensor_maps_for_partners_ecg_labels.py
--rwxr-xr-x   0 sam        (503) staff       (20)    27625 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/metrics.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.580249 ml4h-0.0.8/ml4h/ml4ht_integration/
--rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/ml4ht_integration/__init__.py
--rwxr-xr-x   0 sam        (503) staff       (20)     8093 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/ml4ht_integration/tensor_generator.py
--rwxr-xr-x   0 sam        (503) staff       (20)     5358 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/ml4ht_integration/tensor_map.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.583224 ml4h-0.0.8/ml4h/models/
--rwxr-xr-x   0 sam        (503) staff       (20)      422 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/Block.py
--rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/__init__.py
--rwxr-xr-x   0 sam        (503) staff       (20)     8437 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/basic_blocks.py
--rwxr-xr-x   0 sam        (503) staff       (20)    23869 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/conv_blocks.py
--rwxr-xr-x   0 sam        (503) staff       (20)     6020 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/inspect.py
--rwxr-xr-x   0 sam        (503) staff       (20)     6368 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/layer_wrappers.py
--rwxr-xr-x   0 sam        (503) staff       (20)    67632 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/legacy_models.py
--rwxr-xr-x   0 sam        (503) staff       (20)    13360 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/merge_blocks.py
--rwxr-xr-x   0 sam        (503) staff       (20)    18791 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/model_factory.py
--rwxr-xr-x   0 sam        (503) staff       (20)     8805 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/perceiver_blocks.py
--rwxr-xr-x   0 sam        (503) staff       (20)     3642 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/pretrained_blocks.py
--rwxr-xr-x   0 sam        (503) staff       (20)     4258 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/train.py
--rwxr-xr-x   0 sam        (503) staff       (20)    14436 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/transformer_blocks.py
--rwxr-xr-x   0 sam        (503) staff       (20)     7947 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/models/transformer_blocks_embedding.py
--rwxr-xr-x   0 sam        (503) staff       (20)     2848 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/normalizer.py
--rwxr-xr-x   0 sam        (503) staff       (20)     4238 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/optimizers.py
--rwxr-xr-x   0 sam        (503) staff       (20)   128897 2023-11-03 20:40:52.000000 ml4h-0.0.8/ml4h/plots.py
--rwxr-xr-x   0 sam        (503) staff       (20)    50703 2023-11-03 20:40:52.000000 ml4h-0.0.8/ml4h/recipes.py
--rwxr-xr-x   0 sam        (503) staff       (20)     5424 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/runtime_data_defines.py
--rwxr-xr-x   0 sam        (503) staff       (20)    40052 2023-05-09 09:39:59.000000 ml4h-0.0.8/ml4h/tensor_generators.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.584254 ml4h-0.0.8/ml4h/tensorize/
--rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensorize/__init__.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.584596 ml4h-0.0.8/ml4h/tensorize/dataflow/
--rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensorize/dataflow/__init__.py
--rwxr-xr-x   0 sam        (503) staff       (20)     7724 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensorize/dataflow/bigquery_ukb_queries.py
--rwxr-xr-x   0 sam        (503) staff       (20)     4257 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensorize/merge_hd5s.py
--rwxr-xr-x   0 sam        (503) staff       (20)    18759 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensorize/tensor_writer_mgb.py
--rwxr-xr-x   0 sam        (503) staff       (20)    62179 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensorize/tensor_writer_ukbb.py
--rwxr-xr-x   0 sam        (503) staff       (20)     3243 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensorize/tensorize_dataflow.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.586152 ml4h-0.0.8/ml4h/tensormap/
--rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/__init__.py
--rwxr-xr-x   0 sam        (503) staff       (20)     8657 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/celeba.py
--rwxr-xr-x   0 sam        (503) staff       (20)     2152 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/gatk.py
--rwxr-xr-x   0 sam        (503) staff       (20)     6283 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/general.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.586679 ml4h-0.0.8/ml4h/tensormap/mgb/
--rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/mgb/__init__.py
--rwxr-xr-x   0 sam        (503) staff       (20)    47783 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/mgb/dynamic.py
--rwxr-xr-x   0 sam        (503) staff       (20)    73630 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/mgb/ecg.py
--rwxr-xr-x   0 sam        (503) staff       (20)     4035 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/mnist.py
--rwxr-xr-x   0 sam        (503) staff       (20)    14184 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/tensor_map_maker.py
--rwxr-xr-x   0 sam        (503) staff       (20)     4154 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/text.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.590884 ml4h-0.0.8/ml4h/tensormap/ukb/
--rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/__init__.py
--rwxr-xr-x   0 sam        (503) staff       (20)   250867 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/categorical.py
--rwxr-xr-x   0 sam        (503) staff       (20)   542886 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/continuous.py
--rwxr-xr-x   0 sam        (503) staff       (20)    44560 2023-11-03 20:40:52.000000 ml4h-0.0.8/ml4h/tensormap/ukb/demographics.py
--rwxr-xr-x   0 sam        (503) staff       (20)   101606 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/disease.py
--rwxr-xr-x   0 sam        (503) staff       (20)     7946 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/dxa.py
--rwxr-xr-x   0 sam        (503) staff       (20)    61466 2023-11-03 20:40:52.000000 ml4h-0.0.8/ml4h/tensormap/ukb/ecg.py
--rwxr-xr-x   0 sam        (503) staff       (20)    34805 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/genetics.py
--rwxr-xr-x   0 sam        (503) staff       (20)   128836 2023-11-03 20:40:52.000000 ml4h-0.0.8/ml4h/tensormap/ukb/mri.py
--rwxr-xr-x   0 sam        (503) staff       (20)    12774 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/mri_brain.py
--rwxr-xr-x   0 sam        (503) staff       (20)     6557 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/mri_ecg.py
--rwxr-xr-x   0 sam        (503) staff       (20)    11925 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/mri_vtk.py
--rwxr-xr-x   0 sam        (503) staff       (20)    14905 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/tensormap/ukb/survival.py
--rwxr-xr-x   0 sam        (503) staff       (20)     3316 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/test_utils.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.592833 ml4h-0.0.8/ml4h/visualization_tools/
--rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/__init__.py
--rwxr-xr-x   0 sam        (503) staff       (20)     7219 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/annotation_storage.py
--rwxr-xr-x   0 sam        (503) staff       (20)     5764 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/annotations.py
--rwxr-xr-x   0 sam        (503) staff       (20)    10397 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/batch_image_annotations.py
--rwxr-xr-x   0 sam        (503) staff       (20)    10420 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/dicom_interactive_plots.py
--rwxr-xr-x   0 sam        (503) staff       (20)    15258 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/dicom_plots.py
--rwxr-xr-x   0 sam        (503) staff       (20)     6203 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/ecg_interactive_plots.py
--rwxr-xr-x   0 sam        (503) staff       (20)     9855 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/ecg_reshape.py
--rwxr-xr-x   0 sam        (503) staff       (20)     3106 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/ecg_static_plots.py
--rwxr-xr-x   0 sam        (503) staff       (20)     3329 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/facets.py
--rwxr-xr-x   0 sam        (503) staff       (20)    14368 2023-09-19 15:09:13.000000 ml4h-0.0.8/ml4h/visualization_tools/hd5_mri_plots.py
-drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 20:45:23.579736 ml4h-0.0.8/ml4h.egg-info/
--rw-r--r--   0 sam        (503) staff       (20)     8048 2023-11-03 20:45:23.000000 ml4h-0.0.8/ml4h.egg-info/PKG-INFO
--rw-r--r--   0 sam        (503) staff       (20)     2474 2023-11-03 20:45:23.000000 ml4h-0.0.8/ml4h.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (503) staff       (20)        1 2023-11-03 20:45:23.000000 ml4h-0.0.8/ml4h.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (503) staff       (20)      584 2023-11-03 20:45:23.000000 ml4h-0.0.8/ml4h.egg-info/requires.txt
--rw-r--r--   0 sam        (503) staff       (20)        5 2023-11-03 20:45:23.000000 ml4h-0.0.8/ml4h.egg-info/top_level.txt
--rw-r--r--   0 sam        (503) staff       (20)       38 2023-11-03 20:45:23.593265 ml4h-0.0.8/setup.cfg
--rw-r--r--   0 sam        (503) staff       (20)      753 2023-11-03 20:44:58.000000 ml4h-0.0.8/setup.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.272619 ml4h-0.0.9/
+-rw-r--r--   0 sam        (503) staff       (20)     1633 2023-05-09 09:39:59.000000 ml4h-0.0.9/LICENSE.txt
+-rw-r--r--   0 sam        (503) staff       (20)     4491 2023-05-09 09:39:59.000000 ml4h-0.0.9/NOTICE.txt
+-rw-r--r--   0 sam        (503) staff       (20)     8048 2023-11-03 21:05:35.272477 ml4h-0.0.9/PKG-INFO
+-rw-r--r--   0 sam        (503) staff       (20)     7783 2023-11-03 20:40:56.000000 ml4h-0.0.9/README.md
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.257498 ml4h-0.0.9/ml4h/
+-rwxr-xr-x   0 sam        (503) staff       (20)     2361 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/DatabaseClient.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    23803 2023-11-03 20:40:52.000000 ml4h-0.0.9/ml4h/TensorMap.py
+-rwxr-xr-x   0 sam        (503) staff       (20)       22 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/__init__.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    35600 2023-09-25 18:54:19.000000 ml4h-0.0.9/ml4h/arguments.py
+-rw-r--r--   0 sam        (503) staff       (20)    17485 2023-11-03 20:40:52.000000 ml4h-0.0.9/ml4h/data_descriptions.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     9425 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/defines.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    65687 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/explorations.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     7604 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/hypertuning.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     1846 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/logger.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     6325 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/make_tensor_maps_for_partners_ecg_labels.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    27625 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/metrics.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.258952 ml4h-0.0.9/ml4h/ml4ht_integration/
+-rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/ml4ht_integration/__init__.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     8093 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/ml4ht_integration/tensor_generator.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     5358 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/ml4ht_integration/tensor_map.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.262319 ml4h-0.0.9/ml4h/models/
+-rwxr-xr-x   0 sam        (503) staff       (20)      422 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/Block.py
+-rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/__init__.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     8437 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/basic_blocks.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    23869 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/conv_blocks.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     6020 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/inspect.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     6368 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/layer_wrappers.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    67632 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/legacy_models.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    13360 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/merge_blocks.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    18791 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/model_factory.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     8805 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/perceiver_blocks.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     3642 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/pretrained_blocks.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     4258 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/train.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    14436 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/transformer_blocks.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     7947 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/models/transformer_blocks_embedding.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     2848 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/normalizer.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     4238 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/optimizers.py
+-rwxr-xr-x   0 sam        (503) staff       (20)   128897 2023-11-03 20:40:52.000000 ml4h-0.0.9/ml4h/plots.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    50703 2023-11-03 20:40:52.000000 ml4h-0.0.9/ml4h/recipes.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     5424 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/runtime_data_defines.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    40052 2023-05-09 09:39:59.000000 ml4h-0.0.9/ml4h/tensor_generators.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.263331 ml4h-0.0.9/ml4h/tensorize/
+-rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensorize/__init__.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.263634 ml4h-0.0.9/ml4h/tensorize/dataflow/
+-rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensorize/dataflow/__init__.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     7724 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensorize/dataflow/bigquery_ukb_queries.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     4257 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensorize/merge_hd5s.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    18759 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensorize/tensor_writer_mgb.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    62179 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensorize/tensor_writer_ukbb.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     3243 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensorize/tensorize_dataflow.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.265068 ml4h-0.0.9/ml4h/tensormap/
+-rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/__init__.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     8657 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/celeba.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     2152 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/gatk.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     6283 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/general.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.265659 ml4h-0.0.9/ml4h/tensormap/mgb/
+-rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/mgb/__init__.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    47783 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/mgb/dynamic.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    73630 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/mgb/ecg.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     4035 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/mnist.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    14184 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/tensor_map_maker.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     4154 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/text.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.270302 ml4h-0.0.9/ml4h/tensormap/ukb/
+-rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/__init__.py
+-rwxr-xr-x   0 sam        (503) staff       (20)   250867 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/categorical.py
+-rwxr-xr-x   0 sam        (503) staff       (20)   542886 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/continuous.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    44560 2023-11-03 20:40:52.000000 ml4h-0.0.9/ml4h/tensormap/ukb/demographics.py
+-rwxr-xr-x   0 sam        (503) staff       (20)   101606 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/disease.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     7946 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/dxa.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    61466 2023-11-03 20:40:52.000000 ml4h-0.0.9/ml4h/tensormap/ukb/ecg.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    34805 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/genetics.py
+-rwxr-xr-x   0 sam        (503) staff       (20)   128836 2023-11-03 20:40:52.000000 ml4h-0.0.9/ml4h/tensormap/ukb/mri.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    12774 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/mri_brain.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     6557 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/mri_ecg.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    11925 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/mri_vtk.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    14905 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/tensormap/ukb/survival.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     3316 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/test_utils.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.272251 ml4h-0.0.9/ml4h/visualization_tools/
+-rwxr-xr-x   0 sam        (503) staff       (20)        0 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/__init__.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     7219 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/annotation_storage.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     5764 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/annotations.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    10397 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/batch_image_annotations.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    10420 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/dicom_interactive_plots.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    15258 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/dicom_plots.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     6203 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/ecg_interactive_plots.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     9855 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/ecg_reshape.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     3106 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/ecg_static_plots.py
+-rwxr-xr-x   0 sam        (503) staff       (20)     3329 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/facets.py
+-rwxr-xr-x   0 sam        (503) staff       (20)    14368 2023-09-19 15:09:13.000000 ml4h-0.0.9/ml4h/visualization_tools/hd5_mri_plots.py
+drwxr-xr-x   0 sam        (503) staff       (20)        0 2023-11-03 21:05:35.258441 ml4h-0.0.9/ml4h.egg-info/
+-rw-r--r--   0 sam        (503) staff       (20)     8048 2023-11-03 21:05:35.000000 ml4h-0.0.9/ml4h.egg-info/PKG-INFO
+-rw-r--r--   0 sam        (503) staff       (20)     2474 2023-11-03 21:05:35.000000 ml4h-0.0.9/ml4h.egg-info/SOURCES.txt
+-rw-r--r--   0 sam        (503) staff       (20)        1 2023-11-03 21:05:35.000000 ml4h-0.0.9/ml4h.egg-info/dependency_links.txt
+-rw-r--r--   0 sam        (503) staff       (20)       27 2023-11-03 21:05:35.000000 ml4h-0.0.9/ml4h.egg-info/requires.txt
+-rw-r--r--   0 sam        (503) staff       (20)        5 2023-11-03 21:05:35.000000 ml4h-0.0.9/ml4h.egg-info/top_level.txt
+-rw-r--r--   0 sam        (503) staff       (20)       38 2023-11-03 21:05:35.272667 ml4h-0.0.9/setup.cfg
+-rw-r--r--   0 sam        (503) staff       (20)      767 2023-11-03 21:05:16.000000 ml4h-0.0.9/setup.py
```

### Comparing `ml4h-0.0.8/LICENSE.txt` & `ml4h-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/NOTICE.txt` & `ml4h-0.0.9/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/PKG-INFO` & `ml4h-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4h
-Version: 0.0.8
+Version: 0.0.9
 Summary: Machine Learning for Health python package
 Home-page: https://github.com/broadinstitute/ml4h
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
```

### Comparing `ml4h-0.0.8/README.md` & `ml4h-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/DatabaseClient.py` & `ml4h-0.0.9/ml4h/DatabaseClient.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/TensorMap.py` & `ml4h-0.0.9/ml4h/TensorMap.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/arguments.py` & `ml4h-0.0.9/ml4h/arguments.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/data_descriptions.py` & `ml4h-0.0.9/ml4h/data_descriptions.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/defines.py` & `ml4h-0.0.9/ml4h/defines.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/explorations.py` & `ml4h-0.0.9/ml4h/explorations.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/hypertuning.py` & `ml4h-0.0.9/ml4h/hypertuning.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/logger.py` & `ml4h-0.0.9/ml4h/logger.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/make_tensor_maps_for_partners_ecg_labels.py` & `ml4h-0.0.9/ml4h/make_tensor_maps_for_partners_ecg_labels.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/metrics.py` & `ml4h-0.0.9/ml4h/metrics.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/ml4ht_integration/tensor_generator.py` & `ml4h-0.0.9/ml4h/ml4ht_integration/tensor_generator.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/ml4ht_integration/tensor_map.py` & `ml4h-0.0.9/ml4h/ml4ht_integration/tensor_map.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/basic_blocks.py` & `ml4h-0.0.9/ml4h/models/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/conv_blocks.py` & `ml4h-0.0.9/ml4h/models/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/inspect.py` & `ml4h-0.0.9/ml4h/models/inspect.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/layer_wrappers.py` & `ml4h-0.0.9/ml4h/models/layer_wrappers.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/legacy_models.py` & `ml4h-0.0.9/ml4h/models/legacy_models.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/merge_blocks.py` & `ml4h-0.0.9/ml4h/models/merge_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/model_factory.py` & `ml4h-0.0.9/ml4h/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/perceiver_blocks.py` & `ml4h-0.0.9/ml4h/models/perceiver_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/pretrained_blocks.py` & `ml4h-0.0.9/ml4h/models/pretrained_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/train.py` & `ml4h-0.0.9/ml4h/models/train.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/transformer_blocks.py` & `ml4h-0.0.9/ml4h/models/transformer_blocks.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/models/transformer_blocks_embedding.py` & `ml4h-0.0.9/ml4h/models/transformer_blocks_embedding.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/normalizer.py` & `ml4h-0.0.9/ml4h/normalizer.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/optimizers.py` & `ml4h-0.0.9/ml4h/optimizers.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/plots.py` & `ml4h-0.0.9/ml4h/plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/recipes.py` & `ml4h-0.0.9/ml4h/recipes.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/runtime_data_defines.py` & `ml4h-0.0.9/ml4h/runtime_data_defines.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensor_generators.py` & `ml4h-0.0.9/ml4h/tensor_generators.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensorize/dataflow/bigquery_ukb_queries.py` & `ml4h-0.0.9/ml4h/tensorize/dataflow/bigquery_ukb_queries.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensorize/merge_hd5s.py` & `ml4h-0.0.9/ml4h/tensorize/merge_hd5s.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensorize/tensor_writer_mgb.py` & `ml4h-0.0.9/ml4h/tensorize/tensor_writer_mgb.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensorize/tensor_writer_ukbb.py` & `ml4h-0.0.9/ml4h/tensorize/tensor_writer_ukbb.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensorize/tensorize_dataflow.py` & `ml4h-0.0.9/ml4h/tensorize/tensorize_dataflow.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/celeba.py` & `ml4h-0.0.9/ml4h/tensormap/celeba.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/gatk.py` & `ml4h-0.0.9/ml4h/tensormap/gatk.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/general.py` & `ml4h-0.0.9/ml4h/tensormap/general.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/mgb/dynamic.py` & `ml4h-0.0.9/ml4h/tensormap/mgb/dynamic.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/mgb/ecg.py` & `ml4h-0.0.9/ml4h/tensormap/mgb/ecg.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/mnist.py` & `ml4h-0.0.9/ml4h/tensormap/mnist.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/tensor_map_maker.py` & `ml4h-0.0.9/ml4h/tensormap/tensor_map_maker.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/text.py` & `ml4h-0.0.9/ml4h/tensormap/text.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/categorical.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/categorical.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/continuous.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/continuous.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/demographics.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/demographics.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/disease.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/disease.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/dxa.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/dxa.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/ecg.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/ecg.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/genetics.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/genetics.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/mri.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/mri.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/mri_brain.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/mri_brain.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/mri_ecg.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/mri_ecg.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/mri_vtk.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/mri_vtk.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/tensormap/ukb/survival.py` & `ml4h-0.0.9/ml4h/tensormap/ukb/survival.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/test_utils.py` & `ml4h-0.0.9/ml4h/test_utils.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/annotation_storage.py` & `ml4h-0.0.9/ml4h/visualization_tools/annotation_storage.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/annotations.py` & `ml4h-0.0.9/ml4h/visualization_tools/annotations.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/batch_image_annotations.py` & `ml4h-0.0.9/ml4h/visualization_tools/batch_image_annotations.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/dicom_interactive_plots.py` & `ml4h-0.0.9/ml4h/visualization_tools/dicom_interactive_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/dicom_plots.py` & `ml4h-0.0.9/ml4h/visualization_tools/dicom_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/ecg_interactive_plots.py` & `ml4h-0.0.9/ml4h/visualization_tools/ecg_interactive_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/ecg_reshape.py` & `ml4h-0.0.9/ml4h/visualization_tools/ecg_reshape.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/ecg_static_plots.py` & `ml4h-0.0.9/ml4h/visualization_tools/ecg_static_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/facets.py` & `ml4h-0.0.9/ml4h/visualization_tools/facets.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h/visualization_tools/hd5_mri_plots.py` & `ml4h-0.0.9/ml4h/visualization_tools/hd5_mri_plots.py`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/ml4h.egg-info/PKG-INFO` & `ml4h-0.0.9/ml4h.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml4h
-Version: 0.0.8
+Version: 0.0.9
 Summary: Machine Learning for Health python package
 Home-page: https://github.com/broadinstitute/ml4h
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
```

### Comparing `ml4h-0.0.8/ml4h.egg-info/SOURCES.txt` & `ml4h-0.0.9/ml4h.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml4h-0.0.8/setup.py` & `ml4h-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 # Get the requirements from the requirements file
 requirements = (here / 'docker/vm_boot_images/config/tensorflow-requirements.txt').read_text(encoding='utf-8')
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 setup(
     name='ml4h',
-    version='0.0.8',
+    version='0.0.9',
     description='Machine Learning for Health python package',
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',
     url='https://github.com/broadinstitute/ml4h',
     python_requires='>=3.6',
-    #install_requires=["ml4ht", "tensorflow"], # requirements
-    install_requires=requirements,
+    install_requires=["ml4ht", "tensorflow", "numcodecs"],  # requirements
+    #install_requires=requirements,
     packages=find_packages(),
 )
```

