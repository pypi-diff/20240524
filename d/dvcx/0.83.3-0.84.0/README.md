# Comparing `tmp/dvcx-0.83.3.tar.gz` & `tmp/dvcx-0.84.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.83.3.tar", last modified: Thu May 23 11:23:02 2024, max compression
+gzip compressed data, was "dvcx-0.84.0.tar", last modified: Fri May 24 01:02:46 2024, max compression
```

## Comparing `dvcx-0.83.3.tar` & `dvcx-0.84.0.tar`

### file list

```diff
@@ -1,252 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.159850 dvcx-0.83.3/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-23 11:22:56.000000 dvcx-0.83.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 11:22:56.000000 dvcx-0.83.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.115851 dvcx-0.83.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.115851 dvcx-0.83.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.115851 dvcx-0.83.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-23 11:22:56.000000 dvcx-0.83.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-23 11:22:56.000000 dvcx-0.83.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.115851 dvcx-0.83.3/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 11:22:56.000000 dvcx-0.83.3/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 11:22:56.000000 dvcx-0.83.3/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-23 11:22:56.000000 dvcx-0.83.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-23 11:22:56.000000 dvcx-0.83.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-23 11:22:56.000000 dvcx-0.83.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.119850 dvcx-0.83.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-23 11:22:56.000000 dvcx-0.83.3/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 11:22:56.000000 dvcx-0.83.3/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-23 11:22:56.000000 dvcx-0.83.3/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-23 11:23:02.159850 dvcx-0.83.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-23 11:22:56.000000 dvcx-0.83.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.119850 dvcx-0.83.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-23 11:22:56.000000 dvcx-0.83.3/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.123850 dvcx-0.83.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.123850 dvcx-0.83.3/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.123850 dvcx-0.83.3/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.123850 dvcx-0.83.3/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-23 11:22:56.000000 dvcx-0.83.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-23 11:22:56.000000 dvcx-0.83.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:23:02.159850 dvcx-0.83.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.111851 dvcx-0.83.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.127850 dvcx-0.83.3/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 11:23:01.000000 dvcx-0.83.3/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.127850 dvcx-0.83.3/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72880 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.127850 dvcx-0.83.3/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.131850 dvcx-0.83.3/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46796 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24923 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31659 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.135850 dvcx-0.83.3/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.135850 dvcx-0.83.3/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    61693 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.151850 dvcx-0.83.3/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.143850 dvcx-0.83.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.143850 dvcx-0.83.3/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.143850 dvcx-0.83.3/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   112870 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    28908 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.143850 dvcx-0.83.3/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.147850 dvcx-0.83.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.151850 dvcx-0.83.3/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.151850 dvcx-0.83.3/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.151850 dvcx-0.83.3/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.431903 dvcx-0.84.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-24 01:02:41.000000 dvcx-0.84.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 01:02:41.000000 dvcx-0.84.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.383904 dvcx-0.84.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.383904 dvcx-0.84.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.383904 dvcx-0.84.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-24 01:02:41.000000 dvcx-0.84.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-24 01:02:41.000000 dvcx-0.84.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-24 01:02:41.000000 dvcx-0.84.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.383904 dvcx-0.84.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 01:02:41.000000 dvcx-0.84.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 01:02:41.000000 dvcx-0.84.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-24 01:02:41.000000 dvcx-0.84.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-24 01:02:41.000000 dvcx-0.84.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-24 01:02:41.000000 dvcx-0.84.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.387904 dvcx-0.84.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-24 01:02:41.000000 dvcx-0.84.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 01:02:41.000000 dvcx-0.84.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-24 01:02:41.000000 dvcx-0.84.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-24 01:02:46.431903 dvcx-0.84.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-24 01:02:41.000000 dvcx-0.84.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.387904 dvcx-0.84.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-24 01:02:41.000000 dvcx-0.84.0/docs/cv_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-24 01:02:41.000000 dvcx-0.84.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.387904 dvcx-0.84.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.391904 dvcx-0.84.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.391904 dvcx-0.84.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.391904 dvcx-0.84.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 01:02:41.000000 dvcx-0.84.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-24 01:02:41.000000 dvcx-0.84.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-24 01:02:41.000000 dvcx-0.84.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:02:46.431903 dvcx-0.84.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.379904 dvcx-0.84.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.395904 dvcx-0.84.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 01:02:46.000000 dvcx-0.84.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.395904 dvcx-0.84.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72836 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.399904 dvcx-0.84.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.399904 dvcx-0.84.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46749 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24923 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31659 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.403904 dvcx-0.84.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/vfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.407904 dvcx-0.84.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61693 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.407904 dvcx-0.84.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.407904 dvcx-0.84.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.407904 dvcx-0.84.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.411903 dvcx-0.84.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.411903 dvcx-0.84.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-24 01:02:41.000000 dvcx-0.84.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.423904 dvcx-0.84.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-24 01:02:46.000000 dvcx-0.84.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-24 01:02:46.000000 dvcx-0.84.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:02:46.000000 dvcx-0.84.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 01:02:46.000000 dvcx-0.84.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-24 01:02:46.000000 dvcx-0.84.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 01:02:46.000000 dvcx-0.84.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.411903 dvcx-0.84.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.411903 dvcx-0.84.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16386 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.415903 dvcx-0.84.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112860 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29484 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.415903 dvcx-0.84.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.419903 dvcx-0.84.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.419903 dvcx-0.84.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.423904 dvcx-0.84.0/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:46.423904 dvcx-0.84.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-24 01:02:41.000000 dvcx-0.84.0/tests/utils.py
```

### Comparing `dvcx-0.83.3/.cruft.json` & `dvcx-0.84.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/.github/workflows/benchmarks.yml` & `dvcx-0.84.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/.github/workflows/release.yml` & `dvcx-0.84.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/.github/workflows/tests.yml` & `dvcx-0.84.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/.gitignore` & `dvcx-0.84.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/.pre-commit-config.yaml` & `dvcx-0.84.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/CODE_OF_CONDUCT.rst` & `dvcx-0.84.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/CONTRIBUTING.rst` & `dvcx-0.84.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/LICENSE` & `dvcx-0.84.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/LICENSES/Apache-2.0.txt` & `dvcx-0.84.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/LICENSES/BSD-3-Clause.txt` & `dvcx-0.84.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/LICENSES/Python-2.0.txt` & `dvcx-0.84.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/PKG-INFO` & `dvcx-0.84.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.83.3
+Version: 0.84.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -64,15 +64,14 @@
 Requires-Dist: virtualenv; extra == "tests"
 Requires-Dist: dulwich; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
 Requires-Dist: open_clip_torch; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
