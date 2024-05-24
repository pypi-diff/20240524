# Comparing `tmp/libem-0.0.7.tar.gz` & `tmp/libem-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libem-0.0.7.tar", last modified: Wed May 15 18:52:16 2024, max compression
+gzip compressed data, was "libem-0.0.8.tar", last modified: Fri May 24 00:41:39 2024, max compression
```

## Comparing `libem-0.0.7.tar` & `libem-0.0.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.060260 libem-0.0.7/
--rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.7/LICENSE
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-15 18:52:16.060141 libem-0.0.7/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)     1343 2024-05-09 21:01:57.000000 libem-0.0.7/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.047972 libem-0.0.7/cli/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.7/cli/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1366 2024-05-14 01:22:05.000000 libem-0.0.7/cli/libem
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.049429 libem-0.0.7/libem/
--rw-r--r--   0 silv       (501) staff       (20)      382 2024-05-14 16:05:14.000000 libem-0.0.7/libem/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.050907 libem-0.0.7/libem/browse/
--rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.7/libem/browse/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     3406 2024-05-14 16:05:14.000000 libem-0.0.7/libem/browse/function.py
--rw-r--r--   0 silv       (501) staff       (20)       99 2024-05-15 18:04:36.000000 libem-0.0.7/libem/browse/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      318 2024-05-09 21:57:54.000000 libem-0.0.7/libem/browse/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.051568 libem-0.0.7/libem/calibrate/
--rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-09 20:29:02.000000 libem-0.0.7/libem/calibrate/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     4420 2024-05-09 22:17:00.000000 libem-0.0.7/libem/calibrate/function.py
--rw-r--r--   0 silv       (501) staff       (20)      436 2024-05-09 22:15:40.000000 libem-0.0.7/libem/calibrate/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.051859 libem-0.0.7/libem/calibrate/optimize/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-12 21:34:51.000000 libem-0.0.7/libem/calibrate/optimize/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      851 2024-05-14 16:08:26.000000 libem-0.0.7/libem/constant.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.053773 libem-0.0.7/libem/core/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.7/libem/core/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     3823 2024-05-08 06:37:24.000000 libem-0.0.7/libem/core/eval.py
--rw-r--r--   0 silv       (501) staff       (20)      159 2024-05-14 16:05:14.000000 libem-0.0.7/libem/core/exception.py
--rw-r--r--   0 silv       (501) staff       (20)     3779 2024-05-14 16:05:14.000000 libem-0.0.7/libem/core/log.py
--rw-r--r--   0 silv       (501) staff       (20)     4455 2024-05-14 16:16:25.000000 libem-0.0.7/libem/core/model.py
--rw-r--r--   0 silv       (501) staff       (20)     5185 2024-05-15 18:04:10.000000 libem-0.0.7/libem/core/struct.py
--rw-r--r--   0 silv       (501) staff       (20)      911 2024-05-15 18:14:15.000000 libem-0.0.7/libem/core/telemetry.py
--rw-r--r--   0 silv       (501) staff       (20)     1098 2024-05-08 21:50:28.000000 libem-0.0.7/libem/core/trace.py
--rw-r--r--   0 silv       (501) staff       (20)     1020 2024-05-09 21:08:05.000000 libem-0.0.7/libem/core/util.py
--rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.7/libem/function.py
--rw-r--r--   0 silv       (501) staff       (20)      973 2024-05-14 16:15:38.000000 libem-0.0.7/libem/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.054655 libem-0.0.7/libem/match/
--rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.7/libem/match/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1666 2024-05-15 18:17:15.000000 libem-0.0.7/libem/match/function.py
--rw-r--r--   0 silv       (501) staff       (20)      211 2024-05-15 18:00:54.000000 libem-0.0.7/libem/match/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      668 2024-05-15 17:54:20.000000 libem-0.0.7/libem/match/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-14 16:07:48.000000 libem-0.0.7/libem/parameter.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.055322 libem-0.0.7/libem/prepare/
--rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.7/libem/prepare/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.056686 libem-0.0.7/libem/prepare/datasets/
--rw-r--r--   0 silv       (501) staff       (20)      134 2024-05-09 00:08:47.000000 libem-0.0.7/libem/prepare/datasets/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     2954 2024-05-09 00:05:08.000000 libem-0.0.7/libem/prepare/datasets/abt_buy.py
--rw-r--r--   0 silv       (501) staff       (20)     2698 2024-05-09 00:06:05.000000 libem-0.0.7/libem/prepare/datasets/amazon_google.py
--rw-r--r--   0 silv       (501) staff       (20)     2764 2024-05-14 16:05:14.000000 libem-0.0.7/libem/prepare/datasets/dblp_acm.py
--rw-r--r--   0 silv       (501) staff       (20)     2760 2024-05-09 00:08:21.000000 libem-0.0.7/libem/prepare/datasets/dblp_scholar.py
--rw-r--r--   0 silv       (501) staff       (20)     2792 2024-05-09 00:08:37.000000 libem-0.0.7/libem/prepare/datasets/walmart_amazon.py
--rw-r--r--   0 silv       (501) staff       (20)       72 2024-05-08 23:56:27.000000 libem-0.0.7/libem/prepare/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.7/libem/prepare/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.7/libem/prepare/prompt.py
--rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.7/libem/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.057504 libem-0.0.7/libem/tune/
--rw-r--r--   0 silv       (501) staff       (20)      129 2024-05-08 00:48:47.000000 libem-0.0.7/libem/tune/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       31 2024-05-14 16:19:43.000000 libem-0.0.7/libem/tune/catalog.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.7/libem/tune/function.py
--rw-r--r--   0 silv       (501) staff       (20)      224 2024-05-09 21:34:22.000000 libem-0.0.7/libem/tune/interface.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.058463 libem-0.0.7/libem/tune/learn/
--rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-07 23:38:41.000000 libem-0.0.7/libem/tune/learn/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     3022 2024-05-14 16:12:58.000000 libem-0.0.7/libem/tune/learn/function.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-08 23:52:04.000000 libem-0.0.7/libem/tune/learn/interface.py
--rw-r--r--   0 silv       (501) staff       (20)      131 2024-05-15 17:57:55.000000 libem-0.0.7/libem/tune/learn/parameter.py
--rw-r--r--   0 silv       (501) staff       (20)      730 2024-05-09 23:34:00.000000 libem-0.0.7/libem/tune/learn/prompt.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.058857 libem-0.0.7/libem/tune/load/
--rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.7/libem/tune/load/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.7/libem/tune/load/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.059236 libem-0.0.7/libem/tune/save/
--rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.7/libem/tune/save/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.7/libem/tune/save/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.059652 libem-0.0.7/libem/tune/search/
--rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.7/libem/tune/search/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.7/libem/tune/search/function.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.050106 libem-0.0.7/libem.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)     1575 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)      137 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-15 18:52:16.000000 libem-0.0.7/libem.egg-info/top_level.txt
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-15 18:52:16.059903 libem-0.0.7/serve/
--rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.7/serve/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.7/serve/run.py
--rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-15 18:52:16.060291 libem-0.0.7/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      449 2024-05-15 18:52:02.000000 libem-0.0.7/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.953794 libem-0.0.8/
+-rw-r--r--   0 silv       (501) staff       (20)    11357 2024-05-01 02:16:29.000000 libem-0.0.8/LICENSE
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-24 00:41:39.953636 libem-0.0.8/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1343 2024-05-09 21:01:57.000000 libem-0.0.8/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.938987 libem-0.0.8/cli/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-05 16:25:37.000000 libem-0.0.8/cli/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1366 2024-05-14 01:22:05.000000 libem-0.0.8/cli/libem
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.940860 libem-0.0.8/libem/
+-rw-r--r--   0 silv       (501) staff       (20)      382 2024-05-14 16:05:14.000000 libem-0.0.8/libem/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.942602 libem-0.0.8/libem/browse/
+-rw-r--r--   0 silv       (501) staff       (20)       92 2024-05-05 00:16:54.000000 libem-0.0.8/libem/browse/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3406 2024-05-14 16:05:14.000000 libem-0.0.8/libem/browse/function.py
+-rw-r--r--   0 silv       (501) staff       (20)       99 2024-05-15 18:04:36.000000 libem-0.0.8/libem/browse/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      318 2024-05-09 21:57:54.000000 libem-0.0.8/libem/browse/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.943334 libem-0.0.8/libem/calibrate/
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-09 20:29:02.000000 libem-0.0.8/libem/calibrate/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     4420 2024-05-16 16:16:14.000000 libem-0.0.8/libem/calibrate/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      436 2024-05-09 22:15:40.000000 libem-0.0.8/libem/calibrate/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.943885 libem-0.0.8/libem/calibrate/optimize/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-12 21:34:51.000000 libem-0.0.8/libem/calibrate/optimize/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      851 2024-05-14 16:08:26.000000 libem-0.0.8/libem/constant.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.946414 libem-0.0.8/libem/core/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:45:38.000000 libem-0.0.8/libem/core/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3823 2024-05-08 06:37:24.000000 libem-0.0.8/libem/core/eval.py
+-rw-r--r--   0 silv       (501) staff       (20)      159 2024-05-14 16:05:14.000000 libem-0.0.8/libem/core/exception.py
+-rw-r--r--   0 silv       (501) staff       (20)     3779 2024-05-14 16:05:14.000000 libem-0.0.8/libem/core/log.py
+-rw-r--r--   0 silv       (501) staff       (20)     4986 2024-05-17 06:11:45.000000 libem-0.0.8/libem/core/model.py
+-rw-r--r--   0 silv       (501) staff       (20)     4870 2024-05-16 16:26:57.000000 libem-0.0.8/libem/core/struct.py
+-rw-r--r--   0 silv       (501) staff       (20)      911 2024-05-15 18:14:15.000000 libem-0.0.8/libem/core/telemetry.py
+-rw-r--r--   0 silv       (501) staff       (20)     2128 2024-05-17 06:17:04.000000 libem-0.0.8/libem/core/trace.py
+-rw-r--r--   0 silv       (501) staff       (20)     1020 2024-05-09 21:08:05.000000 libem-0.0.8/libem/core/util.py
+-rw-r--r--   0 silv       (501) staff       (20)       35 2024-05-07 06:37:47.000000 libem-0.0.8/libem/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      973 2024-05-14 16:15:38.000000 libem-0.0.8/libem/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.947341 libem-0.0.8/libem/match/
+-rw-r--r--   0 silv       (501) staff       (20)       90 2024-05-05 00:16:44.000000 libem-0.0.8/libem/match/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1666 2024-05-17 04:39:34.000000 libem-0.0.8/libem/match/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      211 2024-05-15 18:00:54.000000 libem-0.0.8/libem/match/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      684 2024-05-17 05:51:52.000000 libem-0.0.8/libem/match/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-14 16:07:48.000000 libem-0.0.8/libem/parameter.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.948078 libem-0.0.8/libem/prepare/
+-rw-r--r--   0 silv       (501) staff       (20)       94 2024-05-05 04:43:06.000000 libem-0.0.8/libem/prepare/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.949732 libem-0.0.8/libem/prepare/datasets/
+-rw-r--r--   0 silv       (501) staff       (20)      134 2024-05-09 00:08:47.000000 libem-0.0.8/libem/prepare/datasets/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     2954 2024-05-09 00:05:08.000000 libem-0.0.8/libem/prepare/datasets/abt_buy.py
+-rw-r--r--   0 silv       (501) staff       (20)     2698 2024-05-09 00:06:05.000000 libem-0.0.8/libem/prepare/datasets/amazon_google.py
+-rw-r--r--   0 silv       (501) staff       (20)     2764 2024-05-14 16:05:14.000000 libem-0.0.8/libem/prepare/datasets/dblp_acm.py
+-rw-r--r--   0 silv       (501) staff       (20)     2760 2024-05-09 00:08:21.000000 libem-0.0.8/libem/prepare/datasets/dblp_scholar.py
+-rw-r--r--   0 silv       (501) staff       (20)     2792 2024-05-09 00:08:37.000000 libem-0.0.8/libem/prepare/datasets/walmart_amazon.py
+-rw-r--r--   0 silv       (501) staff       (20)       72 2024-05-08 23:56:27.000000 libem-0.0.8/libem/prepare/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-03 06:17:55.000000 libem-0.0.8/libem/prepare/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-05 00:06:37.000000 libem-0.0.8/libem/prepare/prompt.py
+-rw-r--r--   0 silv       (501) staff       (20)      204 2024-05-07 15:43:38.000000 libem-0.0.8/libem/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.950628 libem-0.0.8/libem/tune/
+-rw-r--r--   0 silv       (501) staff       (20)      129 2024-05-08 00:48:47.000000 libem-0.0.8/libem/tune/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       31 2024-05-14 16:19:43.000000 libem-0.0.8/libem/tune/catalog.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:18:54.000000 libem-0.0.8/libem/tune/function.py
+-rw-r--r--   0 silv       (501) staff       (20)      224 2024-05-09 21:34:22.000000 libem-0.0.8/libem/tune/interface.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.951691 libem-0.0.8/libem/tune/learn/
+-rw-r--r--   0 silv       (501) staff       (20)      110 2024-05-07 23:38:41.000000 libem-0.0.8/libem/tune/learn/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     3022 2024-05-16 16:16:36.000000 libem-0.0.8/libem/tune/learn/function.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-08 23:52:04.000000 libem-0.0.8/libem/tune/learn/interface.py
+-rw-r--r--   0 silv       (501) staff       (20)      131 2024-05-15 17:57:55.000000 libem-0.0.8/libem/tune/learn/parameter.py
+-rw-r--r--   0 silv       (501) staff       (20)      730 2024-05-09 23:34:00.000000 libem-0.0.8/libem/tune/learn/prompt.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.952150 libem-0.0.8/libem/tune/load/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.8/libem/tune/load/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:05.000000 libem-0.0.8/libem/tune/load/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.952585 libem-0.0.8/libem/tune/save/
+-rw-r--r--   0 silv       (501) staff       (20)       93 2024-05-07 06:19:35.000000 libem-0.0.8/libem/tune/save/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-05-07 06:19:04.000000 libem-0.0.8/libem/tune/save/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.953042 libem-0.0.8/libem/tune/search/
+-rw-r--r--   0 silv       (501) staff       (20)       97 2024-05-07 06:21:06.000000 libem-0.0.8/libem/tune/search/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      139 2024-05-07 06:36:20.000000 libem-0.0.8/libem/tune/search/function.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.941591 libem-0.0.8/libem.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      272 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1575 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)      127 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)       16 2024-05-24 00:41:39.000000 libem-0.0.8/libem.egg-info/top_level.txt
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-24 00:41:39.953331 libem-0.0.8/serve/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-05-04 23:17:56.000000 libem-0.0.8/serve/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      578 2024-05-04 23:21:19.000000 libem-0.0.8/serve/run.py
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-24 00:41:39.953838 libem-0.0.8/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      449 2024-05-24 00:31:37.000000 libem-0.0.8/setup.py
```

### Comparing `libem-0.0.7/LICENSE` & `libem-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/README.md` & `libem-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/cli/libem` & `libem-0.0.8/cli/libem`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/browse/function.py` & `libem-0.0.8/libem/browse/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/calibrate/function.py` & `libem-0.0.8/libem/calibrate/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/constant.py` & `libem-0.0.8/libem/constant.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/core/eval.py` & `libem-0.0.8/libem/core/eval.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/core/log.py` & `libem-0.0.8/libem/core/log.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/core/model.py` & `libem-0.0.8/libem/core/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,31 +24,35 @@
            model: str, temperature: float,
            max_model_call: int = 3,
            seed: int = None) -> str:
     if not os.environ.get("OPENAI_API_KEY"):
         raise EnvironmentError(f"OPENAI_API_KEY is not set. "
                                f"Check your environment or {libem.LIBEM_CONFIG_FILE}.")
     client = OpenAI()
-    num_model_call, tokens = 0, 0
+
+    # todo: simplify accounting using model response
+    num_model_calls = 0
+    num_input_tokens, num_output_tokens = 0, 0
 
     if len(tools) == 0:
         """ Call with no tool use """
         try:
             response = client.chat.completions.create(
                 model=model,
                 messages=[{"role": "user", "content": prompt}],
                 seed=seed,
                 temperature=temperature,
             )
         except APITimeoutError as e:  # catch timeout error
             raise libem.ModelTimedoutException(e)
 
+        num_model_calls += 1
+        num_input_tokens += response.usage.total_tokens - response.usage.completion_tokens
+        num_output_tokens += response.usage.completion_tokens
         response_message = response.choices[0].message
-        tokens += response.usage.total_tokens
-
     else:
         """ Call with tools """
         # Load the tool modules
         tools = [importlib.import_module(tool) for tool in tools]
 
         # Get the functions from the tools
         available_functions = {
@@ -68,20 +72,22 @@
                 seed=seed,
                 temperature=temperature,
             )
         except APITimeoutError as e:  # catch timeout error
             raise libem.ModelTimedoutException(e)
 
         response_message = response.choices[0].message
-        tokens += response.usage.total_tokens
         tool_calls = response_message.tool_calls
 
+        num_model_calls += 1
+        num_input_tokens += response.usage.total_tokens - response.usage.completion_tokens
+        num_output_tokens += response.usage.completion_tokens
+
         # Call the tools
-        num_model_call = 1
-        while tool_calls and num_model_call < max_model_call:
+        while tool_calls and num_model_calls < max_model_call:
             messages.append(response_message)
             for tool_call in tool_calls:
                 function_name = tool_call.function.name
                 function_to_call = available_functions[function_name]
                 function_args = json.loads(tool_call.function.arguments)
 
                 libem.info(f"Tool: {function_name} - running ..")
@@ -114,23 +120,26 @@
                     seed=seed,
                     temperature=temperature,
                 )
             except APITimeoutError as e:  # catch timeout error
                 raise libem.ModelTimedoutException(e)
 
             response_message = response.choices[0].message
-            tokens += response.usage.total_tokens
             tool_calls = response_message.tool_calls
-            num_model_call += 1
 
-        if num_model_call == max_model_call:
+            num_model_calls += 1
+            num_input_tokens += response.usage.total_tokens - response.usage.completion_tokens
+            num_output_tokens += response.usage.completion_tokens
+
+        if num_model_calls == max_model_call:
             libem.warn(f"Max call reached: {messages}\n{response_message}")
 
     # add model calls to trace
     libem.trace.add({
-        'model': {
-            'num_calls': num_model_call,
-            'tokens': tokens
+        "model": {
+            "num_model_calls": num_model_calls,
+            "num_input_tokens": num_input_tokens,
+            "num_output_tokens": num_output_tokens,
         }
     })
 
     return response_message.content
```

