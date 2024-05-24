# Comparing `tmp/tardis_em-0.2.5.tar.gz` & `tmp/tardis_em-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tardis_em-0.2.5.tar", last modified: Thu May 23 07:21:35 2024, max compression
+gzip compressed data, was "tardis_em-0.2.6.tar", last modified: Fri May 24 08:27:36 2024, max compression
```

## Comparing `tardis_em-0.2.5.tar` & `tardis_em-0.2.6.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.987546 tardis_em-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-23 07:21:31.000000 tardis_em-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-23 07:21:31.000000 tardis_em-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-23 07:21:35.987546 tardis_em-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-23 07:21:31.000000 tardis_em-0.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-23 07:21:31.000000 tardis_em-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-23 07:21:31.000000 tardis_em-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-23 07:21:35.987546 tardis_em-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-23 07:21:31.000000 tardis_em-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.971546 tardis_em-0.2.5/tardis_em/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/benchmarks/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/benchmarks/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/cnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/cnn/data_processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/draw_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/stitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/data_processing/trim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/cnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/datasets/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15300 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/datasets/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/datasets/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.975546 tardis_em-0.2.5/tardis_em/cnn/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/decoder_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/encoder_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/model/init_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18740 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/utils/build_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/cnn/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/compare_spatial_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/model/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/model/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    29804 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16498 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/build_point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/segment_point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/dist_pytorch/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/predict_actin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/predict_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/predict_mem_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/predict_mt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.979546 tardis_em-0.2.5/tardis_em/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16330 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/scripts/czi_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/scripts/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/tardis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.983546 tardis_em-0.2.5/tardis_em/tardis_helper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/tardis_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/tardis_helper/helper_func.py
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/train_DIST.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/train_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.983546 tardis_em-0.2.5/tardis_em/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    20802 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/export_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    29405 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    20740 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/ota_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    53166 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/setup_envir.py
--rw-r--r--   0 runner    (1001) docker     (127)    38169 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/spline_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tardis_em/utils/visualize_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.987546 tardis_em-0.2.5/tardis_em.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 07:21:35.000000 tardis_em-0.2.5/tardis_em.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:21:35.987546 tardis_em-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_draw_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_trim_stitch.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_cnn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_graph_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_img_to_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-05-23 07:21:31.000000 tardis_em-0.2.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.661870 tardis_em-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-24 08:27:31.000000 tardis_em-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-24 08:27:31.000000 tardis_em-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-24 08:27:36.661870 tardis_em-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-24 08:27:31.000000 tardis_em-0.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-24 08:27:32.000000 tardis_em-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-24 08:27:32.000000 tardis_em-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-24 08:27:36.661870 tardis_em-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-24 08:27:32.000000 tardis_em-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.645870 tardis_em-0.2.6/tardis_em/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.645870 tardis_em-0.2.6/tardis_em/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/benchmarks/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/benchmarks/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.645870 tardis_em-0.2.6/tardis_em/cnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.645870 tardis_em-0.2.6/tardis_em/cnn/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/draw_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/stitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/trim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/cnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/datasets/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15300 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/datasets/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/datasets/dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/cnn/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/decoder_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/encoder_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/init_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18740 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/utils/build_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/compare_spatial_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/dist_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/dist_pytorch/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/model/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.653870 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29804 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.653870 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/build_point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/segment_point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/predict_actin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/predict_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/predict_mem_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/predict_mt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.653870 tardis_em-0.2.6/tardis_em/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16330 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/scripts/czi_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/scripts/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/tardis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.653870 tardis_em-0.2.6/tardis_em/tardis_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/tardis_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/tardis_helper/helper_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/train_DIST.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/train_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.657870 tardis_em-0.2.6/tardis_em/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20802 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29405 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20740 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/ota_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53242 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/setup_envir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38169 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/spline_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/visualize_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.661870 tardis_em-0.2.6/tardis_em.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.657870 tardis_em-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_draw_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_trim_stitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_graph_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_img_to_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_utils.py
```

### Comparing `tardis_em-0.2.5/LICENSE` & `tardis_em-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/PKG-INFO` & `tardis_em-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tardis_em
-Version: 0.2.5
+Version: 0.2.6
 Summary: PyTorch segmentation of 2D/3D images such as electron tomography (ET),Cryo-EM or fluorescent microscopy data into 3D segmented point cloud.
 Home-page: https://github.com/SMLC-NYSBC/TARDIS
 Author: Robert Kiewisz, Tristan Bepler
 Author-email: rkiewisz@nysbc.org
 License: MIT
 Keywords: semantic segmentation,instance segmentation,MT segmentation,membrane segmentation,CNN,FNet,DIST
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tardis_em-0.2.5/README.rst` & `tardis_em-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/setup.cfg` & `tardis_em-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/setup.py` & `tardis_em-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/benchmarks/benchmarks.py` & `tardis_em-0.2.6/tardis_em/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/benchmarks/predictor.py` & `tardis_em-0.2.6/tardis_em/benchmarks/predictor.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/cnn.py` & `tardis_em-0.2.6/tardis_em/cnn/cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/data_processing/draw_mask.py` & `tardis_em-0.2.6/tardis_em/cnn/data_processing/draw_mask.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/data_processing/interpolation.py` & `tardis_em-0.2.6/tardis_em/cnn/data_processing/interpolation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/data_processing/stitch.py` & `tardis_em-0.2.6/tardis_em/cnn/data_processing/stitch.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/data_processing/trim.py` & `tardis_em-0.2.6/tardis_em/cnn/data_processing/trim.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/datasets/augmentation.py` & `tardis_em-0.2.6/tardis_em/cnn/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/datasets/build_dataset.py` & `tardis_em-0.2.6/tardis_em/cnn/datasets/build_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/datasets/dataloader.py` & `tardis_em-0.2.6/tardis_em/cnn/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/model/convolution.py` & `tardis_em-0.2.6/tardis_em/cnn/model/convolution.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/model/decoder_blocks.py` & `tardis_em-0.2.6/tardis_em/cnn/model/decoder_blocks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/model/encoder_blocks.py` & `tardis_em-0.2.6/tardis_em/cnn/model/encoder_blocks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/model/init_weights.py` & `tardis_em-0.2.6/tardis_em/cnn/model/init_weights.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/train.py` & `tardis_em-0.2.6/tardis_em/cnn/train.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/trainer.py` & `tardis_em-0.2.6/tardis_em/cnn/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/utils/build_cnn.py` & `tardis_em-0.2.6/tardis_em/cnn/utils/build_cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/cnn/utils/utils.py` & `tardis_em-0.2.6/tardis_em/cnn/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/compare_spatial_graphs.py` & `tardis_em-0.2.6/tardis_em/compare_spatial_graphs.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/augmentation.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/dataloader.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/datasets/patches.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/patches.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/dist.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/dist.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/model/embedding.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/model/embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/model/layers.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/model/layers.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/model/modules.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/model/modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_dist.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_dist.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/embedding.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/layers.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/layers.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/sparse_model/modules.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/train.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/train.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/trainer.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/utils/__init__.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/utils/build_point_cloud.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/utils/build_point_cloud.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/utils/segment_point_cloud.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/utils/segment_point_cloud.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/dist_pytorch/utils/utils.py` & `tardis_em-0.2.6/tardis_em/dist_pytorch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/predict_actin.py` & `tardis_em-0.2.6/tardis_em/predict_actin.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/predict_mem.py` & `tardis_em-0.2.6/tardis_em/predict_mem.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/predict_mem_2d.py` & `tardis_em-0.2.6/tardis_em/predict_mem_2d.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/predict_mt.py` & `tardis_em-0.2.6/tardis_em/predict_mt.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/scripts/czi_predict.py` & `tardis_em-0.2.6/tardis_em/scripts/czi_predict.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/scripts/visualize.py` & `tardis_em-0.2.6/tardis_em/scripts/visualize.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/tardis.py` & `tardis_em-0.2.6/tardis_em/tardis.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/tardis_helper/helper_func.py` & `tardis_em-0.2.6/tardis_em/tardis_helper/helper_func.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/train_DIST.py` & `tardis_em-0.2.6/tardis_em/train_DIST.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/train_cnn.py` & `tardis_em-0.2.6/tardis_em/train_cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/__init__.py` & `tardis_em-0.2.6/tardis_em/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/aws.py` & `tardis_em-0.2.6/tardis_em/utils/aws.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/dataset.py` & `tardis_em-0.2.6/tardis_em/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/device.py` & `tardis_em-0.2.6/tardis_em/utils/device.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/errors.py` & `tardis_em-0.2.6/tardis_em/utils/errors.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/export_data.py` & `tardis_em-0.2.6/tardis_em/utils/export_data.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/load_data.py` & `tardis_em-0.2.6/tardis_em/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/logo.py` & `tardis_em-0.2.6/tardis_em/utils/logo.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/losses.py` & `tardis_em-0.2.6/tardis_em/utils/losses.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/metrics.py` & `tardis_em-0.2.6/tardis_em/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/normalization.py` & `tardis_em-0.2.6/tardis_em/utils/normalization.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/ota_update.py` & `tardis_em-0.2.6/tardis_em/utils/ota_update.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/predictor.py` & `tardis_em-0.2.6/tardis_em/utils/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,15 +708,19 @@
         # Common text for all configurations
         common_text = {
             "text_1": f"Found {len(self.predict_list)} images to predict!",
             "text_2": f"Device: {self.device}",
             "text_3": f"Image {id_ + 1}/{len(self.predict_list)}: {i}",
         }
 