-Requires-Dist: requests<2.32.0; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: dvcx[tests]; extra == "dev"
 Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-ujson; extra == "dev"
```

### Comparing `dvcx-0.83.3/README.rst` & `dvcx-0.84.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/docs/udfs.md` & `dvcx-0.84.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/blip2_image_desc_lib.py` & `dvcx-0.84.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/clip.py` & `dvcx-0.84.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/common_sql_functions.py` & `dvcx-0.84.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/dir_expansion.py` & `dvcx-0.84.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/hf_pipeline.py` & `dvcx-0.84.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/llava2_image_desc_lib.py` & `dvcx-0.84.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/llm-claude-aggregate-query.py` & `dvcx-0.84.0/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/llm-claude-simple-query.py` & `dvcx-0.84.0/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/llm-claude.py` & `dvcx-0.84.0/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/loader.py` & `dvcx-0.84.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/neurips/README` & `dvcx-0.84.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/neurips/distance_to_query.py` & `dvcx-0.84.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/neurips/llm_chat.py` & `dvcx-0.84.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/neurips/single_query.py` & `dvcx-0.84.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/neurips/text_loaders.py` & `dvcx-0.84.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/openai_image_desc_lib.py` & `dvcx-0.84.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/openimage-detect.py` & `dvcx-0.84.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/pose_detection.py` & `dvcx-0.84.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/torch-loader.py` & `dvcx-0.84.0/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/udfs/batching.py` & `dvcx-0.84.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/udfs/image_transformation.py` & `dvcx-0.84.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/udfs/parallel.py` & `dvcx-0.84.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/udfs/simple.py` & `dvcx-0.84.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/udfs/stateful.py` & `dvcx-0.84.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/udfs/stateful_similarity.py` & `dvcx-0.84.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/unstructured-text.py` & `dvcx-0.84.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/wds.py` & `dvcx-0.84.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/wds_filtered.py` & `dvcx-0.84.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/wds_meta.py` & `dvcx-0.84.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/zalando/zalando_clip.py` & `dvcx-0.84.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.84.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/noxfile.py` & `dvcx-0.84.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/pyproject.toml` & `dvcx-0.84.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,15 @@
   "pytest-xdist>=3.3.1",
   "virtualenv",
   "dulwich",
   "hypothesis",
   "numpy",
   "open_clip_torch",
   "aiotools>=1.7.0",
-  "requests-mock",
-  "requests<2.32.0"
+  "requests-mock"
 ]
 dev = [
   "dvcx[tests]",
   "mypy==1.10.0",
   "types-python-dateutil",
   "types-PyYAML",
   "types-requests",
```

### Comparing `dvcx-0.83.3/src/dvcx/asyn.py` & `dvcx-0.84.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/cache.py` & `dvcx-0.84.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/catalog/catalog.py` & `dvcx-0.84.0/src/dvcx/catalog/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1403,18 +1403,19 @@
                 f"Dataset {name} doesn't have version {version}"
             )
 
         if version:
             self.remove_dataset_version(dataset, version)
             return
 
