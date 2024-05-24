# Comparing `tmp/dvcx-0.83.2.tar.gz` & `tmp/dvcx-0.83.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.83.2.tar", last modified: Wed May 22 12:48:21 2024, max compression
+gzip compressed data, was "dvcx-0.83.3.tar", last modified: Thu May 23 11:23:02 2024, max compression
```

## Comparing `dvcx-0.83.2.tar` & `dvcx-0.83.3.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.152004 dvcx-0.83.2/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-22 12:48:14.000000 dvcx-0.83.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 12:48:14.000000 dvcx-0.83.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.108004 dvcx-0.83.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.108004 dvcx-0.83.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.108004 dvcx-0.83.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 12:48:14.000000 dvcx-0.83.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-22 12:48:14.000000 dvcx-0.83.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 12:48:14.000000 dvcx-0.83.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.108004 dvcx-0.83.2/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 12:48:14.000000 dvcx-0.83.2/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 12:48:14.000000 dvcx-0.83.2/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-22 12:48:14.000000 dvcx-0.83.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-22 12:48:14.000000 dvcx-0.83.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-22 12:48:14.000000 dvcx-0.83.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.112004 dvcx-0.83.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-22 12:48:14.000000 dvcx-0.83.2/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-22 12:48:14.000000 dvcx-0.83.2/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-22 12:48:14.000000 dvcx-0.83.2/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-22 12:48:21.152004 dvcx-0.83.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-22 12:48:14.000000 dvcx-0.83.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.112004 dvcx-0.83.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-22 12:48:14.000000 dvcx-0.83.2/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.116004 dvcx-0.83.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.116004 dvcx-0.83.2/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.116004 dvcx-0.83.2/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.116004 dvcx-0.83.2/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 12:48:14.000000 dvcx-0.83.2/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-22 12:48:14.000000 dvcx-0.83.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-22 12:48:14.000000 dvcx-0.83.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:48:21.152004 dvcx-0.83.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.104004 dvcx-0.83.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.120004 dvcx-0.83.2/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-22 12:48:20.000000 dvcx-0.83.2/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.124004 dvcx-0.83.2/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72918 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.124004 dvcx-0.83.2/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.124004 dvcx-0.83.2/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46796 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24927 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31922 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16819 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.128004 dvcx-0.83.2/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    61232 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.132004 dvcx-0.83.2/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-22 12:48:14.000000 dvcx-0.83.2/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.148004 dvcx-0.83.2/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 12:48:21.000000 dvcx-0.83.2/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.136004 dvcx-0.83.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.136004 dvcx-0.83.2/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.136004 dvcx-0.83.2/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   112876 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    28908 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.140004 dvcx-0.83.2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.144004 dvcx-0.83.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.144004 dvcx-0.83.2/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.144004 dvcx-0.83.2/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:21.148004 dvcx-0.83.2/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-22 12:48:14.000000 dvcx-0.83.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.159850 dvcx-0.83.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-23 11:22:56.000000 dvcx-0.83.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 11:22:56.000000 dvcx-0.83.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.115851 dvcx-0.83.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.115851 dvcx-0.83.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.115851 dvcx-0.83.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 11:22:56.000000 dvcx-0.83.3/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-23 11:22:56.000000 dvcx-0.83.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-23 11:22:56.000000 dvcx-0.83.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.115851 dvcx-0.83.3/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 11:22:56.000000 dvcx-0.83.3/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 11:22:56.000000 dvcx-0.83.3/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-23 11:22:56.000000 dvcx-0.83.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-23 11:22:56.000000 dvcx-0.83.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-23 11:22:56.000000 dvcx-0.83.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.119850 dvcx-0.83.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-23 11:22:56.000000 dvcx-0.83.3/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 11:22:56.000000 dvcx-0.83.3/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-23 11:22:56.000000 dvcx-0.83.3/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-23 11:23:02.159850 dvcx-0.83.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-23 11:22:56.000000 dvcx-0.83.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.119850 dvcx-0.83.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-23 11:22:56.000000 dvcx-0.83.3/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.123850 dvcx-0.83.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.123850 dvcx-0.83.3/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.123850 dvcx-0.83.3/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.123850 dvcx-0.83.3/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 11:22:56.000000 dvcx-0.83.3/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-23 11:22:56.000000 dvcx-0.83.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-23 11:22:56.000000 dvcx-0.83.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:23:02.159850 dvcx-0.83.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.111851 dvcx-0.83.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.127850 dvcx-0.83.3/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 11:23:01.000000 dvcx-0.83.3/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.127850 dvcx-0.83.3/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72880 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.127850 dvcx-0.83.3/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.131850 dvcx-0.83.3/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46796 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24923 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31659 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16764 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.135850 dvcx-0.83.3/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.135850 dvcx-0.83.3/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61693 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.139850 dvcx-0.83.3/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-23 11:22:56.000000 dvcx-0.83.3/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.151850 dvcx-0.83.3/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 11:23:02.000000 dvcx-0.83.3/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.143850 dvcx-0.83.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.143850 dvcx-0.83.3/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.143850 dvcx-0.83.3/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112870 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28908 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.143850 dvcx-0.83.3/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.147850 dvcx-0.83.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.151850 dvcx-0.83.3/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.151850 dvcx-0.83.3/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:23:02.151850 dvcx-0.83.3/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-23 11:22:56.000000 dvcx-0.83.3/tests/utils.py
```

### Comparing `dvcx-0.83.2/.cruft.json` & `dvcx-0.83.3/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'de956df5482ba686b8c4a4f2c53052da59e18d4c'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "12bb835c5034be9af72028ae9c5bd06cf571b9d1",
+    "commit": "de956df5482ba686b8c4a4f2c53052da59e18d4c",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/iterative/py-template",
             "author": "Dmitry Petrov",
             "copyright_year": "2022",
             "development_status": "Development Status :: 2 - Pre-Alpha",
             "docs": "False",
```

### Comparing `dvcx-0.83.2/.github/workflows/benchmarks.yml` & `dvcx-0.83.3/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/.github/workflows/release.yml` & `dvcx-0.83.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/.github/workflows/tests.yml` & `dvcx-0.83.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/.gitignore` & `dvcx-0.83.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/.pre-commit-config.yaml` & `dvcx-0.83.3/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
         exclude: '^LICENSES/'
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.4.4'
+    rev: 'v0.4.5'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.5
     hooks:
```

### Comparing `dvcx-0.83.2/CODE_OF_CONDUCT.rst` & `dvcx-0.83.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/CONTRIBUTING.rst` & `dvcx-0.83.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/LICENSE` & `dvcx-0.83.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/LICENSES/Apache-2.0.txt` & `dvcx-0.83.3/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/LICENSES/BSD-3-Clause.txt` & `dvcx-0.83.3/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/LICENSES/Python-2.0.txt` & `dvcx-0.83.3/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/PKG-INFO` & `dvcx-0.83.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.83.2
+Version: 0.83.3
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.83.2/README.rst` & `dvcx-0.83.3/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/docs/udfs.md` & `dvcx-0.83.3/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/blip2_image_desc_lib.py` & `dvcx-0.83.3/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/clip.py` & `dvcx-0.83.3/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/common_sql_functions.py` & `dvcx-0.83.3/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/dir_expansion.py` & `dvcx-0.83.3/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/hf_pipeline.py` & `dvcx-0.83.3/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/llava2_image_desc_lib.py` & `dvcx-0.83.3/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/llm-claude-aggregate-query.py` & `dvcx-0.83.3/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/llm-claude-simple-query.py` & `dvcx-0.83.3/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/llm-claude.py` & `dvcx-0.83.3/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/loader.py` & `dvcx-0.83.3/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/neurips/README` & `dvcx-0.83.3/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/neurips/distance_to_query.py` & `dvcx-0.83.3/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/neurips/llm_chat.py` & `dvcx-0.83.3/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/neurips/single_query.py` & `dvcx-0.83.3/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/neurips/text_loaders.py` & `dvcx-0.83.3/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/openai_image_desc_lib.py` & `dvcx-0.83.3/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/openimage-detect.py` & `dvcx-0.83.3/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/pose_detection.py` & `dvcx-0.83.3/examples/pose_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
             dir_type=0,
             owner_name=entry.owner_name,
             owner_id=entry.owner_id,
             is_latest=entry.is_latest,
             last_modified=entry.last_modified,
             version=entry.version,
             etag=entry.etag,
-            anno=entry.anno,
         )
 
     def __call__(
         self,
         stream,
         *args,
     ):
```

### Comparing `dvcx-0.83.2/examples/torch-loader.py` & `dvcx-0.83.3/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/udfs/batching.py` & `dvcx-0.83.3/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/udfs/image_transformation.py` & `dvcx-0.83.3/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/udfs/parallel.py` & `dvcx-0.83.3/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/udfs/simple.py` & `dvcx-0.83.3/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/udfs/stateful.py` & `dvcx-0.83.3/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/udfs/stateful_similarity.py` & `dvcx-0.83.3/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/unstructured-text.py` & `dvcx-0.83.3/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/wds.py` & `dvcx-0.83.3/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/wds_filtered.py` & `dvcx-0.83.3/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/wds_meta.py` & `dvcx-0.83.3/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/zalando/zalando_clip.py` & `dvcx-0.83.3/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.83.3/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/noxfile.py` & `dvcx-0.83.3/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 @nox.session
 def lint(session: nox.Session) -> None:
     session.install("pre-commit")
     session.install("-e", ".[dev,vector]")
 
     args = *(session.posargs or ("--show-diff-on-failure",)), "--all-files"
     session.run("pre-commit", "run", *args)