### Comparing `libem-0.0.7/libem/core/struct.py` & `libem-0.0.8/libem/core/struct.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,81 +90,65 @@
         def __repr__(self):
             return self.__str__()
 
         def __len__(self):
             return len(self.rules)
 
         def __add__(self, other):
-            assert isinstance(other, self.__class__)
-            return Prompt.Rule(self.rules + other.rules)
+            match other:
+                case str():
+                    return Prompt.Rule(self.rules + [other])
+                case list():
+                    return Prompt.Rule(self.rules + other)
+                case Prompt.Rule():
+                    return Prompt.Rule(self.rules + other.rules)
+                case _:
+                    raise ValueError(f"Invalid rule type "
+                                     f"{type(other)} for {other}")
 
         def add(self, *rules):
-            """rule.add(rule1, rule2, rule3)"""
+            """rule.add(rule1, rule2, ...)"""
             for rule in rules:
-                self.rules.extend(rule.rules)
+                match rule:
+                    case str():
+                        self.rules.append(rule)
+                    case list():
+                        self.rules.extend(rule)
+                    case _:
+                        raise ValueError(f"Invalid rule type "
+                                         f"{type(rule)} for {rule}")
             return self
 
         def export(self, *args, **kwargs):
             _, _ = args, kwargs
             return self.__call__()
 
         def copy(self):
             return copy.deepcopy(self)
 
