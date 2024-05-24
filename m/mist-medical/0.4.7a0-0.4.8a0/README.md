# Comparing `tmp/mist_medical-0.4.7a0.tar.gz` & `tmp/mist_medical-0.4.8a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mist_medical-0.4.7a0.tar", last modified: Mon May 13 15:39:58 2024, max compression
+gzip compressed data, was "mist_medical-0.4.8a0.tar", last modified: Fri May 24 20:56:38 2024, max compression
```

## Comparing `mist_medical-0.4.7a0.tar` & `mist_medical-0.4.8a0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.143692 mist_medical-0.4.7a0/
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 15:39:58.143692 mist_medical-0.4.7a0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2554 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/analyze_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/analyze_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16741 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/analyze_data/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/conversion_tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/conversion_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/conversion_tools/csv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5762 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/conversion_tools/msd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/convert_to_mist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/data_loading/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/data_loading/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12303 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/data_loading/dali_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/eval_preds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/evaluate_preds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/evaluate_preds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5350 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/evaluate_preds/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/inference/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11958 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/inference/main_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3689 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22757 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/metrics/lookup_tables.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18301 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/attn_unet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9112 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/get_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6272 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/layers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/mgnets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16466 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/nnunet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/swin_unetr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/unet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2488 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/post_preds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/postprocess_preds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/postprocess_preds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8387 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/postprocess_preds/postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/preprocess_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/preprocess_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10643 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/preprocess_data/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/runtime/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8099 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/args.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7534 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21551 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22443 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/analyze_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/preprocess_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/run_all_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/train_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.143692 mist_medical-0.4.7a0/mist_medical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:39:58.143692 mist_medical-0.4.7a0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.550101 mist_medical-0.4.8a0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-24 20:56:38.546101 mist_medical-0.4.8a0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2554 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.542101 mist_medical-0.4.8a0/mist/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.542101 mist_medical-0.4.8a0/mist/analyze_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/analyze_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16741 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/analyze_data/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.542101 mist_medical-0.4.8a0/mist/conversion_tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/conversion_tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/conversion_tools/csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5762 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/conversion_tools/msd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/convert_to_mist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.542101 mist_medical-0.4.8a0/mist/data_loading/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/data_loading/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12303 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/data_loading/dali_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1674 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/eval_preds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.542101 mist_medical-0.4.8a0/mist/evaluate_preds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/evaluate_preds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5456 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/evaluate_preds/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.542101 mist_medical-0.4.8a0/mist/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11958 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/inference/main_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3726 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.542101 mist_medical-0.4.8a0/mist/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/metrics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22757 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/metrics/lookup_tables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18301 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.546101 mist_medical-0.4.8a0/mist/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/models/attn_unet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9112 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/models/get_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6272 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/models/layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/models/mgnets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16466 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/models/nnunet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/models/swin_unetr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/models/unet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2577 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/post_preds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.546101 mist_medical-0.4.8a0/mist/postprocess_preds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/postprocess_preds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8429 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/postprocess_preds/postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.546101 mist_medical-0.4.8a0/mist/preprocess_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/preprocess_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10643 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/preprocess_data/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.546101 mist_medical-0.4.8a0/mist/runtime/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/runtime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8188 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/runtime/args.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7534 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/runtime/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/runtime/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21551 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/runtime/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22443 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.546101 mist_medical-0.4.8a0/mist/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/scripts/analyze_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/scripts/preprocess_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/scripts/run_all_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/mist/scripts/train_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:56:38.546101 mist_medical-0.4.8a0/mist_medical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-24 20:56:38.000000 mist_medical-0.4.8a0/mist_medical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-24 20:56:38.000000 mist_medical-0.4.8a0/mist_medical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:56:38.000000 mist_medical-0.4.8a0/mist_medical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 20:56:38.000000 mist_medical-0.4.8a0/mist_medical.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-24 20:56:38.000000 mist_medical-0.4.8a0/mist_medical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 20:56:38.000000 mist_medical-0.4.8a0/mist_medical.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:56:38.550101 mist_medical-0.4.8a0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-05-24 20:56:33.000000 mist_medical-0.4.8a0/setup.py
```

### Comparing `mist_medical-0.4.7a0/PKG-INFO` & `mist_medical-0.4.8a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mist-medical
-Version: 0.4.7a0
+Version: 0.4.8a0
 Summary: MIST is a simple, fully automated framework for 3D medical imaging segmentation.
 Author: Rice University, The University of Texas MD Anderson Cancer Center
 Author-email: Adrian Celaya <aecelaya@rice.edu>, David Fuentes <dtfuentes@mdanderson.org>, Beatrice Riviere <riviere@rice.edu>, Evan Lim <EMLim@mdanderson.org>, Rachel Glenn <rglenn1@mdanderson.org>, Alex Balsells <atb8@rice.edu>
 License: Medical Imaging Segmentation Toolkit (MIST) (c) 2024 by Adrian Celaya
         is licenced under Attribution-NonCommercial-ShareAlike 4.0 International.
         To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: homepage, https://github.com/aecelaya/MIST
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch==2.0.1
-Requires-Dist: monai==1.3.0
-Requires-Dist: antspyx==0.3.8
-Requires-Dist: simpleitk==2.2.1
+Requires-Dist: torch>=2.0.1
+Requires-Dist: monai>=1.3.0
+Requires-Dist: antspyx>=0.3.8
+Requires-Dist: simpleitk>=2.2.1
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: rich
 Requires-Dist: tqdm
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: scikit-image
```

### Comparing `mist_medical-0.4.7a0/README.md` & `mist_medical-0.4.8a0/README.md`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/analyze_data/analyze.py` & `mist_medical-0.4.8a0/mist/analyze_data/analyze.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/conversion_tools/csv.py` & `mist_medical-0.4.8a0/mist/conversion_tools/csv.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/conversion_tools/msd.py` & `mist_medical-0.4.8a0/mist/conversion_tools/msd.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/convert_to_mist.py` & `mist_medical-0.4.8a0/mist/convert_to_mist.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/data_loading/dali_loader.py` & `mist_medical-0.4.8a0/mist/data_loading/dali_loader.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/eval_preds.py` & `mist_medical-0.4.8a0/mist/eval_preds.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
           default=["dice", "haus95"],
           choices=["dice", "surf_dice", "haus95", "avg_surf"],
           help="List of metrics to use for evaluation")
     p.boolean_flag("--normalize-hd", default=False, help="Normalize Hausdorff distances")
     p.boolean_flag("--use-native-spacing",
                    default=False,
                    help="Use native image spacing to compute Hausdorff distances")
+    p.arg("--surf-dice-tol", type=float, default=1.0, help="Tolerance for surface dice")
 
     args = p.parse_args()
     return args
 
 
 def main(args):
     # Set warning levels
@@ -33,15 +34,16 @@
     # Evaluate predictions
     evaluate(args.config,
              args.paths,
              args.preds_dir,
              args.output_csv,
              args.metrics,
              args.normalize_hd,
-             args.use_native_spacing)
+             args.use_native_spacing,
+             args.surf_dice_tol)
 
 
 def mist_eval_entry():
     args = get_eval_args()
     main(args)
```