-        no_segments = np.max(self.segments[:, 0]) if len(self.segments) > 0 else 0
+        if log_id == 7:
+            no_segments = np.max(self.segments[:, 0]) if len(self.segments) > 0 else 0
+        else:
+            no_segments = 'None'
+
         # Define text configurations for each log_id
         text_configurations = {
             0: {
                 **common_text,
                 "text_4": "Original Pixel size: Nan A",
                 "text_7": "Current Task: Preprocessing for CNN...",
             },
```

### Comparing `tardis_em-0.2.5/tardis_em/utils/setup_envir.py` & `tardis_em-0.2.6/tardis_em/utils/setup_envir.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/spline_metric.py` & `tardis_em-0.2.6/tardis_em/utils/spline_metric.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/trainer.py` & `tardis_em-0.2.6/tardis_em/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/utils.py` & `tardis_em-0.2.6/tardis_em/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em/utils/visualize_pc.py` & `tardis_em-0.2.6/tardis_em/utils/visualize_pc.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em.egg-info/PKG-INFO` & `tardis_em-0.2.6/tardis_em.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tardis_em
-Version: 0.2.5
+Version: 0.2.6
 Summary: PyTorch segmentation of 2D/3D images such as electron tomography (ET),Cryo-EM or fluorescent microscopy data into 3D segmented point cloud.
 Home-page: https://github.com/SMLC-NYSBC/TARDIS
 Author: Robert Kiewisz, Tristan Bepler
 Author-email: rkiewisz@nysbc.org
 License: MIT
 Keywords: semantic segmentation,instance segmentation,MT segmentation,membrane segmentation,CNN,FNet,DIST
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tardis_em-0.2.5/tardis_em.egg-info/SOURCES.txt` & `tardis_em-0.2.6/tardis_em.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tardis_em.egg-info/entry_points.txt` & `tardis_em-0.2.6/tardis_em.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_cnn_build_dataset.py` & `tardis_em-0.2.6/tests/test_cnn_build_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_cnn_dataset.py` & `tardis_em-0.2.6/tests/test_cnn_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_cnn_draw_mask.py` & `tardis_em-0.2.6/tests/test_cnn_draw_mask.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_cnn_interpolation.py` & `tardis_em-0.2.6/tests/test_cnn_interpolation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_cnn_nn.py` & `tardis_em-0.2.6/tests/test_cnn_nn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_cnn_trim_stitch.py` & `tardis_em-0.2.6/tests/test_cnn_trim_stitch.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_cnn_utils.py` & `tardis_em-0.2.6/tests/test_cnn_utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_augmentation.py` & `tardis_em-0.2.6/tests/test_dist_augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_data_loader.py` & `tardis_em-0.2.6/tests/test_dist_data_loader.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_embedding.py` & `tardis_em-0.2.6/tests/test_dist_embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_graph_cut.py` & `tardis_em-0.2.6/tests/test_dist_graph_cut.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_img_to_pc.py` & `tardis_em-0.2.6/tests/test_dist_img_to_pc.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_modules.py` & `tardis_em-0.2.6/tests/test_dist_modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_nn.py` & `tardis_em-0.2.6/tests/test_dist_nn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_trainer.py` & `tardis_em-0.2.6/tests/test_dist_trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_dist_utils.py` & `tardis_em-0.2.6/tests/test_dist_utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_losses.py` & `tardis_em-0.2.6/tests/test_losses.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_trainer.py` & `tardis_em-0.2.6/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.5/tests/test_utils.py` & `tardis_em-0.2.6/tests/test_utils.py`

 * *Files identical despite different names*

