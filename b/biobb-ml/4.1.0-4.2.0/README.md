# Comparing `tmp/biobb_ml-4.1.0.tar.gz` & `tmp/biobb_ml-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_ml-4.1.0.tar", last modified: Fri Sep  8 08:44:16 2023, max compression
+gzip compressed data, was "biobb_ml-4.2.0.tar", last modified: Fri May 24 11:29:02 2024, max compression
```

## Comparing `biobb_ml-4.1.0.tar` & `biobb_ml-4.2.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.410286 biobb_ml-4.1.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:34:41.000000 biobb_ml-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5937 2023-09-08 08:44:16.410117 biobb_ml-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5125 2023-09-08 08:43:18.000000 biobb_ml-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.401025 biobb_ml-4.1.0/biobb_ml/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      167 2023-09-08 08:43:04.000000 biobb_ml-4.1.0/biobb_ml/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.402991 biobb_ml-4.1.0/biobb_ml/classification/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      197 2023-04-13 13:36:06.000000 biobb_ml-4.1.0/biobb_ml/classification/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11686 2023-04-13 13:40:15.000000 biobb_ml-4.1.0/biobb_ml/classification/classification_predict.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573    10289 2023-04-13 13:49:25.000000 biobb_ml-4.1.0/biobb_ml/classification/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17780 2023-04-13 13:52:01.000000 biobb_ml-4.1.0/biobb_ml/classification/decision_tree.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17809 2023-04-13 14:01:47.000000 biobb_ml-4.1.0/biobb_ml/classification/k_neighbors.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    14519 2023-04-13 13:57:12.000000 biobb_ml-4.1.0/biobb_ml/classification/k_neighbors_coefficient.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18393 2023-04-13 14:04:43.000000 biobb_ml-4.1.0/biobb_ml/classification/logistic_regression.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17966 2023-04-13 14:07:39.000000 biobb_ml-4.1.0/biobb_ml/classification/random_forest_classifier.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18123 2023-04-13 14:11:02.000000 biobb_ml-4.1.0/biobb_ml/classification/support_vector_machine.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.404280 biobb_ml-4.1.0/biobb_ml/clustering/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      201 2023-04-13 13:36:18.000000 biobb_ml-4.1.0/biobb_ml/clustering/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12105 2023-04-13 14:14:44.000000 biobb_ml-4.1.0/biobb_ml/clustering/agglomerative_clustering.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12287 2023-04-13 14:18:27.000000 biobb_ml-4.1.0/biobb_ml/clustering/agglomerative_coefficient.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10270 2023-04-13 14:21:02.000000 biobb_ml-4.1.0/biobb_ml/clustering/clustering_predict.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573    13035 2023-04-13 14:25:53.000000 biobb_ml-4.1.0/biobb_ml/clustering/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13009 2023-04-13 14:32:49.000000 biobb_ml-4.1.0/biobb_ml/clustering/dbscan.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12058 2023-04-13 14:38:11.000000 biobb_ml-4.1.0/biobb_ml/clustering/k_means.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12347 2023-04-13 14:36:15.000000 biobb_ml-4.1.0/biobb_ml/clustering/k_means_coefficient.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11727 2023-04-13 14:41:12.000000 biobb_ml-4.1.0/biobb_ml/clustering/spectral_clustering.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11152 2023-04-13 14:43:32.000000 biobb_ml-4.1.0/biobb_ml/clustering/spectral_coefficient.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.404877 biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      104 2023-04-13 13:36:26.000000 biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     7981 2023-04-14 13:50:24.000000 biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15828 2023-04-14 13:55:02.000000 biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/pls_components.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11716 2023-04-14 13:57:09.000000 biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/pls_regression.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12413 2023-04-14 14:00:14.000000 biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/principal_component.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.405966 biobb_ml-4.1.0/biobb_ml/neural_networks/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      207 2023-04-13 13:36:52.000000 biobb_ml-4.1.0/biobb_ml/neural_networks/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17700 2023-04-14 10:32:31.000000 biobb_ml-4.1.0/biobb_ml/neural_networks/autoencoder_neural_network.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    23552 2023-04-14 10:32:40.000000 biobb_ml-4.1.0/biobb_ml/neural_networks/classification_neural_network.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573    12742 2023-04-14 09:26:48.000000 biobb_ml-4.1.0/biobb_ml/neural_networks/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10268 2023-04-14 10:00:33.000000 biobb_ml-4.1.0/biobb_ml/neural_networks/neural_network_decode.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11833 2023-04-14 09:47:29.000000 biobb_ml-4.1.0/biobb_ml/neural_networks/neural_network_predict.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18076 2023-04-14 10:32:51.000000 biobb_ml-4.1.0/biobb_ml/neural_networks/recurrent_neural_network.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    22026 2023-04-14 10:32:57.000000 biobb_ml-4.1.0/biobb_ml/neural_networks/regression_neural_network.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.406907 biobb_ml-4.1.0/biobb_ml/regression/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      126 2023-04-13 13:37:06.000000 biobb_ml-4.1.0/biobb_ml/regression/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6076 2023-04-14 10:36:50.000000 biobb_ml-4.1.0/biobb_ml/regression/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16697 2023-04-14 10:40:11.000000 biobb_ml-4.1.0/biobb_ml/regression/linear_regression.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16670 2023-04-14 10:43:10.000000 biobb_ml-4.1.0/biobb_ml/regression/polynomial_regression.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16717 2023-04-14 10:46:32.000000 biobb_ml-4.1.0/biobb_ml/regression/random_forest_regressor.py
--rw-rw-r--   0 gbayarri (1147421021) 1791188573     6870 2021-11-02 17:24:05.000000 biobb_ml-4.1.0/biobb_ml/regression/regression_binding_predict.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10949 2023-04-14 10:48:34.000000 biobb_ml-4.1.0/biobb_ml/regression/regression_predict.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.407935 biobb_ml-4.1.0/biobb_ml/resampling/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       78 2023-04-13 13:37:16.000000 biobb_ml-4.1.0/biobb_ml/resampling/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     8221 2023-04-14 10:51:16.000000 biobb_ml-4.1.0/biobb_ml/resampling/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18986 2023-04-14 10:55:25.000000 biobb_ml-4.1.0/biobb_ml/resampling/oversampling.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5032 2023-04-14 10:57:15.000000 biobb_ml-4.1.0/biobb_ml/resampling/reg_resampler.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17988 2023-04-14 11:01:00.000000 biobb_ml-4.1.0/biobb_ml/resampling/resampling.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    20980 2023-04-14 11:04:38.000000 biobb_ml-4.1.0/biobb_ml/resampling/undersampling.py
--rw-rw-r--   0 gbayarri (1147421021) 1791188573     7132 2021-11-02 17:24:05.000000 biobb_ml-4.1.0/biobb_ml/resampling/undersampling_binding.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.408059 biobb_ml-4.1.0/biobb_ml/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:34:41.000000 biobb_ml-4.1.0/biobb_ml/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.409925 biobb_ml-4.1.0/biobb_ml/utils/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      154 2023-04-13 13:37:29.000000 biobb_ml-4.1.0/biobb_ml/utils/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4138 2023-04-14 11:06:17.000000 biobb_ml-4.1.0/biobb_ml/utils/common.py
--rw-rw-r--   0 gbayarri (1147421021) 1791188573     6117 2021-11-02 17:24:05.000000 biobb_ml-4.1.0/biobb_ml/utils/confusion_matrix.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7518 2023-04-14 11:08:20.000000 biobb_ml-4.1.0/biobb_ml/utils/correlation_matrix.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6749 2023-04-14 11:09:51.000000 biobb_ml-4.1.0/biobb_ml/utils/dendrogram.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6900 2023-04-14 11:11:30.000000 biobb_ml-4.1.0/biobb_ml/utils/drop_columns.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7139 2023-04-14 13:28:19.000000 biobb_ml-4.1.0/biobb_ml/utils/dummy_variables.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7368 2023-04-14 13:30:06.000000 biobb_ml-4.1.0/biobb_ml/utils/map_variables.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7466 2023-04-14 13:31:38.000000 biobb_ml-4.1.0/biobb_ml/utils/pairwise_comparison.py
--rw-rw-r--   0 gbayarri (1147421021) 1791188573    13854 2021-11-02 17:24:05.000000 biobb_ml-4.1.0/biobb_ml/utils/protein_dna_binding.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7179 2023-04-14 13:33:13.000000 biobb_ml-4.1.0/biobb_ml/utils/scale_columns.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-08 08:44:16.401772 biobb_ml-4.1.0/biobb_ml.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5937 2023-09-08 08:44:16.000000 biobb_ml-4.1.0/biobb_ml.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2599 2023-09-08 08:44:16.000000 biobb_ml-4.1.0/biobb_ml.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-09-08 08:44:16.000000 biobb_ml-4.1.0/biobb_ml.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2545 2023-09-08 08:44:16.000000 biobb_ml-4.1.0/biobb_ml.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      126 2023-09-08 08:44:16.000000 biobb_ml-4.1.0/biobb_ml.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2023-09-08 08:44:16.000000 biobb_ml-4.1.0/biobb_ml.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-09-08 08:44:16.410330 biobb_ml-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     4416 2023-09-08 08:42:55.000000 biobb_ml-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.105349 biobb_ml-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:34:41.000000 biobb_ml-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6707 2024-05-24 11:29:02.105093 biobb_ml-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5664 2024-05-24 11:28:18.000000 biobb_ml-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.095552 biobb_ml-4.2.0/biobb_ml/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      167 2024-05-24 11:28:09.000000 biobb_ml-4.2.0/biobb_ml/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.097821 biobb_ml-4.2.0/biobb_ml/classification/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      197 2023-04-13 13:36:06.000000 biobb_ml-4.2.0/biobb_ml/classification/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11686 2023-04-13 13:40:15.000000 biobb_ml-4.2.0/biobb_ml/classification/classification_predict.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    10289 2023-04-13 13:49:25.000000 biobb_ml-4.2.0/biobb_ml/classification/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17780 2023-04-13 13:52:01.000000 biobb_ml-4.2.0/biobb_ml/classification/decision_tree.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17809 2023-04-13 14:01:47.000000 biobb_ml-4.2.0/biobb_ml/classification/k_neighbors.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    14519 2023-04-13 13:57:12.000000 biobb_ml-4.2.0/biobb_ml/classification/k_neighbors_coefficient.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18393 2023-04-13 14:04:43.000000 biobb_ml-4.2.0/biobb_ml/classification/logistic_regression.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17966 2023-04-13 14:07:39.000000 biobb_ml-4.2.0/biobb_ml/classification/random_forest_classifier.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18123 2023-04-13 14:11:02.000000 biobb_ml-4.2.0/biobb_ml/classification/support_vector_machine.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.099177 biobb_ml-4.2.0/biobb_ml/clustering/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      201 2023-04-13 13:36:18.000000 biobb_ml-4.2.0/biobb_ml/clustering/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12105 2023-04-13 14:14:44.000000 biobb_ml-4.2.0/biobb_ml/clustering/agglomerative_clustering.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12287 2023-04-13 14:18:27.000000 biobb_ml-4.2.0/biobb_ml/clustering/agglomerative_coefficient.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10270 2023-04-13 14:21:02.000000 biobb_ml-4.2.0/biobb_ml/clustering/clustering_predict.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    13035 2023-04-13 14:25:53.000000 biobb_ml-4.2.0/biobb_ml/clustering/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13009 2023-04-13 14:32:49.000000 biobb_ml-4.2.0/biobb_ml/clustering/dbscan.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12058 2023-04-13 14:38:11.000000 biobb_ml-4.2.0/biobb_ml/clustering/k_means.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12347 2023-04-13 14:36:15.000000 biobb_ml-4.2.0/biobb_ml/clustering/k_means_coefficient.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11727 2023-04-13 14:41:12.000000 biobb_ml-4.2.0/biobb_ml/clustering/spectral_clustering.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11152 2023-04-13 14:43:32.000000 biobb_ml-4.2.0/biobb_ml/clustering/spectral_coefficient.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.099789 biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      104 2023-04-13 13:36:26.000000 biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     7981 2023-04-14 13:50:24.000000 biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15828 2023-04-14 13:55:02.000000 biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/pls_components.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11716 2023-04-14 13:57:09.000000 biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/pls_regression.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12413 2023-04-14 14:00:14.000000 biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/principal_component.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.100813 biobb_ml-4.2.0/biobb_ml/neural_networks/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      207 2023-04-13 13:36:52.000000 biobb_ml-4.2.0/biobb_ml/neural_networks/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17700 2023-04-14 10:32:31.000000 biobb_ml-4.2.0/biobb_ml/neural_networks/autoencoder_neural_network.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    23552 2023-04-14 10:32:40.000000 biobb_ml-4.2.0/biobb_ml/neural_networks/classification_neural_network.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    12742 2023-04-14 09:26:48.000000 biobb_ml-4.2.0/biobb_ml/neural_networks/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10268 2023-04-14 10:00:33.000000 biobb_ml-4.2.0/biobb_ml/neural_networks/neural_network_decode.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11833 2023-04-14 09:47:29.000000 biobb_ml-4.2.0/biobb_ml/neural_networks/neural_network_predict.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18076 2023-04-14 10:32:51.000000 biobb_ml-4.2.0/biobb_ml/neural_networks/recurrent_neural_network.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    22026 2023-04-14 10:32:57.000000 biobb_ml-4.2.0/biobb_ml/neural_networks/regression_neural_network.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.101812 biobb_ml-4.2.0/biobb_ml/regression/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573      126 2023-04-13 13:37:06.000000 biobb_ml-4.2.0/biobb_ml/regression/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6076 2023-04-14 10:36:50.000000 biobb_ml-4.2.0/biobb_ml/regression/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16697 2023-04-14 10:40:11.000000 biobb_ml-4.2.0/biobb_ml/regression/linear_regression.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16670 2023-04-14 10:43:10.000000 biobb_ml-4.2.0/biobb_ml/regression/polynomial_regression.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16717 2023-04-14 10:46:32.000000 biobb_ml-4.2.0/biobb_ml/regression/random_forest_regressor.py
+-rw-rw-r--   0 gbayarri (1147421021) 1791188573     6870 2021-11-02 17:24:05.000000 biobb_ml-4.2.0/biobb_ml/regression/regression_binding_predict.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10949 2023-04-14 10:48:34.000000 biobb_ml-4.2.0/biobb_ml/regression/regression_predict.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.102735 biobb_ml-4.2.0/biobb_ml/resampling/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       78 2023-04-13 13:37:16.000000 biobb_ml-4.2.0/biobb_ml/resampling/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     8221 2023-04-14 10:51:16.000000 biobb_ml-4.2.0/biobb_ml/resampling/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18986 2023-04-14 10:55:25.000000 biobb_ml-4.2.0/biobb_ml/resampling/oversampling.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5032 2023-04-14 10:57:15.000000 biobb_ml-4.2.0/biobb_ml/resampling/reg_resampler.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17988 2023-04-14 11:01:00.000000 biobb_ml-4.2.0/biobb_ml/resampling/resampling.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    20980 2023-04-14 11:04:38.000000 biobb_ml-4.2.0/biobb_ml/resampling/undersampling.py
+-rw-rw-r--   0 gbayarri (1147421021) 1791188573     7132 2021-11-02 17:24:05.000000 biobb_ml-4.2.0/biobb_ml/resampling/undersampling_binding.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.102890 biobb_ml-4.2.0/biobb_ml/test/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:34:41.000000 biobb_ml-4.2.0/biobb_ml/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.104752 biobb_ml-4.2.0/biobb_ml/utils/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      154 2023-04-13 13:37:29.000000 biobb_ml-4.2.0/biobb_ml/utils/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     4138 2023-04-14 11:06:17.000000 biobb_ml-4.2.0/biobb_ml/utils/common.py
+-rw-rw-r--   0 gbayarri (1147421021) 1791188573     6117 2021-11-02 17:24:05.000000 biobb_ml-4.2.0/biobb_ml/utils/confusion_matrix.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7518 2023-04-14 11:08:20.000000 biobb_ml-4.2.0/biobb_ml/utils/correlation_matrix.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6749 2023-04-14 11:09:51.000000 biobb_ml-4.2.0/biobb_ml/utils/dendrogram.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6900 2023-04-14 11:11:30.000000 biobb_ml-4.2.0/biobb_ml/utils/drop_columns.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7139 2023-04-14 13:28:19.000000 biobb_ml-4.2.0/biobb_ml/utils/dummy_variables.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7368 2023-04-14 13:30:06.000000 biobb_ml-4.2.0/biobb_ml/utils/map_variables.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7466 2023-04-14 13:31:38.000000 biobb_ml-4.2.0/biobb_ml/utils/pairwise_comparison.py
+-rw-rw-r--   0 gbayarri (1147421021) 1791188573    13854 2021-11-02 17:24:05.000000 biobb_ml-4.2.0/biobb_ml/utils/protein_dna_binding.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7179 2023-04-14 13:33:13.000000 biobb_ml-4.2.0/biobb_ml/utils/scale_columns.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 11:29:02.096508 biobb_ml-4.2.0/biobb_ml.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6707 2024-05-24 11:29:02.000000 biobb_ml-4.2.0/biobb_ml.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2599 2024-05-24 11:29:02.000000 biobb_ml-4.2.0/biobb_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 11:29:02.000000 biobb_ml-4.2.0/biobb_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2545 2024-05-24 11:29:02.000000 biobb_ml-4.2.0/biobb_ml.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      126 2024-05-24 11:29:02.000000 biobb_ml-4.2.0/biobb_ml.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2024-05-24 11:29:02.000000 biobb_ml-4.2.0/biobb_ml.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 11:29:02.105399 biobb_ml-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     4416 2024-05-24 11:28:01.000000 biobb_ml-4.2.0/setup.py
```

### Comparing `biobb_ml-4.1.0/LICENSE` & `biobb_ml-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/PKG-INFO` & `biobb_ml-4.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: biobb_ml
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_ml is the Biobb module collection to perform machine learning predictions.
 Home-page: https://github.com/bioexcel/biobb_ml
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
-Project-URL: Documentation, http://biobb_ml.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-ml.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
+Requires-Dist: scikit-learn==0.24.2
+Requires-Dist: pandas>=1.3.0
+Requires-Dist: seaborn==0.10.1
+Requires-Dist: tensorflow>=2.4.2
+Requires-Dist: h5py==2.10.0
+Requires-Dist: imbalanced-learn==0.7.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_ml?label=Version)](https://GitHub.com/bioexcel/biobb_ml/tags/)
 [![](https://img.shields.io/pypi/v/biobb-ml.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-ml/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_ml?label=Conda)](https://anaconda.org/bioconda/biobb_ml)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_ml?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_ml)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_ml?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_ml:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_ml:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_ml)
 [![](https://img.shields.io/pypi/pyversions/biobb-ml.svg?label=Python%20Versions)](https://pypi.org/project/biobb-ml/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_ml)
 
 [![](https://readthedocs.org/projects/biobb-ml/badge/?version=latest&label=Docs)](https://biobb-ml.readthedocs.io/en/latest/?badge=latest)
@@ -38,85 +45,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_ml/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_ml/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_ml/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_ml/coverage/)
 [![](https://docs.bioexcel.eu/biobb_ml/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_ml/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_ml?label=Last%20Commit)](https://github.com/bioexcel/biobb_ml/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_ml.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_ml/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_ml
 
 ### Introduction
 Biobb_ml is the Biobb module collection to perform machine learning predictions.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_ml.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-ml.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_ml>=4.1.0"
+        pip install "biobb_ml>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-ml.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_ml>=4.1.0"
+        conda install -c bioconda "biobb_ml>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-ml.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-ml.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_ml:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_ml:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_ml:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_ml:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_ml.sif https://depot.galaxyproject.org/singularity/biobb_ml:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_ml.sif https://depot.galaxyproject.org/singularity/biobb_ml:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_ml.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-ml.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_ml-4.1.0/README.md` & `biobb_ml-4.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_ml?label=Version)](https://GitHub.com/bioexcel/biobb_ml/tags/)
 [![](https://img.shields.io/pypi/v/biobb-ml.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-ml/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_ml?label=Conda)](https://anaconda.org/bioconda/biobb_ml)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_ml?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_ml)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_ml?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_ml:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_ml:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_ml)
 [![](https://img.shields.io/pypi/pyversions/biobb-ml.svg?label=Python%20Versions)](https://pypi.org/project/biobb-ml/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_ml)
 
 [![](https://readthedocs.org/projects/biobb-ml/badge/?version=latest&label=Docs)](https://biobb-ml.readthedocs.io/en/latest/?badge=latest)
@@ -18,85 +18,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_ml/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_ml/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_ml/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_ml/coverage/)
 [![](https://docs.bioexcel.eu/biobb_ml/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_ml/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_ml?label=Last%20Commit)](https://github.com/bioexcel/biobb_ml/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_ml.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_ml/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_ml
 
 ### Introduction
 Biobb_ml is the Biobb module collection to perform machine learning predictions.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_ml.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-ml.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_ml>=4.1.0"
+        pip install "biobb_ml>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-ml.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_ml>=4.1.0"
+        conda install -c bioconda "biobb_ml>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-ml.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-ml.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_ml:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_ml:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_ml:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_ml:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_ml.sif https://depot.galaxyproject.org/singularity/biobb_ml:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_ml.sif https://depot.galaxyproject.org/singularity/biobb_ml:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_ml.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-ml.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_ml-4.1.0/biobb_ml/classification/classification_predict.py` & `biobb_ml-4.2.0/biobb_ml/classification/classification_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/classification/common.py` & `biobb_ml-4.2.0/biobb_ml/classification/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/classification/decision_tree.py` & `biobb_ml-4.2.0/biobb_ml/classification/decision_tree.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/classification/k_neighbors.py` & `biobb_ml-4.2.0/biobb_ml/classification/k_neighbors.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/classification/k_neighbors_coefficient.py` & `biobb_ml-4.2.0/biobb_ml/classification/k_neighbors_coefficient.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/classification/logistic_regression.py` & `biobb_ml-4.2.0/biobb_ml/classification/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/classification/random_forest_classifier.py` & `biobb_ml-4.2.0/biobb_ml/classification/random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/classification/support_vector_machine.py` & `biobb_ml-4.2.0/biobb_ml/classification/support_vector_machine.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/agglomerative_clustering.py` & `biobb_ml-4.2.0/biobb_ml/clustering/agglomerative_clustering.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/agglomerative_coefficient.py` & `biobb_ml-4.2.0/biobb_ml/clustering/agglomerative_coefficient.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/clustering_predict.py` & `biobb_ml-4.2.0/biobb_ml/clustering/clustering_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/common.py` & `biobb_ml-4.2.0/biobb_ml/clustering/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/dbscan.py` & `biobb_ml-4.2.0/biobb_ml/clustering/dbscan.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/k_means.py` & `biobb_ml-4.2.0/biobb_ml/clustering/k_means.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/k_means_coefficient.py` & `biobb_ml-4.2.0/biobb_ml/clustering/k_means_coefficient.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/spectral_clustering.py` & `biobb_ml-4.2.0/biobb_ml/clustering/spectral_clustering.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/clustering/spectral_coefficient.py` & `biobb_ml-4.2.0/biobb_ml/clustering/spectral_coefficient.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/common.py` & `biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/pls_components.py` & `biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/pls_components.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/pls_regression.py` & `biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/pls_regression.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/dimensionality_reduction/principal_component.py` & `biobb_ml-4.2.0/biobb_ml/dimensionality_reduction/principal_component.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/neural_networks/autoencoder_neural_network.py` & `biobb_ml-4.2.0/biobb_ml/neural_networks/autoencoder_neural_network.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/neural_networks/classification_neural_network.py` & `biobb_ml-4.2.0/biobb_ml/neural_networks/classification_neural_network.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/neural_networks/common.py` & `biobb_ml-4.2.0/biobb_ml/neural_networks/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/neural_networks/neural_network_decode.py` & `biobb_ml-4.2.0/biobb_ml/neural_networks/neural_network_decode.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/neural_networks/neural_network_predict.py` & `biobb_ml-4.2.0/biobb_ml/neural_networks/neural_network_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/neural_networks/recurrent_neural_network.py` & `biobb_ml-4.2.0/biobb_ml/neural_networks/recurrent_neural_network.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/neural_networks/regression_neural_network.py` & `biobb_ml-4.2.0/biobb_ml/neural_networks/regression_neural_network.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/regression/common.py` & `biobb_ml-4.2.0/biobb_ml/regression/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/regression/linear_regression.py` & `biobb_ml-4.2.0/biobb_ml/regression/linear_regression.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/regression/polynomial_regression.py` & `biobb_ml-4.2.0/biobb_ml/regression/polynomial_regression.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/regression/random_forest_regressor.py` & `biobb_ml-4.2.0/biobb_ml/regression/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/regression/regression_binding_predict.py` & `biobb_ml-4.2.0/biobb_ml/regression/regression_binding_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/regression/regression_predict.py` & `biobb_ml-4.2.0/biobb_ml/regression/regression_predict.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/resampling/common.py` & `biobb_ml-4.2.0/biobb_ml/resampling/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/resampling/oversampling.py` & `biobb_ml-4.2.0/biobb_ml/resampling/oversampling.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/resampling/reg_resampler.py` & `biobb_ml-4.2.0/biobb_ml/resampling/reg_resampler.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/resampling/resampling.py` & `biobb_ml-4.2.0/biobb_ml/resampling/resampling.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/resampling/undersampling.py` & `biobb_ml-4.2.0/biobb_ml/resampling/undersampling.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/resampling/undersampling_binding.py` & `biobb_ml-4.2.0/biobb_ml/resampling/undersampling_binding.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/common.py` & `biobb_ml-4.2.0/biobb_ml/utils/common.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/confusion_matrix.py` & `biobb_ml-4.2.0/biobb_ml/utils/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/correlation_matrix.py` & `biobb_ml-4.2.0/biobb_ml/utils/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/dendrogram.py` & `biobb_ml-4.2.0/biobb_ml/utils/dendrogram.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/drop_columns.py` & `biobb_ml-4.2.0/biobb_ml/utils/drop_columns.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/dummy_variables.py` & `biobb_ml-4.2.0/biobb_ml/utils/dummy_variables.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/map_variables.py` & `biobb_ml-4.2.0/biobb_ml/utils/map_variables.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/pairwise_comparison.py` & `biobb_ml-4.2.0/biobb_ml/utils/pairwise_comparison.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/protein_dna_binding.py` & `biobb_ml-4.2.0/biobb_ml/utils/protein_dna_binding.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml/utils/scale_columns.py` & `biobb_ml-4.2.0/biobb_ml/utils/scale_columns.py`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml.egg-info/PKG-INFO` & `biobb_ml-4.2.0/biobb_ml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 Metadata-Version: 2.1
 Name: biobb-ml
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_ml is the Biobb module collection to perform machine learning predictions.
 Home-page: https://github.com/bioexcel/biobb_ml
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
-Project-URL: Documentation, http://biobb_ml.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-ml.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
+Requires-Dist: scikit-learn==0.24.2
+Requires-Dist: pandas>=1.3.0
+Requires-Dist: seaborn==0.10.1
+Requires-Dist: tensorflow>=2.4.2
+Requires-Dist: h5py==2.10.0
+Requires-Dist: imbalanced-learn==0.7.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_ml?label=Version)](https://GitHub.com/bioexcel/biobb_ml/tags/)
 [![](https://img.shields.io/pypi/v/biobb-ml.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-ml/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_ml?label=Conda)](https://anaconda.org/bioconda/biobb_ml)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_ml?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_ml)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_ml?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_ml:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_ml:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_ml)
 [![](https://img.shields.io/pypi/pyversions/biobb-ml.svg?label=Python%20Versions)](https://pypi.org/project/biobb-ml/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_ml)
 
 [![](https://readthedocs.org/projects/biobb-ml/badge/?version=latest&label=Docs)](https://biobb-ml.readthedocs.io/en/latest/?badge=latest)
@@ -38,85 +45,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_ml/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_ml/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_ml/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_ml/coverage/)
 [![](https://docs.bioexcel.eu/biobb_ml/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_ml/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_ml?label=Last%20Commit)](https://github.com/bioexcel/biobb_ml/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_ml.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_ml/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_ml
 
 ### Introduction
 Biobb_ml is the Biobb module collection to perform machine learning predictions.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_ml.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-ml.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_ml>=4.1.0"
+        pip install "biobb_ml>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-ml.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_ml>=4.1.0"
+        conda install -c bioconda "biobb_ml>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-ml.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-ml.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_ml:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_ml:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_ml:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_ml:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_ml.sif https://depot.galaxyproject.org/singularity/biobb_ml:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_ml.sif https://depot.galaxyproject.org/singularity/biobb_ml:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_ml.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-ml.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_ml-4.1.0/biobb_ml.egg-info/SOURCES.txt` & `biobb_ml-4.2.0/biobb_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/biobb_ml.egg-info/entry_points.txt` & `biobb_ml-4.2.0/biobb_ml.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_ml-4.1.0/setup.py` & `biobb_ml-4.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_ml",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_ml is the Biobb module collection to perform machine learning predictions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_ml",
     project_urls={
-        "Documentation": "http://biobb_ml.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-ml.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0', 'scikit-learn ==0.24.2', 'pandas >=1.3.0', 'seaborn ==0.10.1', 'tensorflow>=2.4.2', 'h5py ==2.10.0', 'imbalanced-learn ==0.7.0'],
+    install_requires=['biobb_common==4.2.0', 'scikit-learn ==0.24.2', 'pandas >=1.3.0', 'seaborn ==0.10.1', 'tensorflow>=2.4.2', 'h5py ==2.10.0', 'imbalanced-learn ==0.7.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "classification_predict = biobb_ml.classification.classification_predict:main",
             "decision_tree = biobb_ml.classification.decision_tree:main",
             "k_neighbors_coefficient = biobb_ml.classification.k_neighbors_coefficient:main",
             "k_neighbors = biobb_ml.classification.k_neighbors:main",
```