### Comparing `mist_medical-0.4.7a0/mist/evaluate_preds/evaluate.py` & `mist_medical-0.4.8a0/mist/evaluate_preds/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 def get_worst_case_haus(mask_npy, spacing):
     width = mask_npy.shape[0] * spacing[0]
     height = mask_npy.shape[1] * spacing[1]
     depth = mask_npy.shape[2] * spacing[2]
     return np.sqrt(width ** 2 + height ** 2 + depth ** 2)
 
 
-def evaluate_single_example(pred, truth, patient_id, config, metrics, use_native_spacing):
+def evaluate_single_example(pred, truth, patient_id, config, metrics, use_native_spacing, surf_dice_tol):
     # Get dice and hausdorff distances for final prediction
     row_dict = dict()
     row_dict['id'] = patient_id
 
     # Read prediction and truth nifti files
     pred = ants.image_read(pred)
     truth = ants.image_read(truth)
@@ -84,28 +84,28 @@
             row_dict["{}_haus95".format(key)] = haus95_dist
         if "surf_dice" in metrics:
             if temp_truth_sum == 0 and temp_pred_sum == 0:
                 surf_dice_coef = 1.0
             elif bool(temp_truth_sum == 0) ^ bool(temp_pred_sum == 0):
                 surf_dice_coef = 0.0
             else:
-                surf_dice_coef = compute_surface_dice_at_tolerance(distances, tolerance_mm=1.0)
+                surf_dice_coef = compute_surface_dice_at_tolerance(distances, tolerance_mm=surf_dice_tol)
             row_dict["{}_surf_dice".format(key)] = surf_dice_coef
         if "avg_surf" in metrics:
             if temp_truth_sum == 0 and temp_pred_sum == 0:
                 avg_surf_dist = 0.0
             elif bool(temp_truth_sum == 0) ^ bool(temp_pred_sum == 0):
                 avg_surf_dist = get_worst_case_haus(truth_temp, spacing)
             else:
                 avg_surf_dist = compute_average_surface_distance(distances)
             row_dict["{}_avg_surf".format(key)] = avg_surf_dist
     return row_dict
 
 
-def evaluate(config_json, paths, source_dir, output_csv, metrics, use_native_spacing):
+def evaluate(config_json, paths, source_dir, output_csv, metrics, use_native_spacing, surf_dice_tol):
     with open(config_json, 'r') as file:
         config = json.load(file)
 
     if not isinstance(paths, pd.DataFrame):
         # Convert input to pandas dataframe
         if '.csv' in paths:
             paths = pd.read_csv(paths)
@@ -135,12 +135,13 @@
             truth = paths.loc[paths['id'].astype(str) == patient_id].iloc[0]['mask']
 
             eval_results = evaluate_single_example(pred,
                                                    truth,
                                                    patient_id,
                                                    config,
                                                    metrics,
-                                                   use_native_spacing)
+                                                   use_native_spacing,
+                                                   surf_dice_tol)
             results_df = pd.concat([results_df, pd.DataFrame(eval_results, index=[0])], ignore_index=True)
 
     results_df = compute_results_stats(results_df)
     results_df.to_csv(output_csv, index=False)
```

### Comparing `mist_medical-0.4.7a0/mist/inference/main_inference.py` & `mist_medical-0.4.8a0/mist/inference/main_inference.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/main.py` & `mist_medical-0.4.8a0/mist/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         mist_trainer.fit()
 
         evaluate(args.data,
                  os.path.join(args.results, "train_paths.csv"),
                  os.path.join(args.results, "predictions", "train", "raw"),
                  os.path.join(args.results, "results.csv"),
                  args.metrics,
-                 args.use_native_spacing)
+                 args.use_native_spacing,
+                 args.surf_dice_tol)
 
     if args.exec_mode == "all" or args.exec_mode == "train":
         if has_test_data(args.data):
             test_df = get_files_df(args.data, "test")
             test_df.to_csv(os.path.join(args.results, "test_paths.csv"), index=False)
 
             models = load_test_time_models(os.path.join(args.results, "models"), False)
```

### Comparing `mist_medical-0.4.7a0/mist/metrics/lookup_tables.py` & `mist_medical-0.4.8a0/mist/metrics/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/metrics/metrics.py` & `mist_medical-0.4.8a0/mist/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/models/attn_unet.py` & `mist_medical-0.4.8a0/mist/models/attn_unet.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/models/get_model.py` & `mist_medical-0.4.8a0/mist/models/get_model.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/models/layers.py` & `mist_medical-0.4.8a0/mist/models/layers.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/models/mgnets.py` & `mist_medical-0.4.8a0/mist/models/mgnets.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/models/nnunet.py` & `mist_medical-0.4.8a0/mist/models/nnunet.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/models/swin_unetr.py` & `mist_medical-0.4.8a0/mist/models/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/models/unet.py` & `mist_medical-0.4.8a0/mist/models/unet.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/post_preds.py` & `mist_medical-0.4.8a0/mist/post_preds.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
           nargs="+",
           default=["dice", "haus95"],
           choices=["dice", "surf_dice", "haus95", "avg_surf"],
           help="List of metrics to use for evaluation")
     p.boolean_flag("--use-native-spacing",
                    default=False,
                    help="Use native image spacing to compute Hausdorff distances")
+    p.arg("--surf-dice-tol", type=float, default=1.0, help="Tolerance for surface dice")
 
     args = p.parse_args()
     return args
 
 
 def main(args):
     # Set warning levels
```

### Comparing `mist_medical-0.4.7a0/mist/postprocess_preds/postprocess.py` & `mist_medical-0.4.8a0/mist/postprocess_preds/postprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,16 @@
 
         # Evaluate new predictions
         evaluate(self.config_file,
                  self.train_paths,
                  self.dest_dir,
                  self.new_results_csv,
                  self.metrics,
-                 self.args.use_native_spacing)
+                 self.args.use_native_spacing,
+                 self.args.surf_dice_tol)
 
         # Compute improvement score
         new_results_df = pd.read_csv(self.new_results_csv)
         score = compute_improvement_score(self.base_results_df, new_results_df, self.metrics)
         return score
 
     def run(self):
