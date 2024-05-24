# Comparing `tmp/optimum-nvidia-0.1.0b6.tar.gz` & `tmp/optimum_nvidia-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-nvidia-0.1.0b6.tar", last modified: Thu Apr 11 21:09:44 2024, max compression
+gzip compressed data, was "optimum_nvidia-0.1.0b7.tar", last modified: Fri May 24 12:47:17 2024, max compression
```

## Comparing `optimum-nvidia-0.1.0b6.tar` & `optimum_nvidia-0.1.0b7.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.170442 optimum-nvidia-0.1.0b6/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    11357 2023-12-05 19:15:32.000000 optimum-nvidia-0.1.0b6/LICENSE
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7404 2024-04-11 21:09:44.170442 optimum-nvidia-0.1.0b6/PKG-INFO
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5099 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/README.md
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2795 2024-04-08 21:01:57.000000 optimum-nvidia-0.1.0b6/pyproject.toml
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      584 2024-04-11 21:09:44.170442 optimum-nvidia-0.1.0b6/setup.cfg
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3344 2024-04-08 21:02:05.000000 optimum-nvidia-0.1.0b6/setup.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.165442 optimum-nvidia-0.1.0b6/src/
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.165442 optimum-nvidia-0.1.0b6/src/optimum/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      646 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/__init__.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      853 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/__init__.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      686 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     9713 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/config.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5180 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/local.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7297 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/config.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1855 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/errors.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/generation/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1448 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/generation/logits_process.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    19797 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/hub.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/lang/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3808 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/lang/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      987 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/logging.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.166442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      728 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2612 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/auto.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1365 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/base.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4447 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/gemma.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4426 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/llama.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4483 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/mistral.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    50629 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/whisper.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.167442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4968 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      792 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/base.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     9226 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/text_generation.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.167442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      779 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/__init__.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.167442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      171 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5810 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/config.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4907 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/quantizer.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    10814 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/datasets.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    13945 2024-04-11 20:00:38.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/runtime.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.168442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1422 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4131 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/cli.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1040 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/constants.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1337 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/env.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2655 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/hub.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3098 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/nvml.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2023 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/offload.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2798 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/onnx.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1438 2024-04-05 09:31:00.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/patching.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.168442 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      694 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/__init__.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1972 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/utils.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      754 2024-04-11 21:09:31.000000 optimum-nvidia-0.1.0b6/src/optimum/nvidia/version.py
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.168442 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7404 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/PKG-INFO
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1815 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/SOURCES.txt
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)       24 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/dependency_links.txt
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)        1 2024-04-08 21:15:11.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/not-zip-safe
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      392 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/requires.txt
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)        8 2024-04-11 21:09:44.000000 optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/top_level.txt
-drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-04-11 21:09:44.168442 optimum-nvidia-0.1.0b6/tests/
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2295 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/tests/test_config.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1729 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/tests/test_dtype.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2235 2024-04-05 13:23:27.000000 optimum-nvidia-0.1.0b6/tests/test_hub.py
--rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1331 2024-04-04 13:25:57.000000 optimum-nvidia-0.1.0b6/tests/test_quantization.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.592354 optimum_nvidia-0.1.0b7/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    11357 2023-12-05 19:15:32.000000 optimum_nvidia-0.1.0b7/LICENSE
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7467 2024-05-24 12:47:17.592354 optimum_nvidia-0.1.0b7/PKG-INFO
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5169 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/README.md
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2790 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/pyproject.toml
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      584 2024-05-24 12:47:17.593354 optimum_nvidia-0.1.0b7/setup.cfg
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3330 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/setup.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.587354 optimum_nvidia-0.1.0b7/src/
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.587354 optimum_nvidia-0.1.0b7/src/optimum/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      646 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/__init__.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.588353 optimum_nvidia-0.1.0b7/src/optimum/nvidia/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      853 2024-05-21 08:13:33.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/__init__.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.588353 optimum_nvidia-0.1.0b7/src/optimum/nvidia/builder/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      686 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/builder/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     9713 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/builder/config.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5473 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/builder/local.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7692 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/config.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2027 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/errors.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.588353 optimum_nvidia-0.1.0b7/src/optimum/nvidia/generation/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1448 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/generation/logits_process.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    21839 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/hub.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.588353 optimum_nvidia-0.1.0b7/src/optimum/nvidia/lang/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3808 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/lang/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      987 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/logging.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.589354 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      728 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2687 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/auto.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1365 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/base.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4725 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/gemma.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4778 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/llama.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4755 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/mistral.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4889 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/mixtral.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    51158 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/whisper.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.589354 optimum_nvidia-0.1.0b7/src/optimum/nvidia/pipelines/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5052 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/pipelines/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      792 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/pipelines/base.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     9226 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/pipelines/text_generation.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.589354 optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      779 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/__init__.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.589354 optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/ammo/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      171 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/ammo/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     5810 2024-04-05 13:23:27.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/ammo/config.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4907 2024-04-05 13:23:27.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/ammo/quantizer.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    10814 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/datasets.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)    13954 2024-05-21 11:45:13.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/runtime.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.590354 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1422 2024-05-08 14:27:06.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     4169 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/cli.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1040 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/constants.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1337 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/env.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2655 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/hub.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     3098 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/nvml.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2023 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/offload.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2798 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/onnx.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1438 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/patching.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.590354 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/tests/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      840 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/tests/__init__.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      973 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/tests/assertions.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2084 2024-05-06 07:50:07.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/tests/utils.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      754 2024-05-24 12:46:00.000000 optimum_nvidia-0.1.0b7/src/optimum/nvidia/version.py
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.591354 optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     7467 2024-05-24 12:47:17.000000 optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/PKG-INFO
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1897 2024-05-24 12:47:17.000000 optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/SOURCES.txt
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)       24 2024-05-24 12:47:17.000000 optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/dependency_links.txt
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)        1 2024-05-12 21:18:11.000000 optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/not-zip-safe
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)      385 2024-05-24 12:47:17.000000 optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/requires.txt
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)        8 2024-05-24 12:47:17.000000 optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/top_level.txt
+drwxr-xr-x   0 mfuntowicz  (1000) mfuntowicz  (1000)        0 2024-05-24 12:47:17.591354 optimum_nvidia-0.1.0b7/tests/
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2295 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/tests/test_config.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1729 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/tests/test_dtype.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     2170 2024-05-24 11:19:43.000000 optimum_nvidia-0.1.0b7/tests/test_hub.py
+-rw-r--r--   0 mfuntowicz  (1000) mfuntowicz  (1000)     1331 2024-04-04 13:25:57.000000 optimum_nvidia-0.1.0b7/tests/test_quantization.py
```

### Comparing `optimum-nvidia-0.1.0b6/LICENSE` & `optimum_nvidia-0.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/PKG-INFO` & `optimum_nvidia-0.1.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-nvidia
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Optimum Nvidia is the interface between the Hugging Face Transformers and NVIDIA GPUs. "
 Home-page: https://huggingface.co/hardware/nvidia
 Author: HuggingFace Inc. Machine Learning Optimization Team
 Author-email: "HuggingFace Inc. Machine Learning Optimization Team" <hardware@huggingface.co>
 License: Apache/2.0
 Project-URL: Homepage, https://huggingface.co/hardware/nvidia
 Project-URL: Repository, https://github.com/huggingface/optimum-nvidia
@@ -22,19 +22,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate==0.25
 Requires-Dist: datasets>=2.14.0
 Requires-Dist: huggingface-hub>=0.22.0
 Requires-Dist: hf-transfer
 Requires-Dist: mpmath==1.3.0
-Requires-Dist: numpy>=1.26.0
+Requires-Dist: numpy<2.0.0,>=1.26.0
 Requires-Dist: onnx>=1.12.0
 Requires-Dist: optimum>=1.13.0
 Requires-Dist: setuptools
-Requires-Dist: tensorrt-llm==0.9.0.dev2024031900
+Requires-Dist: tensorrt-llm==0.9.0
 Requires-Dist: torch<=2.3.0a,>=2.2.0a
 Requires-Dist: transformers>=4.38.2
 Requires-Dist: pynvml
 Provides-Extra: tests
 Requires-Dist: mock; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