-    session.run("python", "-m", "mypy")
 
 
 @nox.session
 def safety(session: nox.Session) -> None:
     """Scan dependencies for insecure packages."""
     session.install(".[dev]")
     session.install("safety")
```

### Comparing `dvcx-0.83.2/pyproject.toml` & `dvcx-0.83.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,14 @@
 show-fixes = true
 
 [tool.ruff.lint]
 ignore = [
   "S101",  # assert
   "PLR2004",  # magic-value-comparison
   "PLW2901",  # redefined-loop-name
-  "PLC0105",  # type-name-incorrect-variance
   "ISC001",  # single-line-implicit-string-concatenation, incompatible with ruff format
   "RET502",  # implicit-return-value
   "RET503",  # implicit-return
   "SIM105",  # suppressible-exception
   "SIM108",  # if-else-block-instead-of-if-exp
   "SIM117"  # multiple-with-statements
 ]
```

### Comparing `dvcx-0.83.2/src/dvcx/asyn.py` & `dvcx-0.83.3/src/dvcx/asyn.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     TypeVar,
 )
 
 from fsspec.asyn import get_loop
 
 ASYNC_WORKERS = 20
 
-InputT = TypeVar("InputT", contravariant=True)
-ResultT = TypeVar("ResultT", covariant=True)
+InputT = TypeVar("InputT", contravariant=True)  # noqa: PLC0105
+ResultT = TypeVar("ResultT", covariant=True)  # noqa: PLC0105
 
 
 class AsyncMapper(Generic[InputT, ResultT]):
     """
     Asynchronous unordered mapping iterable compatible with fsspec.
 
     `AsyncMapper(func, it)` is roughly equivalent to `map(func, it)`, except
@@ -69,15 +69,15 @@
                 result = await self.func(item)
                 await self.result_queue.put(result)
             finally:
                 self.work_queue.task_done()
 
     async def init(self) -> None:
         self.work_queue = asyncio.Queue(2 * self.workers)
-        self.result_queue: "asyncio.Queue[Optional[ResultT]]" = asyncio.Queue(
+        self.result_queue: asyncio.Queue[Optional[ResultT]] = asyncio.Queue(
             self.workers
         )
 
     async def run(self) -> None:
         producer = self.start_task(self.produce())
         for _i in range(self.workers):
             self.start_task(self.worker())
@@ -175,15 +175,15 @@
         iterable: Iterable[InputT],
         *,
         workers: int = ASYNC_WORKERS,
         loop: Optional[asyncio.AbstractEventLoop] = None,
     ):
         super().__init__(func, iterable, workers=workers, loop=loop)
         self._waiters: dict[int, Any] = {}
-        self._getters: dict[int, "asyncio.Future[Optional[ResultT]]"] = {}
+        self._getters: dict[int, asyncio.Future[Optional[ResultT]]] = {}
         self.heap: list[tuple[int, Optional[ResultT]]] = []
         self._next_yield = 0
         self._items_seen = 0
         self._window = 2 * workers
 
     def _push_result(self, i: int, result: Optional[ResultT]) -> None:
         if i in self._getters:
```

### Comparing `dvcx-0.83.2/src/dvcx/cache.py` & `dvcx-0.83.3/src/dvcx/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from functools import partial
 from typing import TYPE_CHECKING, Optional
 
 import attrs
 from dvc_data.hashfile.db.local import LocalHashFileDB
 from dvc_objects.fs.local import LocalFileSystem
-from fsspec.callbacks import TqdmCallback
+from fsspec.callbacks import Callback, TqdmCallback
 
 from .progress import Tqdm
 
 if TYPE_CHECKING:
     from dvcx.client import Client
     from dvcx.storage import StorageURI
 
@@ -73,47 +73,50 @@
     def path_from_checksum(self, checksum: str) -> str:
         assert checksum
         return self.odb.oid_to_path(checksum)
 
     def remove(self, uid: UniqueId) -> None:
         self.odb.delete(uid.get_hash())
 
-    async def download(self, uid: UniqueId, client: "Client", callback=None) -> None:
+    async def download(
+        self, uid: UniqueId, client: "Client", callback: Optional[Callback] = None
+    ) -> None:
         from_path = f"{uid.storage}/{uid.path}"
         from dvc_objects.fs.utils import tmp_fname
 
         odb_fs = self.odb.fs
         tmp_info = odb_fs.join(self.odb.tmp_dir, tmp_fname())  # type: ignore[arg-type]
         size = uid.size
         if size < 0:
             size = await client.get_size(from_path)
         cb = callback or TqdmCallback(
             tqdm_kwargs={"desc": odb_fs.name(from_path), "bytes": True},
             tqdm_cls=Tqdm,
             size=size,
         )
-        with cb:
+        try:
             await client.get_file(from_path, tmp_info, callback=cb)
+        finally:
+            if not callback:
+                cb.close()
 
         try:
             oid = uid.get_hash()
             self.odb.add(tmp_info, self.odb.fs, oid)
         finally:
             os.unlink(tmp_info)
 
-    def store_data(self, uid: UniqueId, contents: bytes, callback=None) -> None:
+    def store_data(self, uid: UniqueId, contents: bytes) -> None:
         checksum = uid.get_hash()
         dst = self.path_from_checksum(checksum)
         if not os.path.exists(dst):
             # Create the file only if it's not already in cache
             os.makedirs(os.path.dirname(dst), exist_ok=True)
             with open(dst, mode="wb") as f:
                 f.write(contents)
-        if callback:
-            callback.relative_update(len(contents))
 
     def clear(self):
         """
         Completely clear the cache.
         """
         self.odb.clear()
```

### Comparing `dvcx-0.83.2/src/dvcx/catalog/catalog.py` & `dvcx-0.83.3/src/dvcx/catalog/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
 logger = logging.getLogger("dvcx")
 
 DEFAULT_DATASET_DIR = "dataset"
 DATASET_FILE_SUFFIX = ".edvcx"
 
 TTL_INT = 4 * 60 * 60
-PYTHON_SCRIPT_WRAPPER_CODE = "__ds__"
 
 INDEX_INTERNAL_ERROR_MESSAGE = "Internal error on indexing"
 DATASET_INTERNAL_ERROR_MESSAGE = "Internal error on creating dataset"
 # exit code we use if last statement in query script is not instance of DatasetQuery
 QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE = 10
 # exit code we use if query script was canceled
 QUERY_SCRIPT_CANCELED_EXIT_CODE = 11
```

### Comparing `dvcx-0.83.2/src/dvcx/catalog/datasource.py` & `dvcx-0.83.3/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/catalog/loader.py` & `dvcx-0.83.3/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/cli.py` & `dvcx-0.83.3/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/cli_utils.py` & `dvcx-0.83.3/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/client/azure.py` & `dvcx-0.83.3/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/client/fileslice.py` & `dvcx-0.83.3/src/dvcx/client/fileslice.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,53 @@
 import io
 from typing import IO
 
+from fsspec.callbacks import DEFAULT_CALLBACK, Callback
+
+
+class FileWrapper(io.RawIOBase):
+    """Instrumented wrapper around an existing file object.
+
+    It wraps the file's read() method to update the callback with the number of
+    bytes read.
+
+    It assumes exclusive access to the underlying file object and closes it when it
+    gets closed itself.
+    """
+
+    def __init__(self, fileobj, callback: Callback = DEFAULT_CALLBACK):
+        self.fileobj = fileobj
+        self.callback = callback
+
+    def readable(self) -> bool:
+        return True
+
+    def writable(self) -> bool:
+        return False
+
+    def seekable(self) -> bool:
+        return self.fileobj.seekable()
+
+    def tell(self):
+        """Return the current file position."""
+        return self.fileobj.tell()
+
+    def seek(self, position, whence=io.SEEK_SET):
+        """Seek to a position in the file."""
+        return self.fileobj.seek(position, whence)
+
+    def readinto(self, b) -> int:
+        res = self.fileobj.readinto(b)
+        self.callback.relative_update(res)
+        return res
+
+    def close(self):
+        self.fileobj.close()
+        super().close()
+
 
 class FileSlice(io.RawIOBase):
     """A thin wrapper around an existing file object that provides a part of its data
     as an individual file object.
 
     It assumes exclusive access to the underlying file object and closes it when it
     gets closed itself.
```

### Comparing `dvcx-0.83.2/src/dvcx/client/fsspec.py` & `dvcx-0.83.3/src/dvcx/client/fsspec.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     NamedTuple,
     Optional,
 )
 
 from botocore.exceptions import ClientError
 from dvc_objects.fs.system import reflink
 from fsspec.asyn import get_loop, sync
+from fsspec.callbacks import DEFAULT_CALLBACK, Callback
 from tqdm import tqdm
 
 from dvcx.cache import DVCXCache, UniqueId
-from dvcx.client.fileslice import FileSlice
+from dvcx.client.fileslice import FileSlice, FileWrapper
 from dvcx.error import ClientError as DVCXClientError
 from dvcx.node import Entry
 from dvcx.nodes_fetcher import NodesFetcher
 from dvcx.nodes_thread_pool import NodeChunk
 from dvcx.storage import StorageURI
 from dvcx.utils import TIME_ZERO
 