-        for version in dataset.versions.copy():  # type: ignore [assignment, union-attr]
+        while dataset.versions:
+            version = dataset.versions[0].version
             self.remove_dataset_version(
                 dataset,
-                version.version,  # type: ignore [union-attr]
+                version,
             )
 
     def edit_dataset(
         self,
         name: str,
         new_name: Optional[str] = None,
         description: Optional[str] = None,
```

### Comparing `dvcx-0.83.3/src/dvcx/catalog/datasource.py` & `dvcx-0.84.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/catalog/loader.py` & `dvcx-0.84.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/cli.py` & `dvcx-0.84.0/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/cli_utils.py` & `dvcx-0.84.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/client/azure.py` & `dvcx-0.84.0/src/dvcx/client/azure.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 class AzureClient(Client):
     FS_CLASS = AzureBlobFileSystem
     PREFIX = "az://"
     protocol = "az"
 
     def convert_info(self, v: dict[str, Any], parent: str) -> Entry:
         version_id = v.get("version_id")
-        checksum = v.get("content_settings", {}).get("content_md5", "")
         name = v.get("name", "").split(DELIMITER)[-1]
         if version_id:
             version_suffix = f"?versionid={version_id}"
             if name.endswith(version_suffix):
                 name = name[: -len(version_suffix)]
         return Entry.from_file(
             parent=parent,
             name=name,
-            checksum=checksum or "",
             etag=v.get("etag", "").strip('"'),
             version=version_id or "",
             is_latest=version_id is None or bool(v.get("is_current_version")),
             last_modified=v["last_modified"],
             size=v.get("size", ""),
         )
```

### Comparing `dvcx-0.83.3/src/dvcx/client/fileslice.py` & `dvcx-0.84.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/client/fsspec.py` & `dvcx-0.84.0/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/client/gcs.py` & `dvcx-0.84.0/src/dvcx/client/gcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import os
-from base64 import b64decode
 from datetime import datetime
 from typing import Any, cast
 
 from dateutil.parser import isoparse
 from gcsfs import GCSFileSystem
 
 from dvcx.node import Entry
@@ -45,14 +44,13 @@
         if "generation" in v:
             gen = f"#{v['generation']}"
             if name.endswith(gen):
                 name = name[: -len(gen)]
         return Entry.from_file(
             parent=parent,
             name=name,
-            checksum=b64decode(v.get("md5Hash", "")).hex(),
             etag=v.get("etag", ""),
             version=v.get("generation", ""),
             is_latest=not v.get("timeDeleted"),
             last_modified=self.parse_timestamp(v["updated"]),
             size=v.get("size", ""),
         )
```

### Comparing `dvcx-0.83.3/src/dvcx/client/local.py` & `dvcx-0.84.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/client/s3.py` & `dvcx-0.84.0/src/dvcx/client/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         files = []
         subdirs = set()
         found = False
         async for info in self.fs._iterdir(self.name, prefix=prefix, versions=True):
             full_path = info["name"]
             _, subprefix, _ = self.fs.split_path(full_path)
             if prefix.strip(DELIMITER) == subprefix.strip(DELIMITER):
+                found = True
                 continue
             if info["type"] == "directory":
                 name = full_path.split(DELIMITER)[-1]
                 await result_queue.put(
                     [Entry.from_dir(prefix.rstrip("/"), name, last_modified=TIME_ZERO)]
                 )
                 subdirs.add(subprefix)
```

### Comparing `dvcx-0.83.3/src/dvcx/config.py` & `dvcx-0.84.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/data_storage/db_engine.py` & `dvcx-0.84.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/data_storage/id_generator.py` & `dvcx-0.84.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/data_storage/metastore.py` & `dvcx-0.84.0/src/dvcx/data_storage/metastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1169,17 +1169,16 @@
             )
         )
 
         if dataset.versions and len(dataset.versions) == 1:
             # had only one version, fully deleting dataset
             self.db.execute(self._datasets_delete().where(d.c.id == dataset.id))
 
