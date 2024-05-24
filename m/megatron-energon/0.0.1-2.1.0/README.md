# Comparing `tmp/megatron_energon-0.0.1.tar.gz` & `tmp/megatron_energon-2.1.0.tar.gz`

## Comparing `megatron_energon-0.0.1.tar` & `megatron_energon-2.1.0.tar`

### file list

```diff
@@ -1,5 +1,77 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 megatron_energon-0.0.1/megatron/energon/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 megatron_energon-0.0.1/.gitignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 megatron_energon-0.0.1/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 megatron_energon-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 megatron_energon-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/__init__.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/dataset_config.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/errors.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/loader.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/module_loader.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/retry_stream.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/rng.py
+-rw-r--r--   0        0        0    48843 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/savable_loader.py
+-rw-r--r--   0        0        0    38619 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/typed_converter.py
+-rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/worker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/cli/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/cli/main.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/epathlib/__init__.py
+-rw-r--r--   0        0        0    12483 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/epathlib/epath.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/epathlib/rclone_config.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/__init__.py
+-rw-r--r--   0        0        0    11895 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/base_dataset.py
+-rw-r--r--   0        0        0    32399 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/base_webdataset.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/captioning.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/crude.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/image.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/image_classification.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/interleaved.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/multichoice_vqa.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/ocr.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/similarity_interleaved.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/text.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/vqa.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/vqa_and_ocr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/webdataset/__init__.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/webdataset/config.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/webdataset/field_access.py
+-rw-r--r--   0        0        0     4745 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/webdataset/itar.py
+-rw-r--r--   0        0        0    37671 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/webdataset/sample_loader.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/flavors/webdataset/structs.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/metadataset/__init__.py
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/metadataset/dataset_loader.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/metadataset/loader.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/metadataset/loader_interface.py
+-rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/metadataset/metadataset.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/task_encoder/__init__.py
+-rw-r--r--   0        0        0    19567 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/task_encoder/base.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/task_encoder/cooking.py
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/task_encoder/loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/tools/__init__.py
+-rw-r--r--   0        0        0    19502 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/tools/analyze_debug.py
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/tools/lint.py
+-rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/tools/prepare.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/tools/preview.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/transforms/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/transforms/common.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/transforms/custom.py
+-rw-r--r--   0        0        0    15081 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/transforms/mappers.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/transforms/merge.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/_log_exception.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/base.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/batch_dataset.py
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/blend_dataset.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/concat_dataset.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/epochize_dataset.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/filter_dataset.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/gc_dataset.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/group_batch_dataset.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/iter_map_dataset.py
+-rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/limit_dataset.py
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/log_sample_dataset.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/map_dataset.py
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/mix_batch_dataset.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/repeat_dataset.py
+-rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/shuffle_buffer_dataset.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/megatron/energon/wrappers/skip.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/.gitignore
+-rw-r--r--   0        0        0    25793 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/README.md
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 megatron_energon-2.1.0/PKG-INFO
```

