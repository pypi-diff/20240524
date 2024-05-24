# Comparing `tmp/eis_toolkit-0.5.1.tar.gz` & `tmp/eis_toolkit-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis_toolkit-0.5.1.tar", max compression
+gzip compressed data, was "eis_toolkit-0.5.2.tar", max compression
```

## Comparing `eis_toolkit-0.5.1.tar` & `eis_toolkit-0.5.2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rwxr-xr-x   0        0        0    13827 2024-03-04 07:36:07.783856 eis_toolkit-0.5.1/LICENSE
--rwxr-xr-x   0        0        0     5864 2024-05-13 10:15:39.840704 eis_toolkit-0.5.1/README.md
--rwxr-xr-x   0        0        0       22 2024-02-12 07:36:47.840362 eis_toolkit-0.5.1/eis_toolkit/__init__.py
--rw-r--r--   0        0        0       70 2024-04-04 09:16:19.591131 eis_toolkit-0.5.1/eis_toolkit/__main__.py
--rw-r--r--   0        0        0   115903 2024-05-21 06:37:53.189336 eis_toolkit-0.5.1/eis_toolkit/cli.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/conversions/__init__.py
--rw-r--r--   0        0        0     3840 2024-02-22 09:12:29.156927 eis_toolkit-0.5.1/eis_toolkit/conversions/csv_to_geodataframe.py
--rw-r--r--   0        0        0     2691 2024-04-24 11:26:52.059104 eis_toolkit-0.5.1/eis_toolkit/conversions/raster_to_dataframe.py
--rwxr-xr-x   0        0        0        0 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/__init__.py
--rw-r--r--   0        0        0     4577 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/calculate_base_metrics.py
--rw-r--r--   0        0        0     1233 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/classification_label_evaluation.py
--rw-r--r--   0        0        0     7051 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/classification_probability_evaluation.py
--rw-r--r--   0        0        0     2153 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_confusion_matrix.py
--rw-r--r--   0        0        0     2644 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_nn_model_performance.py
--rw-r--r--   0        0        0     3829 2024-04-25 10:25:47.561371 eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_prediction_area_curves.py
--rw-r--r--   0        0        0     2003 2024-04-25 10:25:47.565371 eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_rate_curve.py
--rw-r--r--   0        0        0     2587 2024-04-25 10:25:47.565371 eis_toolkit-0.5.1/eis_toolkit/evaluation/scoring.py
--rw-r--r--   0        0        0     2739 2024-05-21 06:37:53.189336 eis_toolkit-0.5.1/eis_toolkit/exceptions.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/__init__.py
--rw-r--r--   0        0        0      286 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/basic_plots_seaborn.py
--rw-r--r--   0        0        0     2302 2024-03-06 08:47:28.563567 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/chi_square_test.py
--rw-r--r--   0        0        0     4015 2024-04-15 11:24:32.422063 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/correlation_matrix.py
--rw-r--r--   0        0        0     2416 2024-03-06 08:47:28.563567 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/covariance_matrix.py
--rw-r--r--   0        0        0     6937 2024-04-15 11:24:32.422063 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/dbscan.py
--rw-r--r--   0        0        0     2627 2024-04-02 08:33:51.299185 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/descriptive_statistics.py
--rw-r--r--   0        0        0     2030 2024-03-04 09:08:14.566054 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/feature_importance.py
--rw-r--r--   0        0        0     6361 2024-04-15 11:24:32.422063 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/k_means_cluster.py
--rw-r--r--   0        0        0     2602 2024-03-04 07:36:07.783856 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/local_morans_i.py
--rw-r--r--   0        0        0     4981 2024-03-06 08:47:28.563567 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/normality_test.py
--rw-r--r--   0        0        0     7540 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/parallel_coordinates.py
--rw-r--r--   0        0        0    11017 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/pca.py
--rw-r--r--   0        0        0      445 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/plot_utils.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/prediction/__init__.py
--rw-r--r--   0        0        0     5350 2024-04-30 08:53:14.418579 eis_toolkit-0.5.1/eis_toolkit/prediction/fuzzy_overlay.py
--rw-r--r--   0        0        0    10930 2024-03-12 10:30:37.976282 eis_toolkit-0.5.1/eis_toolkit/prediction/gradient_boosting.py
--rw-r--r--   0        0        0     4424 2024-03-12 10:30:37.976282 eis_toolkit-0.5.1/eis_toolkit/prediction/logistic_regression.py
--rw-r--r--   0        0        0    16273 2024-05-20 10:32:28.957217 eis_toolkit-0.5.1/eis_toolkit/prediction/machine_learning_general.py
--rw-r--r--   0        0        0     3251 2024-05-21 06:37:53.189336 eis_toolkit-0.5.1/eis_toolkit/prediction/machine_learning_predict.py
--rw-r--r--   0        0        0    13658 2024-03-12 10:30:37.976282 eis_toolkit-0.5.1/eis_toolkit/prediction/mlp.py
--rw-r--r--   0        0        0     8686 2024-04-03 07:14:14.999244 eis_toolkit-0.5.1/eis_toolkit/prediction/random_forests.py
--rw-r--r--   0        0        0    17390 2024-04-24 15:28:57.740112 eis_toolkit-0.5.1/eis_toolkit/prediction/weights_of_evidence.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/raster_processing/__init__.py
--rwxr-xr-x   0        0        0     2042 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/clipping.py
--rw-r--r--   0        0        0     6940 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/create_constant_raster.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/__init__.py
--rw-r--r--   0        0        0     4355 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/classification.py
--rw-r--r--   0        0        0     9871 2024-04-03 09:12:33.201055 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/parameters.py
--rw-r--r--   0        0        0     6922 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/partial_derivatives.py
--rw-r--r--   0        0        0     1435 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/utilities.py
--rw-r--r--   0        0        0    10388 2024-04-29 09:13:31.923148 eis_toolkit-0.5.1/eis_toolkit/raster_processing/distance_to_anomaly.py
--rw-r--r--   0        0        0     2931 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/extract_values_from_raster.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/__init__.py
--rw-r--r--   0        0        0     5820 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/focal.py
--rw-r--r--   0        0        0     3521 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/kernels.py
--rw-r--r--   0        0        0    17984 2024-03-06 08:46:24.150688 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/speckle.py
--rw-r--r--   0        0        0     3656 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/utilities.py
--rw-r--r--   0        0        0    15084 2024-03-04 07:36:07.787855 eis_toolkit-0.5.1/eis_toolkit/raster_processing/reclassify.py
--rw-r--r--   0        0        0     2573 2024-04-03 09:32:00.769041 eis_toolkit-0.5.1/eis_toolkit/raster_processing/reprojecting.py
--rw-r--r--   0        0        0     2745 2024-04-03 09:32:00.769041 eis_toolkit-0.5.1/eis_toolkit/raster_processing/resampling.py
--rw-r--r--   0        0        0     4343 2024-04-03 09:01:39.672155 eis_toolkit-0.5.1/eis_toolkit/raster_processing/snapping.py
--rw-r--r--   0        0        0     4834 2024-04-03 09:32:00.769041 eis_toolkit-0.5.1/eis_toolkit/raster_processing/unifying.py
--rw-r--r--   0        0        0     2050 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/raster_processing/unique_combinations.py
--rw-r--r--   0        0        0     3390 2023-11-10 08:05:31.345266 eis_toolkit-0.5.1/eis_toolkit/raster_processing/windowing.py
--rw-r--r--   0        0        0        0 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/training_data_tools/__init__.py
--rw-r--r--   0        0        0     1840 2024-02-22 09:12:29.160927 eis_toolkit-0.5.1/eis_toolkit/training_data_tools/class_balancing.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/transformations/__init__.py
--rw-r--r--   0        0        0     3639 2024-04-08 06:45:40.454759 eis_toolkit-0.5.1/eis_toolkit/transformations/binarize.py
--rw-r--r--   0        0        0     4696 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/clip.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/__init__.py
--rw-r--r--   0        0        0     3054 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/alr.py
--rw-r--r--   0        0        0     2338 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/clr.py
--rw-r--r--   0        0        0     3628 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/ilr.py
--rw-r--r--   0        0        0     2504 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/pairwise.py
--rw-r--r--   0        0        0     4136 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/coda/plr.py
--rw-r--r--   0        0        0     7699 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/linear.py
--rw-r--r--   0        0        0     4883 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/logarithmic.py
--rw-r--r--   0        0        0     5205 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/one_hot_encoding.py
--rw-r--r--   0        0        0     5163 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/transformations/sigmoid.py
--rw-r--r--   0        0        0     6767 2024-04-08 08:42:37.268163 eis_toolkit-0.5.1/eis_toolkit/transformations/winsorize.py
--rw-r--r--   0        0        0        0 2023-12-06 09:22:12.535287 eis_toolkit-0.5.1/eis_toolkit/utilities/__init__.py
--rw-r--r--   0        0        0     1107 2024-04-05 07:27:18.360688 eis_toolkit-0.5.1/eis_toolkit/utilities/aitchison_geometry.py
--rwxr-xr-x   0        0        0        0 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-05 07:27:18.360688 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/compositional.py
--rw-r--r--   0        0        0     1672 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/dataframe.py
--rwxr-xr-x   0        0        0      599 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/geometry.py
--rw-r--r--   0        0        0     2353 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/parameter.py
--rw-r--r--   0        0        0     5837 2024-04-03 09:32:00.769041 eis_toolkit-0.5.1/eis_toolkit/utilities/checks/raster.py
--rw-r--r--   0        0        0     1467 2024-02-22 09:12:29.164927 eis_toolkit-0.5.1/eis_toolkit/utilities/conversions.py
--rw-r--r--   0        0        0     8640 2024-05-03 06:58:41.674662 eis_toolkit-0.5.1/eis_toolkit/utilities/file_io.py
--rw-r--r--   0        0        0    12203 2024-04-24 06:18:14.118407 eis_toolkit-0.5.1/eis_toolkit/utilities/miscellaneous.py
--rw-r--r--   0        0        0     4947 2024-04-24 06:18:14.118407 eis_toolkit-0.5.1/eis_toolkit/utilities/nodata.py
--rw-r--r--   0        0        0     6041 2024-04-24 11:26:53.983156 eis_toolkit-0.5.1/eis_toolkit/utilities/raster.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.1/eis_toolkit/vector_processing/__init__.py
--rw-r--r--   0        0        0     1098 2024-02-22 09:12:29.168927 eis_toolkit-0.5.1/eis_toolkit/vector_processing/calculate_geometry.py
--rw-r--r--   0        0        0    22658 2024-02-22 09:12:29.168927 eis_toolkit-0.5.1/eis_toolkit/vector_processing/cell_based_association.py
--rw-r--r--   0        0        0     3240 2024-05-02 10:42:43.425579 eis_toolkit-0.5.1/eis_toolkit/vector_processing/distance_computation.py
--rw-r--r--   0        0        0     1942 2024-02-22 09:12:29.168927 eis_toolkit-0.5.1/eis_toolkit/vector_processing/extract_shared_lines.py
--rw-r--r--   0        0        0     3747 2024-04-25 15:11:32.909910 eis_toolkit-0.5.1/eis_toolkit/vector_processing/idw_interpolation.py
--rw-r--r--   0        0        0     4092 2024-04-24 11:26:53.983156 eis_toolkit-0.5.1/eis_toolkit/vector_processing/kriging_interpolation.py
--rw-r--r--   0        0        0     4827 2024-04-24 14:32:11.183266 eis_toolkit-0.5.1/eis_toolkit/vector_processing/rasterize_vector.py
--rw-r--r--   0        0        0      703 2023-11-10 08:05:31.345266 eis_toolkit-0.5.1/eis_toolkit/vector_processing/reproject_vector.py
--rw-r--r--   0        0        0     1523 2024-04-24 14:32:41.807458 eis_toolkit-0.5.1/eis_toolkit/vector_processing/vector_density.py
--rwxr-xr-x   0        0        0     1778 2024-05-21 06:38:06.857439 eis_toolkit-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 eis_toolkit-0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0    13827 2024-03-04 07:36:07.783856 eis_toolkit-0.5.2/LICENSE
+-rwxr-xr-x   0        0        0     5864 2024-05-13 10:15:39.840704 eis_toolkit-0.5.2/README.md
+-rwxr-xr-x   0        0        0       22 2024-02-12 07:36:47.840362 eis_toolkit-0.5.2/eis_toolkit/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-04 09:16:19.591131 eis_toolkit-0.5.2/eis_toolkit/__main__.py
+-rw-r--r--   0        0        0   116811 2024-05-24 11:29:42.222707 eis_toolkit-0.5.2/eis_toolkit/cli.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/conversions/__init__.py
+-rw-r--r--   0        0        0     3840 2024-02-22 09:12:29.156927 eis_toolkit-0.5.2/eis_toolkit/conversions/csv_to_geodataframe.py
+-rw-r--r--   0        0        0     2691 2024-04-24 11:26:52.059104 eis_toolkit-0.5.2/eis_toolkit/conversions/raster_to_dataframe.py
+-rwxr-xr-x   0        0        0        0 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/__init__.py
+-rw-r--r--   0        0        0     4577 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/calculate_base_metrics.py
+-rw-r--r--   0        0        0     1233 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/classification_label_evaluation.py
+-rw-r--r--   0        0        0     7051 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/classification_probability_evaluation.py
+-rw-r--r--   0        0        0     2153 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_confusion_matrix.py
+-rw-r--r--   0        0        0     2644 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_nn_model_performance.py
+-rw-r--r--   0        0        0     3829 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_prediction_area_curves.py
+-rw-r--r--   0        0        0     2003 2024-04-25 10:25:47.565371 eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_rate_curve.py
+-rw-r--r--   0        0        0     2587 2024-04-25 10:25:47.565371 eis_toolkit-0.5.2/eis_toolkit/evaluation/scoring.py
+-rw-r--r--   0        0        0     2739 2024-05-21 06:37:53.189336 eis_toolkit-0.5.2/eis_toolkit/exceptions.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/__init__.py
+-rw-r--r--   0        0        0      286 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/basic_plots_seaborn.py
+-rw-r--r--   0        0        0     2302 2024-03-06 08:47:28.563567 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/chi_square_test.py
+-rw-r--r--   0        0        0     4015 2024-04-15 11:24:32.422063 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/correlation_matrix.py
+-rw-r--r--   0        0        0     2416 2024-03-06 08:47:28.563567 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/covariance_matrix.py
+-rw-r--r--   0        0        0     6937 2024-04-15 11:24:32.422063 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/dbscan.py
+-rw-r--r--   0        0        0     2627 2024-04-02 08:33:51.299185 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/descriptive_statistics.py
+-rw-r--r--   0        0        0     2030 2024-03-04 09:08:14.566054 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/feature_importance.py
+-rw-r--r--   0        0        0     6361 2024-04-15 11:24:32.422063 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/k_means_cluster.py
+-rw-r--r--   0        0        0     2602 2024-03-04 07:36:07.783856 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/local_morans_i.py
+-rw-r--r--   0        0        0     4981 2024-03-06 08:47:28.563567 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/normality_test.py
+-rw-r--r--   0        0        0     7540 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/parallel_coordinates.py
+-rw-r--r--   0        0        0    11017 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/pca.py
+-rw-r--r--   0        0        0      445 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/plot_utils.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/prediction/__init__.py
+-rw-r--r--   0        0        0     5350 2024-04-30 08:53:14.418579 eis_toolkit-0.5.2/eis_toolkit/prediction/fuzzy_overlay.py
+-rw-r--r--   0        0        0    10930 2024-03-12 10:30:37.976282 eis_toolkit-0.5.2/eis_toolkit/prediction/gradient_boosting.py
+-rw-r--r--   0        0        0     4424 2024-03-12 10:30:37.976282 eis_toolkit-0.5.2/eis_toolkit/prediction/logistic_regression.py
+-rw-r--r--   0        0        0    16273 2024-05-20 10:32:28.957217 eis_toolkit-0.5.2/eis_toolkit/prediction/machine_learning_general.py
+-rw-r--r--   0        0        0     3251 2024-05-21 08:40:59.424283 eis_toolkit-0.5.2/eis_toolkit/prediction/machine_learning_predict.py
+-rw-r--r--   0        0        0    13658 2024-03-12 10:30:37.976282 eis_toolkit-0.5.2/eis_toolkit/prediction/mlp.py
+-rw-r--r--   0        0        0     8686 2024-04-03 07:14:14.999244 eis_toolkit-0.5.2/eis_toolkit/prediction/random_forests.py
+-rw-r--r--   0        0        0    17390 2024-04-24 15:28:57.740112 eis_toolkit-0.5.2/eis_toolkit/prediction/weights_of_evidence.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/raster_processing/__init__.py
+-rwxr-xr-x   0        0        0     2042 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/clipping.py
+-rw-r--r--   0        0        0     6940 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/create_constant_raster.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/__init__.py
+-rw-r--r--   0        0        0     4355 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/classification.py
+-rw-r--r--   0        0        0     9871 2024-04-03 09:12:33.201055 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/parameters.py
+-rw-r--r--   0        0        0     6922 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/partial_derivatives.py
+-rw-r--r--   0        0        0     1435 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/utilities.py
+-rw-r--r--   0        0        0    10388 2024-04-29 09:13:31.923148 eis_toolkit-0.5.2/eis_toolkit/raster_processing/distance_to_anomaly.py
+-rw-r--r--   0        0        0     2931 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/extract_values_from_raster.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/__init__.py
+-rw-r--r--   0        0        0     5820 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/focal.py
+-rw-r--r--   0        0        0     3521 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/kernels.py
+-rw-r--r--   0        0        0    17984 2024-03-06 08:46:24.150688 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/speckle.py
+-rw-r--r--   0        0        0     3656 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/utilities.py
+-rw-r--r--   0        0        0    15084 2024-03-04 07:36:07.787855 eis_toolkit-0.5.2/eis_toolkit/raster_processing/reclassify.py
+-rw-r--r--   0        0        0     2573 2024-04-03 09:32:00.769041 eis_toolkit-0.5.2/eis_toolkit/raster_processing/reprojecting.py
+-rw-r--r--   0        0        0     2745 2024-04-03 09:32:00.769041 eis_toolkit-0.5.2/eis_toolkit/raster_processing/resampling.py
+-rw-r--r--   0        0        0     4343 2024-04-03 09:01:39.672155 eis_toolkit-0.5.2/eis_toolkit/raster_processing/snapping.py
+-rw-r--r--   0        0        0     4834 2024-04-03 09:32:00.769041 eis_toolkit-0.5.2/eis_toolkit/raster_processing/unifying.py
+-rw-r--r--   0        0        0     2050 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/unique_combinations.py
+-rw-r--r--   0        0        0     3390 2023-11-10 08:05:31.345266 eis_toolkit-0.5.2/eis_toolkit/raster_processing/windowing.py
+-rw-r--r--   0        0        0        0 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/training_data_tools/__init__.py
+-rw-r--r--   0        0        0     1840 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/training_data_tools/class_balancing.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/transformations/__init__.py
+-rw-r--r--   0        0        0     3639 2024-04-08 06:45:40.454759 eis_toolkit-0.5.2/eis_toolkit/transformations/binarize.py
+-rw-r--r--   0        0        0     4696 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/clip.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/__init__.py
+-rw-r--r--   0        0        0     3054 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/alr.py
+-rw-r--r--   0        0        0     2338 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/clr.py
+-rw-r--r--   0        0        0     3628 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/ilr.py
+-rw-r--r--   0        0        0     2504 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/pairwise.py
+-rw-r--r--   0        0        0     4136 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/plr.py
+-rw-r--r--   0        0        0     7699 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/linear.py
+-rw-r--r--   0        0        0     4883 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/logarithmic.py
+-rw-r--r--   0        0        0     5205 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/one_hot_encoding.py
+-rw-r--r--   0        0        0     5163 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/sigmoid.py
+-rw-r--r--   0        0        0     6767 2024-04-08 08:42:37.268163 eis_toolkit-0.5.2/eis_toolkit/transformations/winsorize.py
+-rw-r--r--   0        0        0        0 2023-12-06 09:22:12.535287 eis_toolkit-0.5.2/eis_toolkit/utilities/__init__.py
+-rw-r--r--   0        0        0     1107 2024-04-05 07:27:18.360688 eis_toolkit-0.5.2/eis_toolkit/utilities/aitchison_geometry.py
+-rwxr-xr-x   0        0        0        0 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-05 07:27:18.360688 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/compositional.py
+-rw-r--r--   0        0        0     1672 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/dataframe.py
+-rwxr-xr-x   0        0        0      599 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/geometry.py
+-rw-r--r--   0        0        0     2353 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/parameter.py
+-rw-r--r--   0        0        0     5837 2024-04-03 09:32:00.769041 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/raster.py
+-rw-r--r--   0        0        0     1467 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/conversions.py
+-rw-r--r--   0        0        0     8640 2024-05-03 06:58:41.674662 eis_toolkit-0.5.2/eis_toolkit/utilities/file_io.py
+-rw-r--r--   0        0        0    12203 2024-04-24 06:18:14.118407 eis_toolkit-0.5.2/eis_toolkit/utilities/miscellaneous.py
+-rw-r--r--   0        0        0     4947 2024-04-24 06:18:14.118407 eis_toolkit-0.5.2/eis_toolkit/utilities/nodata.py
+-rw-r--r--   0        0        0     6041 2024-04-24 11:26:53.983156 eis_toolkit-0.5.2/eis_toolkit/utilities/raster.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/vector_processing/__init__.py
+-rw-r--r--   0        0        0     1098 2024-02-22 09:12:29.168927 eis_toolkit-0.5.2/eis_toolkit/vector_processing/calculate_geometry.py
+-rw-r--r--   0        0        0    22761 2024-05-24 06:00:52.148295 eis_toolkit-0.5.2/eis_toolkit/vector_processing/cell_based_association.py
+-rw-r--r--   0        0        0     3240 2024-05-02 10:42:43.425579 eis_toolkit-0.5.2/eis_toolkit/vector_processing/distance_computation.py
+-rw-r--r--   0        0        0     1942 2024-02-22 09:12:29.168927 eis_toolkit-0.5.2/eis_toolkit/vector_processing/extract_shared_lines.py
+-rw-r--r--   0        0        0     3747 2024-04-25 15:11:32.909910 eis_toolkit-0.5.2/eis_toolkit/vector_processing/idw_interpolation.py
+-rw-r--r--   0        0        0     4092 2024-04-24 11:26:53.983156 eis_toolkit-0.5.2/eis_toolkit/vector_processing/kriging_interpolation.py
+-rw-r--r--   0        0        0     4827 2024-04-24 14:32:11.183266 eis_toolkit-0.5.2/eis_toolkit/vector_processing/rasterize_vector.py
+-rw-r--r--   0        0        0      703 2023-11-10 08:05:31.345266 eis_toolkit-0.5.2/eis_toolkit/vector_processing/reproject_vector.py
+-rw-r--r--   0        0        0     1523 2024-04-24 14:32:41.807458 eis_toolkit-0.5.2/eis_toolkit/vector_processing/vector_density.py
+-rwxr-xr-x   0        0        0     1778 2024-05-24 11:29:42.222707 eis_toolkit-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 eis_toolkit-0.5.2/PKG-INFO
```

### Comparing `eis_toolkit-0.5.1/LICENSE` & `eis_toolkit-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/README.md` & `eis_toolkit-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/cli.py` & `eis_toolkit-0.5.2/eis_toolkit/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,23 +327,23 @@
     from eis_toolkit.exploratory_analyses.normality_test import normality_test_array
 
     typer.echo("Progress: 10%")
 
     with rasterio.open(input_raster) as raster:
         data = raster.read()
         typer.echo("Progress: 25%")