-    class Experience:
+    class Experience(Rule):
         def __init__(self, mistakes: list[str] = None,
                      intro: str = "Mistakes to avoid:",
-                     sep="\n", bullet="-"):
-            self.mistakes = mistakes or []
-            self.intro = intro
-            self.sep = sep
-            self.bullet = bullet
-
-        def __call__(self, *args, **kwargs):
-            if len(self.mistakes) == 0:
-                return ""
-            mistakes = [f"{self.bullet} {mistake}" for mistake in self.mistakes
-                        if len(mistake.strip()) != ""]
-            return f"{self.intro}\n" \
-                   f"{self.sep.join(mistakes)}"
-
-        def __str__(self):
-            return str(self.__call__())
-
-        def __repr__(self):
-            return self.__str__()
-
-        def __len__(self):
-            return len(self.mistakes)
-
-        def __add__(self, other):
-            assert isinstance(other, self.__class__)
-            return Prompt.Experience(self.mistakes + other.mistakes)
-
-        def add(self, *mistakes):
-            """mistake.add(mistake1, mistake2, mistake3)"""
-            for mistake in mistakes:
-                self.mistakes.extend(mistake.miscakes)
-            return self
-
-        def export(self, *args, **kwargs):
-            _, _ = args, kwargs
-            return self.__call__()
-
-        def copy(self):
-            return copy.deepcopy(self)
+                     sep="\n", bullet="*"):
+            super().__init__(rules=mistakes,
+                             intro=intro,
+                             sep=sep,
+                             bullet=bullet)
 
     @classmethod
     def join(cls, *prompts, sep="\n"):
         to_join = []
         for prompt in prompts:
-            if isinstance(prompt, str):
-                to_join.append(prompt)
-            elif isinstance(prompt, (cls.Rule, cls.Experience)):
-                to_join.append(prompt())
+            match prompt:
+                case str():
+                    to_join.append(prompt)
+                case cls.Rule():
+                    to_join.append(prompt())
+                case cls.Experience():
+                    to_join.append(prompt())
         return sep.join(to_join)
 
     def add(self, *prompts, sep="\n"):
         self.update(Prompt.join(self.value, *prompts, sep=sep))
         return self
 
     def prepend(self, *prompts, sep="\n"):
```

### Comparing `libem-0.0.7/libem/core/telemetry.py` & `libem-0.0.8/libem/core/telemetry.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/core/util.py` & `libem-0.0.8/libem/core/util.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/interface.py` & `libem-0.0.8/libem/interface.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/match/function.py` & `libem-0.0.8/libem/match/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/match/prompt.py` & `libem-0.0.8/libem/match/prompt.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 query = Prompt(
     default="Do the two entity descriptions refer to the same real-world entity?\n"
             "Entity 1: {left}.\nEntity 2: {right}.",
     options=[""],
 )
 
 rule = Prompt(
-    default=Prompt.Rule(rules=[]),
+    default=Prompt.Rule(),
     options=[Prompt.Rule(rules=["Color distinguishes entities."])],
 )
 
 experience = Prompt(
-    default=Prompt.Experience(),
+    default=Prompt.Experience(intro="Rules to follow:"),
 )
 
 output = Prompt(
     default="Answer with 'Yes' if they do and 'No' if they do not.",
     options=["Explain your answer step by step and end with 'yes' or 'no' only."  # CoT
              "Answer only 1 or 0.",
              "Answer with 'yes' or 'no' only, in lower case.", ],
```

### Comparing `libem-0.0.7/libem/prepare/datasets/abt_buy.py` & `libem-0.0.8/libem/prepare/datasets/abt_buy.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/prepare/datasets/amazon_google.py` & `libem-0.0.8/libem/prepare/datasets/amazon_google.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/prepare/datasets/dblp_acm.py` & `libem-0.0.8/libem/prepare/datasets/dblp_acm.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/prepare/datasets/dblp_scholar.py` & `libem-0.0.8/libem/prepare/datasets/dblp_scholar.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/prepare/datasets/walmart_amazon.py` & `libem-0.0.8/libem/prepare/datasets/walmart_amazon.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/tune/learn/function.py` & `libem-0.0.8/libem/tune/learn/function.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem/tune/learn/prompt.py` & `libem-0.0.8/libem/tune/learn/prompt.py`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/libem.egg-info/SOURCES.txt` & `libem-0.0.8/libem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libem-0.0.7/serve/run.py` & `libem-0.0.8/serve/run.py`

 * *Files identical despite different names*

