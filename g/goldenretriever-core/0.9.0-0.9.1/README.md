# Comparing `tmp/goldenretriever-core-0.9.0.tar.gz` & `tmp/goldenretriever_core-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goldenretriever-core-0.9.0.tar", last modified: Wed Feb  7 18:19:00 2024, max compression
+gzip compressed data, was "goldenretriever_core-0.9.1.tar", last modified: Fri May 24 14:35:19 2024, max compression
```

## Comparing `goldenretriever-core-0.9.0.tar` & `goldenretriever_core-0.9.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.262896 goldenretriever-core-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-02-07 18:19:00.262896 goldenretriever-core-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.246896 goldenretriever-core-0.9.0/goldenretriever/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.246896 goldenretriever-core-0.9.0/goldenretriever/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/callbacks/evaluation_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/callbacks/prediction_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/callbacks/training_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/callbacks/utils_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.246896 goldenretriever-core-0.9.0/goldenretriever/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/common/from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/common/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/common/model_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/common/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/common/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/common/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    20253 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.246896 goldenretriever-core-0.9.0/goldenretriever/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.246896 goldenretriever-core-0.9.0/goldenretriever/data/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/data/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/data/base/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    27031 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/data/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.250896 goldenretriever-core-0.9.0/goldenretriever/indexers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/indexers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/indexers/document.py
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/indexers/faiss.py
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/indexers/inmemory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/indexers/voyager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.250896 goldenretriever-core-0.9.0/goldenretriever/lightning_modules/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/lightning_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/lightning_modules/pl_data_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/lightning_modules/pl_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.250896 goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    23613 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.250896 goldenretriever-core-0.9.0/goldenretriever/serve/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.250896 goldenretriever-core-0.9.0/goldenretriever/serve/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.250896 goldenretriever-core-0.9.0/goldenretriever/serve/data/splitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/splitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/splitters/base_sentence_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/splitters/spacy_sentence_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/splitters/window_based_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.254896 goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/base_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/regex_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/spacy_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/whitespace_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.254896 goldenretriever-core-0.9.0/goldenretriever/serve/data/window/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/data/window/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.254896 goldenretriever-core-0.9.0/goldenretriever/serve/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.254896 goldenretriever-core-0.9.0/goldenretriever/serve/server/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/backend/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/backend/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/backend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.254896 goldenretriever-core-0.9.0/goldenretriever/serve/server/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/frontend/relik_front.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/server/ray_old.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.254896 goldenretriever-core-0.9.0/goldenretriever/serve/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/serve/utils/gunicorn_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.254896 goldenretriever-core-0.9.0/goldenretriever/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43349 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/trainer/train.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/goldenretriever/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 18:19:00.258896 goldenretriever-core-0.9.0/goldenretriever_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-02-07 18:19:00.000000 goldenretriever-core-0.9.0/goldenretriever_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-07 18:19:00.000000 goldenretriever-core-0.9.0/goldenretriever_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 18:19:00.000000 goldenretriever-core-0.9.0/goldenretriever_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-07 18:19:00.000000 goldenretriever-core-0.9.0/goldenretriever_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 18:19:00.000000 goldenretriever-core-0.9.0/goldenretriever_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 18:19:00.262896 goldenretriever-core-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-02-07 18:18:48.000000 goldenretriever-core-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.399412 goldenretriever_core-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-24 14:35:19.399412 goldenretriever_core-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.383412 goldenretriever_core-0.9.1/goldenretriever/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.383412 goldenretriever_core-0.9.1/goldenretriever/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/callbacks/evaluation_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/callbacks/prediction_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/callbacks/training_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/callbacks/utils_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.387412 goldenretriever_core-0.9.1/goldenretriever/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/common/from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/common/model_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/common/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/common/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/common/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20253 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.387412 goldenretriever_core-0.9.1/goldenretriever/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.387412 goldenretriever_core-0.9.1/goldenretriever/data/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/data/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/data/base/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27434 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/data/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.387412 goldenretriever_core-0.9.1/goldenretriever/indexers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16841 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/indexers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/indexers/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/indexers/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/indexers/inmemory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/indexers/voyager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.387412 goldenretriever_core-0.9.1/goldenretriever/lightning_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/lightning_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/lightning_modules/pl_data_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/lightning_modules/pl_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23613 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/serve/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/serve/data/splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/splitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/splitters/base_sentence_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/splitters/spacy_sentence_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/splitters/window_based_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/base_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/regex_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/whitespace_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/serve/data/window/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/data/window/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/serve/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/serve/server/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/backend/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/backend/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/backend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.391412 goldenretriever_core-0.9.1/goldenretriever/serve/server/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/frontend/relik_front.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/server/ray_old.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.395413 goldenretriever_core-0.9.1/goldenretriever/serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/serve/utils/gunicorn_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.395413 goldenretriever_core-0.9.1/goldenretriever/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44064 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/trainer/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/goldenretriever/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:35:19.395413 goldenretriever_core-0.9.1/goldenretriever_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-24 14:35:19.000000 goldenretriever_core-0.9.1/goldenretriever_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-24 14:35:19.000000 goldenretriever_core-0.9.1/goldenretriever_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:35:19.000000 goldenretriever_core-0.9.1/goldenretriever_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-24 14:35:19.000000 goldenretriever_core-0.9.1/goldenretriever_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 14:35:19.000000 goldenretriever_core-0.9.1/goldenretriever_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 14:35:19.399412 goldenretriever_core-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-24 14:35:13.000000 goldenretriever_core-0.9.1/setup.py
```

### Comparing `goldenretriever-core-0.9.0/PKG-INFO` & `goldenretriever_core-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goldenretriever-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dense Retriever
 Home-page: https://github.com/Riccorl/golden-retriever
 Author: Riccardo Orlando
 Author-email: orlandorcc@gmail.com
 License: Apache
 Keywords: NLP deep learning transformer pytorch retriever rag dpr
 Classifier: Intended Audience :: Science/Research