-        result_ds = copy.deepcopy(dataset)
-        result_ds.remove_version(version)
-        return result_ds
+        dataset.remove_version(version)
+        return dataset
 
     def update_dataset_status(
         self,
         dataset: DatasetRecord,
         status: int,
         version: Optional[int] = None,
         error_message="",
```

### Comparing `dvcx-0.83.3/src/dvcx/data_storage/schema.py` & `dvcx-0.84.0/src/dvcx/data_storage/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,14 @@
     def dataset_default_columns(cls) -> list[sa.Column]:
         return [
             sa.Column("id", Int, primary_key=True),
             sa.Column("vtype", String, nullable=False, index=True),
             sa.Column("dir_type", Int, index=True),
             sa.Column("parent", String, index=True),
             sa.Column("name", String, nullable=False, index=True),
-            sa.Column("checksum", String),
             sa.Column("etag", String),
             sa.Column("version", String),
             sa.Column("is_latest", Boolean),
             sa.Column("last_modified", DateTime(timezone=True)),
             sa.Column("size", Int64, nullable=False, index=True),
             sa.Column("owner_name", String),
             sa.Column("owner_id", String),
```

### Comparing `dvcx-0.83.3/src/dvcx/data_storage/serializer.py` & `dvcx-0.84.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/data_storage/sqlite.py` & `dvcx-0.84.0/src/dvcx/data_storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/data_storage/warehouse.py` & `dvcx-0.84.0/src/dvcx/data_storage/warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/dataset.py` & `dvcx-0.84.0/src/dvcx/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,15 +487,14 @@
 @attrs.define
 class DatasetRow:
     id: int
     vtype: str
     dir_type: int
     parent: str
     name: str
-    checksum: str
     etag: str
     version: str
     is_latest: bool
     last_modified: Optional[datetime]
     size: int
     owner_name: str
     owner_id: str
@@ -543,15 +542,14 @@
     def to_preview(self):
         return {
             "id": self.id,
             "vtype": self.vtype,
             "dir_type": self.dir_type,
             "parent": self.parent,
             "name": self.name,
-            "checksum": self.checksum,
             "etag": self.etag,
             "version": self.version,
             "is_latest": self.is_latest,
             "last_modified": (
                 self.last_modified.isoformat() if self.last_modified else None
             ),
             "size": self.size,
```

### Comparing `dvcx-0.83.3/src/dvcx/error.py` & `dvcx-0.84.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/cached_stream.py` & `dvcx-0.84.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/claude.py` & `dvcx-0.84.0/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/dataset.py` & `dvcx-0.84.0/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/feature.py` & `dvcx-0.84.0/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/feature_types.py` & `dvcx-0.84.0/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/feature_udf.py` & `dvcx-0.84.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/file.py` & `dvcx-0.84.0/src/dvcx/lib/file.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 from random import getrandbits
 from typing import ClassVar, Optional, Union
 
 from pydantic import Field, field_validator
 
 from dvcx.cache import UniqueId
+from dvcx.client.fileslice import FileSlice
 from dvcx.lib.cached_stream import PreCachedStream, PreDownloadStream
 from dvcx.lib.feature import ShallowFeature
 from dvcx.lib.utils import DvcxError
 from dvcx.utils import TIME_ZERO
 
 
 class FileFeature(ShallowFeature):
@@ -45,16 +46,46 @@
 
     @classmethod
     @abstractmethod
     def open(cls, file: "File", location: list[dict]):
         pass
 
 
+class TarVFile(VFile):
+    @classmethod
+    def get_vtype(cls) -> str:
+        return "tar"
+
+    @classmethod
+    def open(cls, file: "File", location: list[dict]):
+        if len(location) > 1:
+            VFileError(file, "multiple 'location's are not supported yet")
+
+        loc = location[0]
+
+        if (offset := loc.get("offset", None)) is None:
+            VFileError(file, "'offset' is not specified")
+
+        if (size := loc.get("size", None)) is None:
+            VFileError(file, "'size' is not specified")
+
+        if (parent := loc.get("parent", None)) is None:
+            VFileError(file, "'parent' is not specified")
+
+        tar_file = File(**parent)
+        tar_file.set_catalog(file._catalog)
+
+        tar_file_uid = tar_file.get_uid()
+        client = file._catalog.get_client(tar_file_uid.storage)
+        fd = client.open_object(tar_file_uid, use_cache=file._caching_enabled)
+        return FileSlice(fd, offset, size, file.name)
+
+
 class VFileRegistry:
-    _vtype_readers: ClassVar[dict[str, type["VFile"]]] = {}
+    _vtype_readers: ClassVar[dict[str, type["VFile"]]] = {"tar": TarVFile}
 
     @classmethod
     def register(cls, reader: type["VFile"]):
         cls._vtype_readers[reader.get_vtype()] = reader
 
     @classmethod
     def resolve(cls, file: "File", location: list[dict]):
@@ -189,14 +220,13 @@
     dir_type: int = Field(default=0)
     owner_name: str = Field(default="")
     owner_id: str = Field(default="")
     is_latest: bool = Field(default=True)
     last_modified: datetime = Field(default=TIME_ZERO)
     version: str = Field(default="")
     etag: str = Field(default="")
-    checksum: str = Field(default="")
     random: int = Field(default_factory=lambda: getrandbits(63))
 
     @field_validator("location", mode="before")
     @classmethod
     def validate_location(cls, v):
         return File.to_dict(v)
```

### Comparing `dvcx-0.83.3/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.84.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.84.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.84.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/image.py` & `dvcx-0.84.0/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/image_transform.py` & `dvcx-0.84.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.84.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/pytorch.py` & `dvcx-0.84.0/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/reader.py` & `dvcx-0.84.0/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/text.py` & `dvcx-0.84.0/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/udf.py` & `dvcx-0.84.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/unstructured.py` & `dvcx-0.84.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/utils.py` & `dvcx-0.84.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/webdataset.py` & `dvcx-0.84.0/src/dvcx/lib/webdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from collections.abc import Sequence
 from typing import Any, ClassVar, Optional, Union, get_args, get_origin
 
 from pydantic import Field
 
 from dvcx.lib.feature import Feature
 from dvcx.lib.feature_udf import FeatureGenerator
-from dvcx.lib.file import File, FileInfo
-from dvcx.lib.tar_file import TarVFile
+from dvcx.lib.file import File, FileInfo, TarVFile
 from dvcx.lib.utils import DvcxError
 
 
 class WDSError(DvcxError):
     def __init__(self, tar_stream, message: str):
         super().__init__(f"WebDataset error '{tar_stream.get_full_name()}': {message}")
```

### Comparing `dvcx-0.83.3/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.84.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.84.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/listing.py` & `dvcx-0.84.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/node.py` & `dvcx-0.84.0/src/dvcx/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 @attrs.define
 class Node:
     id: int = 0
     vtype: str = ""
     dir_type: Optional[int] = None
     parent: str = ""
     name: str = ""
-    checksum: str = ""
     etag: str = ""
     version: Optional[str] = None
     is_latest: bool = True
     last_modified: Optional[datetime] = None
     size: int = 0
     owner_name: str = ""
     owner_id: str = ""
@@ -121,15 +120,14 @@
 
 @attrs.define
 class Entry:
     vtype: str = ""
     dir_type: Optional[int] = None
     parent: str = ""
     name: str = ""
-    checksum: str = ""
     etag: str = ""
     version: str = ""
     is_latest: bool = True
     last_modified: Optional[datetime] = None
     size: int = 0
     owner_name: str = ""
     owner_id: str = ""
```

### Comparing `dvcx-0.83.3/src/dvcx/nodes_fetcher.py` & `dvcx-0.84.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/nodes_thread_pool.py` & `dvcx-0.84.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/progress.py` & `dvcx-0.84.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/query/batch.py` & `dvcx-0.84.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/query/builtins.py` & `dvcx-0.84.0/src/dvcx/query/builtins.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         C.dir_type,
         C.owner_name,
         C.owner_id,
         C.is_latest,
         C.last_modified,
         C.version,
         C.etag,
-        C.checksum,
         Object(load_tar),
     ),
     DatasetRow.schema,
 )
 def index_tar(
     source,
     name,
@@ -45,15 +44,14 @@
     dir_type,
     owner_name,
     owner_id,
     is_latest,
     last_modified,
     version,
     etag,
-    checksum,
     tar_entries,
 ):
     # generate original tar files as well, along with subobjects
     yield DatasetRow.create(
         name,
         source=source,
         parent=parent,
@@ -62,15 +60,14 @@
         dir_type=dir_type,
         owner_name=owner_name,
         owner_id=owner_id,
         is_latest=bool(is_latest),
         last_modified=last_modified,
         version=version,
         etag=etag,
-        checksum=checksum,
     )
 
     parent_path = name if not parent else f"{parent}/{name}"
     for info in tar_entries:
         if info.isfile():
             full_path = f"{parent_path}/{info.name}"
             parent_dir, name = full_path.rsplit("/", 1)
```

### Comparing `dvcx-0.83.3/src/dvcx/query/dataset.py` & `dvcx-0.84.0/src/dvcx/query/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/query/dispatch.py` & `dvcx-0.84.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/query/params.py` & `dvcx-0.84.0/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/query/schema.py` & `dvcx-0.84.0/src/dvcx/query/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,14 @@
         "dir_type": Int,
         "owner_name": String,
         "owner_id": String,
         "is_latest": Boolean,
         "last_modified": DateTime,
         "version": String,
         "etag": String,
-        "checksum": String,
         # system column
         "random": Int,
     }
 
     @staticmethod
     def create(
         name: str,
@@ -233,30 +232,28 @@
         dir_type: int = 0,
         owner_name: str = "",
         owner_id: str = "",
         is_latest: bool = True,
         last_modified: Optional[datetime] = None,
         version: str = "",
         etag: str = "",
-        checksum: str = "",
     ) -> tuple[
         str,
         str,
         str,
         int,
         Optional[str],
         str,
         int,
         str,
         str,
         bool,
         datetime,
         str,
         str,
-        str,
         int,
     ]:
         if location:
             location = json.dumps([location])  # type: ignore [assignment]
 
         last_modified = last_modified or datetime.now(timezone.utc)
 
