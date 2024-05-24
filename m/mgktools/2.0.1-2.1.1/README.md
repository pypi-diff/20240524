# Comparing `tmp/mgktools-2.0.1.tar.gz` & `tmp/mgktools-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgktools-2.0.1.tar", last modified: Wed Mar 27 04:24:44 2024, max compression
+gzip compressed data, was "mgktools-2.1.1.tar", last modified: Fri May 24 01:46:49 2024, max compression
```

## Comparing `mgktools-2.0.1.tar` & `mgktools-2.1.1.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1067 2023-10-31 20:49:58.000000 mgktools-2.0.1/LICENSE
--rw-r--r--   0 yanxiang  (1000) yanxiang  (1000)     1809 2024-03-27 04:24:44.262046 mgktools-2.0.1/PKG-INFO
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1064 2023-11-01 16:05:15.000000 mgktools-2.0.1/README.md
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.258046 mgktools-2.0.1/mgktools/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       70 2024-03-27 04:24:39.000000 mgktools-2.0.1/mgktools/__init__.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.258046 mgktools-2.0.1/mgktools/data/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      178 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/data/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    26121 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/data/data.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.258046 mgktools-2.0.1/mgktools/data/public/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      121 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/data/public/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      618 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/data/public/_get.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2348 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/data/public/qm7.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2726 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/data/public/qm9.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     8969 2024-03-15 15:53:40.000000 mgktools-2.0.1/mgktools/data/split.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.258046 mgktools-2.0.1/mgktools/evaluators/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/evaluators/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    17730 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/evaluators/cross_validation.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2034 2023-12-14 23:06:09.000000 mgktools-2.0.1/mgktools/evaluators/metric.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.258046 mgktools-2.0.1/mgktools/features_mol/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      227 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/features_mol/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     5470 2024-03-15 15:53:40.000000 mgktools-2.0.1/mgktools/features_mol/features_generators.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2626 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/features_mol/utils.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.258046 mgktools-2.0.1/mgktools/graph/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       79 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/graph/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    19334 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/graph/from_rdkit.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     8026 2023-12-02 03:27:18.000000 mgktools-2.0.1/mgktools/graph/hashgraph.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.258046 mgktools-2.0.1/mgktools/hyperparameters/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      735 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/__init__.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.258046 mgktools-2.0.1/mgktools/hyperparameters/configs/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4291 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/additive-msnorm.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4288 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/additive-norm.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     3135 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/additive-pnorm.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4289 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/additive.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       99 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/dot_product.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1927 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/product-msnorm.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1905 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/product-norm.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1912 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/product-pnorm.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1904 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/product.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       91 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/configs/rbf.json
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    10106 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/hyperopt.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     9879 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/hyperparameters/optuna.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/interpret/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/interpret/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      938 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/interpret/gpr.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    10353 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/interpret/interpret.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     9352 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/interpret/interpret_slow.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     6121 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/interpret/subgraph.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2944 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/interpret/subgraph_search.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      868 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/interpret/utils.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/kernels/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     3227 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/kernels/FeatureKernel.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     9779 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/kernels/GraphKernel.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     7977 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/kernels/HybridKernel.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     9247 2024-03-27 04:24:39.000000 mgktools-2.0.1/mgktools/kernels/PreComputed.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/kernels/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    10714 2024-03-27 04:24:39.000000 mgktools-2.0.1/mgktools/kernels/base.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     5398 2024-03-24 00:58:51.000000 mgktools-2.0.1/mgktools/kernels/normalization.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4444 2024-03-27 04:24:39.000000 mgktools-2.0.1/mgktools/kernels/utils.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2431 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/__init__.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/classification/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       87 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/classification/__init__.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/classification/gpc/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      122 2023-11-21 19:48:32.000000 mgktools-2.0.1/mgktools/models/classification/gpc/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    13401 2023-11-21 19:37:08.000000 mgktools-2.0.1/mgktools/models/classification/gpc/gpc.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/classification/svm/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      110 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/classification/svm/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1732 2023-11-05 13:43:17.000000 mgktools-2.0.1/mgktools/models/classification/svm/svm.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/regression/
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/regression/GPRgraphdot/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       93 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/GPRgraphdot/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     3200 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/GPRgraphdot/gpr.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2933 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/GPRgraphdot/sgd.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/regression/GPRsklearn/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/GPRsklearn/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     7009 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/GPRsklearn/gpr.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/regression/ScalableGPR/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4304 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/ScalableGPR/NLE.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      159 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/ScalableGPR/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      163 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/ScalableGPR/nystrom.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      185 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4859 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/consensus.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools/models/regression/svm/
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/svm/__init__.py
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      107 2023-10-31 20:49:58.000000 mgktools-2.0.1/mgktools/models/regression/svm/svm.py
-drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-27 04:24:44.262046 mgktools-2.0.1/mgktools.egg-info/
--rw-r--r--   0 yanxiang  (1000) yanxiang  (1000)     1809 2024-03-27 04:24:44.000000 mgktools-2.0.1/mgktools.egg-info/PKG-INFO
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2597 2024-03-27 04:24:44.000000 mgktools-2.0.1/mgktools.egg-info/SOURCES.txt
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        1 2024-03-27 04:24:44.000000 mgktools-2.0.1/mgktools.egg-info/dependency_links.txt
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      405 2024-03-27 04:24:44.000000 mgktools-2.0.1/mgktools.egg-info/entry_points.txt
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      173 2024-03-27 04:24:44.000000 mgktools-2.0.1/mgktools.egg-info/requires.txt
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        9 2024-03-27 04:24:44.000000 mgktools-2.0.1/mgktools.egg-info/top_level.txt
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       38 2024-03-27 04:24:44.262046 mgktools-2.0.1/setup.cfg
--rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1954 2024-03-24 01:04:36.000000 mgktools-2.0.1/setup.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1067 2023-10-31 20:49:58.000000 mgktools-2.1.1/LICENSE
+-rw-r--r--   0 yanxiang  (1000) yanxiang  (1000)     1870 2024-05-24 01:46:49.096348 mgktools-2.1.1/PKG-INFO
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1064 2023-11-01 16:05:15.000000 mgktools-2.1.1/README.md
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.088348 mgktools-2.1.1/mgktools/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       70 2024-05-24 01:46:03.000000 mgktools-2.1.1/mgktools/__init__.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.088348 mgktools-2.1.1/mgktools/data/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      178 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/data/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    26121 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/data/data.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.088348 mgktools-2.1.1/mgktools/data/public/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      121 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/data/public/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      618 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/data/public/_get.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2348 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/data/public/qm7.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2726 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/data/public/qm9.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     8969 2024-03-15 15:53:40.000000 mgktools-2.1.1/mgktools/data/split.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.088348 mgktools-2.1.1/mgktools/evaluators/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/evaluators/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    19800 2024-04-27 21:28:48.000000 mgktools-2.1.1/mgktools/evaluators/cross_validation.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2034 2024-05-24 01:23:38.000000 mgktools-2.1.1/mgktools/evaluators/metric.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.092348 mgktools-2.1.1/mgktools/exe/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    16493 2024-04-27 21:28:48.000000 mgktools-2.1.1/mgktools/exe/args.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2019 2024-03-15 15:53:40.000000 mgktools-2.1.1/mgktools/exe/model.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    18211 2024-04-27 21:28:48.000000 mgktools-2.1.1/mgktools/exe/run.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.092348 mgktools-2.1.1/mgktools/features_mol/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      227 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/features_mol/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     5470 2024-03-15 15:53:40.000000 mgktools-2.1.1/mgktools/features_mol/features_generators.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2626 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/features_mol/utils.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.092348 mgktools-2.1.1/mgktools/graph/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       79 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/graph/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    19334 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/graph/from_rdkit.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     8026 2023-12-02 03:27:18.000000 mgktools-2.1.1/mgktools/graph/hashgraph.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.092348 mgktools-2.1.1/mgktools/hyperparameters/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      735 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/__init__.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.092348 mgktools-2.1.1/mgktools/hyperparameters/configs/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4291 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/additive-msnorm.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4288 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/additive-norm.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     3135 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/additive-pnorm.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4289 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/additive.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       99 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/dot_product.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1927 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/product-msnorm.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1905 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/product-norm.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1912 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/product-pnorm.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1904 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/product.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       91 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/hyperparameters/configs/rbf.json
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    10115 2024-05-23 23:38:11.000000 mgktools-2.1.1/mgktools/hyperparameters/hyperopt.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     9888 2024-05-23 23:38:11.000000 mgktools-2.1.1/mgktools/hyperparameters/optuna.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.092348 mgktools-2.1.1/mgktools/interpret/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/interpret/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      938 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/interpret/gpr.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    10353 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/interpret/interpret.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     9352 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/interpret/interpret_slow.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     6121 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/interpret/subgraph.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2944 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/interpret/subgraph_search.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2781 2024-05-24 01:22:56.000000 mgktools-2.1.1/mgktools/interpret/utils.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.092348 mgktools-2.1.1/mgktools/kernels/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     3227 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/kernels/FeatureKernel.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     9779 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/kernels/GraphKernel.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     7977 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/kernels/HybridKernel.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     9247 2024-03-27 04:24:39.000000 mgktools-2.1.1/mgktools/kernels/PreComputed.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/kernels/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    10714 2024-03-27 04:24:39.000000 mgktools-2.1.1/mgktools/kernels/base.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     5398 2024-03-24 00:58:51.000000 mgktools-2.1.1/mgktools/kernels/normalization.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4944 2024-04-27 21:28:48.000000 mgktools-2.1.1/mgktools/kernels/utils.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2431 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/__init__.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/classification/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       87 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/classification/__init__.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/classification/gpc/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      122 2023-11-21 19:48:32.000000 mgktools-2.1.1/mgktools/models/classification/gpc/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)    13401 2023-11-21 19:37:08.000000 mgktools-2.1.1/mgktools/models/classification/gpc/gpc.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/classification/svm/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      110 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/classification/svm/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     1732 2023-11-05 13:43:17.000000 mgktools-2.1.1/mgktools/models/classification/svm/svm.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/regression/
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/regression/GPRgraphdot/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       93 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/GPRgraphdot/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     3200 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/GPRgraphdot/gpr.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2933 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/GPRgraphdot/sgd.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/regression/GPRsklearn/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/GPRsklearn/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     7009 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/GPRsklearn/gpr.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/regression/ScalableGPR/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4304 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/ScalableGPR/NLE.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      159 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/ScalableGPR/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      163 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/ScalableGPR/nystrom.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      185 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     4859 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/consensus.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools/models/regression/svm/
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        0 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/svm/__init__.py
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      107 2023-10-31 20:49:58.000000 mgktools-2.1.1/mgktools/models/regression/svm/svm.py
+drwxrwxr-x   0 yanxiang  (1000) yanxiang  (1000)        0 2024-05-24 01:46:49.096348 mgktools-2.1.1/mgktools.egg-info/
+-rw-r--r--   0 yanxiang  (1000) yanxiang  (1000)     1870 2024-05-24 01:46:49.000000 mgktools-2.1.1/mgktools.egg-info/PKG-INFO
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2660 2024-05-24 01:46:49.000000 mgktools-2.1.1/mgktools.egg-info/SOURCES.txt
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        1 2024-05-24 01:46:49.000000 mgktools-2.1.1/mgktools.egg-info/dependency_links.txt
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      405 2024-05-24 01:46:49.000000 mgktools-2.1.1/mgktools.egg-info/entry_points.txt
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)      203 2024-05-24 01:46:49.000000 mgktools-2.1.1/mgktools.egg-info/requires.txt
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)        9 2024-05-24 01:46:49.000000 mgktools-2.1.1/mgktools.egg-info/top_level.txt
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)       38 2024-05-24 01:46:49.096348 mgktools-2.1.1/setup.cfg
+-rw-rw-r--   0 yanxiang  (1000) yanxiang  (1000)     2051 2024-05-24 01:46:14.000000 mgktools-2.1.1/setup.py
```

### Comparing `mgktools-2.0.1/LICENSE` & `mgktools-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/PKG-INFO` & `mgktools-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: mgktools
-Version: 2.0.1
+Version: 2.1.1
 Summary: Marginalized graph kernel library for molecular property prediction
 Home-page: https://github.com/xiangyan93/mgktools
 Author: Yan Xiang
 Author-email: 1993.xiangyan@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: scikit-learn>=0.24.1
 Requires-Dist: tqdm>=4.62.0
 Requires-Dist: hyperopt>=0.2.5
 Requires-Dist: optuna>=3.6.0
 Requires-Dist: scipy>=1.6.2
 Requires-Dist: mendeleev>=0.7
 Requires-Dist: rxntools>=0.0.2
 Requires-Dist: pycuda>=2022.1
 Requires-Dist: rdkit>=2022.9.2
 Requires-Dist: deepchem==2.7.2.dev20231207083329