@@ -72,17 +73,15 @@
 
         if url.lower().startswith(ClientS3.PREFIX):
             return ClientS3
         if url.lower().startswith(GCSClient.PREFIX):
             return GCSClient
         if url.lower().startswith(AzureClient.PREFIX):
             return AzureClient
-        if url.lower().startswith(FileClient.PREFIX) or url == "":
-            return FileClient
-        raise RuntimeError(f"Unsupported data source format '{url}'")
+        return FileClient
 
     @staticmethod
     def is_data_source_uri(name: str) -> bool:
         # Returns True if name is one of supported data sources URIs, e.g s3 bucket
         return DATA_SOURCE_URI_PATTERN.match(name) is not None
 
     @staticmethod
@@ -286,21 +285,23 @@
 
         try:
             reflink(src, dst)
         except OSError:
             # Default to copy if reflinks are not supported
             copy2(src, dst)
 
-    def open_object(self, uid: UniqueId, use_cache: bool = True) -> BinaryIO:
+    def open_object(
+        self, uid: UniqueId, use_cache: bool = True, cb: Callback = DEFAULT_CALLBACK
+    ) -> BinaryIO:
         """Open a file, including files in tar archives."""
         if uid.vtype == "tar":
             return self._open_tar(uid, use_cache=True)
         if use_cache and (cache_path := self.cache.get_path(uid)):
             return open(cache_path, mode="rb")  # noqa: SIM115
-        return self.fs.open(self.get_full_path(uid.path))
+        return FileWrapper(self.fs.open(self.get_full_path(uid.path)), cb)  # type: ignore[return-value]
 
     def _open_tar(self, uid: UniqueId, use_cache: bool = True):
         assert uid.location is not None
         loc_stack = (
             json.loads(uid.location) if isinstance(uid.location, str) else uid.location
         )
         if len(loc_stack) > 1:
@@ -317,27 +318,29 @@
             size=-1,
             vtype="",
             location=None,
         )
         f = self.open_object(parent_uid, use_cache=use_cache)
         return FileSlice(f, offset, size, posixpath.basename(uid.path))
 
-    def download(self, uid: UniqueId, *, callback=None) -> None:
+    def download(self, uid: UniqueId, *, callback: Callback = DEFAULT_CALLBACK) -> None:
         sync(get_loop(), functools.partial(self._download, uid, callback=callback))
 
-    async def _download(self, uid: UniqueId, *, callback=None) -> None:
+    async def _download(self, uid: UniqueId, *, callback: "Callback" = None) -> None:
         if self.cache.contains(uid):
             # Already in cache, so there's nothing to do.
             return
         await self._put_in_cache(uid, callback=callback)
 
-    def put_in_cache(self, uid: UniqueId, *, callback=None) -> None:
+    def put_in_cache(self, uid: UniqueId, *, callback: "Callback" = None) -> None:
         sync(get_loop(), functools.partial(self._put_in_cache, uid, callback=callback))
 
-    async def _put_in_cache(self, uid: UniqueId, *, callback=None) -> None:
+    async def _put_in_cache(
+        self, uid: UniqueId, *, callback: "Callback" = None
+    ) -> None:
         if uid.vtype == "tar":
             loop = asyncio.get_running_loop()
             await loop.run_in_executor(
                 None, functools.partial(self._download_from_tar, uid, callback=callback)
             )
             # self._download_from_tar(uid, callback=callback)
             return
@@ -346,11 +349,11 @@
             if uid.etag != etag:
                 raise FileNotFoundError(
                     f"Invalid etag for {uid.storage}/{uid.path}: "
                     f"expected {uid.etag}, got {etag}"
                 )
         await self.cache.download(uid, self, callback=callback)
 
-    def _download_from_tar(self, uid, *, callback=None):
+    def _download_from_tar(self, uid, *, callback: "Callback" = None):
         with self._open_tar(uid, use_cache=False) as f:
             contents = f.read()
-        self.cache.store_data(uid, contents, callback=callback)
+        self.cache.store_data(uid, contents)
```

### Comparing `dvcx-0.83.2/src/dvcx/client/gcs.py` & `dvcx-0.83.3/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/client/local.py` & `dvcx-0.83.3/src/dvcx/client/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import posixpath
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
+from urllib.parse import urlparse
 
 from fsspec.implementations.local import LocalFileSystem
 
 from dvcx.node import Entry
 from dvcx.storage import StorageURI
 
 from .fsspec import Client
@@ -52,29 +53,46 @@
         return Path(FileClient.root_dir())
 
     @classmethod
     def ls_buckets(cls, **kwargs):
         return []
 
     @classmethod
+    def path_to_uri(cls, path: str) -> str:
+        """
+        Resolving path, that can be absolute or relative, to file URI which
+        starts with file:/// prefix
+        In unix like systems we support home shortcut as well.
+        Examples:
+            ./animals -> file:///home/user/working_dir/animals
+            ~/animals -> file:///home/user/animals
+            /home/user/animals -> file:///home/user/animals
+            C:\\windows\animals -> file:///C:/windows/animals
+        """
+        return Path(path).expanduser().absolute().resolve().as_uri()
+
+    @classmethod
     def split_url(cls, url: str) -> tuple[str, str]:
         """
         Splits url into two components:
             1. root of the FS which will later on become the name of the storage
             2. path which will later on become partial path
         Note that URL needs to be have file:/// protocol.
         Examples:
             file:///tmp/dir -> / + tmp/dir
             file:///c:/windows/files -> c:/ + windows/files
         """
-        # scheme / protocol is case insensitive
-        scheme, rest = url.split(":", 1)
-        url = f"{scheme.lower()}:{rest}"
+        parsed = urlparse(url)
+        if parsed.scheme == "file":
+            scheme, rest = url.split(":", 1)
+            uri = f"{scheme.lower()}:{rest}"
+        else:
+            uri = cls.path_to_uri(url)
 
-        return cls.root_dir(), url.removeprefix(cls.root_path().as_uri())
+        return cls.root_dir(), uri.removeprefix(cls.root_path().as_uri())
 
     @classmethod
     def from_name(
         cls, name: str, metastore: "AbstractMetastore", cache, kwargs
     ) -> "FileClient":
         use_symlinks = kwargs.pop("use_symlinks", False)
         return cls(name, cls.create_fs(**kwargs), cache, use_symlinks=use_symlinks)
```

### Comparing `dvcx-0.83.2/src/dvcx/client/s3.py` & `dvcx-0.83.3/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/config.py` & `dvcx-0.83.3/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/data_storage/db_engine.py` & `dvcx-0.83.3/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/data_storage/id_generator.py` & `dvcx-0.83.3/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/data_storage/metastore.py` & `dvcx-0.83.3/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/data_storage/schema.py` & `dvcx-0.83.3/src/dvcx/data_storage/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,15 @@
             row_list[idx] = t.on_read_convert(row_list[idx], dialect)
 
         yield tuple(row_list)
 
 
 class Table:
     def __init__(self, name: str, metadata: Optional["sa.MetaData"] = None):
-        self.metadata: "sa.MetaData" = (
-            metadata if metadata is not None else sa.MetaData()
-        )
+        self.metadata: sa.MetaData = metadata if metadata is not None else sa.MetaData()
         self.name: str = name
 
     def adjust_default_column_types(self, table: "sa.Table") -> None:
         """
         Adjusting types of default columns to be instances of our SQLType since
         when getting table by reflection, that information is lost
         """
@@ -229,15 +227,14 @@
             sa.Column("etag", String),
             sa.Column("version", String),
             sa.Column("is_latest", Boolean),
             sa.Column("last_modified", DateTime(timezone=True)),
             sa.Column("size", Int64, nullable=False, index=True),
             sa.Column("owner_name", String),
             sa.Column("owner_id", String),
-            sa.Column("anno", JSON),
             sa.Column("random", Int64, nullable=False),
             sa.Column("location", JSON),
             sa.Column("source", String, nullable=False),
         ]
 
     @property
     def custom_columns(self) -> list[sa.Column]:
```

### Comparing `dvcx-0.83.2/src/dvcx/data_storage/serializer.py` & `dvcx-0.83.3/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/data_storage/sqlite.py` & `dvcx-0.83.3/src/dvcx/data_storage/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,15 @@
         self,
         id_generator: "SQLiteIDGenerator",
         uri: StorageURI = StorageURI(""),
         partial_id: Optional[int] = None,
         db: Optional["SQLiteDatabaseEngine"] = None,
         db_file: Optional[str] = None,
     ):
-        self.schema: "DefaultSchema" = DefaultSchema()
+        self.schema: DefaultSchema = DefaultSchema()
         super().__init__(id_generator, uri, partial_id)
 
         # needed for dropping tables in correct order for tests because of
         # foreign keys
         self.default_table_names: list[str] = []
 
         self.db = db or SQLiteDatabaseEngine.from_db_file(db_file)
@@ -505,15 +505,15 @@
 
     def __init__(
         self,
         id_generator: "SQLiteIDGenerator",
         db: Optional["SQLiteDatabaseEngine"] = None,
         db_file: Optional[str] = None,
     ):
-        self.schema: "DefaultSchema" = DefaultSchema()
+        self.schema: DefaultSchema = DefaultSchema()
         super().__init__(id_generator)
 
         self.db = db or SQLiteDatabaseEngine.from_db_file(db_file)
 
     def clone(self, use_new_connection: bool = False) -> "SQLiteWarehouse":
         return SQLiteWarehouse(self.id_generator.clone(), db=self.db.clone())