@@ -69,38 +69,42 @@
 </p>
 <p align="center">
   <a href="https://github.com/Riccorl/golden-retriever/releases"><img alt="release" src="https://img.shields.io/github/v/release/Riccorl/golden-retriever"></a>
   <a href="https://github.com/Riccorl/golden-retriever/actions/workflows/python-publish-pypi.yml"><img alt="gh-status" src="https://github.com/Riccorl/golden-retriever/actions/workflows/python-publish-pypi.yml/badge.svg"></a>
 
 </p>
 
+# WIP: distributed-compatible codebase
+
+A distributed-compatible codebase is under development. Check the `distributed` [branch](https://github.com/Riccorl/golden-retriever/tree/distributed) for the latest updates.
+
 # How to use
 
-Install the library from [PyPI]():
+Install the library from [PyPI](https://pypi.org/project/goldenretriever-core/):
 
 ```bash
-pip install goldenretriever
+pip install goldenretriever-core
 ```
 
 or from source:
 
 ```bash
 git clone https://github.com/Riccorl/golden-retriever.git
-cd goldenretriever
+cd golden-retriever
 pip install -e .
 ```
 
 # Usage
 
 ## How to run an experiment
 
 ### Training
 
 Here a simple example on how to train a DPR-like Retriever on the NQ dataset.
-First download the dataset from (DPR)[]. The run the following code:
+First download the dataset from [DPR](https://github.com/facebookresearch/DPR?tab=readme-ov-file#retriever-input-data-format). The run the following code:
 
 ```python
 from goldenretriever.trainer import Trainer
 from goldenretriever import GoldenRetriever
 from goldenretriever.data.datasets import InBatchNegativesDataset
 
 # create a retriever
@@ -196,34 +200,34 @@
 ### Input data
 
 The retriever expects a jsonl file similar to [DPR](https://github.com/facebookresearch/DPR):
 
 ```json lines
 [
   {
-	"question": "....",
-	"answers": ["...", "...", "..."],
-	"positive_ctxs": [{
-		"title": "...",
-		"text": "...."
-	}],
-	"negative_ctxs": ["..."],
-	"hard_negative_ctxs": ["..."]
+  "question": "....",
+  "answers": ["...", "...", "..."],
+  "positive_ctxs": [{
+    "title": "...",
+    "text": "...."
+  }],
+  "negative_ctxs": ["..."],
+  "hard_negative_ctxs": ["..."]
   },
   ...
 ]
 ```
 
 ### Index data
 
-The document to index can be either a jsonl file or a tsv file similar to 
+The document to index can be either a jsonl file or a tsv file similar to
 [DPR](https://github.com/facebookresearch/DPR):
 
 - `jsonl`: each line is a json object with the following keys: `id`, `text`, `metadata`
-- `tsv`: each line is a tab-separated string with the `id` and `text` column, 
+- `tsv`: each line is a tab-separated string with the `id` and `text` column,
   followed by any other column that will be stored in the `metadata` field
 
 jsonl example:
 
 ```json lines
 [
   {
@@ -237,8 +241,7 @@
 
 tsv example:
 
 ```tsv
 id \t text \t any other column
 ...
 ```
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: goldenretriever-core Version: 0.9.0 Summary: Dense
+Metadata-Version: 2.1 Name: goldenretriever-core Version: 0.9.1 Summary: Dense
 Retriever Home-page: https://github.com/Riccorl/golden-retriever Author:
 Riccardo Orlando Author-email: orlandorcc@gmail.com License: Apache Keywords:
 NLP deep learning transformer pytorch retriever rag dpr Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
 >=3.10 Description-Content-Type: text/markdown Requires-Dist: torch<2.3,>=2.1
@@ -30,25 +30,30 @@
 [standard]<0.28,>=0.24; extra == "serve" Requires-Dist: gunicorn==21.2.0; extra
 == "serve" Requires-Dist: ray[serve]<=2.10,>=2.8; extra == "serve" Provides-
 Extra: dev Requires-Dist: pre-commit; extra == "dev" Requires-Dist: black[d];
 extra == "dev" Requires-Dist: isort; extra == "dev"
                       ************ ?ð??¦?® GGoollddeenn RReettrriieevveerr ************
                 _[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_v_s_c_o_d_e_]
                              _[_r_e_l_e_a_s_e_]_[_g_h_-_s_t_a_t_u_s_]
-# How to use Install the library from [PyPI](): ```bash pip install
-goldenretriever ``` or from source: ```bash git clone https://github.com/
-Riccorl/golden-retriever.git cd goldenretriever pip install -e . ``` # Usage ##
-How to run an experiment ### Training Here a simple example on how to train a
-DPR-like Retriever on the NQ dataset. First download the dataset from (DPR)[].
-The run the following code: ```python from goldenretriever.trainer import
-Trainer from goldenretriever import GoldenRetriever from
-goldenretriever.data.datasets import InBatchNegativesDataset # create a
-retriever retriever = GoldenRetriever( question_encoder="intfloat/e5-small-v2",
-passage_encoder="intfloat/e5-small-v2" ) # create a dataset train_dataset =
-InBatchNegativesDataset( name="webq_train", path="path/to/webq_train.json",
+# WIP: distributed-compatible codebase A distributed-compatible codebase is
+under development. Check the `distributed` [branch](https://github.com/Riccorl/
+golden-retriever/tree/distributed) for the latest updates. # How to use Install
+the library from [PyPI](https://pypi.org/project/goldenretriever-core/):
+```bash pip install goldenretriever-core ``` or from source: ```bash git clone
+https://github.com/Riccorl/golden-retriever.git cd golden-retriever pip install
+-e . ``` # Usage ## How to run an experiment ### Training Here a simple example
+on how to train a DPR-like Retriever on the NQ dataset. First download the
+dataset from [DPR](https://github.com/facebookresearch/DPR?tab=readme-ov-
+file#retriever-input-data-format). The run the following code: ```python from
+goldenretriever.trainer import Trainer from goldenretriever import
+GoldenRetriever from goldenretriever.data.datasets import
+InBatchNegativesDataset # create a retriever retriever = GoldenRetriever
+( question_encoder="intfloat/e5-small-v2", passage_encoder="intfloat/e5-small-
+v2" ) # create a dataset train_dataset = InBatchNegativesDataset
+( name="webq_train", path="path/to/webq_train.json",
 tokenizer=retriever.question_tokenizer, question_batch_size=64,
 passage_batch_size=400, max_passage_length=64, shuffle=True, ) val_dataset =
 InBatchNegativesDataset( name="webq_dev", path="path/to/webq_dev.json",
 tokenizer=retriever.question_tokenizer, question_batch_size=64,
 passage_batch_size=400, max_passage_length=64, ) trainer = Trainer
 ( retriever=retriever, train_dataset=train_dataset, val_dataset=val_dataset,
 max_steps=25_000, wandb_online_mode=True, wandb_project_name="golden-retriever-
```

### Comparing `goldenretriever-core-0.9.0/README.md` & `goldenretriever_core-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,38 +10,42 @@
 </p>
 <p align="center">
   <a href="https://github.com/Riccorl/golden-retriever/releases"><img alt="release" src="https://img.shields.io/github/v/release/Riccorl/golden-retriever"></a>
   <a href="https://github.com/Riccorl/golden-retriever/actions/workflows/python-publish-pypi.yml"><img alt="gh-status" src="https://github.com/Riccorl/golden-retriever/actions/workflows/python-publish-pypi.yml/badge.svg"></a>
 
 </p>
 
+# WIP: distributed-compatible codebase
+
+A distributed-compatible codebase is under development. Check the `distributed` [branch](https://github.com/Riccorl/golden-retriever/tree/distributed) for the latest updates.
+
 # How to use
 
-Install the library from [PyPI]():
+Install the library from [PyPI](https://pypi.org/project/goldenretriever-core/):
 
 ```bash
-pip install goldenretriever
+pip install goldenretriever-core
 ```
 
 or from source:
 
 ```bash
 git clone https://github.com/Riccorl/golden-retriever.git
-cd goldenretriever
+cd golden-retriever
 pip install -e .
 ```
 
 # Usage
 
 ## How to run an experiment
 
 ### Training
 
 Here a simple example on how to train a DPR-like Retriever on the NQ dataset.
-First download the dataset from (DPR)[]. The run the following code:
+First download the dataset from [DPR](https://github.com/facebookresearch/DPR?tab=readme-ov-file#retriever-input-data-format). The run the following code:
 
 ```python
 from goldenretriever.trainer import Trainer
 from goldenretriever import GoldenRetriever
 from goldenretriever.data.datasets import InBatchNegativesDataset
 
 # create a retriever
@@ -137,34 +141,34 @@
 ### Input data
 
 The retriever expects a jsonl file similar to [DPR](https://github.com/facebookresearch/DPR):
 
 ```json lines
 [
   {
-	"question": "....",
-	"answers": ["...", "...", "..."],
-	"positive_ctxs": [{
-		"title": "...",
-		"text": "...."
-	}],
-	"negative_ctxs": ["..."],
-	"hard_negative_ctxs": ["..."]
+  "question": "....",
+  "answers": ["...", "...", "..."],
+  "positive_ctxs": [{
+    "title": "...",
+    "text": "...."
+  }],
+  "negative_ctxs": ["..."],
+  "hard_negative_ctxs": ["..."]
   },
   ...
 ]
 ```
 
 ### Index data
 
-The document to index can be either a jsonl file or a tsv file similar to 
+The document to index can be either a jsonl file or a tsv file similar to
 [DPR](https://github.com/facebookresearch/DPR):
 
 - `jsonl`: each line is a json object with the following keys: `id`, `text`, `metadata`
-- `tsv`: each line is a tab-separated string with the `id` and `text` column, 
+- `tsv`: each line is a tab-separated string with the `id` and `text` column,
   followed by any other column that will be stored in the `metadata` field
 
 jsonl example:
 
 ```json lines
 [
   {
@@ -178,8 +182,7 @@
 
 tsv example:
 
 ```tsv
 id \t text \t any other column
 ...
 ```
-
```

#### html2text {}

```diff
@@ -1,21 +1,26 @@
                       ************ ?ð??¦?® GGoollddeenn RReettrriieevveerr ************
                 _[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_v_s_c_o_d_e_]
                              _[_r_e_l_e_a_s_e_]_[_g_h_-_s_t_a_t_u_s_]
-# How to use Install the library from [PyPI](): ```bash pip install
-goldenretriever ``` or from source: ```bash git clone https://github.com/
-Riccorl/golden-retriever.git cd goldenretriever pip install -e . ``` # Usage ##
-How to run an experiment ### Training Here a simple example on how to train a
-DPR-like Retriever on the NQ dataset. First download the dataset from (DPR)[].
-The run the following code: ```python from goldenretriever.trainer import
-Trainer from goldenretriever import GoldenRetriever from
-goldenretriever.data.datasets import InBatchNegativesDataset # create a
-retriever retriever = GoldenRetriever( question_encoder="intfloat/e5-small-v2",
-passage_encoder="intfloat/e5-small-v2" ) # create a dataset train_dataset =
-InBatchNegativesDataset( name="webq_train", path="path/to/webq_train.json",
+# WIP: distributed-compatible codebase A distributed-compatible codebase is
+under development. Check the `distributed` [branch](https://github.com/Riccorl/
+golden-retriever/tree/distributed) for the latest updates. # How to use Install
+the library from [PyPI](https://pypi.org/project/goldenretriever-core/):
+```bash pip install goldenretriever-core ``` or from source: ```bash git clone
+https://github.com/Riccorl/golden-retriever.git cd golden-retriever pip install
+-e . ``` # Usage ## How to run an experiment ### Training Here a simple example
+on how to train a DPR-like Retriever on the NQ dataset. First download the
+dataset from [DPR](https://github.com/facebookresearch/DPR?tab=readme-ov-
+file#retriever-input-data-format). The run the following code: ```python from
+goldenretriever.trainer import Trainer from goldenretriever import
+GoldenRetriever from goldenretriever.data.datasets import
+InBatchNegativesDataset # create a retriever retriever = GoldenRetriever
+( question_encoder="intfloat/e5-small-v2", passage_encoder="intfloat/e5-small-
+v2" ) # create a dataset train_dataset = InBatchNegativesDataset
+( name="webq_train", path="path/to/webq_train.json",
 tokenizer=retriever.question_tokenizer, question_batch_size=64,
 passage_batch_size=400, max_passage_length=64, shuffle=True, ) val_dataset =
 InBatchNegativesDataset( name="webq_dev", path="path/to/webq_dev.json",
 tokenizer=retriever.question_tokenizer, question_batch_size=64,
 passage_batch_size=400, max_passage_length=64, ) trainer = Trainer
 ( retriever=retriever, train_dataset=train_dataset, val_dataset=val_dataset,
 max_steps=25_000, wandb_online_mode=True, wandb_project_name="golden-retriever-
```

### Comparing `goldenretriever-core-0.9.0/goldenretriever/callbacks/base.py` & `goldenretriever_core-0.9.1/goldenretriever/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/callbacks/evaluation_callbacks.py` & `goldenretriever_core-0.9.1/goldenretriever/callbacks/evaluation_callbacks.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/callbacks/prediction_callbacks.py` & `goldenretriever_core-0.9.1/goldenretriever/callbacks/prediction_callbacks.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/callbacks/training_callbacks.py` & `goldenretriever_core-0.9.1/goldenretriever/callbacks/training_callbacks.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/callbacks/utils_callbacks.py` & `goldenretriever_core-0.9.1/goldenretriever/callbacks/utils_callbacks.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/common/from_config.py` & `goldenretriever_core-0.9.1/goldenretriever/common/from_config.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/common/log.py` & `goldenretriever_core-0.9.1/goldenretriever/common/log.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/common/model_inputs.py` & `goldenretriever_core-0.9.1/goldenretriever/common/model_inputs.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/common/sampler.py` & `goldenretriever_core-0.9.1/goldenretriever/common/sampler.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/common/torch_utils.py` & `goldenretriever_core-0.9.1/goldenretriever/common/torch_utils.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/common/upload.py` & `goldenretriever_core-0.9.1/goldenretriever/common/upload.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/common/utils.py` & `goldenretriever_core-0.9.1/goldenretriever/common/utils.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/data/base/datasets.py` & `goldenretriever_core-0.9.1/goldenretriever/data/base/datasets.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/data/datasets.py` & `goldenretriever_core-0.9.1/goldenretriever/data/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         name: str,
         path: Union[str, os.PathLike, List[str], List[os.PathLike]] = None,
         data: Any = None,
         tokenizer: Optional[Union[str, tr.PreTrainedTokenizer]] = None,
         passage_batch_size: int = 32,
         question_batch_size: int = 32,
         max_positives: int = -1,
-        max_negatives: int = 0,
-        max_hard_negatives: int = 0,
+        max_negatives: int = -1,
+        max_hard_negatives: int = -1,
         max_question_length: int = 256,
         max_passage_length: int = 64,
         shuffle: bool = False,
         subsample_strategy: str | None = SubsampleStrategyEnum.NONE,
         subsample_portion: float = 0.1,
         num_proc: int | None = None,
         load_from_cache_file: bool = True,
@@ -396,15 +396,18 @@
     def to_torch_dataset(self) -> torch.utils.data.Dataset:
         shuffle_this_time = self.shuffle
 
         if (
             self.subsample_strategy
             and self.subsample_strategy != SubsampleStrategyEnum.NONE
         ):
-            number_of_samples = int(len(self.data) * self.subsample_portion)
+            if isinstance(self.subsample_portion, int):
+                number_of_samples = self.subsample_portion
+            else:
+                number_of_samples = int(len(self.data) * self.subsample_portion)
             if self.subsample_strategy == SubsampleStrategyEnum.RANDOM:
                 logger.info(
                     f"Random subsampling {number_of_samples} samples from {len(self.data)}"
                 )
                 data = (
                     deepcopy(self.data)
                     .shuffle(seed=42 + self.number_of_complete_iterations)
@@ -513,16 +516,25 @@
         passage = [dict(zip(passage, t)) for t in zip(*passage.values())]
 
         output = dict(
             question=question,
             passage=passage,
             positive_pssgs=passage[: len(positives)],
             positives=positives,
-            negatives=negatives,
-            hard_negatives=hard_negatives,
+            negatives=(
+                negatives
+                if len(negatives) > 0
+                else None
+            ),
+            hard_negatives=(
+                hard_negatives
+                if len(hard_negatives) > 0
+                # else datasets.Sequence(datasets.Value("string"))
+                else None
+            ),
         )
         return output
 
     @staticmethod
     def batch_fn(
         data: Dataset,
         passage_batch_size: int,
```

### Comparing `goldenretriever-core-0.9.0/goldenretriever/data/labels.py` & `goldenretriever_core-0.9.1/goldenretriever/data/labels.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/data/utils.py` & `goldenretriever_core-0.9.1/goldenretriever/data/utils.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/indexers/base.py` & `goldenretriever_core-0.9.1/goldenretriever/indexers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         Args:
             index (`int`):
                 The index of the document.
 
         Returns:
             `str`: The document.
         """
-        return self.documents.get_document_from_id(index)
+        return self.documents.get_document_from_index(index)
 
     def get_passage_from_index(self, index: int) -> str:
         """
         Get the document from the index.
 
         Args:
             index (`int`):
```

### Comparing `goldenretriever-core-0.9.0/goldenretriever/indexers/document.py` & `goldenretriever_core-0.9.1/goldenretriever/indexers/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,29 @@
 
         Returns:
             Optional[Document]: The document with the given text, or None if it does not exist.
         """
         if text not in self._documents_reverse_index:
             logger.warning(f"Document with text `{text}` does not exist, skipping")
         return self._documents_reverse_index.get(text, None)
+    
+    def get_document_from_index(self, index: int) -> Document | None:
+        """
+        Retrieve the document by its index.
+
+        Args:
+            index (`int`):
+                The index of the document to retrieve.
+
+        Returns:
+            Optional[Document]: The document with the given index, or None if it does not exist.
+        """
+        if index >= len(self._documents):
+            logger.warning(f"Document with index `{index}` does not exist, skipping")
+        return self._documents[index]
 
     def add_documents(self, documents: List[Document] | List[str] | List[Dict]) -> List[Document]:
         """
         Add a list of documents to the document store.
 
         Args:
             documents (`List[Document]`):
@@ -171,21 +186,25 @@
             metadata (`Dict`, optional, defaults to None):
                 The metadata of the document to add.
 
         Returns:
             Document: The document just added.
         """
         if isinstance(text, str):
+            # check if the document already exists
+            if text in self:
+                logger.warning(f"Document `{text}` already exists, skipping")
+                return self._documents_reverse_index[text]
             if id is None:
                 # get the len of the documents and add 1
                 id = len(self._documents)  # + 1
             text = Document(text, id, metadata)
 
         if text in self:
-            logger.warning(f"Document {text} already exists, skipping")
+            logger.warning(f"Document `{text}` already exists, skipping")
             return self._documents_index[text.id]
 
         self._documents.append(text)
         self._documents_index[text.id] = text
         self._documents_reverse_index[text.text] = text
         return text
         # if id in self._documents_index:
```

### Comparing `goldenretriever-core-0.9.0/goldenretriever/indexers/faiss.py` & `goldenretriever_core-0.9.1/goldenretriever/indexers/faiss.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
 
         # get int values (second element of the tuple)
         batch_top_k: List[List[int]] = retriever_out[1].detach().cpu().tolist()
         # get float values (first element of the tuple)
         batch_scores: List[List[float]] = retriever_out[0].detach().cpu().tolist()
         # Retrieve the passages corresponding to the indices
         batch_docs = [
-            [self.documents.get_document_from_id(i) for i in indices if i != -1]
+            [self.get_document_from_index(i) for i in indices if i != -1]
             for indices in batch_top_k
         ]
         # build the output object
         # build the output object
         batch_retrieved_samples = [
             [
                 RetrievedSample(document=doc, score=score)
```

### Comparing `goldenretriever-core-0.9.0/goldenretriever/indexers/inmemory.py` & `goldenretriever_core-0.9.1/goldenretriever/indexers/inmemory.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 
         # get int values
         batch_top_k: List[List[int]] = retriever_out.indices.detach().cpu().tolist()
         # get float values
         batch_scores: List[List[float]] = retriever_out.values.detach().cpu().tolist()
         # Retrieve the passages corresponding to the indices
         batch_docs = [
-            [self.documents.get_document_from_id(i) for i in indices]
+            [self.get_document_from_index(i) for i in indices]
             for indices in batch_top_k
         ]
         # build the output object
         batch_retrieved_samples = [
             [
                 RetrievedSample(document=doc, score=score)
                 for doc, score in zip(docs, scores)
```

### Comparing `goldenretriever-core-0.9.0/goldenretriever/indexers/voyager.py` & `goldenretriever_core-0.9.1/goldenretriever/indexers/voyager.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/lightning_modules/pl_data_modules.py` & `goldenretriever_core-0.9.1/goldenretriever/lightning_modules/pl_data_modules.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/lightning_modules/pl_modules.py` & `goldenretriever_core-0.9.1/goldenretriever/lightning_modules/pl_modules.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/__init__.py` & `goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/hf.py` & `goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/hf.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/loss.py` & `goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/loss.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/model.py` & `goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/model.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/optim.py` & `goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/optim.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/pytorch_modules/scheduler.py` & `goldenretriever_core-0.9.1/goldenretriever/pytorch_modules/scheduler.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/objects.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/objects.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/splitters/base_sentence_splitter.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/splitters/base_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/splitters/spacy_sentence_splitter.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/splitters/spacy_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/splitters/window_based_splitter.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/splitters/window_based_splitter.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/__init__.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/base_tokenizer.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/regex_tokenizer.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/regex_tokenizer.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/spacy_tokenizer.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/tokenizers/whitespace_tokenizer.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/tokenizers/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/data/window/manager.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/data/window/manager.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/server/backend/fastapi.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/server/backend/fastapi.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/server/backend/ray.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/server/backend/ray.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/server/backend/utils.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/server/backend/utils.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/server/frontend/relik_front.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/server/frontend/relik_front.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/server/frontend/utils.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/server/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/server/ray_old.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/server/ray_old.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/serve/utils/gunicorn_conf.py` & `goldenretriever_core-0.9.1/goldenretriever/serve/utils/gunicorn_conf.py`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever/trainer/train.py` & `goldenretriever_core-0.9.1/goldenretriever/trainer/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         # hard negatives callback parameters
         max_hard_negatives_to_mine: int = 15,
         hard_negatives_threshold: float = 0.0,
         metrics_to_monitor_for_hard_negatives: str | None = None,
         mine_hard_negatives_with_probability: float = 1.0,
         # other parameters
         seed: int = 42,
-        float32_matmul_precision: str = "medium",
+        float32_matmul_precision: str = "high",
         **kwargs,
     ):
         # put all the parameters in the class
         self.retriever = retriever
         # datasets
         self.train_dataset = train_dataset
         self.val_dataset = val_dataset
@@ -277,14 +277,15 @@
         self.last_checkpoint_kwargs: dict | None = None
         if self.save_last:
             last_checkpoint_kwargs = deepcopy(self.checkpoint_kwargs)
             last_checkpoint_kwargs["save_top_k"] = 1
             last_checkpoint_kwargs["filename"] = "last-{epoch}-{step}"
             last_checkpoint_kwargs["monitor"] = "step"
             last_checkpoint_kwargs["mode"] = "max"
+            last_checkpoint_kwargs["save_retriever"] = False
             self.last_checkpoint_kwargs = last_checkpoint_kwargs
 
         # early stopping callback
         early_stopping_kwargs = dict(
             monitor=self.metric_to_monitor,
             mode=self.monitor_mode,
             patience=self.early_stopping_patience,
@@ -329,35 +330,38 @@
     def configure_lightning_module(self, *args, **kwargs):
         # check if Index is empty
         if len(self.retriever.document_index) == 0:
             # add the docs from the datasets
             logger.info("Document Index is empty. Adding documents from the datasets.")
             documents = self.retriever.document_index.documents
             for sample in tqdm(self.train_dataset, desc="Adding documents from train"):
-                [documents.add_document(s) for s in sample["positives"]]
-                [documents.add_document(s) for s in sample["negatives"]]
-                [documents.add_document(s) for s in sample["hard_negatives"]]
+                if sample["positives"]:
+                    [documents.add_document(s) for s in sample["positives"]]
+                if sample["negatives"]:
+                    [documents.add_document(s) for s in sample["negatives"]]
+                if sample["hard_negatives"]:
+                    [documents.add_document(s) for s in sample["hard_negatives"]]
 
             if self.val_dataset is not None:
                 val_passages = []
                 for ds in self.val_dataset:
                     for sample in ds:
-                        val_passages.extend(sample["positives"])
-                        val_passages.extend(sample["negatives"])
-                        val_passages.extend(sample["hard_negatives"])
+                        val_passages.extend(sample["positives"] if sample["positives"] else [])
+                        val_passages.extend(sample["negatives"] if sample["negatives"] else [])
+                        val_passages.extend(sample["hard_negatives"] if sample["hard_negatives"] else [])
                 for sample in tqdm(val_passages, desc="Adding documents from val"):
                     documents.add_document(sample)
 
             if self.test_dataset is not None:
                 test_passages = []
                 for ds in self.test_dataset:
                     for sample in ds:
-                        test_passages.extend(sample["positives"])
-                        test_passages.extend(sample["negatives"])
-                        test_passages.extend(sample["hard_negatives"])
+                        test_passages.extend(sample["positives"] if sample["positives"] else [])
+                        test_passages.extend(sample["negatives"] if sample["negatives"] else [])
+                        test_passages.extend(sample["hard_negatives"] if sample["hard_negatives"] else [])
                 for sample in tqdm(test_passages, desc="Adding documents from test"):
                     documents.add_document(sample)
 
         # add loss object to the retriever
         if self.retriever.loss_type is None:
             self.retriever.loss_type = self.loss()
 
@@ -508,22 +512,25 @@
         mode: str,
         verbose: bool = True,
         save_top_k: int = 1,
         save_last: bool = False,
         filename: str | os.PathLike | None = None,
         dirpath: str | os.PathLike | None = None,
         auto_insert_metric_name: bool = False,
+        save_retriever: bool = True,
         *args,
         **kwargs,
     ) -> ModelCheckpoint:
         logger.info("Enabling Model Checkpointing")
         if dirpath is None:
             dirpath = (
                 self.experiment_path / "checkpoints" if self.experiment_path else None
             )
+        else:
+            dirpath = Path(dirpath) / self.wandb_project_name
         if filename is None:
             filename = (
                 "checkpoint-" + monitor + "_{" + monitor + ":.4f}-epoch_{epoch:02d}"
             )
         self.checkpoint_path = dirpath / filename if dirpath is not None else None
         logger.info(f"Checkpoint directory: {dirpath}")
         logger.info(f"Checkpoint filename: {filename}")
@@ -549,14 +556,18 @@
         # )
         # modelcheckpoint_kwargs = dict(
         #     dirpath=self.checkpoint_dir,
         #     filename=self.checkpoint_filename,
         # )
         # modelcheckpoint_kwargs.update(kwargs)
         self.model_checkpoint_callback = ModelCheckpoint(**kwargs)
+        self.callbacks_store.append(self.model_checkpoint_callback)
+
+        if save_retriever:
+            self.callbacks_store.append(SaveRetrieverCallback(saving_dir=dirpath / "retriever"))
         return self.model_checkpoint_callback
 
     def configure_hard_negatives_callback(self):
         metrics_to_monitor = (
             self.metrics_to_monitor_for_hard_negatives or self.metric_to_monitor
         )
         hard_negatives_callback = NegativeAugmentationCallback(
@@ -573,22 +584,22 @@
         return hard_negatives_callback
 
     def training_callbacks(self):
         if self.model_checkpointing:
             self.model_checkpoint_callback = self.configure_model_checkpoint(
                 **self.checkpoint_kwargs
             )
-            self.callbacks_store.append(self.model_checkpoint_callback)
+            # self.callbacks_store.append(self.model_checkpoint_callback)
             if self.save_last:
                 self.latest_model_checkpoint_callback = self.configure_model_checkpoint(
                     **self.last_checkpoint_kwargs
                 )
-                self.callbacks_store.append(self.latest_model_checkpoint_callback)
+                # self.callbacks_store.append(self.latest_model_checkpoint_callback)
 
-            self.callbacks_store.append(SaveRetrieverCallback())
+            # self.callbacks_store.append(SaveRetrieverCallback(saving_dir=))
         if self.early_stopping:
             self.early_stopping_callback = self.configure_early_stopping(
                 **self.early_stopping_kwargs
             )
         return self.callbacks_store
 
     def configure_metrics_callbacks(
```

### Comparing `goldenretriever-core-0.9.0/goldenretriever_core.egg-info/PKG-INFO` & `goldenretriever_core-0.9.1/goldenretriever_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goldenretriever-core
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dense Retriever
 Home-page: https://github.com/Riccorl/golden-retriever
 Author: Riccardo Orlando
 Author-email: orlandorcc@gmail.com
 License: Apache
 Keywords: NLP deep learning transformer pytorch retriever rag dpr
 Classifier: Intended Audience :: Science/Research
@@ -69,38 +69,42 @@
 </p>
 <p align="center">
   <a href="https://github.com/Riccorl/golden-retriever/releases"><img alt="release" src="https://img.shields.io/github/v/release/Riccorl/golden-retriever"></a>
   <a href="https://github.com/Riccorl/golden-retriever/actions/workflows/python-publish-pypi.yml"><img alt="gh-status" src="https://github.com/Riccorl/golden-retriever/actions/workflows/python-publish-pypi.yml/badge.svg"></a>
 
 </p>
 
+# WIP: distributed-compatible codebase
+
+A distributed-compatible codebase is under development. Check the `distributed` [branch](https://github.com/Riccorl/golden-retriever/tree/distributed) for the latest updates.
+
 # How to use
 
-Install the library from [PyPI]():
+Install the library from [PyPI](https://pypi.org/project/goldenretriever-core/):
 
 ```bash
-pip install goldenretriever
+pip install goldenretriever-core
 ```
 
 or from source:
 
 ```bash
 git clone https://github.com/Riccorl/golden-retriever.git
-cd goldenretriever
+cd golden-retriever
 pip install -e .
 ```
 
 # Usage
 
 ## How to run an experiment
 
 ### Training
 
 Here a simple example on how to train a DPR-like Retriever on the NQ dataset.
-First download the dataset from (DPR)[]. The run the following code:
+First download the dataset from [DPR](https://github.com/facebookresearch/DPR?tab=readme-ov-file#retriever-input-data-format). The run the following code:
 
 ```python
 from goldenretriever.trainer import Trainer
 from goldenretriever import GoldenRetriever
 from goldenretriever.data.datasets import InBatchNegativesDataset
 
 # create a retriever
@@ -196,34 +200,34 @@
 ### Input data
 
 The retriever expects a jsonl file similar to [DPR](https://github.com/facebookresearch/DPR):
 
 ```json lines
 [
   {
-	"question": "....",
-	"answers": ["...", "...", "..."],
-	"positive_ctxs": [{
-		"title": "...",
-		"text": "...."
-	}],
-	"negative_ctxs": ["..."],
-	"hard_negative_ctxs": ["..."]
+  "question": "....",
+  "answers": ["...", "...", "..."],
+  "positive_ctxs": [{
+    "title": "...",
+    "text": "...."
+  }],
+  "negative_ctxs": ["..."],
+  "hard_negative_ctxs": ["..."]
   },
   ...
 ]
 ```
 
 ### Index data
 
-The document to index can be either a jsonl file or a tsv file similar to 
+The document to index can be either a jsonl file or a tsv file similar to
 [DPR](https://github.com/facebookresearch/DPR):
 
 - `jsonl`: each line is a json object with the following keys: `id`, `text`, `metadata`
-- `tsv`: each line is a tab-separated string with the `id` and `text` column, 
+- `tsv`: each line is a tab-separated string with the `id` and `text` column,
   followed by any other column that will be stored in the `metadata` field
 
 jsonl example:
 
 ```json lines
 [
   {
@@ -237,8 +241,7 @@
 
 tsv example:
 
 ```tsv
 id \t text \t any other column
 ...
 ```
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: goldenretriever-core Version: 0.9.0 Summary: Dense
+Metadata-Version: 2.1 Name: goldenretriever-core Version: 0.9.1 Summary: Dense
 Retriever Home-page: https://github.com/Riccorl/golden-retriever Author:
 Riccardo Orlando Author-email: orlandorcc@gmail.com License: Apache Keywords:
 NLP deep learning transformer pytorch retriever rag dpr Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
 >=3.10 Description-Content-Type: text/markdown Requires-Dist: torch<2.3,>=2.1
@@ -30,25 +30,30 @@
 [standard]<0.28,>=0.24; extra == "serve" Requires-Dist: gunicorn==21.2.0; extra
 == "serve" Requires-Dist: ray[serve]<=2.10,>=2.8; extra == "serve" Provides-
 Extra: dev Requires-Dist: pre-commit; extra == "dev" Requires-Dist: black[d];
 extra == "dev" Requires-Dist: isort; extra == "dev"
                       ************ ?ð??¦?® GGoollddeenn RReettrriieevveerr ************
                 _[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_v_s_c_o_d_e_]
                              _[_r_e_l_e_a_s_e_]_[_g_h_-_s_t_a_t_u_s_]
-# How to use Install the library from [PyPI](): ```bash pip install
-goldenretriever ``` or from source: ```bash git clone https://github.com/
-Riccorl/golden-retriever.git cd goldenretriever pip install -e . ``` # Usage ##
-How to run an experiment ### Training Here a simple example on how to train a
-DPR-like Retriever on the NQ dataset. First download the dataset from (DPR)[].
-The run the following code: ```python from goldenretriever.trainer import
-Trainer from goldenretriever import GoldenRetriever from
-goldenretriever.data.datasets import InBatchNegativesDataset # create a
-retriever retriever = GoldenRetriever( question_encoder="intfloat/e5-small-v2",
-passage_encoder="intfloat/e5-small-v2" ) # create a dataset train_dataset =
-InBatchNegativesDataset( name="webq_train", path="path/to/webq_train.json",
+# WIP: distributed-compatible codebase A distributed-compatible codebase is
+under development. Check the `distributed` [branch](https://github.com/Riccorl/
+golden-retriever/tree/distributed) for the latest updates. # How to use Install
+the library from [PyPI](https://pypi.org/project/goldenretriever-core/):
+```bash pip install goldenretriever-core ``` or from source: ```bash git clone
+https://github.com/Riccorl/golden-retriever.git cd golden-retriever pip install
+-e . ``` # Usage ## How to run an experiment ### Training Here a simple example
+on how to train a DPR-like Retriever on the NQ dataset. First download the
+dataset from [DPR](https://github.com/facebookresearch/DPR?tab=readme-ov-
+file#retriever-input-data-format). The run the following code: ```python from
+goldenretriever.trainer import Trainer from goldenretriever import
+GoldenRetriever from goldenretriever.data.datasets import
+InBatchNegativesDataset # create a retriever retriever = GoldenRetriever
+( question_encoder="intfloat/e5-small-v2", passage_encoder="intfloat/e5-small-
+v2" ) # create a dataset train_dataset = InBatchNegativesDataset
+( name="webq_train", path="path/to/webq_train.json",
 tokenizer=retriever.question_tokenizer, question_batch_size=64,
 passage_batch_size=400, max_passage_length=64, shuffle=True, ) val_dataset =
 InBatchNegativesDataset( name="webq_dev", path="path/to/webq_dev.json",
 tokenizer=retriever.question_tokenizer, question_batch_size=64,
 passage_batch_size=400, max_passage_length=64, ) trainer = Trainer
 ( retriever=retriever, train_dataset=train_dataset, val_dataset=val_dataset,
 max_steps=25_000, wandb_online_mode=True, wandb_project_name="golden-retriever-
```

### Comparing `goldenretriever-core-0.9.0/goldenretriever_core.egg-info/SOURCES.txt` & `goldenretriever_core-0.9.1/goldenretriever_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/goldenretriever_core.egg-info/requires.txt` & `goldenretriever_core-0.9.1/goldenretriever_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/requirements.txt` & `goldenretriever_core-0.9.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `goldenretriever-core-0.9.0/setup.py` & `goldenretriever_core-0.9.1/setup.py`

 * *Files identical despite different names*