+Requires-Dist: typed-argument-parser
+Requires-Dist: ipython
 
 # mgktools
 Python Package using marginalized graph kernel (MGK) to predict molecular properties.
 
 ## Installation
 Suggested Package Versions:
 Python==3.10, GCC==11.2, CUDA==11.7.
```

### Comparing `mgktools-2.0.1/README.md` & `mgktools-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/data/data.py` & `mgktools-2.1.1/mgktools/data/data.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/data/public/_get.py` & `mgktools-2.1.1/mgktools/data/public/_get.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/data/public/qm7.py` & `mgktools-2.1.1/mgktools/data/public/qm7.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/data/public/qm9.py` & `mgktools-2.1.1/mgktools/data/public/qm9.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/data/split.py` & `mgktools-2.1.1/mgktools/data/split.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/evaluators/cross_validation.py` & `mgktools-2.1.1/mgktools/evaluators/cross_validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,54 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
+import itertools
 from typing import Dict, Iterator, List, Optional, Union, Literal, Tuple
 import math
 from tqdm import tqdm
 import pandas as pd
 import numpy as np
 from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
 from sklearn.model_selection import KFold
 from ..interpret.utils import save_mols_pkl
 from ..data import Dataset
 from ..data.split import get_data_from_index, dataset_split
 from .metric import Metric, eval_metric_func
 
 