```

### Comparing `mist_medical-0.4.7a0/mist/predict.py` & `mist_medical-0.4.8a0/mist/predict.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/preprocess_data/preprocess.py` & `mist_medical-0.4.8a0/mist/preprocess_data/preprocess.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/runtime/args.py` & `mist_medical-0.4.8a0/mist/runtime/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,13 +172,14 @@
           nargs="+",
           default=["dice", "haus95"],
           choices=["dice", "surf_dice", "haus95", "avg_surf"],
           help="List of metrics to use for evaluation")
     p.boolean_flag("--use-native-spacing",
                    default=False,
                    help="Use native image spacing to compute Hausdorff distances")
+    p.arg("--surf-dice-tol", type=float, default=1.0, help="Tolerance for surface dice")
 
     # Uncertainty
     p.boolean_flag("--output-std", default=False, help="Output standard deviation for ensemble predictions")
 
     args = p.parse_args()
     return args
```

### Comparing `mist_medical-0.4.7a0/mist/runtime/loss.py` & `mist_medical-0.4.8a0/mist/runtime/loss.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/runtime/progress_bar.py` & `mist_medical-0.4.8a0/mist/runtime/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/runtime/run.py` & `mist_medical-0.4.8a0/mist/runtime/run.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/runtime/utils.py` & `mist_medical-0.4.8a0/mist/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/scripts/run_all_entrypoint.py` & `mist_medical-0.4.8a0/mist/scripts/run_all_entrypoint.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist/scripts/train_entrypoint.py` & `mist_medical-0.4.8a0/mist/scripts/train_entrypoint.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/mist_medical.egg-info/PKG-INFO` & `mist_medical-0.4.8a0/mist_medical.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mist-medical
-Version: 0.4.7a0
+Version: 0.4.8a0
 Summary: MIST is a simple, fully automated framework for 3D medical imaging segmentation.
 Author: Rice University, The University of Texas MD Anderson Cancer Center
 Author-email: Adrian Celaya <aecelaya@rice.edu>, David Fuentes <dtfuentes@mdanderson.org>, Beatrice Riviere <riviere@rice.edu>, Evan Lim <EMLim@mdanderson.org>, Rachel Glenn <rglenn1@mdanderson.org>, Alex Balsells <atb8@rice.edu>
 License: Medical Imaging Segmentation Toolkit (MIST) (c) 2024 by Adrian Celaya
         is licenced under Attribution-NonCommercial-ShareAlike 4.0 International.
         To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: homepage, https://github.com/aecelaya/MIST
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch==2.0.1
-Requires-Dist: monai==1.3.0
-Requires-Dist: antspyx==0.3.8
-Requires-Dist: simpleitk==2.2.1
+Requires-Dist: torch>=2.0.1
+Requires-Dist: monai>=1.3.0
+Requires-Dist: antspyx>=0.3.8
+Requires-Dist: simpleitk>=2.2.1
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: rich
 Requires-Dist: tqdm
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: scikit-image
```

### Comparing `mist_medical-0.4.7a0/mist_medical.egg-info/SOURCES.txt` & `mist_medical-0.4.8a0/mist_medical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.7a0/pyproject.toml` & `mist_medical-0.4.8a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mist-medical"
-version = "0.4.7-alpha"
+version = "0.4.8-alpha"
 requires-python = ">= 3.8"
 description = "MIST is a simple, fully automated framework for 3D medical imaging segmentation."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Adrian Celaya", email = "aecelaya@rice.edu"},
     {name = "David Fuentes", email = "dtfuentes@mdanderson.org"},
@@ -33,18 +33,18 @@
     "U-Net",
     "unet",
     "vision transformers",
     "UNETR",
     "unetr"
 ]
 dependencies = [
-    "torch==2.0.1",
-    "monai==1.3.0",
-    "antspyx==0.3.8",
-    "simpleitk==2.2.1",
+    "torch>=2.0.1",
+    "monai>=1.3.0",
+    "antspyx>=0.3.8",
+    "simpleitk>=2.2.1",
     "numpy",
     "pandas",
     "rich",
     "tqdm",
     "scipy",
     "scikit-learn",
     "scikit-image",
```