-        print(bands)
         if len(bands) == 0:
             bands = None
         results_dict = normality_test_array(data=data, bands=bands, nodata_value=raster.nodata)
 
     typer.echo("Progress: 75%")
 
     json_str = json.dumps(results_dict)
     typer.echo("Progress: 100%")
+
     typer.echo(f"Results: {json_str}")
     typer.echo("Normality test (raster) completed")
 
 
 # NORMALITY TEST VECTOR
 @app.command()
 def normality_test_vector_cli(input_vector: INPUT_FILE_OPTION, columns: Optional[List[str]] = None):
@@ -357,14 +357,15 @@
 
     results_dict = normality_test_dataframe(data=geodataframe, columns=columns)
 
     typer.echo("Progress: 75%")
 
     json_str = json.dumps(results_dict)
     typer.echo("Progress: 100%")
+
     typer.echo(f"Results: {json_str}")
     typer.echo("Normality test (vector) completed")
 
 
 # CHI-SQUARE_TEST
 @app.command()
 def chi_square_test_cli(
@@ -382,14 +383,15 @@
 
     results_dict = chi_square_test(data=geodataframe, target_column=target_column, columns=columns)
 
     typer.echo("Progress: 75%")
 
     json_str = json.dumps(results_dict)
     typer.echo("Progress: 100%")
+
     typer.echo(f"Results: {json_str}")
     typer.echo("Chi-square test completed")
 
 
 # CORRELATION MATRIX
 @app.command()
 def correlation_matrix_cli(
@@ -661,14 +663,15 @@
         variances_ratios_dict[name] = variance_ratio
     json_str = json.dumps(variances_ratios_dict)
 
     with rasterio.open(output_raster, "w", **out_profile) as dst:
         dst.write(pca_array)
 
     typer.echo("Progress: 100%")
+
     typer.echo(f"Results: {json_str}")
     typer.echo(f"PCA computation (raster) completed, output raster saved to {output_raster}.")
 
 
 # PCA FOR VECTOR DATA
 @app.command()
 def compute_pca_vector_cli(
@@ -701,14 +704,15 @@
     for i, variance_ratio in enumerate(variance_ratios):
         name = "PC " + str(i) + " explained variance"
         variances_ratios_dict[name] = variance_ratio
     json_str = json.dumps(variances_ratios_dict)
 
     pca_gdf.to_file(output_vector)
     typer.echo("Progress: 100%")
+
     typer.echo(f"Results: {json_str}")
     typer.echo(f"PCA computation (vector) completed, output vector saved to {output_vector}.")
 
 
 # DESCRIPTIVE STATISTICS (RASTER)
 @app.command()
 def descriptive_statistics_raster_cli(input_file: INPUT_FILE_OPTION):
@@ -718,21 +722,18 @@
     typer.echo("Progress: 10%")
 
     with rasterio.open(input_file) as raster:
         typer.echo("Progress: 25%")
         results_dict = descriptive_statistics_raster(raster)
     typer.echo("Progress: 75%")
 
-    # json_str = json.dumps(results_dict)
+    json_str = json.dumps(results_dict)
     typer.echo("Progress: 100%\n")
-    # typer.echo(f"Results: {json_str}")
-    # typer.echo("Results:\n")
-    for key, value in results_dict.items():
-        typer.echo(f"{key}: {value}")
 
+    typer.echo(f"Results: {json_str}")
     typer.echo("\nDescriptive statistics (raster) completed")
 
 
 # DESCRIPTIVE STATISTICS (VECTOR)
 @app.command()
 def descriptive_statistics_vector_cli(input_file: INPUT_FILE_OPTION, column: str = None):
     """Generate descriptive statistics from vector or tabular data."""
@@ -2019,15 +2020,50 @@
         dst.write(out_image, 1)
     typer.echo("Progress: 100%")
 
     typer.echo(f"Distance computation completed, writing raster to {output_raster}.")
 
 
 # CBA
-# TODO
+@app.command()
+def cell_based_association_cli(
+    input_vector: INPUT_FILE_OPTION,
+    output_raster: OUTPUT_FILE_OPTION,
+    cell_size: int = typer.Option(),
+    column: Optional[str] = None,
+    subset_target_attribute_values: Optional[List[str]] = None,
+    add_name: Optional[str] = None,
+    add_buffer: Optional[float] = None,
+):
+    """Create a CBA matrix."""
+    from eis_toolkit.vector_processing.cell_based_association import cell_based_association
+
+    typer.echo("Progress: 10%")
+
+    geodataframe = gpd.read_file(input_vector)
+    typer.echo("Progress: 25%")
+
+    if subset_target_attribute_values is not None:
+        subset_target_attribute_values = [value.strip() for value in subset_target_attribute_values]
+
+    cell_based_association(
+        cell_size=cell_size,
+        geodata=[geodataframe],
+        output_path=output_raster,
+        column=column if column is None else [column],
+        subset_target_attribute_values=subset_target_attribute_values
+        if subset_target_attribute_values is None
+        else [subset_target_attribute_values],
+        add_name=add_name if add_name is None else [add_name],
+        add_buffer=add_buffer if add_buffer is None else [add_buffer],
+    )
+
+    typer.echo("Progress: 100%")
+
+    typer.echo(f"Cell based association completed, writing raster to {output_raster}.")
 
 
 # --- PREDICTION ---
 
 
 # LOGISTIC REGRESSION
 @app.command()
@@ -2348,20 +2384,18 @@
     out_profile.update({"count": 1, "dtype": np.float32})
 
     with rasterio.open(output_raster_probability, "w", **out_profile) as dst:
         dst.write(probabilities_reshaped, 1)
     with rasterio.open(output_raster_classified, "w", **out_profile) as dst:
         dst.write(predictions_reshaped, 1)
 
-    typer.echo("\n")
-    for key, value in metrics_dict.items():
-        typer.echo(f"{key}: {value}")
-    typer.echo("\n")
+    json_str = json.dumps(metrics_dict)
+    typer.echo("Progress: 100% \n")
 
-    typer.echo("Progress: 100%")
+    typer.echo(f"Results: {json_str}")
     typer.echo(
         (
             "Testing classifier model completed, writing rasters to "
             f"{output_raster_probability} and {output_raster_classified}."
         )
     )
 
@@ -2394,21 +2428,18 @@
 
     out_profile = reference_profile.copy()
     out_profile.update({"count": 1, "dtype": np.float32})
 
     with rasterio.open(output_raster, "w", **out_profile) as dst:
         dst.write(predictions_reshaped, 1)
 
-    typer.echo("\n")
-    for key, value in metrics_dict.items():
-        typer.echo(f"{key}: {value}")
-    typer.echo("\n")
-
-    typer.echo("Progress: 100%\n")
+    json_str = json.dumps(metrics_dict)
+    typer.echo("Progress: 100% \n")
 
+    typer.echo(f"Results: {json_str}")
     typer.echo(f"Testing regressor model completed, writing raster to {output_raster}.")
 
 
 # PREDICT WITH TRAINED ML MODEL
 @app.command()
 def classifier_predict_cli(
     input_rasters: INPUT_FILES_ARGUMENT,
@@ -3080,20 +3111,18 @@
     (y_prob, y_true), _, _ = read_data_for_evaluation([probabilities, true_labels])
     typer.echo("Progress: 25%")
 
     results_dict = summarize_probability_metrics(y_true=y_true, y_prob=y_prob)
 
     typer.echo("Progress: 75%")
 
-    # json_str = json.dumps(results_dict)
+    json_str = json.dumps(results_dict)
     typer.echo("Progress: 100% \n")
-    # typer.echo("Results:\n")
-    for key, value in results_dict.items():
-        typer.echo(f"{key}: {value}")
-    # typer.echo(f"Results: {json_str}")
+
+    typer.echo(f"Results: {json_str}")
     typer.echo("\nGenerating probability metrics summary completed.")
 
 
 @app.command()
 def summarize_label_metrics_binary_cli(true_labels: INPUT_FILE_OPTION, predictions: INPUT_FILE_OPTION):
     """
     Generate a comprehensive report of various evaluation metrics for binary classification results.
@@ -3108,19 +3137,18 @@
 
     (y_pred, y_true), _, _ = read_data_for_evaluation([predictions, true_labels])
     typer.echo("Progress: 25%")
 
     results_dict = summarize_label_metrics_binary(y_true=y_true, y_pred=y_pred)
     typer.echo("Progress: 75%")
 
-    # json_str = json.dumps(results_dict)
+    json_str = json.dumps(results_dict)
     typer.echo("Progress: 100% \n")
-    for key, value in results_dict.items():
-        typer.echo(f"{key}: {value}")
-    # typer.echo(f"Results: {json_str}")
+
+    typer.echo(f"Results: {json_str}")
     typer.echo("\n Generating prediction label metrics summary completed.")
 
 
 @app.command()
 def plot_roc_curve_cli(
     true_labels: INPUT_FILE_OPTION,
     probabilities: INPUT_FILE_OPTION,
```

### Comparing `eis_toolkit-0.5.1/eis_toolkit/conversions/csv_to_geodataframe.py` & `eis_toolkit-0.5.2/eis_toolkit/conversions/csv_to_geodataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/conversions/raster_to_dataframe.py` & `eis_toolkit-0.5.2/eis_toolkit/conversions/raster_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/evaluation/calculate_base_metrics.py` & `eis_toolkit-0.5.2/eis_toolkit/evaluation/calculate_base_metrics.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/evaluation/classification_label_evaluation.py` & `eis_toolkit-0.5.2/eis_toolkit/evaluation/classification_label_evaluation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/evaluation/classification_probability_evaluation.py` & `eis_toolkit-0.5.2/eis_toolkit/evaluation/classification_probability_evaluation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_confusion_matrix.py` & `eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_nn_model_performance.py` & `eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_nn_model_performance.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_prediction_area_curves.py` & `eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_prediction_area_curves.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/evaluation/plot_rate_curve.py` & `eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_rate_curve.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/evaluation/scoring.py` & `eis_toolkit-0.5.2/eis_toolkit/evaluation/scoring.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exceptions.py` & `eis_toolkit-0.5.2/eis_toolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/chi_square_test.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/chi_square_test.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/correlation_matrix.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/covariance_matrix.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/dbscan.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/dbscan.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/descriptive_statistics.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/descriptive_statistics.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/feature_importance.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/feature_importance.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/k_means_cluster.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/k_means_cluster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/local_morans_i.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/local_morans_i.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/normality_test.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/normality_test.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/parallel_coordinates.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/exploratory_analyses/pca.py` & `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/pca.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/prediction/fuzzy_overlay.py` & `eis_toolkit-0.5.2/eis_toolkit/prediction/fuzzy_overlay.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/prediction/gradient_boosting.py` & `eis_toolkit-0.5.2/eis_toolkit/prediction/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/prediction/logistic_regression.py` & `eis_toolkit-0.5.2/eis_toolkit/prediction/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/prediction/machine_learning_general.py` & `eis_toolkit-0.5.2/eis_toolkit/prediction/machine_learning_general.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/prediction/machine_learning_predict.py` & `eis_toolkit-0.5.2/eis_toolkit/prediction/machine_learning_predict.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/prediction/mlp.py` & `eis_toolkit-0.5.2/eis_toolkit/prediction/mlp.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/prediction/random_forests.py` & `eis_toolkit-0.5.2/eis_toolkit/prediction/random_forests.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/prediction/weights_of_evidence.py` & `eis_toolkit-0.5.2/eis_toolkit/prediction/weights_of_evidence.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/clipping.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/clipping.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/create_constant_raster.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/create_constant_raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/classification.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/classification.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/parameters.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/parameters.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/partial_derivatives.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/partial_derivatives.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/derivatives/utilities.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/utilities.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/distance_to_anomaly.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/distance_to_anomaly.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/extract_values_from_raster.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/extract_values_from_raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/focal.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/focal.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/kernels.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/kernels.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/speckle.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/speckle.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/filters/utilities.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/utilities.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/reclassify.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/reclassify.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/reprojecting.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/reprojecting.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/resampling.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/resampling.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/snapping.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/snapping.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/unifying.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/unifying.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/unique_combinations.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/unique_combinations.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/raster_processing/windowing.py` & `eis_toolkit-0.5.2/eis_toolkit/raster_processing/windowing.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/training_data_tools/class_balancing.py` & `eis_toolkit-0.5.2/eis_toolkit/training_data_tools/class_balancing.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/binarize.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/binarize.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/clip.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/clip.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/alr.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/alr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/clr.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/clr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/ilr.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/ilr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/pairwise.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/pairwise.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/coda/plr.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/plr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/linear.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/linear.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/logarithmic.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/logarithmic.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/one_hot_encoding.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/sigmoid.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/transformations/winsorize.py` & `eis_toolkit-0.5.2/eis_toolkit/transformations/winsorize.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/aitchison_geometry.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/aitchison_geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/compositional.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/compositional.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/dataframe.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/dataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/geometry.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/parameter.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/parameter.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/checks/raster.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/conversions.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/conversions.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/file_io.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/file_io.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/miscellaneous.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/nodata.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/nodata.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/utilities/raster.py` & `eis_toolkit-0.5.2/eis_toolkit/utilities/raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/calculate_geometry.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/calculate_geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/cell_based_association.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/cell_based_association.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import warnings
 from numbers import Number
+from os import PathLike
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import rasterio
 from beartype import beartype
 from beartype.typing import List, Optional, Tuple, Union
@@ -18,15 +19,15 @@
 os.environ["USE_PYGEOS"] = "0"
 
 
 @beartype
 def cell_based_association(
     cell_size: int,
     geodata: List[gpd.GeoDataFrame],
-    output_path: str,
+    output_path: Union[str, PathLike],
     column: Optional[List[str]] = None,
     subset_target_attribute_values: Optional[List[Union[None, list, str]]] = None,
     add_name: Optional[List[Union[str, None]]] = None,
     add_buffer: Optional[List[Union[Number, bool]]] = None,
 ) -> gpd.GeoDataFrame:
     """Creation of CBA matrix.
 
@@ -35,15 +36,16 @@
     Allows to add multiple vector data to the matrix, based on targeted shapes
     and/or attributes.
 
     Args:
         cell_size: Size of the cells.
         geodata: GeoDataFrame to create the CBA matrix. Additional
             GeoDataFrame(s) can be imputed to add to the CBA matrix.
-        output_path: Name of the saved .tif file.
+        output_path: Name of the saved .tif file. Include file extension (.tif)
+            in the path.
         column: Name of the column of interest. If no attribute is specified,
             then an artificial attribute is created representing the presence
             or absence of the geometries of this file for each cell of the CBA
             grid. A categorical attribute will generate as many columns (binary)
             in the CBA matrix than values considered of interest (dummification).
             See parameter <subset_target_attribute_values>. Additional
             column(s) can be imputed for each added GeoDataFrame(s).
@@ -84,18 +86,16 @@
         if column[i] == "":
             if subset_target_attribute_values[i] is not None:
                 raise InvalidParameterValueException("Can't use subset of values if no column is targeted.")
         elif column[i] not in geodata[i]:
             raise InvalidColumnException("Targeted column not found in the GeoDataFrame.")
 
     for i, subset in enumerate(subset_target_attribute_values):
-        if subset is not None:
-            for value in subset:
-                if value not in geodata[i][column[i]].unique():
-                    raise InvalidParameterValueException("Subset of value(s) not found in the targeted column.")
+        if subset is not None and not all(value in geodata[i][column[i]].tolist() for value in subset):
+            raise InvalidParameterValueException("Subset of value(s) not found in the targeted column.")
 
     # Computation
     for i, data in enumerate(geodata):
         if i == 0:
             # Initialization of the CBA matrix
             grid, cba = _init_from_vector_data(cell_size, geodata[0], column[0], subset_target_attribute_values[0])
         else:
@@ -524,22 +524,22 @@
     tmp["geometry"] = tmp.geometry.apply(lambda x: wkt.dumps(x))
     # tmp = tmp.drop("geometry", axis=1)
     tmp["cell_id"] = cba.index
     tmp.to_csv(output_path + "__" + str(crs_txt).replace(":", "_") + ".csv", index=False)
 
 
 @beartype
-def _to_raster(cba: gpd.GeoDataFrame, output_path: str, nan_val: int = -9999) -> None:
+def _to_raster(cba: gpd.GeoDataFrame, output_path: Union[str, PathLike], nan_val: int = -9999) -> None:
     """Intermediate utility.
 
     Saves the object as a raster TIFF file.
 
     Args:
         cba: CBA matrix to save.
-        output_path: Name of the saved file.
+        output_path: Name of the saved file, include file extension (.tif).
         nan_val: values taken by cells with no values in them (outside the study
         area).
 
     Returns:
         None
     """
 
@@ -575,15 +575,15 @@
     points_grid = points_grid.sjoin(cba, how="left")
     points_grid = points_grid.fillna(nan_val)
     col_name = list(points_grid.drop(["X", "Y", "coords", "index_right"], axis=1).columns)
 
     transform = rasterio.transform.from_bounds(min_x, min_y, max_x, max_y, width=width, height=height)
 
     with rasterio.open(
-        output_path + ".tif",
+        output_path,
         mode="w",
         driver="GTiff",
         height=height,
         width=width,
         count=count,
         dtype="int32",
         crs=crs_txt,
```

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/distance_computation.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/distance_computation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/extract_shared_lines.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/extract_shared_lines.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/idw_interpolation.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/idw_interpolation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/kriging_interpolation.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/kriging_interpolation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/rasterize_vector.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/rasterize_vector.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/reproject_vector.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/reproject_vector.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/eis_toolkit/vector_processing/vector_density.py` & `eis_toolkit-0.5.2/eis_toolkit/vector_processing/vector_density.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.1/pyproject.toml` & `eis_toolkit-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eis_toolkit"
-version = "0.5.1"
+version = "0.5.2"
 description = "EIS Toolkit is a comprehensive collection of tools suitable for mineral prospectivity mapping. This toolkit has been developed as part of the Exploration Information System project which has been funded by European Union."
 authors = []
 maintainers = ["Gispo Ltd. <info@gispo.fi>"]
 license = "EUPL-1.2"
 readme = "README.md"
 homepage = "https://eis-he.eu"
 repository = "https://github.com/GispoCoding/eis_toolkit"
```

### Comparing `eis_toolkit-0.5.1/PKG-INFO` & `eis_toolkit-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis_toolkit
-Version: 0.5.1
+Version: 0.5.2
 Summary: EIS Toolkit is a comprehensive collection of tools suitable for mineral prospectivity mapping. This toolkit has been developed as part of the Exploration Information System project which has been funded by European Union.
 Home-page: https://eis-he.eu
 License: EUPL-1.2
 Keywords: Development Status :: 4 - Beta,Topic :: Scientific/Engineering :: GIS,Programming Language :: Python :: 3 :: Only
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 Requires-Python: >=3.9,<3.11
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_l7ecwo4f_/tmpjwzq0a8__TarContainer/0/103", line 41, column 35: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eis_toolkit Version: 0.5.1 Summary: EIS Toolkit is
+Metadata-Version: 2.1 Name: eis_toolkit Version: 0.5.2 Summary: EIS Toolkit is
 a comprehensive collection of tools suitable for mineral prospectivity mapping.
 This toolkit has been developed as part of the Exploration Information System
 project which has been funded by European Union. Home-page: https://eis-he.eu
 License: EUPL-1.2 Keywords: Development Status :: 4 - Beta,Topic :: Scientific/
 Engineering :: GIS,Programming Language :: Python :: 3 :: Only Maintainer:
 Gispo Ltd. Maintainer-email: info@gispo.fi Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL
```