+def data_augmentation(dataset: Dataset) -> List[Dataset]:
+    """
+    Data augmentation for the dataset.
+    """
+    n_p = len(dataset.data[0].data.data_p)
+    n_m = len(dataset.data[0].data.data_m)
+    n_cr = len(dataset.data[0].data.data_cr)
+    n_3d = len(dataset.data[0].data.data_3d)
+    assert n_p > 1 or n_m > 1 or n_cr > 1 or n_3d > 1, 'No need to augment data.'
+    datasets_copy = []
+    # create all shuffling index
+    for idx_p in itertools.permutations(range(n_p)):
+        for idx_m in itertools.permutations(range(n_m)):
+            for idx_cr in itertools.permutations(range(n_cr)):
+                for idx_3d in itertools.permutations(range(n_3d)):
+                    dataset_copy = dataset.copy()
+                    for data in dataset_copy.data:
+                        if n_p > 1:
+                            data.data.data_p = [data.data.data_p[i] for i in idx_p]
+                        if n_m > 1:
+                            data.data.data_m = [data.data.data_m[i] for i in idx_m]
+                        if n_cr > 1:
+                            data.data.data_cr = [data.data.data_cr[i] for i in idx_cr]
+                        if n_3d > 1:
+                            data.data.data_3d = [data.data.data_3d[i] for i in idx_3d]
+                        data.data.data = data.data.data_p + data.data.data_m + data.data.data_cr + data.data.data_3d
+                    datasets_copy.append(dataset_copy)
+    return datasets_copy
+
+
 class Evaluator:
     def __init__(self,
                  save_dir: str,
                  dataset: Dataset,
                  model,
                  task_type: Literal['regression', 'binary', 'multi-class'],
                  metrics: List[Metric],
@@ -25,39 +56,44 @@
                  nfold: int = None,
                  split_type: Literal['random', 'scaffold_order', 'scaffold_random'] = None,
                  split_sizes: List[float] = None,
                  num_folds: int = 1,
                  return_std: bool = False,
                  return_proba: bool = False,
                  evaluate_train: bool = False,
+                 augment_data: bool = False,
                  n_similar: Optional[int] = None,
                  kernel=None,
                  n_core: int = None,
                  atomic_attribution: bool = False,
                  seed: int = 0,
                  verbose: bool = True
                  ):
         """Evaluator that evaluate the performance of Monte Carlo cross-validation.
 
         Parameters
         ----------
         save_dir:
             The directory that save all output files.
         dataset:
+            The dataset for cross-validation or the training data.
         model:
+            The machine learning model.
         task_type:
         split_type
         split_sizes
         metrics
         num_folds
         return_std:
             If True, the regression model will output posterior uncertainty.
         return_proba:
             If True, the classification model will output probability.
         evaluate_train
+        augment_data:
+            If True, the dataset will be augmented by shuffling the order of the equivalent columns of the data.
         n_similar:
             n_similar molecules in the training set that are most similar to the molecule to be predicted will be
             outputed.
         kernel:
             if n_similar is not None, kernel must not be None, too.
         n_core:
             useful for nystrom approximation. number of sample to be randomly selected in the core set.
@@ -74,14 +110,15 @@
         self.split_type = split_type
         self.split_sizes = split_sizes
         self.metrics = metrics
         self.num_folds = num_folds
         self.return_std = return_std
         self.return_proba = return_proba
         self.evaluate_train = evaluate_train
+        self.augment_data = augment_data
         self.n_similar = n_similar
         self.kernel = kernel
         self.n_core = n_core
         self.atomic_attribution = atomic_attribution
         self.seed = seed
         self.verbose = verbose
 
@@ -176,14 +213,19 @@
         return np.nanmean(test_metrics_results[self.metrics[0]])
 
     def evaluate_train_test(self, dataset_train: Dataset,
                             dataset_test: Dataset,
                             output_tag: str = '0') -> Tuple[Optional[List[float]],
                                                             Optional[
                                                             List[float]]]:
+        if self.augment_data:
+            for dataset in data_augmentation(dataset_train)[1:]:
+                dataset_train.data.extend(dataset.data)
+            for dataset in data_augmentation(dataset_test)[1:]:
+                dataset_test.data.extend(dataset.data)
         train_log = 'train_%s.csv' % output_tag
         test_log = 'test_%s.csv' % output_tag
 
         X_train = dataset_train.X
         y_train = dataset_train.y
         if y_train.shape[1] == 1:
             y_train = y_train.ravel()
```

### Comparing `mgktools-2.0.1/mgktools/evaluators/metric.py` & `mgktools-2.1.1/mgktools/evaluators/metric.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/features_mol/features_generators.py` & `mgktools-2.1.1/mgktools/features_mol/features_generators.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/features_mol/utils.py` & `mgktools-2.1.1/mgktools/features_mol/utils.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/graph/from_rdkit.py` & `mgktools-2.1.1/mgktools/graph/from_rdkit.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/graph/hashgraph.py` & `mgktools-2.1.1/mgktools/graph/hashgraph.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/__init__.py` & `mgktools-2.1.1/mgktools/hyperparameters/__init__.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/configs/additive-msnorm.json` & `mgktools-2.1.1/mgktools/hyperparameters/configs/additive-msnorm.json`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/configs/additive-norm.json` & `mgktools-2.1.1/mgktools/hyperparameters/configs/additive-norm.json`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/configs/additive-pnorm.json` & `mgktools-2.1.1/mgktools/hyperparameters/configs/additive-pnorm.json`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/configs/additive.json` & `mgktools-2.1.1/mgktools/hyperparameters/configs/additive.json`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/configs/product-msnorm.json` & `mgktools-2.1.1/mgktools/hyperparameters/configs/product-msnorm.json`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/configs/product-norm.json` & `mgktools-2.1.1/mgktools/hyperparameters/configs/product-norm.json`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/configs/product-pnorm.json` & `mgktools-2.1.1/mgktools/hyperparameters/configs/product-pnorm.json`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/configs/product.json` & `mgktools-2.1.1/mgktools/hyperparameters/configs/product.json`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/hyperopt.py` & `mgktools-2.1.1/mgktools/hyperparameters/hyperopt.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     datasets: List[Dataset],
     kernel_config,
     task_type: Literal["regression", "binary", "multi-class"],
     model_type: Literal[
         "gpr", "gpr-sod", "gpr-nystrom", "gpr-nle", "svr", "gpc", "svc"
     ],
     metric: Literal[Metric, "log_likelihood"],
-    cross_validation: Literal["nfold", "loocv", "Monte-Carlo"],
+    cross_validation: Literal["n-fold", "leave-one-out", "Monte-Carlo"],
     nfold: int = None,
     split_type: Literal["random", "scaffold_balanced", "assigned"] = None,
     split_sizes: List[float] = None,
     num_folds: int = 10,
     num_iters: int = 100,
     alpha: float = 0.01,
     alpha_bounds: Tuple[float, float] = None,
```

### Comparing `mgktools-2.0.1/mgktools/hyperparameters/optuna.py` & `mgktools-2.1.1/mgktools/hyperparameters/optuna.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     datasets: List[Dataset],
     kernel_config,
     task_type: Literal["regression", "binary", "multi-class"],
     model_type: Literal[
         "gpr", "gpr-sod", "gpr-nystrom", "gpr-nle", "svr", "gpc", "svc"
     ],
     metric: Literal[Metric, "log_likelihood"],
-    cross_validation: Literal["nfold", "loocv", "Monte-Carlo"],
+    cross_validation: Literal["n-fold", "leave-one-out", "Monte-Carlo"],
     nfold: int = None,
     split_type: Literal["random", "scaffold_balanced", "assigned"] = None,
     split_sizes: List[float] = None,
     num_folds: int = 10,
     num_iters: int = 100,
     alpha: float = 0.01,
     alpha_bounds: Tuple[float, float] = None,
```

### Comparing `mgktools-2.0.1/mgktools/interpret/gpr.py` & `mgktools-2.1.1/mgktools/interpret/gpr.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/interpret/interpret.py` & `mgktools-2.1.1/mgktools/interpret/interpret.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/interpret/interpret_slow.py` & `mgktools-2.1.1/mgktools/interpret/interpret_slow.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/interpret/subgraph.py` & `mgktools-2.1.1/mgktools/interpret/subgraph.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/interpret/subgraph_search.py` & `mgktools-2.1.1/mgktools/interpret/subgraph_search.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/kernels/FeatureKernel.py` & `mgktools-2.1.1/mgktools/kernels/FeatureKernel.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/kernels/GraphKernel.py` & `mgktools-2.1.1/mgktools/kernels/GraphKernel.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/kernels/HybridKernel.py` & `mgktools-2.1.1/mgktools/kernels/HybridKernel.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/kernels/PreComputed.py` & `mgktools-2.1.1/mgktools/kernels/PreComputed.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/kernels/base.py` & `mgktools-2.1.1/mgktools/kernels/base.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/kernels/normalization.py` & `mgktools-2.1.1/mgktools/kernels/normalization.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/kernels/utils.py` & `mgktools-2.1.1/mgktools/kernels/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,22 @@
 
     if graph_kernel_type == "pre-computed":
         n_features = dataset.N_features_add
     else:
         n_features = dataset.N_features_mol + dataset.N_features_add
 
     if features_hyperparameters_file is not None:
+        if not os.path.exists(features_hyperparameters_file):
+            saved_features_hyperparameters_file = os.path.join(
+                os.path.dirname(__file__), "../hyperparameters/configs", features_hyperparameters_file
+            )
+            if os.path.exists(saved_features_hyperparameters_file):
+                features_hyperparameters_file = saved_features_hyperparameters_file
+            else:
+                raise FileNotFoundError(f"{features_hyperparameters_file} not found.")
         features_kernel_config = FeatureKernelConfig.load(
             path=".", name=features_hyperparameters_file, idx=0
         )
     else:
         if features_kernel_type is None:
             features_kernel_config = None
         else:
```

### Comparing `mgktools-2.0.1/mgktools/models/__init__.py` & `mgktools-2.1.1/mgktools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/models/classification/gpc/gpc.py` & `mgktools-2.1.1/mgktools/models/classification/gpc/gpc.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/models/classification/svm/svm.py` & `mgktools-2.1.1/mgktools/models/classification/svm/svm.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/models/regression/GPRgraphdot/gpr.py` & `mgktools-2.1.1/mgktools/models/regression/GPRgraphdot/gpr.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/models/regression/GPRgraphdot/sgd.py` & `mgktools-2.1.1/mgktools/models/regression/GPRgraphdot/sgd.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/models/regression/GPRsklearn/gpr.py` & `mgktools-2.1.1/mgktools/models/regression/GPRsklearn/gpr.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/models/regression/ScalableGPR/NLE.py` & `mgktools-2.1.1/mgktools/models/regression/ScalableGPR/NLE.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools/models/regression/consensus.py` & `mgktools-2.1.1/mgktools/models/regression/consensus.py`

 * *Files identical despite different names*

### Comparing `mgktools-2.0.1/mgktools.egg-info/PKG-INFO` & `mgktools-2.1.1/mgktools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: mgktools
-Version: 2.0.1
+Version: 2.1.1
 Summary: Marginalized graph kernel library for molecular property prediction
 Home-page: https://github.com/xiangyan93/mgktools
 Author: Yan Xiang
 Author-email: 1993.xiangyan@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: scikit-learn>=0.24.1
 Requires-Dist: tqdm>=4.62.0
 Requires-Dist: hyperopt>=0.2.5
 Requires-Dist: optuna>=3.6.0
 Requires-Dist: scipy>=1.6.2
 Requires-Dist: mendeleev>=0.7
 Requires-Dist: rxntools>=0.0.2
 Requires-Dist: pycuda>=2022.1
 Requires-Dist: rdkit>=2022.9.2
 Requires-Dist: deepchem==2.7.2.dev20231207083329
+Requires-Dist: typed-argument-parser
+Requires-Dist: ipython
 
 # mgktools
 Python Package using marginalized graph kernel (MGK) to predict molecular properties.
 
 ## Installation
 Suggested Package Versions:
 Python==3.10, GCC==11.2, CUDA==11.7.
```

### Comparing `mgktools-2.0.1/mgktools.egg-info/SOURCES.txt` & `mgktools-2.1.1/mgktools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 mgktools/data/public/__init__.py
 mgktools/data/public/_get.py
 mgktools/data/public/qm7.py
 mgktools/data/public/qm9.py
 mgktools/evaluators/__init__.py
 mgktools/evaluators/cross_validation.py
 mgktools/evaluators/metric.py
+mgktools/exe/args.py
+mgktools/exe/model.py
+mgktools/exe/run.py
 mgktools/features_mol/__init__.py
 mgktools/features_mol/features_generators.py
 mgktools/features_mol/utils.py
 mgktools/graph/__init__.py
 mgktools/graph/from_rdkit.py
 mgktools/graph/hashgraph.py
 mgktools/hyperparameters/__init__.py
```

### Comparing `mgktools-2.0.1/setup.py` & `mgktools-2.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,28 @@
 
 
 long_description = read('README.md')
 
 setuptools.setup(
     name='mgktools',
     version=__version__,
-    python_requires='>=3.8',
+    python_requires='>=3.10',
     install_requires=[
         'scikit-learn>=0.24.1',
         'tqdm>=4.62.0',
         'hyperopt>=0.2.5',
         'optuna>=3.6.0',
         'scipy>=1.6.2',
         'mendeleev>=0.7',
         'rxntools>=0.0.2',
         'pycuda>=2022.1',
         'rdkit>=2022.9.2',
         'deepchem==2.7.2.dev20231207083329',
+        'typed-argument-parser',
+        'ipython',
     ],
     entry_points={
         'console_scripts': [
             'mgk_read_data=mgktools.exe.run:mgk_read_data',
             'mgk_kernel_calc=mgktools.exe.run:mgk_kernel_calc',
             'mgk_model_evaluate=mgktools.exe.run:mgk_model_evaluate',
             'mgk_hyperopt=mgktools.exe.run:mgk_hyperopt',
@@ -47,15 +49,15 @@
         ]
     },
     author='Yan Xiang',
     author_email='1993.xiangyan@gmail.com',
     description='Marginalized graph kernel library for molecular property prediction',
     long_description=long_description,
     url='https://github.com/xiangyan93/mgktools',
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_namespace_packages(include=['mgktools', 'mgktools.*']),
     classifiers=[
         'Programming Language :: Python',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     include_package_data=True,
     package_data={'': ['hyperparameters/configs/*.json']}
```

