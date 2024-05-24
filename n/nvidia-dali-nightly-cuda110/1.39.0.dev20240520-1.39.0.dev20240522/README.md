# Comparing `tmp/nvidia_dali_nightly_cuda110-1.39.0.dev20240520.tar.gz` & `tmp/nvidia_dali_nightly_cuda110-1.39.0.dev20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_nightly_cuda110-1.39.0.dev20240520.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_nightly_cuda110-1.39.0.dev20240522.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_nightly_cuda110-1.39.0.dev20240520.tar` & `nvidia_dali_nightly_cuda110-1.39.0.dev20240522.tar`

### PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.39.0.dev20240520
-Summary: NVIDIA DALI nightly  for CUDA 11.0. Git SHA: 306221661a585ed7791857141e15b69e28952905
+Version: 1.39.0.dev20240522
+Summary: NVIDIA DALI nightly  for CUDA 11.0. Git SHA: 708af6048e71e55eb117718a53c8bf7649eecb38
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