```

### Comparing `dvcx-0.83.2/src/dvcx/data_storage/warehouse.py` & `dvcx-0.83.3/src/dvcx/data_storage/warehouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,19 +39,14 @@
 
 logger = logging.getLogger("dvcx")
 
 RANDOM_BITS = 63  # size of the random integer field
 
 SELECT_BATCH_SIZE = 100_000  # number of rows to fetch at a time
 
-# special string to wrap around dataset name in a user query script stdout, which
-# is run in a Python subprocess, so that we can find it later on after script is
-# done since there is no other way to return results from it
-PYTHON_SCRIPT_WRAPPER_CODE = "__ds__"
-
 
 class AbstractWarehouse(ABC, Serializable):
     """
     Abstract Warehouse class, to be implemented by any Database Adapters
     for a specific database system. This manages the storing, searching, and
     retrieval of datasets data, and has shared logic for all database
     systems currently in use.
```

### Comparing `dvcx-0.83.2/src/dvcx/dataset.py` & `dvcx-0.83.3/src/dvcx/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,15 +495,14 @@
     etag: str
     version: str
     is_latest: bool
     last_modified: Optional[datetime]
     size: int
     owner_name: str
     owner_id: str
-    anno: Optional[str]
     random: int
     location: Optional[str]
     source: "StorageURI"
     custom: Optional[dict] = attrs.field(factory=dict)
 
     @classmethod
     def from_result_row(cls, columns: list[str], values: Iterable[Any]) -> "DatasetRow":
@@ -554,15 +553,14 @@
             "is_latest": self.is_latest,
             "last_modified": (
                 self.last_modified.isoformat() if self.last_modified else None
             ),
             "size": self.size,
             "owner_name": self.owner_name,
             "owner_id": self.owner_id,
-            "anno": self.anno,
             "random": self.random,
             "location": self.location,
             "source": self.source,
             "custom": (
                 json.dumps(self.custom, cls=JSONSerialize) if self.custom else None
             ),
         }
```

### Comparing `dvcx-0.83.2/src/dvcx/error.py` & `dvcx-0.83.3/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/cached_stream.py` & `dvcx-0.83.3/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/claude.py` & `dvcx-0.83.3/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/dataset.py` & `dvcx-0.83.3/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/feature.py` & `dvcx-0.83.3/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/feature_types.py` & `dvcx-0.83.3/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/feature_udf.py` & `dvcx-0.83.3/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/file.py` & `dvcx-0.83.3/src/dvcx/lib/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,13 @@
     owner_name: str = Field(default="")
     owner_id: str = Field(default="")
     is_latest: bool = Field(default=True)
     last_modified: datetime = Field(default=TIME_ZERO)
     version: str = Field(default="")
     etag: str = Field(default="")
     checksum: str = Field(default="")
-    anno: Optional[Union[dict, list[dict]]] = Field(default=None)
     random: int = Field(default_factory=lambda: getrandbits(63))
 
-    @field_validator("location", "anno", mode="before")
+    @field_validator("location", mode="before")
     @classmethod
     def validate_location(cls, v):
         return File.to_dict(v)
```

### Comparing `dvcx-0.83.2/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.83.3/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.83.3/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.83.3/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/image.py` & `dvcx-0.83.3/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/image_transform.py` & `dvcx-0.83.3/src/dvcx/lib/image_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,9 +97,8 @@
             dir_type=record["dir_type"],
             owner_name=entry.owner_name,
             owner_id=entry.owner_id,
             is_latest=record["is_latest"],
             last_modified=entry.last_modified,
             version=entry.version,
             etag=entry.etag,
-            anno=record["anno"],
         )
```

### Comparing `dvcx-0.83.2/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.83.3/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/pytorch.py` & `dvcx-0.83.3/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/reader.py` & `dvcx-0.83.3/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/tar_file.py` & `dvcx-0.83.3/src/dvcx/lib/tar_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/text.py` & `dvcx-0.83.3/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/udf.py` & `dvcx-0.83.3/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/unstructured.py` & `dvcx-0.83.3/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/utils.py` & `dvcx-0.83.3/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/webdataset.py` & `dvcx-0.83.3/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.83.3/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.83.3/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/listing.py` & `dvcx-0.83.3/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/node.py` & `dvcx-0.83.3/src/dvcx/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     etag: str = ""
     version: Optional[str] = None
     is_latest: bool = True
     last_modified: Optional[datetime] = None
     size: int = 0
     owner_name: str = ""
     owner_id: str = ""
-    anno: Optional[str] = None
     random: int = -1
     location: Optional[str] = None
     source: StorageURI = StorageURI("")
 
     @property
     def path(self) -> str:
         return f"{self.parent}/{self.name}" if self.parent else self.name
@@ -130,15 +129,14 @@
     etag: str = ""
     version: str = ""
     is_latest: bool = True
     last_modified: Optional[datetime] = None
     size: int = 0
     owner_name: str = ""
     owner_id: str = ""
-    anno: Optional[str] = None
     location: Optional[str] = None
 
     @property
     def is_dir(self) -> bool:
         return self.dir_type == DirType.DIR
 
     @classmethod
```

### Comparing `dvcx-0.83.2/src/dvcx/nodes_fetcher.py` & `dvcx-0.83.3/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/nodes_thread_pool.py` & `dvcx-0.83.3/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/progress.py` & `dvcx-0.83.3/src/dvcx/progress.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import os
 import re
 import sys
 from threading import RLock
 from typing import Any, ClassVar
 
+from fsspec.callbacks import TqdmCallback
 from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 tqdm.set_lock(RLock())
 
 
 def env2bool(var, undefined=False):
@@ -135,7 +136,14 @@
         if ncols_left:
             d["ncols_desc"] = d["ncols_info"] = ncols_left
         else:
             # work-around for zero-width description
             d["ncols_desc"] = d["ncols_info"] = 1
             d["prefix"] = ""
         return d
+
+
+class CombinedDownloadCallback(TqdmCallback):
+    def set_size(self, size):
+        # This is a no-op to prevent fsspec's .get_file() from setting the combined
+        # download size to the size of the current file.
+        pass
```

### Comparing `dvcx-0.83.2/src/dvcx/query/batch.py` & `dvcx-0.83.3/src/dvcx/query/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         execute: Callable,
         query: sa.sql.selectable.Select,
     ) -> Generator[DatasetRowsBatch, None, None]:
         # choose page size that is a multiple of the batch size
         page_size = math.ceil(SELECT_BATCH_SIZE / self.count) * self.count
 
         # select rows in batches
-        results: list["DatasetRow"] = []
+        results: list[DatasetRow] = []
 
         with contextlib.closing(
             execute(query, page_size=page_size, limit=query._limit)
         ) as rows:
             for row in rows:
                 results.append(row)
                 if len(results) >= self.count:
@@ -90,15 +90,15 @@
 
     def __call__(
         self,
         execute: Callable,
         query: sa.sql.selectable.Select,
     ) -> Generator[DatasetRowsBatch, None, None]:
         current_partition: Optional[int] = None
-        batch: list["DatasetRow"] = []
+        batch: list[DatasetRow] = []
 
         with contextlib.closing(
             execute(query, order_by=(PARTITION_COLUMN_ID, "id"), limit=query._limit)
         ) as rows:
             for row in rows:
                 partition = row[PARTITION_COLUMN_ID]
                 if current_partition != partition:
```

### Comparing `dvcx-0.83.2/src/dvcx/query/builtins.py` & `dvcx-0.83.3/src/dvcx/query/builtins.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         C.owner_name,
         C.owner_id,
         C.is_latest,
         C.last_modified,
         C.version,
         C.etag,
         C.checksum,
-        C.anno,
         Object(load_tar),
     ),
     DatasetRow.schema,
 )
 def index_tar(
     source,
     name,
@@ -47,15 +46,14 @@
     owner_name,
     owner_id,
     is_latest,
     last_modified,
     version,
     etag,
     checksum,
-    anno,
     tar_entries,
 ):
     # generate original tar files as well, along with subobjects
     yield DatasetRow.create(
         name,
         source=source,
         parent=parent,
@@ -65,15 +63,14 @@
         owner_name=owner_name,
         owner_id=owner_id,
         is_latest=bool(is_latest),
         last_modified=last_modified,
         version=version,
         etag=etag,
         checksum=checksum,
-        anno=anno,
     )
 
     parent_path = name if not parent else f"{parent}/{name}"
     for info in tar_entries:
         if info.isfile():
             full_path = f"{parent_path}/{info.name}"
             parent_dir, name = full_path.rsplit("/", 1)
```

### Comparing `dvcx-0.83.2/src/dvcx/query/dataset.py` & `dvcx-0.83.3/src/dvcx/query/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     PARTITION_COLUMN_ID,
     partition_col_names,
     partition_columns,
 )
 from dvcx.dataset import DatasetRow
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetNotFoundError, QueryScriptCancelError
+from dvcx.progress import CombinedDownloadCallback
 from dvcx.sql.functions import rand
 from dvcx.sql.types import SQLType
 from dvcx.storage import Storage, StorageURI
 from dvcx.utils import batched, determine_processes
 
 from .batch import DatasetRowsBatch
 from .schema import C, UDFParamSpec, normalize_param
@@ -369,15 +370,15 @@
     warehouse: "AbstractWarehouse",
     udf_table: "Table",
     udf_results: Iterator[Iterable["UDFResult"]],
     udf: UDFBase,
     batch_size=INSERT_BATCH_SIZE,
     cb: Callback = DEFAULT_CALLBACK,
 ) -> None:
-    rows: list["UDFResult"] = []
+    rows: list[UDFResult] = []
     for udf_output in udf_results:
         if not udf_output:
             continue
         for row in udf_output:
             cb.relative_update()
             rows.append(adjust_outputs(warehouse, row, udf))
             if len(rows) >= batch_size:
@@ -386,31 +387,43 @@
                 rows.clear()
 
     if rows:
         for row_chunk in batched(rows, batch_size):
             warehouse.insert_rows(udf_table, row_chunk)
 
 
+def get_download_callback() -> Callback:
+    return CombinedDownloadCallback(
+        {"desc": "Download", "unit": "B", "unit_scale": True, "unit_divisor": 1024}
+    )
+
+
 def get_processed_callback() -> Callback:
     return TqdmCallback({"desc": "Processed", "unit": " rows"})
 
 
 def get_generated_callback(is_generator: bool = False) -> Callback:
     if is_generator:
         return TqdmCallback({"desc": "Generated", "unit": " rows"})
     return DEFAULT_CALLBACK
 
 
 def run_udf(
-    udf, udf_inputs, catalog, is_generator, cache, cb: Callback = DEFAULT_CALLBACK
+    udf,
+    udf_inputs,
+    catalog,
+    is_generator,
+    cache,
+    download_cb: Callback = DEFAULT_CALLBACK,
+    processed_cb: Callback = DEFAULT_CALLBACK,
 ) -> Iterator[Iterable["UDFResult"]]:
     for batch in udf_inputs:
         n_rows = len(batch.rows) if isinstance(batch, DatasetRowsBatch) else 1
-        output = udf(catalog, batch, is_generator, cache)
-        cb.relative_update(n_rows)
+        output = udf(catalog, batch, is_generator, cache, cb=download_cb)
+        processed_cb.relative_update(n_rows)
         yield output
 
 
 @frozen
 class UDF(Step, ABC):
     udf: UDFType
     catalog: "Catalog"
@@ -519,33 +532,36 @@
                 if hasattr(udf.func, "bootstrap") and callable(udf.func.bootstrap):
                     udf.func.bootstrap()
                 warehouse = self.catalog.warehouse
 
                 with contextlib.closing(
                     batching(warehouse.dataset_select_paginated, query)
                 ) as udf_inputs:
+                    download_cb = get_download_callback()
                     processed_cb = get_processed_callback()
                     generated_cb = get_generated_callback(self.is_generator)
                     try:
                         udf_results = run_udf(
                             udf,
                             udf_inputs,
                             self.catalog,
                             self.is_generator,
                             self.cache,
+                            download_cb,
                             processed_cb,
                         )
                         process_udf_outputs(
                             warehouse,
                             udf_table,
                             udf_results,
                             udf,
                             cb=generated_cb,
                         )
                     finally:
+                        download_cb.close()
                         processed_cb.close()
                         generated_cb.close()
 
                 warehouse.insert_rows_done(udf_table)
 
                 if hasattr(udf.func, "teardown") and callable(udf.func.teardown):
                     udf.func.teardown()
@@ -1046,15 +1062,15 @@
         version: Optional[int] = None,
         catalog: Optional["Catalog"] = None,
         client_config=None,
         recursive: Optional[bool] = True,
         session: Optional[Session] = None,
         anon: bool = False,
     ):
-        self.steps: list["Step"] = []
+        self.steps: list[Step] = []
         self.catalog = catalog or get_catalog(client_config=client_config)
         self._chunk_index: Optional[int] = None
         self._chunk_total: Optional[int] = None
         self.temp_table_names: list[str] = []
         self.dependencies: set[DatasetDependencyType] = set()
         self.table = self.get_table()
         self.starting_step: StartingStep
@@ -1637,15 +1653,15 @@
             ]
             if missing_default_columns:
                 raise RuntimeError(
                     'Missing default columns from final query: '
                     f'{", ".join(missing_default_columns)}'
                 )
 
-            custom_columns: list["sqlalchemy.Column"] = [
+            custom_columns: list[sqlalchemy.Column] = [
                 sqlalchemy.Column(col.name, col.type)
                 for col in query.columns
                 if col.name not in DATASET_CORE_COLUMN_NAMES
             ]
 
             dataset = self.catalog.create_dataset(
                 name,
```

### Comparing `dvcx-0.83.2/src/dvcx/query/dispatch.py` & `dvcx-0.83.3/src/dvcx/query/dispatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,37 @@
 from multiprocessing import cpu_count
 from queue import Empty, Full, Queue
 from sys import stdin
 from time import sleep
 from types import GeneratorType
 from typing import Any, Optional
 
+import attrs
+import multiprocess
 from dill import load
 from fsspec.callbacks import DEFAULT_CALLBACK, Callback
 from multiprocess import get_context
 
 from dvcx.catalog import Catalog
 from dvcx.catalog.loader import get_distributed_class
 from dvcx.query.batch import DatasetRowsBatch
 from dvcx.query.dataset import (
+    get_download_callback,
     get_generated_callback,
     get_processed_callback,
     process_udf_outputs,
 )
-from dvcx.query.udf import UDFFactory, UDFResult
+from dvcx.query.udf import UDFBase, UDFFactory, UDFResult
 
 DEFAULT_BATCH_SIZE = 10000
 STOP_SIGNAL = "STOP"
 OK_STATUS = "OK"
 FINISHED_STATUS = "FINISHED"
 FAILED_STATUS = "FAILED"
+NOTIFY_STATUS = "NOTIFY"
 
 
 def full_module_type_path(typ: type) -> str:
     return f"{typ.__module__}.{typ.__qualname__}"
 
 
 def get_n_workers_from_arg(n_workers: Optional[int] = None) -> int:
@@ -109,22 +113,27 @@
     if n_workers is True:
         # Use default number of CPUs (cores)
         n_workers = None
 
     with contextlib.closing(
         batching(warehouse.dataset_select_paginated, query)
     ) as udf_inputs:
+        download_cb = get_download_callback()
         processed_cb = get_processed_callback()
         generated_cb = get_generated_callback(dispatch.is_generator)
         try:
             udf_results = dispatch.run_udf_parallel(
-                udf_inputs, n_workers=n_workers, cb=processed_cb
+                udf_inputs,
+                n_workers=n_workers,
+                processed_cb=processed_cb,
+                download_cb=download_cb,
             )
             process_udf_outputs(warehouse, table, udf_results, udf, cb=generated_cb)
         finally:
+            download_cb.close()
             processed_cb.close()
             generated_cb.close()
 
     warehouse.insert_rows_done(table)
 
     return 0
 
@@ -170,15 +179,14 @@
             self.warehouse_class,
             self.warehouse_args,
             self.warehouse_kwargs,
         ) = warehouse_clone_params
         self.is_generator = is_generator
         self.cache = cache
         self.catalog = None
-        self.initialized = False
         self.task_queue = None
         self.done_queue = None
         self.buffer_size = buffer_size
         self.ctx = get_context("spawn")
 
     @property
     def batch_size(self):
@@ -189,15 +197,15 @@
                 self.udf.properties, "batch"
             ):
                 self._batch_size = self.udf.properties.batch
             else:
                 self._batch_size = 1
         return self._batch_size
 
-    def _init_worker(self):
+    def _create_worker(self) -> "UDFWorker":
         if not self.catalog:
             id_generator = self.id_generator_class(
                 *self.id_generator_args, **self.id_generator_kwargs
             )
             metastore = self.metastore_class(
                 *self.metastore_args, **self.metastore_kwargs
             )
@@ -206,47 +214,31 @@
             )
             self.catalog = Catalog(
                 id_generator, metastore, warehouse, **self.catalog_init_params
             )
         if not self.udf:
             self.udf = self.udf_factory()
 
-        if hasattr(self.udf.func, "bootstrap") and callable(self.udf.func.bootstrap):
-            self.udf.func.bootstrap()
-
-        self.initialized = True
+        return UDFWorker(
+            self.catalog,
+            self.udf,
+            self.task_queue,
+            self.done_queue,
+            self.is_generator,
+            self.cache,
+        )
 
-    def _run_worker(self):
+    def _run_worker(self) -> None:
         try:
-            self._init_worker()
-            while (batch := get_from_queue(self.task_queue)) != STOP_SIGNAL:
-                n_rows = len(batch.rows) if isinstance(batch, DatasetRowsBatch) else 1
-                udf_output = self._call_udf(batch)
-                if isinstance(udf_output, GeneratorType):
-                    udf_output = list(udf_output)  # can not pickle generator
-                put_into_queue(
-                    self.done_queue,
-                    {"status": OK_STATUS, "result": udf_output, "processed": n_rows},
-                )
-
-            if hasattr(self.udf.func, "teardown") and callable(self.udf.func.teardown):
-                self.udf.func.teardown()
-
-            put_into_queue(self.done_queue, {"status": FINISHED_STATUS})
+            worker = self._create_worker()
+            worker.run()
         except (Exception, KeyboardInterrupt) as e:
             put_into_queue(self.done_queue, {"status": FAILED_STATUS, "exception": e})
             raise
 
-    def _call_udf(self, row):
-        if not self.initialized:
-            raise RuntimeError("Internal Error: Attempted to call uninitialized UDF!")
-        return self.udf(
-            self.catalog, row, is_generator=self.is_generator, cache=self.cache
-        )
-
     @staticmethod
     def send_stop_signal_to_workers(task_queue, n_workers: Optional[int] = None):
         n_workers = get_n_workers_from_arg(n_workers)
         for _ in range(n_workers):
             put_into_queue(task_queue, STOP_SIGNAL)
 
     def create_input_queue(self):
@@ -254,15 +246,16 @@
 
     def run_udf_parallel(  # noqa: C901, PLR0912
         self,
         input_rows,
         n_workers: Optional[int] = None,
         cache: bool = False,
         input_queue=None,
-        cb: Callback = DEFAULT_CALLBACK,
+        processed_cb: Callback = DEFAULT_CALLBACK,
+        download_cb: Callback = DEFAULT_CALLBACK,
     ) -> Iterator[Sequence[UDFResult]]:
         n_workers = get_n_workers_from_arg(n_workers)
 
         if self.buffer_size < n_workers:
             raise RuntimeError(
                 f"Parallel run error: buffer size is smaller than "
                 f"number of workers: {self.buffer_size} < {n_workers}"
@@ -300,19 +293,21 @@
                         input_finished = True
                         break
 
             # Process all tasks
             while n_workers > 0:
                 result = get_from_queue(self.done_queue)
                 status = result["status"]
-                if status == FINISHED_STATUS:
+                if status == NOTIFY_STATUS:
+                    download_cb.relative_update(result["downloaded"])
+                elif status == FINISHED_STATUS:
                     # Worker finished
                     n_workers -= 1
                 elif status == OK_STATUS:
-                    cb.relative_update(result["processed"])
+                    processed_cb.relative_update(result["processed"])
                     yield result["result"]
                 else:  # Failed / error
                     n_workers -= 1
                     exc = result.get("exception")
                     if exc:
                         raise exc
                     raise RuntimeError("Internal error: Parallel UDF execution failed")
@@ -345,7 +340,54 @@
                     status = result["status"]
                     if status != OK_STATUS:
                         n_workers -= 1
 
             # Wait for workers to stop
             for p in pool:
                 p.join()
+
+
+class WorkerCallback(Callback):
+    def __init__(self, queue: multiprocess.Queue):
+        self.queue = queue
+
+    def relative_update(self, inc: int = 1) -> None:
+        put_into_queue(self.queue, {"status": NOTIFY_STATUS, "downloaded": inc})
+
+
+@attrs.define
+class UDFWorker:
+    catalog: Catalog
+    udf: UDFBase
+    task_queue: multiprocess.Queue
+    done_queue: multiprocess.Queue
+    is_generator: bool
+    cache: bool
+    cb: Callback = attrs.field()
+
+    @cb.default
+    def _default_callback(self) -> WorkerCallback:
+        return WorkerCallback(self.done_queue)
+
+    def run(self) -> None:
+        if hasattr(self.udf.func, "bootstrap") and callable(self.udf.func.bootstrap):
+            self.udf.func.bootstrap()
+        while (batch := get_from_queue(self.task_queue)) != STOP_SIGNAL:
+            n_rows = len(batch.rows) if isinstance(batch, DatasetRowsBatch) else 1
+            udf_output = self.udf(
+                self.catalog,
+                batch,
+                is_generator=self.is_generator,
+                cache=self.cache,
+                cb=self.cb,
+            )
+            if isinstance(udf_output, GeneratorType):
+                udf_output = list(udf_output)  # can not pickle generator
+            put_into_queue(
+                self.done_queue,
+                {"status": OK_STATUS, "result": udf_output, "processed": n_rows},
+            )
+
+        if hasattr(self.udf.func, "teardown") and callable(self.udf.func.teardown):
+            self.udf.func.teardown()
+
+        put_into_queue(self.done_queue, {"status": FINISHED_STATUS})
```

### Comparing `dvcx-0.83.2/src/dvcx/query/params.py` & `dvcx-0.83.3/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/query/schema.py` & `dvcx-0.83.3/src/dvcx/query/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import datetime, timezone
 from fnmatch import fnmatch
 from random import getrandbits
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Optional, Union
 
 import attrs
 import sqlalchemy as sa
+from fsspec.callbacks import DEFAULT_CALLBACK, Callback
 
 from dvcx.data_storage.warehouse import RANDOM_BITS
 from dvcx.sql.types import JSON, Boolean, DateTime, Int, SQLType, String
 
 if TYPE_CHECKING:
     from dvcx.catalog import Catalog
     from dvcx.dataset import DatasetRow as Row
@@ -59,59 +60,87 @@
     Object is used as a placeholder parameter to indicate the actual stored object
     being passed as a parameter to the UDF.
     """
 
     reader: Callable
 
     def get_value(
-        self, catalog: "Catalog", row: "Row", *, cache: bool = False, **kwargs
+        self,
+        catalog: "Catalog",
+        row: "Row",
+        *,
+        cache: bool = False,
+        cb: Callback = DEFAULT_CALLBACK,
+        **kwargs,
     ) -> Any:
         client = catalog.get_client(row.source)
         uid = row.as_uid()
         if cache:
-            client.download(uid)
-        with client.open_object(uid, use_cache=cache) as f:
+            client.download(uid, callback=cb)
+        with client.open_object(uid, use_cache=cache, cb=cb) as f:
             return self.reader(f)
 
     async def get_value_async(
-        self, catalog: "Catalog", row: "Row", mapper, *, cache: bool = False, **kwargs
+        self,
+        catalog: "Catalog",
+        row: "Row",
+        mapper,
+        *,
+        cache: bool = False,
+        cb: Callback = DEFAULT_CALLBACK,
+        **kwargs,
     ) -> Any:
         client = catalog.get_client(row.source)
         uid = row.as_uid()
         if cache:
-            await client._download(uid)
+            await client._download(uid, callback=cb)
         obj = await mapper.to_thread(
-            functools.partial(client.open_object, uid, use_cache=cache)
+            functools.partial(client.open_object, uid, use_cache=cache, cb=cb)
         )
         with obj:
             return await mapper.to_thread(self.reader, obj)
 
 
 @attrs.define(slots=False)
 class Stream(UDFParameter):
     """
     A Stream() parameter receives a binary stream over the object contents.
     """
 
-    def get_value(self, catalog, row, *, cache=False, **kwargs) -> Any:
+    def get_value(
+        self,
+        catalog: "Catalog",
+        row: "Row",
+        *,
+        cache: bool = False,
+        cb: Callback = DEFAULT_CALLBACK,
+        **kwargs,
+    ) -> Any:
         client = catalog.get_client(row.source)
         uid = row.as_uid()
         if cache:
-            client.download(uid)
-        return client.open_object(uid, use_cache=cache)
+            client.download(uid, callback=cb)
+        return client.open_object(uid, use_cache=cache, cb=cb)
 
     async def get_value_async(
-        self, catalog, row, mapper, *, cache=False, **kwargs
+        self,
+        catalog: "Catalog",
+        row: "Row",
+        mapper,
+        *,
+        cache: bool = False,
+        cb: Callback = DEFAULT_CALLBACK,
+        **kwargs,
     ) -> Any:
         client = catalog.get_client(row.source)
         uid = row.as_uid()
         if cache:
-            await client._download(uid)
+            await client._download(uid, callback=cb)
         return await mapper.to_thread(
-            functools.partial(client.open_object, uid, use_cache=cache)
+            functools.partial(client.open_object, uid, use_cache=cache, cb=cb)
         )
 
 
 @attrs.define(slots=False)
 class LocalFilename(UDFParameter):
     """
     Placeholder parameter representing the local path to a cached copy of the object.
@@ -119,34 +148,48 @@
     If glob is None, then all files will be returned. If glob is specified,
     then only files matching the glob will be returned,
     otherwise None will be returned.
     """
 
     glob: Optional[str] = None
 
-    def get_value(self, catalog: "Catalog", row: "Row", **kwargs) -> Optional[str]:
+    def get_value(
+        self,
+        catalog: "Catalog",
+        row: "Row",
+        *,
+        cb: Callback = DEFAULT_CALLBACK,
+        **kwargs,
+    ) -> Optional[str]:
         if self.glob and not fnmatch(row.name, self.glob):  # type: ignore[type-var]
             # If the glob pattern is specified and the row filename
             # does not match it, then return None
             return None
         client = catalog.get_client(row.source)
         uid = row.as_uid()
-        client.download(uid)
+        client.download(uid, callback=cb)
         return client.cache.get_path(uid)
 
     async def get_value_async(
-        self, catalog: "Catalog", row: "Row", mapper, **kwargs
+        self,
+        catalog: "Catalog",
+        row: "Row",
+        mapper,
+        *,
+        cache: bool = False,
+        cb: Callback = DEFAULT_CALLBACK,
+        **kwargs,
     ) -> Optional[str]:
         if self.glob and not fnmatch(row.name, self.glob):  # type: ignore[type-var]
             # If the glob pattern is specified and the row filename
             # does not match it, then return None
             return None
         client = catalog.get_client(row.source)
         uid = row.as_uid()
-        await client._download(uid)
+        await client._download(uid, callback=cb)
         return client.cache.get_path(uid)
 
 
 UDFParamSpec = Union[str, Column, UDFParameter]
 
 
 def normalize_param(param: UDFParamSpec) -> UDFParameter:
@@ -171,15 +214,14 @@
         "owner_name": String,
         "owner_id": String,
         "is_latest": Boolean,
         "last_modified": DateTime,
         "version": String,
         "etag": String,
         "checksum": String,
-        "anno": JSON,
         # system column
         "random": Int,
     }
 
     @staticmethod
     def create(
         name: str,
@@ -192,15 +234,14 @@
         owner_name: str = "",
         owner_id: str = "",
         is_latest: bool = True,
         last_modified: Optional[datetime] = None,
         version: str = "",
         etag: str = "",
         checksum: str = "",
-        anno: Optional[dict[str, Any]] = None,
     ) -> tuple[
         str,
         str,
         str,
         int,
         Optional[str],
         str,
@@ -208,23 +249,19 @@
         str,
         str,
         bool,
         datetime,
         str,
         str,
         str,
-        Optional[str],
         int,
     ]:
         if location:
             location = json.dumps([location])  # type: ignore [assignment]
 
-        if anno:
-            anno = json.dumps(anno)  # type: ignore [assignment]
-
         last_modified = last_modified or datetime.now(timezone.utc)
 
         random = getrandbits(RANDOM_BITS)
 
         return (  # type: ignore [return-value]
             source,
             parent,
@@ -236,15 +273,14 @@
             owner_name,
             owner_id,
             is_latest,
             last_modified,
             version,
             etag,
             checksum,
-            anno,
             random,
         )
 
     @staticmethod
     def extend(**columns):
         cols = {**DatasetRow.schema}
         cols.update(columns)
```

### Comparing `dvcx-0.83.2/src/dvcx/query/session.py` & `dvcx-0.83.3/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/query/udf.py` & `dvcx-0.83.3/src/dvcx/query/udf.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Optional,
     Union,
 )
 