@@ -139,15 +139,18 @@
 + from optimum.nvidia import AutoModelForCausalLM
 from transformers import AutoTokenizer
 
 tokenizer = AutoTokenizer.from_pretrained("meta-llama/Llama-2-7b-chat-hf", padding_side="left")
 
 model = AutoModelForCausalLM.from_pretrained(
   "meta-llama/Llama-2-7b-chat-hf",
-+ use_fp8=True,  
++ use_fp8=True,
++ max_prompt_length=1024,
++ max_output_length=2048, # Must be at least size of max_prompt_length + max_new_tokens
++ max_batch_size=8,
 )
 
 model_inputs = tokenizer(["How is autonomous vehicle technology transforming the future of transportation and urban planning?"], return_tensors="pt").to("cuda")
 
 generated_ids = model.generate(
     **model_inputs, 
     top_k=40, 
@@ -160,15 +163,14 @@
 
 To learn more about text generation with LLMs, check out [this guide](https://huggingface.co/docs/transformers/llm_tutorial)!
 
 <!-- For more details, read our [documentation](https://huggingface.com/docs/optimum/nvidia/index). -->
 
 # Support Matrix
 We test Optimum-NVIDIA on 4090, L40S, and H100 Tensor Core GPUs, though it is expected to work on any GPU based on the following architectures: 
-* Turing (with experimental support for T4 / RTX Quadro x000)
 * Ampere (A100/A30 are supported. Experimental support for A10, A40, RTX Ax000)
 * Hopper
 * Ada-Lovelace
 
 Note that FP8 support is only available on GPUs based on Hopper and Ada-Lovelace architectures.
 
 Optimum-NVIDIA works on Linux will support Windows soon.
```

### Comparing `optimum-nvidia-0.1.0b6/README.md` & `optimum_nvidia-0.1.0b7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -84,15 +84,18 @@
 + from optimum.nvidia import AutoModelForCausalLM
 from transformers import AutoTokenizer
 
 tokenizer = AutoTokenizer.from_pretrained("meta-llama/Llama-2-7b-chat-hf", padding_side="left")
 
 model = AutoModelForCausalLM.from_pretrained(
   "meta-llama/Llama-2-7b-chat-hf",
-+ use_fp8=True,  
++ use_fp8=True,
++ max_prompt_length=1024,
++ max_output_length=2048, # Must be at least size of max_prompt_length + max_new_tokens
++ max_batch_size=8,
 )
 
 model_inputs = tokenizer(["How is autonomous vehicle technology transforming the future of transportation and urban planning?"], return_tensors="pt").to("cuda")
 
 generated_ids = model.generate(
     **model_inputs, 
     top_k=40, 
@@ -105,15 +108,14 @@
 
 To learn more about text generation with LLMs, check out [this guide](https://huggingface.co/docs/transformers/llm_tutorial)!
 
 <!-- For more details, read our [documentation](https://huggingface.com/docs/optimum/nvidia/index). -->
 
 # Support Matrix
 We test Optimum-NVIDIA on 4090, L40S, and H100 Tensor Core GPUs, though it is expected to work on any GPU based on the following architectures: 
-* Turing (with experimental support for T4 / RTX Quadro x000)
 * Ampere (A100/A30 are supported. Experimental support for A10, A40, RTX Ax000)
 * Hopper
 * Ada-Lovelace
 
 Note that FP8 support is only available on GPUs based on Hopper and Ada-Lovelace architectures.
 
 Optimum-NVIDIA works on Linux will support Windows soon.
```

### Comparing `optimum-nvidia-0.1.0b6/pyproject.toml` & `optimum_nvidia-0.1.0b7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 # List dependencies
 dependencies = [
     "accelerate == 0.25",
     "datasets >= 2.14.0",
     "huggingface-hub >= 0.22.0",
     "hf-transfer",
     "mpmath == 1.3.0",
-    "numpy >= 1.26.0",
+    "numpy >= 1.26.0, < 2.0.0",
     "onnx >= 1.12.0",
     "optimum >= 1.13.0",
     "setuptools",
-    "tensorrt-llm == 0.9.0.dev2024031900",
+    "tensorrt-llm == 0.9.0",
     "torch>=2.2.0a,<=2.3.0a",
     "transformers >= 4.38.2",
     "pynvml"
 ]
 
 
 [project.urls]
```

### Comparing `optimum-nvidia-0.1.0b6/setup.cfg` & `optimum_nvidia-0.1.0b7/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/setup.py` & `optimum_nvidia-0.1.0b7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "huggingface-hub >= 0.22.0",
     "hf-transfer",
     "mpmath == 1.3.0",
     "numpy >= 1.26.0",
     "onnx >= 1.12.0",
     "optimum >= 1.13.0",
     "setuptools",
-    "tensorrt-llm == 0.9.0.dev2024031900",
+    "tensorrt-llm == 0.9.0",
     "torch>=2.2.0a,<=2.3.0a",
     "transformers >= 4.38.2",
     "pynvml"
 ]
 
 TESTS_REQUIRES = [
     "mock",
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/config.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/builder/config.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/builder/local.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/builder/local.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,15 +55,18 @@
 
 
 class LocalEngineBuilder:
     TRTLLM_BUILD_EXEC = "trtllm-build"
 
     @staticmethod
     def build_cli_command(
-        root: Path, model_config: TensorRTConfig, build_config: EngineConfig
+        checkpoints: Path,
+        engines: Path,
+        model_config: TensorRTConfig,
+        build_config: EngineConfig,
     ) -> Dict[str, Any]:
         workload_params = {
             "--max_batch_size": build_config.workload_profile.max_batch_size,
             "--max_input_len": build_config.workload_profile.max_input_len,
             "--max_output_len": build_config.workload_profile.max_output_len,
         }
 
@@ -79,48 +82,53 @@
         plugins_params = {
             f"--{name}": process_plugin_flag(name, value)
             for name in CLI_PLUGIN_NAMES
             if (value := getattr(build_config.plugins_config, name)) is not None
         }
 
         build_params = {
-            "--checkpoint_dir": root,
-            "--output_dir": root,
-            "--model_config": root / "config.json",
+            "--checkpoint_dir": checkpoints,
+            "--output_dir": engines,
+            "--model_config": checkpoints / "model.json",
             "--builder_opt": build_config.optimisation_level,
             "--logits_dtype": build_config.logits_dtype,
+            "--tp_size": model_config.mapping.tp_size,
+            "--pp_size": model_config.mapping.pp_size,
         }
 
         if hasattr(model_config, "trt_model_class") and hasattr(
             model_config, "trt_model_file"
         ):
             build_params["--model_cls_file"] = model_config.trt_model_file
             build_params["--model_cls_name"] = model_config.trt_model_class
 
         if model_config.supports_strong_typing():
             build_params["--strongly_typed"] = None
 
         return build_params | generation_params | workload_params | plugins_params
 
-    def __init__(self, config: TensorRTConfig, output_folder: Path):
+    def __init__(
+        self, config: TensorRTConfig, checkpoint_folder: Path, output_folder: Path
+    ):
         self._config = config
+        self._checkpoint_folder = checkpoint_folder
         self._output_folder = output_folder
 
     def build(self, config: EngineConfig):
         cli_params = LocalEngineBuilder.build_cli_command(
-            self._output_folder, self._config, config
+            self._checkpoint_folder, self._output_folder, self._config, config
         )
         cli_params_list = [str(t) for t in chain.from_iterable(cli_params.items())]
         cli_params_list = [i for i in cli_params_list if i != "None"]
 
         LOGGER.info(f"trtllm-build parameters: {cli_params_list}")
 
         for rank in range(self._config.mapping.world_size):
             ranked_checkpoint = f"rank{rank}.safetensors"
-            if not (self._output_folder / ranked_checkpoint).exists():
+            if not (self._checkpoint_folder / ranked_checkpoint).exists():
                 raise ValueError(
                     f"Missing rank-{rank} checkpoints (rank{rank}.safetensors), cannot build."
                 )
 
         # TODO: Remove BuilderPatcher once TensorRT-LLM updates its codebase to allow to disable `optimize(network)`.
         with BuilderPatcher():
             # Run the build
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/config.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 import json
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Optional, Union
 
 import torch
 from tensorrt_llm import Mapping
+from tensorrt_llm.layers import MoeConfig
 from tensorrt_llm.models import PretrainedConfig as TensorRTPretrainedConfig
 from tensorrt_llm.models.modeling_utils import (
-    QuantizationConfig as TensorRTQuantizationConfig,
+    QuantConfig as TensorRTQuantizationConfig,
 )
 from tensorrt_llm.plugin import PluginConfig
 from tensorrt_llm.quantization import QuantMode
 from transformers import AutoConfig, PretrainedConfig
 
 from optimum.nvidia.quantization import AmmoQuantizationConfig
 from optimum.nvidia.utils import get_user_agent
@@ -111,15 +112,15 @@
             use_int4_weights=weight_num_bits == 4,
         )
         return mode, f"W{weight_num_bits}A16_GPTQ"
     else:
         raise ValueError(f"Unsupported quantization method: {method}")
 
 
-class TensorRTConfig(ABC, TensorRTPretrainedConfig):
+class TensorRTConfig(TensorRTPretrainedConfig, ABC):
     @staticmethod
     def get_quantization_config(
         config: PretrainedConfig,
     ) -> (QuantMode, AmmoQuantizationConfig):
         if hasattr(config, "quantization_config"):
             qconfig = config.quantization_config
             num_bits = qconfig.num_bits
@@ -140,36 +141,51 @@
         else:
             return QuantMode.from_description(), TensorRTQuantizationConfig(
                 None, None, None, False, None
             )
 
     @staticmethod
     @abstractmethod
-    def from_config(config: PretrainedConfig) -> "TensorRTConfig":
+    def from_config(
+        config: PretrainedConfig, mapping: Optional[Mapping]
+    ) -> "TensorRTConfig":
         raise NotImplementedError()
 
     @staticmethod
     def from_pretrained(
         model_id_or_path: str,
+        *,
         revision: Optional[str] = None,
         token: Union[bool, str, None] = None,
+        mapping: Optional[Mapping] = None,
     ):
         config = AutoConfig.from_pretrained(
             model_id_or_path,
             revision=revision,
             token=token,
             user_agent=get_user_agent(),
         )
-        return TensorRTConfig.from_config(config)
+        return TensorRTConfig.from_config(config, mapping)
 
     @staticmethod
     @abstractmethod
     def supports_strong_typing() -> bool:
         raise NotImplementedError()
 
+    @property
+    def has_moe(self) -> bool:
+        return getattr(self, "moe_num_experts", 1)
+
+    @property
+    def moe_config(self) -> Optional[MoeConfig]:
+        if self.has_moe:
+            return MoeConfig()
+        else:
+            return None
+
     def shard(
         self,
         world_size: int,
         gpus_per_node: int,
         rank: int = 0,
         tp_degree: int = 1,
         pp_degree: int = 1,
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/errors.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,49 +8,54 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+from typing import Optional
 
 from optimum.nvidia.utils.nvml import SM_FP8_SUPPORTED
 
 
 class OptimumNvidiaException(Exception):
-    def __init__(self, operation: str, msg: str):
-        super().__init__(f"[{operation}] {msg}.")
+    def __init__(self, msg: str, operation: Optional[str] = None):
+        if operation:
+            super().__init__(f"[{operation}] {msg}.")
+        else:
+            super().__init__(f"{msg}")
 
 
 ### Model support
 class UnsupportedModelException(OptimumNvidiaException):
     def __init__(self, model_type: str):
-        super(
+        super().__init__(
             f"Model of type {model_type} is not supported. "
             "Please open-up an issue at https://github.com/huggingface/optimum-nvidia/issues"
         )
 
 
 ### Unsupported features blocks
 class UnsupportedHardwareFeature(OptimumNvidiaException):
     """
     Base exception class for all features not supported by underlying hardware
     """
 
-    def __init__(self, msg):
-        super("feature", msg)
+    def __init__(self, msg, feature: str):
+        super(msg)
 
     @classmethod
     def float8(cls) -> "UnsupportedHardwareFeature":
         return Float8NotSupported()
 
 
 class Float8NotSupported(UnsupportedHardwareFeature):
     """
     Thrown when attempting to target float8 inference but the underlying hardware doesn't support it
     """
 
     def __init__(self):
-        super(
+        super().__init__(
             "float8 is not supported on your device. "
-            f"Please use a device with compute capabilities {SM_FP8_SUPPORTED}"
+            f"Please use a device with compute capabilities {SM_FP8_SUPPORTED}",
+            "float8",
         )
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/generation/logits_process.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/generation/logits_process.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/hub.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,35 +31,45 @@
 from warnings import warn
 
 import numpy as np
 import torch
 from huggingface_hub import ModelHubMixin, snapshot_download
 from huggingface_hub.hub_mixin import T
 from safetensors.torch import save_file as to_safetensors
+from tensorrt_llm import Mapping
 from tensorrt_llm._utils import numpy_to_torch
 from tensorrt_llm.models.modeling_utils import PretrainedConfig, PretrainedModel
 from transformers import AutoConfig, AutoTokenizer, GenerationConfig
 from transformers import PreTrainedModel as TransformersPretrainedModel
 from transformers.utils import SAFE_WEIGHTS_INDEX_NAME
 
 from optimum.nvidia import TensorRTConfig
 from optimum.nvidia.builder import LocalEngineBuilder
 from optimum.nvidia.builder.config import EngineConfigBuilder
 from optimum.nvidia.quantization import AutoQuantizationConfig
 from optimum.nvidia.quantization.ammo import AmmoQuantizer
 from optimum.nvidia.utils import get_user_agent, maybe_offload_weights_to_cpu
-from optimum.nvidia.utils.nvml import get_max_memory
 
 
 ATTR_TRTLLM_ENGINE_FOLDER = "__trtllm_engine_folder__"
+ATTR_TRTLLM_CHECKPOINT_FOLDER = "__trtllm_checkpoint_folder__"
+FOLDER_TRTLLM_CHECKPOINTS = "checkpoints"
 FOLDER_TRTLLM_ENGINES = "engines"
+FILE_TRTLLM_CHECKPOINT_PATTERN = "rank[0-9]*.safetensors"
 FILE_TRTLLM_ENGINE_PATTERN = "rank[0-9]*.engine"
 
 HUB_TRTLLM_ENGINE_PATTERNS = ["**/config.json", f"**/{FILE_TRTLLM_ENGINE_PATTERN}"]
 HUB_SAFETENSORS_PATTERNS = ["config.json", "*.safetensors", SAFE_WEIGHTS_INDEX_NAME]
+
+SHARDING_KWARGS = {"tp_size", "pp_size", "world_size", "gpus_per_node", "rank"}
+SHARDING_KWARGS_ALIASES = {
+    "tp": "tp_size",
+    "pp": "pp_size",
+}
+
 LOGGER = getLogger()
 LOGGER.setLevel(level="INFO")
 
 
 def extract_model_type(config: Dict[str, Any]) -> Tuple[Optional[str], bool]:
     if "model_type" in config:
         model_type = config["model_type"]
@@ -111,18 +121,50 @@
     if len(relative_folders) == 2 and "decoder" in relative_folders[0].as_posix():
         folders.reverse()
         relative_folders.reverse()
 
     return folders, relative_folders
 
 
+def get_sharding_info(**kwargs):
+    mapping_kwargs = {}
+
+    for name_, value in kwargs.items():
+        # Handle aliased args
+        if name_ in SHARDING_KWARGS_ALIASES:
+            name = SHARDING_KWARGS_ALIASES[name_]
+        else:
+            name = name_
+
+        # Ensure we are targeting a sharding kwarg
+        if name in SHARDING_KWARGS:
+            # Check if not already present
+            if name in mapping_kwargs and name != name_:
+                LOGGER.warning(f"Parameter {name} already defined through {name_}")
+
+            mapping_kwargs[name] = value
+
+    if mapping_kwargs:
+        if "world_size" not in mapping_kwargs:
+            mapping_kwargs["world_size"] = (
+                mapping_kwargs["tp_size"] * mapping_kwargs["pp_size"]
+            )
+            LOGGER.debug(
+                f"Set sharding_info's world_size to {mapping_kwargs['world_size']}"
+            )
+        return Mapping(**mapping_kwargs)
+    else:
+        return None
+
+
 @runtime_checkable
 class SupportsTensorrtConversion(Protocol):
     MODEL_CONFIG: Type[TensorRTConfig]
     HF_LIBRARY_TARGET_MODEL_CLASS: Type[ModelHubMixin]
+
     TRT_LLM_TARGET_MODEL_CLASS: Type[PretrainedModel]
 
     @staticmethod
     def convert_weights(
         target: PretrainedModel,
         source: TransformersPretrainedModel,
         config: PretrainedConfig,
@@ -135,41 +177,47 @@
         cls,
         local_path: Path,
         hf_model_config: Dict,
         engine_save_path: Optional[Path] = None,
         hf_model: Optional[TransformersPretrainedModel] = None,
         config_class: Optional[TensorRTConfig] = None,
         **model_kwargs,
-    ) -> Tuple[List[Path], List[Path]]:
+    ) -> Tuple[List[Path], List[Path], List[Path]]:
         """
         :param local_path:
         :param hf_model_config:
         :param model_kwargs:
         :return:
         """
 
         # Path where will be stored the engines
-        if engine_save_path is None:
-            engine_save_path = local_path
-            engines_folder = local_path / FOLDER_TRTLLM_ENGINES
-            engines_folder.mkdir(exist_ok=True, parents=True)
-        else:
-            engines_folder = engine_save_path / FOLDER_TRTLLM_ENGINES
-            engines_folder.mkdir(exist_ok=True, parents=True)
+        root = engine_save_path if engine_save_path else local_path
+        checkpoint_folder = root / FOLDER_TRTLLM_CHECKPOINTS
+        engines_folder = root / FOLDER_TRTLLM_ENGINES
+
+        # Ensure all the tree exists
+        checkpoint_folder.mkdir(exist_ok=True, parents=True)
+        engines_folder.mkdir(exist_ok=True, parents=True)
 
         # Retrieve configuration
         config = AutoConfig.for_model(**hf_model_config)
         if "torch_dtype" in model_kwargs:
             config.torch_dtype = model_kwargs["torch_dtype"]
 
+        # Get sharding information to forward to the config converted
+        model_kwargs["mapping"] = get_sharding_info(**model_kwargs)
+
         # Convert the original config to a model config TRTLLM understands
         model_config = HuggingFaceHubModel.convert_config_to_trtllm(
             cls, config, config_class=config_class, **model_kwargs
         )
 
+        if model_config.has_moe:
+            model_config.moe_config.validate()
+
         # We now have a TRTLLM compatible config, so let's feed it to the target TRTLLM model to create a checkpoint
         LOGGER.debug("Allocating TRTLLM model to build the checkpoint")
         model = cls.TRT_LLM_TARGET_MODEL_CLASS.from_config(model_config)
 
         # Retrieve the parameters for building the engine
         if "engine_config" in model_kwargs:
             engine_config = model_kwargs.pop("engine_config")
@@ -177,25 +225,23 @@
             builder = EngineConfigBuilder.from_dict(model_config, **model_kwargs)
             builder.with_plugins_config(model_config.get_plugins_config())
             engine_config = builder.build()
 
         if engine_config.plugins_config is None:
             engine_config.plugins_config = model_config.get_plugins_config()
 
-        max_memory = get_max_memory()
-
         if hf_model is None:
             LOGGER.debug(
                 f"Loading weights from {local_path} into the model ({cls.HF_LIBRARY_TARGET_MODEL_CLASS.__name__})"
             )
 
             hf_model = cls.HF_LIBRARY_TARGET_MODEL_CLASS.from_pretrained(
                 local_path,
-                device_map="auto",
-                max_memory=max_memory,
+                torch_dtype="auto",
+                device_map="cpu",
                 local_files_only=True,
             )
         else:
             if not isinstance(hf_model, cls.HF_LIBRARY_TARGET_MODEL_CLASS):
                 raise ValueError(
                     f"Expected a {cls.HF_LIBRARY_TARGET_MODEL_CLASS.__name__} model to be provided, but the argument `hf_model` is a {hf_model.__class__.__name__}."
                 )
@@ -243,15 +289,15 @@
                     "you can control the quantization process manually with this API: "
                     "qconfig = AutoQuantizationConfig.from_description(weight='float8', activation='float8', ...) "
                     "forwarding the configuration to .from_pretrained(..., quantization_config=qconfig)"
                 )
 
             hf_quantizer = AmmoQuantizer(
                 quantization_config=qconfig,
-                artifact_path=engines_folder,
+                artifact_path=checkpoint_folder,
                 tensor_parallel_degree=engine_config.sharding_profile.tensor_parallelism,
                 pipeline_parallel_degree=engine_config.sharding_profile.pipeline_parallelism,
                 export_tensorrt_llm_config=True,
             )
 
             hf_quantizer.preprocess_model(hf_model, batch_size=1)
             hf_quantizer.postprocess_model(hf_model)
@@ -260,40 +306,48 @@
             # Apply the conversion from Hugging Face weights to TRTLLM
             for rank in range(model_config.mapping.world_size):
                 LOGGER.debug(
                     f"Converting weights from Hugging Face checkpoint for rank {rank}"
                 )
                 model_config.set_rank(rank)
                 converted_weights = cls.convert_weights(model, hf_model, model_config)
-                converted_weights = {
-                    name: numpy_to_torch(tensor)
-                    for name, tensor in converted_weights.items()
-                }
 
                 # Bind the converted weights against the TRTLLM model
                 model.load(converted_weights)
 
                 # Write ranked-checkpoints
+                converted_weights = {
+                    name: numpy_to_torch(tensor)
+                    if isinstance(tensor, np.ndarray)
+                    else tensor
+                    for name, tensor in converted_weights.items()
+                }
                 to_safetensors(
                     converted_weights,
-                    engines_folder / f"rank{model_config.mapping.rank}.safetensors",
+                    checkpoint_folder / f"rank{model_config.mapping.rank}.safetensors",
                 )
 
             # Write global config
-            model_config.save_pretrained(engines_folder)
+            model_config.save_pretrained(checkpoint_folder)
 
         # We are freeing memory used by the HF Model to let the engine build goes forward
         del hf_model
         torch.cuda.empty_cache()
 
         # Build
-        engine_builder = LocalEngineBuilder(model_config, engines_folder)
+        engine_builder = LocalEngineBuilder(
+            model_config, checkpoint_folder, engines_folder
+        )
         engine_builder.build(engine_config)
 
-        return [engines_folder], [engines_folder.relative_to(local_path)]
+        return (
+            [checkpoint_folder],
+            [engines_folder],
+            [engines_folder.relative_to(local_path)],
+        )
 
     @classmethod
     def _from_pretrained(
         cls: Type[T],
         *,
         model_id: str,
         config: Dict[str, Any],
@@ -302,14 +356,19 @@
         force_download: bool,
         proxies: Optional[Dict],
         resume_download: bool,
         local_files_only: bool,
         token: Optional[Union[str, bool]],
         **model_kwargs,
     ) -> T:
+        # Config attributes are being injected also along "config"...
+        for key in config.keys():
+            if key in model_kwargs:
+                model_kwargs.pop(key)
+
         if not isinstance(cls, SupportsTensorrtConversion):
             raise ValueError(
                 f"{cls} doesn't support converting from Hugging Face Hub model."
                 " Please open up an issue at https://github.com/huggingface/optimum-nvidia/issues"
             )
 
         # Check if we are using a local path
@@ -330,16 +389,17 @@
                 resume_download,
                 local_files_only,
                 token,
                 prebuilt_engines_only=True,
             )
 
         # Look for prebuilt engine files, if none found, we convert and build
-        engines_folders, relative_paths_engines_folders = find_prebuilt_engines(
-            local_path
+        checkpoints_folders, (engines_folders, relative_paths_engines_folders) = (
+            None,
+            find_prebuilt_engines(local_path),
         )
         if len(engines_folders) == 0:
             LOGGER.info(
                 f"No engine file found in {local_path}, converting and building engines"
             )
 
             # If local_path exists and is not empty we have a local snapshot
@@ -359,16 +419,16 @@
                     proxies,
                     resume_download,
                     local_files_only,
                     token,
                     prebuilt_engines_only=False,
                 )
 
-            engines_folders, relative_paths_engines_folders = cls.convert_and_build(
-                local_path, config, **model_kwargs
+            checkpoint_folders, engines_folders, relative_paths_engines_folders = (
+                cls.convert_and_build(local_path, config, **model_kwargs)
             )
         else:
             LOGGER.info(f"Found pre-built engines at: {engines_folders}")
 
         try:
             generation_config = GenerationConfig.from_pretrained(
                 model_id,
@@ -388,14 +448,15 @@
             engines_folders,
             gpus_per_node=model_kwargs.pop("gpus_per_node", 1),
             use_cuda_graph=model_kwargs.pop("use_cuda_graph", False),
             generation_config=generation_config,
             transformers_config=transformers_config,
         )
 
+        setattr(model, ATTR_TRTLLM_CHECKPOINT_FOLDER, checkpoints_folders)
         setattr(model, ATTR_TRTLLM_ENGINE_FOLDER, engines_folders)
         model._relative_path_engines_folders = relative_paths_engines_folders
         return model
 
     def _save_pretrained(self, save_directory: Path) -> None:
         if not hasattr(self, ATTR_TRTLLM_ENGINE_FOLDER):
             raise ValueError(
@@ -451,15 +512,17 @@
         :param config_class: An optional custom TensorRTConfig subclass to load into.
         :param additional_params:
         :return: `tensorrt_llm.modeling_utils.PretrainedConfig`
         """
         if config_class is None:
             config_class = cls.MODEL_CONFIG
 
-        trt_config = config_class.from_config(config)
+        mapping = additional_params.get("mapping", None)
+
+        trt_config = config_class.from_config(config, mapping)
         if hasattr(trt_config, "check_config"):
             trt_config.check_config()
 
         return trt_config
 
     @staticmethod
     def retrieve_snapshot_from_hub(
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/lang/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/logging.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/logging.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/auto.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/auto.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,21 @@
 
 from optimum.nvidia.errors import UnsupportedModelException
 
 from ..hub import extract_model_type
 from .gemma import GemmaForCausalLM
 from .llama import LlamaForCausalLM
 from .mistral import MistralForCausalLM
+from .mixtral import MixtralForCausalLM
 
 
 _SUPPORTED_MODEL_CLASS = {
     "llama": LlamaForCausalLM,
     "mistral": MistralForCausalLM,
+    "mixtral": MixtralForCausalLM,
     "gemma": GemmaForCausalLM,
 }
 
 
 class AutoModelForCausalLM(ModelHubMixin):
     """ """
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/base.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/base.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/gemma.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/llama.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,106 +8,113 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-
 from logging import getLogger
-from typing import Dict
+from typing import Dict, Optional
 
-import torch
+import numpy as np
+from tensorrt_llm import Mapping
 from tensorrt_llm.models import PretrainedConfig, PretrainedModel
-from tensorrt_llm.models.gemma.model import GemmaForCausalLM as TrtGemmaForCausalLM
-from tensorrt_llm.models.gemma.weight import load_from_hf_gemma
+from tensorrt_llm.models.llama.convert import load_weights_from_hf
+from tensorrt_llm.models.llama.model import LLaMAForCausalLM
 from tensorrt_llm.plugin import PluginConfig
-from transformers import GemmaForCausalLM as TransformersGemmaForCausalLM
+from transformers import LlamaForCausalLM as TransformersLlamaForCausalLM
 from transformers import PretrainedConfig as TransformersPretrainedConfig
 from transformers import PreTrainedModel as TransformersPretrainedModel
 
 from optimum.nvidia import TensorRTConfig
 from optimum.nvidia.config import dtype_to_str
 from optimum.nvidia.hub import HuggingFaceHubModel
 from optimum.nvidia.runtime import CausalLM
 
 
 LOGGER = getLogger(__name__)
 
 
-class GemmaConfig(TensorRTConfig):
+class LlamaConfig(TensorRTConfig):
     r"""
-    This is the configuration class to store the configuration of a [`LlamaGemmaConfig`]. It is used to instantiate an Gemma
+    This is the configuration class to store the configuration of a [`LlamaModel`]. It is used to instantiate an LLaMA
     model according to the specified arguments, defining the model architecture. Instantiating a configuration with the
-    defaults will yield a similar configuration to that of the Gemma-7B.
+    defaults will yield a similar configuration to that of the LLaMA-7B.
 
     Configuration objects inherit from [`TensorRTConfig`] and can be used to control the model outputs. Read the
     documentation from [`TensorRTConfig`] for more information.
     """
 
     @staticmethod
-    def from_config(config: TransformersPretrainedConfig) -> "TensorRTConfig":
+    def from_config(
+        config: TransformersPretrainedConfig, mapping: Optional[Mapping] = None
+    ) -> "TensorRTConfig":
+        mapping = mapping or Mapping()
+
         # Retrieve the quantization from the transformers config (if provided)
         _, qconfig = TensorRTConfig.get_quantization_config(config)
 
-        trt_config = GemmaConfig(
+        trt_config = LlamaConfig(
             architecture=config.architectures[0],
             dtype=dtype_to_str(config.torch_dtype),
             logits_dtype="float32",
             vocab_size=config.vocab_size,
             max_position_embeddings=config.max_position_embeddings,
             hidden_size=config.hidden_size,
             num_hidden_layers=config.num_hidden_layers,
             num_attention_heads=config.num_attention_heads,
             num_key_value_heads=getattr(
                 config, "num_key_value_heads", config.num_attention_heads
             ),
-            head_size=config.head_dim,
             hidden_act=config.hidden_act,
             intermediate_size=config.intermediate_size,
             norm_epsilon=config.rms_norm_eps,
             position_embedding_type="rope_gpt_neox",
-            world_size=1,
-            tp_size=1,
-            pp_size=1,
+            rotary_base=getattr(config, "rope_theta", 10000.0),
+            rotary_scaling=getattr(config, "rope_scaling", None),
+            world_size=mapping.world_size,
+            tp_size=mapping.tp_size,
+            pp_size=mapping.pp_size,
             use_prompt_tuning=False,
             use_parallel_embedding=False,
             embedding_sharding_dim=0,
             share_embedding_table=False,
             max_lora_rank=64,
+            head_size=config.hidden_size // config.num_attention_heads,
             quantization=qconfig,
-            rotary_base=config.rope_theta,
         )
 
         trt_config.mapping.gpus_per_node = min(trt_config.mapping.world_size, 8)
 
         return trt_config
 
     def get_plugins_config(self) -> PluginConfig:
         config = super().get_plugins_config()
-        config.moe_plugin = "disable"
+        config.moe_plugin = "disable"  # TODO : Mixtral?
         config.bert_attention_plugin = "disable"
         config.gpt_attention_plugin = self.dtype
         config.gemm_plugin = self.dtype
 
         return config
 
     @staticmethod
     def supports_strong_typing() -> bool:
         return False
 
 
-class GemmaForCausalLM(CausalLM, HuggingFaceHubModel):
-    MODEL_CONFIG = GemmaConfig
-    HF_LIBRARY_TARGET_MODEL_CLASS = TransformersGemmaForCausalLM
-    TRT_LLM_TARGET_MODEL_CLASS = TrtGemmaForCausalLM
+class LlamaForCausalLM(CausalLM, HuggingFaceHubModel):
+    MODEL_CONFIG = LlamaConfig
+    HF_LIBRARY_TARGET_MODEL_CLASS = TransformersLlamaForCausalLM
+    TRT_LLM_TARGET_MODEL_CLASS = LLaMAForCausalLM
 
     @staticmethod
     def convert_weights(
         target: PretrainedModel,
         source: TransformersPretrainedModel,
         config: PretrainedConfig,
-    ) -> Dict[str, torch.Tensor]:
+    ) -> Dict[str, np.ndarray]:
         if config.quant_mode.has_any_quant():
             raise NotImplementedError("Quantization is not supported yet.")
 
-        return load_from_hf_gemma(target, source, config.mapping, config.dtype)
+        return load_weights_from_hf(
+            config=config.to_dict(), mapping=config.mapping, model=source
+        )
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/llama.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/gemma.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,104 +8,112 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+
 from logging import getLogger
-from typing import Dict
+from typing import Dict, Optional
 
-import numpy as np
+import torch
+from tensorrt_llm import Mapping
 from tensorrt_llm.models import PretrainedConfig, PretrainedModel
-from tensorrt_llm.models.llama.model import LLaMAForCausalLM
-from tensorrt_llm.models.llama.weight import load_from_hf_llama
+from tensorrt_llm.models.gemma.model import GemmaForCausalLM as TrtGemmaForCausalLM
+from tensorrt_llm.models.gemma.weight import load_from_hf_gemma
 from tensorrt_llm.plugin import PluginConfig
-from transformers import LlamaForCausalLM as TransformersLlamaForCausalLM
+from transformers import GemmaForCausalLM as TransformersGemmaForCausalLM
 from transformers import PretrainedConfig as TransformersPretrainedConfig
 from transformers import PreTrainedModel as TransformersPretrainedModel
 
 from optimum.nvidia import TensorRTConfig
 from optimum.nvidia.config import dtype_to_str
 from optimum.nvidia.hub import HuggingFaceHubModel
 from optimum.nvidia.runtime import CausalLM
 
 
 LOGGER = getLogger(__name__)
 
 
-class LlamaConfig(TensorRTConfig):
+class GemmaConfig(TensorRTConfig):
     r"""
-    This is the configuration class to store the configuration of a [`LlamaModel`]. It is used to instantiate an LLaMA
+    This is the configuration class to store the configuration of a [`LlamaGemmaConfig`]. It is used to instantiate an Gemma
     model according to the specified arguments, defining the model architecture. Instantiating a configuration with the
-    defaults will yield a similar configuration to that of the LLaMA-7B.
+    defaults will yield a similar configuration to that of the Gemma-7B.
 
     Configuration objects inherit from [`TensorRTConfig`] and can be used to control the model outputs. Read the
     documentation from [`TensorRTConfig`] for more information.
     """
 
     @staticmethod
-    def from_config(config: TransformersPretrainedConfig) -> "TensorRTConfig":
+    def from_config(
+        config: TransformersPretrainedConfig, mapping: Optional[Mapping] = None
+    ) -> "TensorRTConfig":
+        mapping = mapping or Mapping()
+
         # Retrieve the quantization from the transformers config (if provided)
         _, qconfig = TensorRTConfig.get_quantization_config(config)
 
-        trt_config = LlamaConfig(
+        trt_config = GemmaConfig(
             architecture=config.architectures[0],
             dtype=dtype_to_str(config.torch_dtype),
             logits_dtype="float32",
             vocab_size=config.vocab_size,
             max_position_embeddings=config.max_position_embeddings,
             hidden_size=config.hidden_size,
             num_hidden_layers=config.num_hidden_layers,
             num_attention_heads=config.num_attention_heads,
             num_key_value_heads=getattr(
                 config, "num_key_value_heads", config.num_attention_heads
             ),
+            head_size=config.head_dim,
             hidden_act=config.hidden_act,
             intermediate_size=config.intermediate_size,
             norm_epsilon=config.rms_norm_eps,
             position_embedding_type="rope_gpt_neox",
-            world_size=1,
-            tp_size=1,
-            pp_size=1,
+            rotary_base=getattr(config, "rope_theta", 10000.0),
+            rotary_scaling=getattr(config, "rope_scaling", None),
+            world_size=mapping.world_size,
+            tp_size=mapping.tp_size,
+            pp_size=mapping.pp_size,
             use_prompt_tuning=False,
-            use_parallel_embedding=False,
+            use_parallel_embedding=mapping.tp_size > 1,
             embedding_sharding_dim=0,
             share_embedding_table=False,
             max_lora_rank=64,
-            head_size=config.hidden_size / config.num_attention_heads,
             quantization=qconfig,
         )
 
         trt_config.mapping.gpus_per_node = min(trt_config.mapping.world_size, 8)
 
         return trt_config
 
     def get_plugins_config(self) -> PluginConfig:
         config = super().get_plugins_config()
-        config.moe_plugin = "disable"  # TODO : Mixtral?
+        config.moe_plugin = "disable"
         config.bert_attention_plugin = "disable"
         config.gpt_attention_plugin = self.dtype
         config.gemm_plugin = self.dtype
 
         return config
 
     @staticmethod
     def supports_strong_typing() -> bool:
         return False
 
 
-class LlamaForCausalLM(CausalLM, HuggingFaceHubModel):
-    MODEL_CONFIG = LlamaConfig
-    HF_LIBRARY_TARGET_MODEL_CLASS = TransformersLlamaForCausalLM
-    TRT_LLM_TARGET_MODEL_CLASS = LLaMAForCausalLM
+class GemmaForCausalLM(CausalLM, HuggingFaceHubModel):
+    MODEL_CONFIG = GemmaConfig
+    HF_LIBRARY_TARGET_MODEL_CLASS = TransformersGemmaForCausalLM
+    TRT_LLM_TARGET_MODEL_CLASS = TrtGemmaForCausalLM
 
     @staticmethod
     def convert_weights(
         target: PretrainedModel,
         source: TransformersPretrainedModel,
         config: PretrainedConfig,
-    ) -> Dict[str, np.ndarray]:
+    ) -> Dict[str, torch.Tensor]:
         if config.quant_mode.has_any_quant():
             raise NotImplementedError("Quantization is not supported yet.")
 
-        return load_from_hf_llama(target, source, config.mapping, config.dtype)
+        return load_from_hf_gemma(target, source, config.mapping, config.dtype)
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/mistral.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/mistral.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from logging import getLogger
-from typing import Dict
+from typing import Dict, Optional
 
 import numpy as np
+from tensorrt_llm import Mapping
 from tensorrt_llm.models import PretrainedConfig, PretrainedModel
 from tensorrt_llm.models.llama.model import LLaMAForCausalLM
 from tensorrt_llm.models.llama.weight import load_from_hf_llama
 from tensorrt_llm.plugin import PluginConfig
 from transformers import MistralForCausalLM as TransformersMistralForCausalLM
 from transformers import PretrainedConfig as TransformersPretrainedConfig
 from transformers import PreTrainedModel as TransformersPretrainedModel
@@ -40,15 +41,19 @@
     defaults will yield a similar configuration to that of the LLaMA-7B.
 
     Configuration objects inherit from [`TensorRTConfig`] and can be used to control the model outputs. Read the
     documentation from [`TensorRTConfig`] for more information.
     """
 
     @staticmethod
-    def from_config(config: TransformersPretrainedConfig) -> "TensorRTConfig":
+    def from_config(
+        config: TransformersPretrainedConfig, mapping: Optional[Mapping]
+    ) -> "TensorRTConfig":
+        mapping = mapping or Mapping()
+
         # Retrieve the quantization from the transformers config (if provided)
         _, qconfig = TensorRTConfig.get_quantization_config(config)
 
         trt_config = MistralConfig(
             architecture=config.architectures[0],
             dtype=dtype_to_str(config.torch_dtype),
             logits_dtype="float32",
@@ -60,25 +65,26 @@
             num_key_value_heads=getattr(
                 config, "num_key_value_heads", config.num_attention_heads
             ),
             hidden_act=config.hidden_act,
             intermediate_size=config.intermediate_size,
             norm_epsilon=config.rms_norm_eps,
             position_embedding_type="rope_gpt_neox",
-            world_size=1,
-            tp_size=1,
-            pp_size=1,
+            rotary_base=getattr(config, "rope_theta", 10000.0),
+            rotary_scaling=getattr(config, "rope_scaling", None),
+            world_size=mapping.world_size,
+            tp_size=mapping.tp_size,
+            pp_size=mapping.pp_size,
             use_prompt_tuning=False,
-            use_parallel_embedding=False,
+            use_parallel_embedding=mapping.tp_size > 1,
             embedding_sharding_dim=0,
             share_embedding_table=False,
             max_lora_rank=64,
-            head_size=config.hidden_size / config.num_attention_heads,
+            head_size=config.hidden_size // config.num_attention_heads,
             quantization=qconfig,
-            rotary_base=config.rope_theta,
         )
 
         trt_config.mapping.gpus_per_node = min(trt_config.mapping.world_size, 8)
 
         return trt_config
 
     def get_plugins_config(self) -> PluginConfig:
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/models/whisper.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/models/whisper.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,15 +378,19 @@
             )
 
     return weights
 
 
 class WhisperEncoderConfig(TensorRTConfig):
     @classmethod
-    def from_config(cls, config: "TransformersPretrainedConfig") -> "TensorRTConfig":
+    def from_config(
+        cls, config: "TransformersPretrainedConfig", mapping: Optional[Mapping] = None
+    ) -> "TensorRTConfig":
+        mapping = mapping or Mapping()
+
         # Retrieve the quantization from the transformers config (if provided)
         _, qconfig = TensorRTConfig.get_quantization_config(config)
 
         trt_config = cls(
             architecture=config.architectures[0],
             dtype=dtype_to_str(config.torch_dtype),  # TODO: always float32?
             logits_dtype="float32",
@@ -396,20 +400,20 @@
             num_hidden_layers=config.encoder_layers,
             num_attention_heads=config.encoder_attention_heads,
             num_key_value_heads=config.encoder_attention_heads,
             hidden_act=config.activation_function,
             intermediate_size=None,
             norm_epsilon=None,
             position_embedding_type="learned_absolute",
-            world_size=1,
-            tp_size=1,
-            pp_size=1,
+            world_size=mapping.world_size,
+            tp_size=mapping.tp_size,
+            pp_size=mapping.pp_size,
             quantization=qconfig,
-            use_parallel_embedding=None,
-            embedding_sharding_dim=None,
+            use_parallel_embedding=mapping.tp_size > 1,
+            embedding_sharding_dim=0 if mapping.tp_size > 1 else None,
             share_embedding_table=None,
             head_size=-1,  # We need to set it otherwise TRT-LLM tries to compute `hidden_size // num_attention_heads`
             max_source_positions=config.max_source_positions,
             num_mel_bins=config.num_mel_bins,
             trt_model_class="TrtWhisperEncoderPretrainedModel",
             trt_model_file=pathlib.Path(__file__),
         )
@@ -441,15 +445,19 @@
     @staticmethod
     def supports_strong_typing() -> bool:
         return False
 
 
 class WhisperDecoderConfig(TensorRTConfig):
     @classmethod
-    def from_config(cls, config: "TransformersPretrainedConfig") -> "TensorRTConfig":
+    def from_config(
+        cls, config: "TransformersPretrainedConfig", mapping: Optional[Mapping]
+    ) -> "TensorRTConfig":
+        mapping = mapping or Mapping()
+
         # Retrieve the quantization from the transformers config (if provided)
         _, qconfig = TensorRTConfig.get_quantization_config(config)
 
         trt_config = cls(
             architecture=config.architectures[0],
             dtype=dtype_to_str(config.torch_dtype),  # TODO: always float32?
             logits_dtype="float32",
@@ -459,17 +467,17 @@
             num_hidden_layers=config.decoder_layers,
             num_attention_heads=config.decoder_attention_heads,
             num_key_value_heads=config.decoder_attention_heads,
             hidden_act=config.activation_function,
             intermediate_size=None,
             norm_epsilon=None,
             position_embedding_type="learned_absolute",
-            world_size=1,
-            tp_size=1,
-            pp_size=1,
+            world_size=mapping.world_size,
+            tp_size=mapping.tp_size,
+            pp_size=mapping.pp_size,
             quantization=qconfig,
             use_parallel_embedding=None,
             embedding_sharding_dim=None,
             share_embedding_table=None,
             head_size=-1,  # We need to set it otherwise TRT-LLM tries to compute `hidden_size // num_attention_heads`
             max_source_positions=config.max_source_positions,
             decoder_ffn_dim=config.decoder_ffn_dim,
@@ -578,14 +586,15 @@
         max_num_tokens: int = None,
         prompt_embedding_table_size: int = 0,
         position_encoding_2d: bool = False,
         max_draft_len: int = 0,
         gather_context_logits: bool = False,
         gather_generation_logits: bool = False,
         lora_target_modules: List[str] = None,
+        **kwargs,
     ):
         if not use_cache:
             raise NotImplementedError("use_cache=False is not implemented for Whisper.")
 
         (
             input_ids,
             encoder_output,
@@ -763,42 +772,48 @@
             )
 
         if engine_save_path is None:
             engine_save_path = local_path
 
         LOGGER.info("Building Whisper encoder...")
         (
+            encoder_checkpoints_folder,
             encoder_engines_folder,
             encoder_engines_relative_folder,
         ) = OptimumWhisperEncoder.convert_and_build(
             local_path,
             hf_model_config,
             engine_save_path=Path(engine_save_path, "encoder"),
             hf_model=hf_model.model.encoder,
             config_class=WhisperEncoderConfig,
             **model_kwargs,
         )
 
         LOGGER.info("Building Whisper decoder...")
         (
+            decoder_checkpoints_folder,
             decoder_engines_folder,
             decoder_engines_relative_folder,
         ) = OptimumWhisperDecoder.convert_and_build(
             local_path,
             hf_model_config,
             engine_save_path=Path(engine_save_path, "decoder"),
             hf_model=hf_model.model.decoder,
             config_class=WhisperDecoderConfig,
             **model_kwargs,
         )
 
-        return [encoder_engines_folder[0], decoder_engines_folder[0]], [
-            encoder_engines_relative_folder[0],
-            decoder_engines_relative_folder[0],
-        ]
+        return (
+            [encoder_checkpoints_folder[0], decoder_checkpoints_folder[0]],
+            [encoder_engines_folder[0], decoder_engines_folder[0]],
+            [
+                encoder_engines_relative_folder[0],
+                decoder_engines_relative_folder[0],
+            ],
+        )
 
     def encoder(
         self,
         input_features: torch.Tensor,
     ):
         if dtype_to_str(input_features.dtype) != self.dtype:
             LOGGER.warning(
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/pipelines/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from .base import Pipeline
 
 
 SUPPORTED_MODEL_WITH_TASKS: Dict[str, Dict[str, Tuple[Type[Pipeline], Type]]] = {
     "gemma": {"text-generation": (TextGenerationPipeline, AutoModelForCausalLM)},
     "llama": {"text-generation": (TextGenerationPipeline, AutoModelForCausalLM)},
     "mistral": {"text-generation": (TextGenerationPipeline, AutoModelForCausalLM)},
+    "mixtral": {"text-generation": (TextGenerationPipeline, AutoModelForCausalLM)},
 }
 
 
 def get_target_class_for_model_and_task(task: str, architecture: str) -> Optional[Type]:
     task_ = SUPPORTED_MODEL_WITH_TASKS.get(task, None)
     if not task:
         raise NotImplementedError(f"Task {task} is not supported yet.")
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/base.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/pipelines/text_generation.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/pipelines/text_generation.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/config.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/ammo/config.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/ammo/quantizer.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/ammo/quantizer.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/quantization/datasets.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/quantization/datasets.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/runtime.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,27 +236,27 @@
 
         if generation_config.min_new_tokens is not None:
             sampling_config.min_length = [generation_config.min_new_tokens]
 
         input_ids, _, model_kwargs = self._prepare_model_inputs(
             inputs, generation_config.bos_token_id, model_kwargs
         )
+        input_length = input_ids.shape[1]
 
         with torch.no_grad():
             if not isinstance(input_ids, torch.Tensor):
                 raise TypeError("input_ids should be a PyTorch tensor (torch.Tensor)")
 
             attention_mask = model_kwargs["attention_mask"]
             input_ids, lengths = self._prepare_inputs(input_ids, attention_mask)
             if torch.any(torch.gt(lengths, self.max_prompt_length)):
                 raise ValueError(
                     f"Input length {lengths} is bigger than maximum prompt length ({self.max_prompt_length})."
                 )
 
-            input_length = input_ids.shape[1]
             trt_inputs = ctrrt.GenerationInput(
                 end_id=generation_config.eos_token_id,
                 pad_id=generation_config.pad_token_id,
                 ids=input_ids.to(device),
                 lengths=lengths.to(device),
                 packed=self._use_packed_inputs,
             )
@@ -271,18 +271,18 @@
             trt_outputs = ctrrt.GenerationOutput(
                 ids=torch.empty(0, device=device, dtype=torch.int32),
                 lengths=torch.empty(0, device=device, dtype=torch.int32),
             )
 
             self._session.generate(trt_outputs, trt_inputs, sampling_config)
 
-            total_length = trt_outputs.lengths
+            total_length = trt_outputs.lengths.max().item()
             output_ids = trt_outputs.ids.flatten(0, 1)
 
-            # For some reason not in line with Transformers in case we finish early with BOS token (missing last BOS token).
+            # For some reason not in line with Transformers in case we finish early with EOS token (missing last EOS token).
             if total_length - input_length < max_new_tokens:
                 total_length += 1
 
             return output_ids[:, :total_length], total_length
 
     def _prepare_inputs(
         self, input_ids: torch.Tensor, attention_mask: Optional[torch.Tensor] = None
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/cli.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 
 # Model topology (sharding, pipelining, dtype)
 def register_common_model_topology_args(parser: ArgumentParser) -> ArgumentParser:
     parser.add_argument(
         "--tensor-parallelism",
         type=int,
         default=1,
+        dest="tp",
         help="Define the number of slice for each tensor each GPU will receive.",
     )
     parser.add_argument(
         "--pipeline-parallelism",
         type=int,
         default=1,
+        dest="pp",
         help="Define the number of sections to split neural network layers",
     )
     parser.add_argument(
         "--world-size",
         type=int,
         default=1,
         help="Total number of GPUs over all the nodes.",
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/constants.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/env.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/env.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/hub.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/hub.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/nvml.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/nvml.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/offload.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/offload.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/onnx.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/patching.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/patching.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/__init__.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/tests/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,8 +9,12 @@
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from .utils import nightly, requires_gpu, slow
+from .assertions import (
+    assert_generated_partially_match,
+    assert_generated_text_partially_match,
+)
+from .utils import nightly, requires_float8, requires_gpu, requires_multi_gpu, slow
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/utils/tests/utils.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/utils/tests/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 
 requires_gpu = pytest.mark.skipif(
     parse_flag_from_env(ENVVAR_NAME_RUN_CPU_ONLY, False) or not get_device_count(),
     reason=f"RUN_CPU_ONLY={parse_flag_from_env(ENVVAR_NAME_RUN_CPU_ONLY, False)} or "
     f"no GPU detected (num_gpus={get_device_count()})",
 )
 
+requires_multi_gpu = pytest.mark.skipif(
+    get_device_count() < 2, reason="At least two GPUs are required"
+)
+
 
 def requires_gpu_compute_capabilities_ge(min_capabilities: int, device: int = 0):
     (major, minor) = get_device_compute_capabilities(device)
     compute_capabilities = major * 10 + minor
     return pytest.mark.skipif(
         compute_capabilities < min_capabilities,
         reason=f"Require compute capabilities >= sm_{min_capabilities} but current GPU is sm_{compute_capabilities}",
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum/nvidia/version.py` & `optimum_nvidia-0.1.0b7/src/optimum/nvidia/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from distutils.version import StrictVersion
 
 
-__version__ = "0.1.0b6"
+__version__ = "0.1.0b7"
 VERSION = StrictVersion(__version__)
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/PKG-INFO` & `optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-nvidia
-Version: 0.1.0b6
+Version: 0.1.0b7
 Summary: Optimum Nvidia is the interface between the Hugging Face Transformers and NVIDIA GPUs. "
 Home-page: https://huggingface.co/hardware/nvidia
 Author: HuggingFace Inc. Machine Learning Optimization Team
 Author-email: "HuggingFace Inc. Machine Learning Optimization Team" <hardware@huggingface.co>
 License: Apache/2.0
 Project-URL: Homepage, https://huggingface.co/hardware/nvidia
 Project-URL: Repository, https://github.com/huggingface/optimum-nvidia
@@ -22,19 +22,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate==0.25
 Requires-Dist: datasets>=2.14.0
 Requires-Dist: huggingface-hub>=0.22.0
 Requires-Dist: hf-transfer
 Requires-Dist: mpmath==1.3.0
-Requires-Dist: numpy>=1.26.0
+Requires-Dist: numpy<2.0.0,>=1.26.0
 Requires-Dist: onnx>=1.12.0
 Requires-Dist: optimum>=1.13.0
 Requires-Dist: setuptools
-Requires-Dist: tensorrt-llm==0.9.0.dev2024031900
+Requires-Dist: tensorrt-llm==0.9.0
 Requires-Dist: torch<=2.3.0a,>=2.2.0a
 Requires-Dist: transformers>=4.38.2
 Requires-Dist: pynvml
 Provides-Extra: tests
 Requires-Dist: mock; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
@@ -139,15 +139,18 @@
 + from optimum.nvidia import AutoModelForCausalLM
 from transformers import AutoTokenizer
 
 tokenizer = AutoTokenizer.from_pretrained("meta-llama/Llama-2-7b-chat-hf", padding_side="left")
 
 model = AutoModelForCausalLM.from_pretrained(
   "meta-llama/Llama-2-7b-chat-hf",
-+ use_fp8=True,  
++ use_fp8=True,
++ max_prompt_length=1024,
++ max_output_length=2048, # Must be at least size of max_prompt_length + max_new_tokens
++ max_batch_size=8,
 )
 
 model_inputs = tokenizer(["How is autonomous vehicle technology transforming the future of transportation and urban planning?"], return_tensors="pt").to("cuda")
 
 generated_ids = model.generate(
     **model_inputs, 
     top_k=40, 
@@ -160,15 +163,14 @@
 
 To learn more about text generation with LLMs, check out [this guide](https://huggingface.co/docs/transformers/llm_tutorial)!
 
 <!-- For more details, read our [documentation](https://huggingface.com/docs/optimum/nvidia/index). -->
 
 # Support Matrix
 We test Optimum-NVIDIA on 4090, L40S, and H100 Tensor Core GPUs, though it is expected to work on any GPU based on the following architectures: 
-* Turing (with experimental support for T4 / RTX Quadro x000)
 * Ampere (A100/A30 are supported. Experimental support for A10, A40, RTX Ax000)
 * Hopper
 * Ada-Lovelace
 
 Note that FP8 support is only available on GPUs based on Hopper and Ada-Lovelace architectures.
 
 Optimum-NVIDIA works on Linux will support Windows soon.
```

### Comparing `optimum-nvidia-0.1.0b6/src/optimum_nvidia.egg-info/SOURCES.txt` & `optimum_nvidia-0.1.0b7/src/optimum_nvidia.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/optimum/nvidia/lang/__init__.py
 src/optimum/nvidia/models/__init__.py
 src/optimum/nvidia/models/auto.py
 src/optimum/nvidia/models/base.py
 src/optimum/nvidia/models/gemma.py
 src/optimum/nvidia/models/llama.py
 src/optimum/nvidia/models/mistral.py
+src/optimum/nvidia/models/mixtral.py
 src/optimum/nvidia/models/whisper.py
 src/optimum/nvidia/pipelines/__init__.py
 src/optimum/nvidia/pipelines/base.py
 src/optimum/nvidia/pipelines/text_generation.py
 src/optimum/nvidia/quantization/__init__.py
 src/optimum/nvidia/quantization/datasets.py
 src/optimum/nvidia/quantization/ammo/__init__.py
@@ -37,14 +38,15 @@
 src/optimum/nvidia/utils/env.py
 src/optimum/nvidia/utils/hub.py
 src/optimum/nvidia/utils/nvml.py
 src/optimum/nvidia/utils/offload.py
 src/optimum/nvidia/utils/onnx.py
 src/optimum/nvidia/utils/patching.py
 src/optimum/nvidia/utils/tests/__init__.py
+src/optimum/nvidia/utils/tests/assertions.py
 src/optimum/nvidia/utils/tests/utils.py
 src/optimum_nvidia.egg-info/PKG-INFO
 src/optimum_nvidia.egg-info/SOURCES.txt
 src/optimum_nvidia.egg-info/dependency_links.txt
 src/optimum_nvidia.egg-info/not-zip-safe
 src/optimum_nvidia.egg-info/requires.txt
 src/optimum_nvidia.egg-info/top_level.txt
```

### Comparing `optimum-nvidia-0.1.0b6/tests/test_config.py` & `optimum_nvidia-0.1.0b7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/tests/test_dtype.py` & `optimum_nvidia-0.1.0b7/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `optimum-nvidia-0.1.0b6/tests/test_hub.py` & `optimum_nvidia-0.1.0b7/tests/test_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
             model = HfAutoModelForCausalLM.from_config(config)
             model.save_pretrained(hf_out)
 
             model = AutoModelForCausalLM.from_pretrained(hf_out)
             model.save_pretrained(trtllm_out)
 
             assert trtllm_out.exists()
-            assert (trtllm_out / FOLDER_TRTLLM_ENGINES).exists()
             assert (trtllm_out / FOLDER_TRTLLM_ENGINES / "rank0.engine").exists()
 
         def _reload():
             with mock.patch("optimum.nvidia.hub.HuggingFaceHubModel.convert_and_build"):
                 model = AutoModelForCausalLM.from_pretrained(trtllm_out)
                 assert model is not None
                 assert (
```

### Comparing `optimum-nvidia-0.1.0b6/tests/test_quantization.py` & `optimum_nvidia-0.1.0b7/tests/test_quantization.py`

 * *Files identical despite different names*