@@ -272,15 +269,14 @@
             dir_type,
             owner_name,
             owner_id,
             is_latest,
             last_modified,
             version,
             etag,
-            checksum,
             random,
         )
 
     @staticmethod
     def extend(**columns):
         cols = {**DatasetRow.schema}
         cols.update(columns)
```

### Comparing `dvcx-0.83.3/src/dvcx/query/session.py` & `dvcx-0.84.0/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/query/udf.py` & `dvcx-0.84.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/remote/studio.py` & `dvcx-0.84.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/sql/default/base.py` & `dvcx-0.84.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/sql/functions/array.py` & `dvcx-0.84.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/sql/functions/path.py` & `dvcx-0.84.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/sql/selectable.py` & `dvcx-0.84.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/sql/sqlite/base.py` & `dvcx-0.84.0/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/sql/sqlite/types.py` & `dvcx-0.84.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/sql/types.py` & `dvcx-0.84.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/sql/utils.py` & `dvcx-0.84.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/storage.py` & `dvcx-0.84.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/src/dvcx/utils.py` & `dvcx-0.84.0/src/dvcx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,14 @@
         options.extend(("display.max_columns", None))  # show all columns
         options.extend(("display.max_colwidth", None))  # do not truncate cells
         options.extend(("display.width", None))  #  do not truncate table
 
     if not system_columns:
         df.drop(
             columns=[
-                "checksum",
                 "dir_type",
                 "etag",
                 "is_latest",
                 "last_modified",
                 "owner_id",
                 "owner_name",
                 "size",
```

### Comparing `dvcx-0.83.3/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.84.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.83.3
+Version: 0.84.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -64,15 +64,14 @@
 Requires-Dist: virtualenv; extra == "tests"
 Requires-Dist: dulwich; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
 Requires-Dist: open_clip_torch; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
-Requires-Dist: requests<2.32.0; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: dvcx[tests]; extra == "dev"
 Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: types-ujson; extra == "dev"
```

### Comparing `dvcx-0.83.3/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.84.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 .github/workflows/release.yml
 .github/workflows/tests.yml
 .github/workflows/update-template.yaml
 .reuse/dep5
 LICENSES/Apache-2.0.txt
 LICENSES/BSD-3-Clause.txt
 LICENSES/Python-2.0.txt
+docs/cv_intro.md
 docs/udfs.md
 examples/blip2_image_desc_lib.py
 examples/clip.py
 examples/common_sql_functions.py
 examples/dir_expansion.py
 examples/hf_pipeline.py
 examples/iptc_exif_xmp_lib.py
@@ -113,19 +114,19 @@
 src/dvcx/lib/hf_image_to_text.py
 src/dvcx/lib/hf_pipeline.py
 src/dvcx/lib/image.py
 src/dvcx/lib/image_transform.py
 src/dvcx/lib/iptc_exif_xmp.py
 src/dvcx/lib/pytorch.py
 src/dvcx/lib/reader.py
-src/dvcx/lib/tar_file.py
 src/dvcx/lib/text.py
 src/dvcx/lib/udf.py
 src/dvcx/lib/unstructured.py
 src/dvcx/lib/utils.py
+src/dvcx/lib/vfile.py
 src/dvcx/lib/webdataset.py
 src/dvcx/lib/webdataset_laion.py
 src/dvcx/lib/webdataset_meta.py
 src/dvcx/query/__init__.py
 src/dvcx/query/batch.py
 src/dvcx/query/builtins.py
 src/dvcx/query/dataset.py
```

### Comparing `dvcx-0.83.3/src/dvcx.egg-info/requires.txt` & `dvcx-0.84.0/src/dvcx.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -56,12 +56,11 @@
 virtualenv
 dulwich
 hypothesis
 numpy
 open_clip_torch
 aiotools>=1.7.0
 requests-mock
-requests<2.32.0
 
 [vector]
 numpy
 scipy
```

### Comparing `dvcx-0.83.3/tests/benchmarks/conftest.py` & `dvcx-0.84.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/conftest.py` & `dvcx-0.84.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,14 @@
                 "is_latest": True,
                 "name": f"dql_1m_meta_text_emd.parquet_3_{i}_0.snappy.parquet",
                 "etag": f"72b35c8e9b8eed1636c91eb94241c2f8-{i}",
                 "owner_id": "owner",
                 "owner_name": "aws-iterative-sandbox",
                 "last_modified": "2024-02-23T10:42:31.842944+00:00",
                 "size": 49807360,
-                "checksum": "",
                 "random": 12123123123,
                 "custom": {
                     "int_col": 5,
                     "int_col_32": 5,
                     "int_col_64": 5,
                     "float_col": 0.5,
                     "float_col_32": 0.5,
```

### Comparing `dvcx-0.83.3/tests/data.py` & `dvcx-0.84.0/tests/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,122 +6,112 @@
 TIME_ZERO = datetime.fromtimestamp(0, tz=utc)
 
 ENTRIES = [
     Entry.from_dir(
         parent="",
         name="cats",
         last_modified=TIME_ZERO,
-        checksum="",
         etag="",
         version="",
         is_latest=True,
         size=0,
         owner_name="",
         owner_id="",
     ),
     Entry.from_dir(
         parent="",
         name="dogs",
         last_modified=TIME_ZERO,
-        checksum="",
         etag="",
         version="",
         is_latest=True,
         size=0,
         owner_name="",
         owner_id="",
     ),
     Entry.from_file(
         parent="",
         name="description",
-        checksum="",
         etag="60a7605e934638ab9113e0f9cf852239",
         version="7e589b7d-382c-49a5-931f-2b999c930c5e",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=13,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
     ),
     Entry.from_file(
         parent="cats",
         name="cat1",
-        checksum="",
         etag="4a4be40c96ac6314e91d93f38043a634",
         version="309eb4a4-bba9-47c1-afcd-d7c51110af6f",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
     ),
     Entry.from_file(
         parent="cats",
         name="cat2",
-        checksum="",
         etag="0268c692ff940a830e1e7296aa48c176",
         version="f9d168d3-6d1b-47ef-8f6a-81fce48de141",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
     ),
     Entry.from_dir(
         parent="dogs",
         name="others",
         last_modified=TIME_ZERO,
-        checksum="",
         etag="",
         version="",
         is_latest=True,
         size=0,
         owner_name="",
         owner_id="",
     ),
     Entry.from_file(
         parent="dogs",
         name="dog1",
-        checksum="",
         etag="8fdb60801e9d39a5286aa01dd1f4f4f3",
         version="b9c31cf7-d011-466a-bf16-cf9da0cb422a",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
     ),
     Entry.from_file(
         parent="dogs",
         name="dog2",
-        checksum="",
         etag="2d50c921b22aa164a56c68d71eeb4100",
         version="3a8bb6d9-38db-47a8-8bcb-8972ea95aa20",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=3,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
     ),
     Entry.from_file(
         parent="dogs",
         name="dog3",
-        checksum="",
         etag="33c6c2397a1b079e903c474df792d0e2",
         version="ee49e963-36a8-492a-b03a-e801b93afb40",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
     ),
     Entry.from_file(
         parent="dogs/others",
         name="dog4",
-        checksum="",
         etag="a5e1a5d93ff242b745f5cf87aeb726d5",
         version="c5969421-6900-4060-bc39-d54f4a49b9fc",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
@@ -132,39 +122,36 @@
 #   dogs/others/
 #   dogs/others
 #   dogs/
 INVALID_ENTRIES = [
     Entry.from_file(
         parent="dogs/others",
         name="",
-        checksum="",
         etag="68b329da9893e34099c7d8ad5cb9c940",
         version="85969421-6900-4060-bc39-d54f4a49b9ab",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
     ),
     Entry.from_file(
         parent="dogs",
         name="others",
-        checksum="",
         etag="68b329da9893e34099c7d8ad5cb9c940",
         version="85969421-6900-4060-bc39-d54f4a49b9ab",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
     ),
     Entry.from_file(
         parent="dogs",
         name="",
-        checksum="",
         etag="68b329da9893e34099c7d8ad5cb9c940",
         version="85969421-6900-4060-bc39-d54f4a49b9ab",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
```

### Comparing `dvcx-0.83.3/tests/func/test_catalog.py` & `dvcx-0.84.0/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/func/test_client.py` & `dvcx-0.84.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/func/test_dataset_query.py` & `dvcx-0.84.0/tests/func/test_dataset_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
         )
         result = new_query.results(row_factory=lambda c, v: dict(zip(c, v)))
         dataset_record = catalog.get_dataset(ds_name)
         assert dataset_record.status == DatasetStatus.COMPLETE
     else:
         result = q.results(row_factory=lambda c, v: dict(zip(c, v)))
     assert len(result) == 4
-    assert len(result[0]) == 21
+    assert len(result[0]) == 20
     cols = {"size10x", "size1000x", "s2", "s3", "s4"}
     new_data = [[v for k, v in r.items() if k in cols] for r in result]
     assert new_data == [
         [130, 13000, 26, 39, 52],
         [40, 4000, 8, 12, 16],
         [40, 4000, 8, 12, 16],
         [30, 3000, 6, 9, 12],
@@ -3635,10 +3635,10 @@
     catalog = cloud_test_catalog.catalog
     path = f"{cloud_test_catalog.src_uri}/cats"
     with pytest.raises(RuntimeError) as exc_info:
         DatasetQuery(path=path, catalog=catalog).select(C.name).save("cats", version=1)
 
     assert str(exc_info.value) == (
         "Missing default columns from final query: id, vtype, dir_type, "
-        "parent, checksum, etag, version, is_latest, last_modified, size, "
+        "parent, etag, version, is_latest, last_modified, size, "
         "owner_name, owner_id, random, location, source"
     )
```

### Comparing `dvcx-0.83.3/tests/func/test_datasets.py` & `dvcx-0.84.0/tests/func/test_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,14 +506,30 @@
 
     dataset_table_name = catalog.warehouse.dataset_table_name(dogs_dataset.name, 1)
     assert get_table_row_count(catalog.warehouse.db, dataset_table_name) is None
 
     assert catalog.metastore.get_direct_dataset_dependencies(dogs_dataset, 1) == []
 
 
+def test_remove_dataset_with_multiple_versions(cloud_test_catalog, dogs_dataset):
+    catalog = cloud_test_catalog.catalog
+
+    updated_dogs_dataset = catalog.create_new_dataset_version(dogs_dataset, 2)
+    assert updated_dogs_dataset.has_version(2)
+    assert updated_dogs_dataset.has_version(1)
+
+    catalog.remove_dataset(updated_dogs_dataset.name, force=True)
+    with pytest.raises(DatasetNotFoundError):
+        catalog.get_dataset(updated_dogs_dataset.name)
+
+    assert (
+        catalog.metastore.get_direct_dataset_dependencies(updated_dogs_dataset, 1) == []
+    )
+
+
 def test_remove_dataset_dataset_not_found(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
 
     with pytest.raises(DatasetNotFoundError):
         catalog.remove_dataset("wrong_name", force=True)
```

### Comparing `dvcx-0.83.3/tests/func/test_ls.py` & `dvcx-0.84.0/tests/func/test_ls.py`

 * *Files 4% similar despite different names*

```diff
@@ -278,45 +278,42 @@
 owner_id = "a13a3ff923430363b098ce9c769e450724e74e646332b08ca6b3ac4f96dae083"
 REMOTE_DATA: dict[str, list[dict[str, Any]]] = {
     "": [
         {
             "id": 816,
             "dir_type": 1,
             "name": "cats",
-            "checksum": "",
             "etag": "",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2023, 1, 17, 21, 39, 0, 88564),
             "size": 0,
             "owner_name": "",
             "owner_id": "",
             "path_str": "{src}/cats",
             "path": [],
         },
         {
             "id": 825,
             "dir_type": 1,
             "name": "dogs",
-            "checksum": "",
             "etag": "",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2023, 1, 17, 21, 39, 0, 88567),
             "size": 0,
             "owner_name": "",
             "owner_id": "",
             "path_str": "{src}/dogs",
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
             "name": "description",
-            "checksum": "",
             "etag": "20664550afa2654017377ceb266a1f82",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 2, 10, 3, 39, 9),
             "size": 350496,
             "owner_name": "",
             "owner_id": owner_id,
@@ -325,15 +322,14 @@
         },
     ],
     "dogs/others": [
         {
             "id": None,
             "dir_type": 0,
             "name": "dog4",
-            "checksum": "",
             "etag": "c4e42ce24d92bb5b4c4be9a99b237502",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 32975,
             "owner_name": "",
             "owner_id": owner_id,
@@ -342,45 +338,42 @@
         },
     ],
     "dogs": [
         {
             "id": None,
             "dir_type": 0,
             "name": "dog1",
-            "checksum": "",
             "etag": "44a632238558e0aa4c54bdb901bf9cff",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 101,
             "owner_name": "",
             "owner_id": owner_id,
             "path_str": "{src}/dogs/dog1",
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
             "name": "dog2",
-            "checksum": "",
             "etag": "76556c960239c50e5a8f8569daf85355",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 29759,
             "owner_name": "",
             "owner_id": owner_id,
             "path_str": "{src}/dogs/dog2",
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
             "name": "dog3",
-            "checksum": "",
             "etag": "b1c99fedcf77bf5fa62984e93db1955c",
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 102,
             "owner_name": "",
             "owner_id": owner_id,
```

### Comparing `dvcx-0.83.3/tests/func/test_pull.py` & `dvcx-0.84.0/tests/func/test_pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     return {
         "id": {"type": "UInt64"},
         "vtype": {"type": "String"},
         "dir_type": {"type": "Int32"},
         "parent_id": {"type": "Int64"},
         "parent": {"type": "String"},
         "name": {"type": "String"},
-        "checksum": {"type": "String"},
         "etag": {"type": "String"},
         "version": {"type": "String"},
         "is_latest": {"type": "Boolean"},
         "last_modified": {"type": "DateTime"},
         "size": {"type": "Int64"},
         "owner_name": {"type": "String"},
         "owner_id": {"type": "String"},
```

### Comparing `dvcx-0.83.3/tests/func/test_pytorch.py` & `dvcx-0.84.0/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/func/test_query.py` & `dvcx-0.84.0/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/scripts/name_len_normal.py` & `dvcx-0.84.0/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/scripts/name_len_slow.py` & `dvcx-0.84.0/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/test_cli_e2e.py` & `dvcx-0.84.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/test_query_e2e.py` & `dvcx-0.84.0/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_cached_stream.py` & `dvcx-0.84.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_feature.py` & `dvcx-0.84.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_feature_udf.py` & `dvcx-0.84.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_file.py` & `dvcx-0.84.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_image.py` & `dvcx-0.84.0/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_reader.py` & `dvcx-0.84.0/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_text.py` & `dvcx-0.84.0/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_webdataset.py` & `dvcx-0.84.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.84.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/sql/test_array.py` & `dvcx-0.84.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/sql/test_conditional.py` & `dvcx-0.84.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/sql/test_path.py` & `dvcx-0.84.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/sql/test_selectable.py` & `dvcx-0.84.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/sql/test_string.py` & `dvcx-0.84.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_asyn.py` & `dvcx-0.84.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_cache.py` & `dvcx-0.84.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_catalog.py` & `dvcx-0.84.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_catalog_loader.py` & `dvcx-0.84.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_cli_parsing.py` & `dvcx-0.84.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_client.py` & `dvcx-0.84.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_client_s3.py` & `dvcx-0.84.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_data_storage.py` & `dvcx-0.84.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_database_engine.py` & `dvcx-0.84.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_dataset.py` & `dvcx-0.84.0/tests/unit/test_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         "\n"
         'CREATE TABLE IF NOT EXISTS "ds-1" (\n'
         "\tid INTEGER NOT NULL, \n"
         "\tvtype VARCHAR NOT NULL, \n"
         "\tdir_type INTEGER, \n"
         "\tparent VARCHAR, \n"
         "\tname VARCHAR NOT NULL, \n"
-        "\tchecksum VARCHAR, \n"
         "\tetag VARCHAR, \n"
         "\tversion VARCHAR, \n"
         "\tis_latest BOOLEAN, \n"
         "\tlast_modified DATETIME, \n"
         "\tsize INTEGER NOT NULL, \n"
         "\towner_name VARCHAR, \n"
         "\towner_id VARCHAR, \n"
```

### Comparing `dvcx-0.83.3/tests/unit/test_dataset_row.py` & `dvcx-0.84.0/tests/unit/test_dataset_row.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 def test_dataset_row_from_dict():
     row = DatasetRow(
         id=37,
         vtype="",
         dir_type=1,
         parent="000002",
         name="0000020572.json",
-        checksum="",
         etag="c16a68901b0a3222beccaa53c34a6c0c",
         version="",
         is_latest=True,
         last_modified=datetime.datetime(2022, 12, 27, 1, 16, 57),
         size=625,
         owner_name="",
         owner_id="",
```

### Comparing `dvcx-0.83.3/tests/unit/test_dispatch.py` & `dvcx-0.84.0/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_fileslice.py` & `dvcx-0.84.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_id_generator.py` & `dvcx-0.84.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_listing.py` & `dvcx-0.84.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_metastore.py` & `dvcx-0.84.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_query_params.py` & `dvcx-0.84.0/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_serializer.py` & `dvcx-0.84.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_session.py` & `dvcx-0.84.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_storage.py` & `dvcx-0.84.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_udf.py` & `dvcx-0.84.0/tests/unit/test_udf.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
     row = DatasetRow(
         id=6,
         vtype="",
         dir_type=1,
         parent="",
         name="obj",
-        checksum="",
         last_modified=None,
         etag="",
         version="",
         is_latest=True,
         size=7,
         owner_name="",
         owner_id="",
@@ -41,15 +40,14 @@
 
     row = DatasetRow(
         id=6,
         vtype="",
         dir_type=1,
         parent="",
         name="obj",
-        checksum="",
         last_modified=None,
         etag="",
         version="",
         is_latest=True,
         size=7,
         owner_name="",
         owner_id="",
@@ -71,15 +69,14 @@
     for size, row_id in inputs:
         row = DatasetRow(
             id=row_id,
             vtype="",
             dir_type=1,
             parent="",
             name="obj",
-            checksum="",
             last_modified=None,
             etag="",
             version="",
             is_latest=True,
             size=size,
             owner_name="",
             owner_id="",
@@ -112,15 +109,14 @@
     for size in inputs:
         row = DatasetRow(
             id=5,
             vtype="",
             dir_type=1,
             parent="",
             name="obj",
-            checksum="",
             last_modified=None,
             etag="",
             version="",
             is_latest=True,
             size=size,
             owner_name="",
             owner_id="",
```

### Comparing `dvcx-0.83.3/tests/unit/test_utils.py` & `dvcx-0.84.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/unit/test_warehouse.py` & `dvcx-0.84.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.3/tests/utils.py` & `dvcx-0.84.0/tests/utils.py`

 * *Files identical despite different names*