+from fsspec.callbacks import DEFAULT_CALLBACK, Callback
+
 from dvcx.dataset import DatasetRow
 
 from .batch import Batch, BatchingStrategy, DatasetRowsBatch, NoBatching, Partition
 from .schema import (
     UDFParameter,
     UDFParamSpec,
     normalize_param,
@@ -116,23 +118,25 @@
 
     def __call__(
         self,
         catalog: "Catalog",
         param: "BatchingResult",
         is_generator: bool = False,
         cache: bool = False,
+        cb: Callback = DEFAULT_CALLBACK,
     ) -> Iterable[UDFResult]:
         if isinstance(param, DatasetRowsBatch):
             udf_inputs = [
-                self.parameter_parser(catalog, row, cache=cache) for row in param.rows
+                self.parameter_parser(catalog, row, cache=cache, cb=cb)
+                for row in param.rows
             ]
             udf_outputs = self.func(udf_inputs)
             return self._process_results(param.rows, udf_outputs, is_generator)
         if isinstance(param, DatasetRow):
-            udf_inputs = self.parameter_parser(catalog, param, cache=cache)
+            udf_inputs = self.parameter_parser(catalog, param, cache=cache, cb=cb)
             udf_outputs = self.func(*udf_inputs)
             if not is_generator:
                 # udf_outputs is generator already if is_generator=True
                 udf_outputs = [udf_outputs]
             return self._process_results([param], udf_outputs, is_generator)
         raise ValueError(f"unexpected UDF parameter {param}")
```

### Comparing `dvcx-0.83.2/src/dvcx/remote/studio.py` & `dvcx-0.83.3/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/sql/default/base.py` & `dvcx-0.83.3/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/sql/functions/array.py` & `dvcx-0.83.3/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/sql/functions/path.py` & `dvcx-0.83.3/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/sql/selectable.py` & `dvcx-0.83.3/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/sql/sqlite/base.py` & `dvcx-0.83.3/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/sql/sqlite/types.py` & `dvcx-0.83.3/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/sql/types.py` & `dvcx-0.83.3/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/sql/utils.py` & `dvcx-0.83.3/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/storage.py` & `dvcx-0.83.3/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/src/dvcx/utils.py` & `dvcx-0.83.3/src/dvcx/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,14 @@
         options.extend(("display.max_columns", None))  # show all columns
         options.extend(("display.max_colwidth", None))  # do not truncate cells
         options.extend(("display.width", None))  #  do not truncate table
 
     if not system_columns:
         df.drop(
             columns=[
-                "anno",
                 "checksum",
                 "dir_type",
                 "etag",
                 "is_latest",
                 "last_modified",
                 "owner_id",
                 "owner_name",
```

### Comparing `dvcx-0.83.2/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.83.3/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.83.2
+Version: 0.83.3
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.83.2/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.83.3/src/dvcx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 CONTRIBUTING.rst
 LICENSE
 README.rst
 noxfile.py
 pyproject.toml
 .github/codecov.yaml
 .github/dependabot.yml
-.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/bug_report.yml
 .github/ISSUE_TEMPLATE/empty_issue.md
-.github/ISSUE_TEMPLATE/epic-or-story.md
+.github/ISSUE_TEMPLATE/feature_request.yml
 .github/workflows/benchmarks.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 .github/workflows/update-template.yaml
 .reuse/dep5
 LICENSES/Apache-2.0.txt
 LICENSES/BSD-3-Clause.txt
```

### Comparing `dvcx-0.83.2/src/dvcx.egg-info/requires.txt` & `dvcx-0.83.3/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/benchmarks/conftest.py` & `dvcx-0.83.3/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/conftest.py` & `dvcx-0.83.3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,15 +521,14 @@
                 "name": f"dql_1m_meta_text_emd.parquet_3_{i}_0.snappy.parquet",
                 "etag": f"72b35c8e9b8eed1636c91eb94241c2f8-{i}",
                 "owner_id": "owner",
                 "owner_name": "aws-iterative-sandbox",
                 "last_modified": "2024-02-23T10:42:31.842944+00:00",
                 "size": 49807360,
                 "checksum": "",
-                "anno": None,
                 "random": 12123123123,
                 "custom": {
                     "int_col": 5,
                     "int_col_32": 5,
                     "int_col_64": 5,
                     "float_col": 0.5,
                     "float_col_32": 0.5,
```

### Comparing `dvcx-0.83.2/tests/data.py` & `dvcx-0.83.3/tests/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,41 +37,38 @@
         etag="60a7605e934638ab9113e0f9cf852239",
         version="7e589b7d-382c-49a5-931f-2b999c930c5e",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=13,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
     Entry.from_file(
         parent="cats",
         name="cat1",
         checksum="",
         etag="4a4be40c96ac6314e91d93f38043a634",
         version="309eb4a4-bba9-47c1-afcd-d7c51110af6f",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
     Entry.from_file(
         parent="cats",
         name="cat2",
         checksum="",
         etag="0268c692ff940a830e1e7296aa48c176",
         version="f9d168d3-6d1b-47ef-8f6a-81fce48de141",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
     Entry.from_dir(
         parent="dogs",
         name="others",
         last_modified=TIME_ZERO,
         checksum="",
         etag="",
@@ -88,54 +85,50 @@
         etag="8fdb60801e9d39a5286aa01dd1f4f4f3",
         version="b9c31cf7-d011-466a-bf16-cf9da0cb422a",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
     Entry.from_file(
         parent="dogs",
         name="dog2",
         checksum="",
         etag="2d50c921b22aa164a56c68d71eeb4100",
         version="3a8bb6d9-38db-47a8-8bcb-8972ea95aa20",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=3,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
     Entry.from_file(
         parent="dogs",
         name="dog3",
         checksum="",
         etag="33c6c2397a1b079e903c474df792d0e2",
         version="ee49e963-36a8-492a-b03a-e801b93afb40",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
     Entry.from_file(
         parent="dogs/others",
         name="dog4",
         checksum="",
         etag="a5e1a5d93ff242b745f5cf87aeb726d5",
         version="c5969421-6900-4060-bc39-d54f4a49b9fc",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
 ]
 
 # files with directory name collisions:
 #   dogs/others/
 #   dogs/others
 #   dogs/
@@ -147,36 +140,33 @@
         etag="68b329da9893e34099c7d8ad5cb9c940",
         version="85969421-6900-4060-bc39-d54f4a49b9ab",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
     Entry.from_file(
         parent="dogs",
         name="others",
         checksum="",
         etag="68b329da9893e34099c7d8ad5cb9c940",
         version="85969421-6900-4060-bc39-d54f4a49b9ab",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
     Entry.from_file(
         parent="dogs",
         name="",
         checksum="",
         etag="68b329da9893e34099c7d8ad5cb9c940",
         version="85969421-6900-4060-bc39-d54f4a49b9ab",
         is_latest=True,
         last_modified=datetime(2023, 2, 27, 18, 28, 54, tzinfo=utc),
         size=4,
         owner_name="webfile",
         owner_id="75aa57f09aa0c8caeab4f8c24e99d10f8e7faeebf76c078efc7c6caea54ba06a",
-        anno=None,
     ),
 ]
```

### Comparing `dvcx-0.83.2/tests/func/test_catalog.py` & `dvcx-0.83.3/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/func/test_client.py` & `dvcx-0.83.3/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/func/test_dataset_query.py` & `dvcx-0.83.3/tests/func/test_dataset_query.py`

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
-    assert len(result[0]) == 22
+    assert len(result[0]) == 21
     cols = {"size10x", "size1000x", "s2", "s3", "s4"}
     new_data = [[v for k, v in r.items() if k in cols] for r in result]
     assert new_data == [
         [130, 13000, 26, 39, 52],
         [40, 4000, 8, 12, 16],
         [40, 4000, 8, 12, 16],
         [30, 3000, 6, 9, 12],
@@ -3636,9 +3636,9 @@
     path = f"{cloud_test_catalog.src_uri}/cats"
     with pytest.raises(RuntimeError) as exc_info:
         DatasetQuery(path=path, catalog=catalog).select(C.name).save("cats", version=1)
 
     assert str(exc_info.value) == (
         "Missing default columns from final query: id, vtype, dir_type, "
         "parent, checksum, etag, version, is_latest, last_modified, size, "
-        "owner_name, owner_id, anno, random, location, source"
+        "owner_name, owner_id, random, location, source"
     )
```

### Comparing `dvcx-0.83.2/tests/func/test_datasets.py` & `dvcx-0.83.3/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/func/test_ls.py` & `dvcx-0.83.3/tests/func/test_ls.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,15 +287,14 @@
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2023, 1, 17, 21, 39, 0, 88564),
             "size": 0,
             "owner_name": "",
             "owner_id": "",
             "path_str": "{src}/cats",
-            "anno": None,
             "path": [],
         },
         {
             "id": 825,
             "dir_type": 1,
             "name": "dogs",
             "checksum": "",
@@ -303,15 +302,14 @@
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2023, 1, 17, 21, 39, 0, 88567),
             "size": 0,
             "owner_name": "",
             "owner_id": "",
             "path_str": "{src}/dogs",
-            "anno": None,
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
             "name": "description",
             "checksum": "",
@@ -319,15 +317,14 @@
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 2, 10, 3, 39, 9),
             "size": 350496,
             "owner_name": "",
             "owner_id": owner_id,
             "path_str": "{src}/description",
-            "anno": None,
             "path": [],
         },
     ],
     "dogs/others": [
         {
             "id": None,
             "dir_type": 0,
@@ -337,15 +334,14 @@
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 32975,
             "owner_name": "",
             "owner_id": owner_id,
             "path_str": "{src}/dogs/others/dog4",
-            "anno": None,
             "path": [],
         },
     ],
     "dogs": [
         {
             "id": None,
             "dir_type": 0,
@@ -355,15 +351,14 @@
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 101,
             "owner_name": "",
             "owner_id": owner_id,
             "path_str": "{src}/dogs/dog1",
-            "anno": None,
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
             "name": "dog2",
             "checksum": "",
@@ -371,15 +366,14 @@
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 29759,
             "owner_name": "",
             "owner_id": owner_id,
             "path_str": "{src}/dogs/dog2",
-            "anno": None,
             "path": [],
         },
         {
             "id": None,
             "dir_type": 0,
             "name": "dog3",
             "checksum": "",
@@ -387,12 +381,11 @@
             "version": "",
             "is_latest": True,
             "last_modified": datetime(2022, 6, 28, 22, 39, 1),
             "size": 102,
             "owner_name": "",
             "owner_id": owner_id,
             "path_str": "{src}/dogs/dog3",
-            "anno": None,
             "path": [],
         },
     ],
 }
```

### Comparing `dvcx-0.83.2/tests/func/test_pull.py` & `dvcx-0.83.3/tests/func/test_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         "etag": {"type": "String"},
         "version": {"type": "String"},
         "is_latest": {"type": "Boolean"},
         "last_modified": {"type": "DateTime"},
         "size": {"type": "Int64"},
         "owner_name": {"type": "String"},
         "owner_id": {"type": "String"},
-        "anno": {"type": "String"},
         "random": {"type": "Int64"},
         "location": {"type": "String"},
         "source": {"type": "String"},
     }
 
 
 @pytest.fixture
```

### Comparing `dvcx-0.83.2/tests/func/test_pytorch.py` & `dvcx-0.83.3/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/func/test_query.py` & `dvcx-0.83.3/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/scripts/name_len_normal.py` & `dvcx-0.83.3/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/scripts/name_len_slow.py` & `dvcx-0.83.3/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/test_cli_e2e.py` & `dvcx-0.83.3/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/test_query_e2e.py` & `dvcx-0.83.3/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/lib/test_cached_stream.py` & `dvcx-0.83.3/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/lib/test_feature.py` & `dvcx-0.83.3/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/lib/test_feature_udf.py` & `dvcx-0.83.3/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/lib/test_file.py` & `dvcx-0.83.3/tests/unit/lib/test_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,15 +147,13 @@
     assert file.location == d
 
     with pytest.raises(ValueError):
         File(name="something", location="{not a json}")
 
 
 def test_file_info_jsons():
-    file = FileInfo(name="something", location="", anno="")
+    file = FileInfo(name="something", location="")
     assert file.location is None
-    assert file.anno is None
 
     d = {"e": 12}
-    file = FileInfo(name="something", location=json.dumps(d), anno=json.dumps(d))
+    file = FileInfo(name="something", location=json.dumps(d))
     assert file.location == d
-    assert file.anno == d
```

### Comparing `dvcx-0.83.2/tests/unit/lib/test_image.py` & `dvcx-0.83.3/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/lib/test_reader.py` & `dvcx-0.83.3/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/lib/test_text.py` & `dvcx-0.83.3/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/lib/test_webdataset.py` & `dvcx-0.83.3/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.83.3/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/sql/test_array.py` & `dvcx-0.83.3/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/sql/test_conditional.py` & `dvcx-0.83.3/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/sql/test_path.py` & `dvcx-0.83.3/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/sql/test_selectable.py` & `dvcx-0.83.3/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/sql/test_string.py` & `dvcx-0.83.3/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_asyn.py` & `dvcx-0.83.3/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_cache.py` & `dvcx-0.83.3/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_catalog.py` & `dvcx-0.83.3/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_catalog_loader.py` & `dvcx-0.83.3/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_cli_parsing.py` & `dvcx-0.83.3/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_client_s3.py` & `dvcx-0.83.3/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_data_storage.py` & `dvcx-0.83.3/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_database_engine.py` & `dvcx-0.83.3/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_dataset.py` & `dvcx-0.83.3/tests/unit/test_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         "\tetag VARCHAR, \n"
         "\tversion VARCHAR, \n"
         "\tis_latest BOOLEAN, \n"
         "\tlast_modified DATETIME, \n"
         "\tsize INTEGER NOT NULL, \n"
         "\towner_name VARCHAR, \n"
         "\towner_id VARCHAR, \n"
-        "\tanno JSON, \n"
         "\trandom INTEGER NOT NULL, \n"
         "\tlocation JSON, \n"
         "\tsource VARCHAR NOT NULL, \n"
         "\tscore FLOAT NOT NULL, \n"
         "\tmeta_info JSON, \n"
         "\tPRIMARY KEY (id)\n"
         ")\n"
```

### Comparing `dvcx-0.83.2/tests/unit/test_dataset_row.py` & `dvcx-0.83.3/tests/unit/test_dataset_row.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         etag="c16a68901b0a3222beccaa53c34a6c0c",
         version="",
         is_latest=True,
         last_modified=datetime.datetime(2022, 12, 27, 1, 16, 57),
         size=625,
         owner_name="",
         owner_id="",
-        anno=None,
         random=1234,
         location=None,
         source=StorageURI("s3://bucket-name"),
         custom={},
     )
 
     row_dict = json.loads(json.dumps(attrs.asdict(row), cls=JSONSerialize))
```

### Comparing `dvcx-0.83.2/tests/unit/test_dispatch.py` & `dvcx-0.83.3/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_fileslice.py` & `dvcx-0.83.3/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_id_generator.py` & `dvcx-0.83.3/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_listing.py` & `dvcx-0.83.3/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_metastore.py` & `dvcx-0.83.3/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_query_params.py` & `dvcx-0.83.3/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_serializer.py` & `dvcx-0.83.3/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_session.py` & `dvcx-0.83.3/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_storage.py` & `dvcx-0.83.3/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_udf.py` & `dvcx-0.83.3/tests/unit/test_udf.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         id=6,
         vtype="",
         dir_type=1,
         parent="",
         name="obj",
         checksum="",
         last_modified=None,
-        anno={},
         etag="",
         version="",
         is_latest=True,
         size=7,
         owner_name="",
         owner_id="",
         source="",
@@ -44,15 +43,14 @@
         id=6,
         vtype="",
         dir_type=1,
         parent="",
         name="obj",
         checksum="",
         last_modified=None,
-        anno={},
         etag="",
         version="",
         is_latest=True,
         size=7,
         owner_name="",
         owner_id="",
         source="",
@@ -75,15 +73,14 @@
             id=row_id,
             vtype="",
             dir_type=1,
             parent="",
             name="obj",
             checksum="",
             last_modified=None,
-            anno={},
             etag="",
             version="",
             is_latest=True,
             size=size,
             owner_name="",
             owner_id="",
             source="",
@@ -117,15 +114,14 @@
             id=5,
             vtype="",
             dir_type=1,
             parent="",
             name="obj",
             checksum="",
             last_modified=None,
-            anno={},
             etag="",
             version="",
             is_latest=True,
             size=size,
             owner_name="",
             owner_id="",
             source="",
```

### Comparing `dvcx-0.83.2/tests/unit/test_utils.py` & `dvcx-0.83.3/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/unit/test_warehouse.py` & `dvcx-0.83.3/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.83.2/tests/utils.py` & `dvcx-0.83.3/tests/utils.py`

 * *Files identical despite different names*

