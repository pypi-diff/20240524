# Comparing `tmp/kerch-0.2.2.tar.gz` & `tmp/kerch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerch-0.2.2.tar", last modified: Wed Nov 30 13:09:38 2022, max compression
+gzip compressed data, was "kerch-0.3.1.tar", last modified: Thu May 23 19:14:23 2024, max compression
```

## Comparing `kerch-0.2.2.tar` & `kerch-0.3.1.tar`

### file list

```diff
@@ -1,128 +1,22 @@
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.365934 kerch-0.2.2/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1071 2022-05-17 14:49:15.000000 kerch-0.2.2/LICENSE
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     6409 2022-11-30 13:09:38.365934 kerch-0.2.2/PKG-INFO
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     3567 2022-11-24 16:23:36.000000 kerch-0.2.2/README.md
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.344934 kerch-0.2.2/kerch/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      904 2022-11-30 13:07:56.000000 kerch-0.2.2/kerch/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.346934 kerch-0.2.2/kerch/_archive/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)        0 2022-07-04 11:00:00.000000 kerch-0.2.2/kerch/_archive/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.347934 kerch-0.2.2/kerch/_archive/expes/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)        0 2022-07-04 11:00:00.000000 kerch-0.2.2/kerch/_archive/expes/__init__.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     8160 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/_archive/expes/data.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     3345 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/expes/run.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4470 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/expes/tests.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.347934 kerch-0.2.2/kerch/_archive/model/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      767 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/_archive/model/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.348934 kerch-0.2.2/kerch/_archive/model/kpca/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      784 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/kpca/HardKPCA.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      772 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/kpca/SoftKPCA.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     3130 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/kpca/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.349934 kerch-0.2.2/kerch/_archive/model/level/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2686 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/level/DualLinear.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2060 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/level/IDXK.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     6009 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/level/Level.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1010 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/_archive/model/level/Linear.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1343 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/level/PrimalLinear.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      198 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/_archive/model/level/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.350934 kerch-0.2.2/kerch/_archive/model/lssvm/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      756 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/lssvm/HardLSSVM.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1010 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/lssvm/SoftLSSVM.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     6173 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/lssvm/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.350934 kerch-0.2.2/kerch/_archive/model/nn/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4032 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/nn/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.350934 kerch-0.2.2/kerch/_archive/model/rkm/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)    12984 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/model/rkm/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.351934 kerch-0.2.2/kerch/_archive/plot/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1377 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/plot/__init__.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     6576 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/plot/plot_legacy.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1546 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/_archive/plot/plotenv_parent.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4425 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/plot/plotenv_tensorboard.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4643 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/_archive/plot/plotenv_wandb.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1283 2022-07-05 16:51:09.000000 kerch-0.2.2/kerch/_cache.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4508 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/_dataholder.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2912 2022-11-28 17:04:49.000000 kerch-0.2.2/kerch/_logger.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2138 2022-07-05 12:57:43.000000 kerch-0.2.2/kerch/_module.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)    10083 2022-07-05 13:02:41.000000 kerch-0.2.2/kerch/_sample.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4068 2022-07-05 12:57:21.000000 kerch-0.2.2/kerch/_stochastic.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.351934 kerch-0.2.2/kerch/dataset/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     7271 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/dataset/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.354934 kerch-0.2.2/kerch/kernel/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      579 2022-11-30 12:15:22.000000 kerch-0.2.2/kerch/kernel/__init__.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1074 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/kernel/additive_chi2.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)    15292 2022-07-04 12:27:08.000000 kerch-0.2.2/kerch/kernel/base.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1361 2022-07-04 12:49:48.000000 kerch-0.2.2/kerch/kernel/cosine.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1343 2022-07-04 15:45:23.000000 kerch-0.2.2/kerch/kernel/explicit.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1488 2022-07-04 15:45:23.000000 kerch-0.2.2/kerch/kernel/explicit_nn.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4925 2022-07-04 14:54:52.000000 kerch-0.2.2/kerch/kernel/exponential.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1106 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/kernel/factory.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2778 2022-07-04 16:43:02.000000 kerch-0.2.2/kerch/kernel/hat.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      914 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/kernel/implicit.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1548 2022-07-04 14:45:26.000000 kerch-0.2.2/kerch/kernel/implicit_nn.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4993 2022-07-04 14:54:52.000000 kerch-0.2.2/kerch/kernel/indicator.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1086 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/kernel/laplacian.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      985 2022-07-05 16:51:09.000000 kerch-0.2.2/kerch/kernel/linear.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     6779 2022-11-28 17:00:59.000000 kerch-0.2.2/kerch/kernel/nystrom.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2736 2022-07-05 13:39:43.000000 kerch-0.2.2/kerch/kernel/polynomial.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      919 2022-07-04 12:27:40.000000 kerch-0.2.2/kerch/kernel/rbf.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     5150 2022-11-30 13:06:30.000000 kerch-0.2.2/kerch/kernel/rff.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2122 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/kernel/sigmoid.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2242 2022-07-04 14:54:52.000000 kerch-0.2.2/kerch/kernel/skewed_chi2.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.355934 kerch-0.2.2/kerch/model/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      779 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/model/LSSVM.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4654 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/model/Model.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)        0 2022-10-06 14:54:04.000000 kerch-0.2.2/kerch/model/RKM.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)       25 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/model/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.355934 kerch-0.2.2/kerch/opt/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2693 2022-07-12 14:15:02.000000 kerch-0.2.2/kerch/opt/__init__.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.357934 kerch-0.2.2/kerch/opt/stiefel/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)    11819 2022-07-08 15:18:04.000000 kerch-0.2.2/kerch/opt/stiefel/grassmann_optimizer.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     3007 2022-07-12 13:17:11.000000 kerch-0.2.2/kerch/opt/stiefel/gutils.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)    12081 2022-07-12 13:12:17.000000 kerch-0.2.2/kerch/opt/stiefel/stiefel_optimizer.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2461 2022-07-08 15:18:04.000000 kerch-0.2.2/kerch/opt/stiefel/utils.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.358934 kerch-0.2.2/kerch/opt/stiefel_old/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     3125 2022-07-05 16:40:46.000000 kerch-0.2.2/kerch/opt/stiefel_old/gutils.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)    12149 2022-07-08 12:36:11.000000 kerch-0.2.2/kerch/opt/stiefel_old/stiefel_optimizer.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2628 2022-07-05 16:35:15.000000 kerch-0.2.2/kerch/opt/stiefel_old/utils_cayley.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.359934 kerch-0.2.2/kerch/plot/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)       39 2022-07-05 09:47:08.000000 kerch-0.2.2/kerch/plot/__init__.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2887 2022-10-11 15:03:22.000000 kerch-0.2.2/kerch/plot/model.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      842 2022-07-05 09:47:08.000000 kerch-0.2.2/kerch/plot/rkm.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.360934 kerch-0.2.2/kerch/rkm/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      202 2022-11-24 16:40:28.000000 kerch-0.2.2/kerch/rkm/__init__.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     8677 2022-11-28 17:02:04.000000 kerch-0.2.2/kerch/rkm/_kpca.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     5093 2022-11-24 15:46:29.000000 kerch-0.2.2/kerch/rkm/_level.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)    11443 2022-11-24 16:49:22.000000 kerch-0.2.2/kerch/rkm/_view.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      892 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/rkm/kpca.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2276 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/rkm/level.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4364 2022-10-12 14:36:32.000000 kerch-0.2.2/kerch/rkm/lssvm.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.361934 kerch-0.2.2/kerch/rkm/multiview/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)       27 2022-11-24 16:36:44.000000 kerch-0.2.2/kerch/rkm/multiview/__init__.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     6608 2022-11-24 14:03:27.000000 kerch-0.2.2/kerch/rkm/multiview/multiview.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     7236 2022-11-29 15:08:10.000000 kerch-0.2.2/kerch/rkm/multiview/mvkpca.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1044 2022-11-24 16:39:58.000000 kerch-0.2.2/kerch/rkm/multiview/mvlevel.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1202 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/rkm/ridge.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     7608 2022-11-24 16:49:22.000000 kerch-0.2.2/kerch/rkm/view.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.363934 kerch-0.2.2/kerch/utils/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      149 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/utils/__init__.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      645 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/utils/arch.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1297 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/utils/cast.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      288 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/utils/decorators.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      346 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/utils/doc.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1610 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/utils/errors.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     1121 2022-07-12 15:27:28.000000 kerch-0.2.2/kerch/utils/math.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      213 2022-07-04 12:03:14.000000 kerch-0.2.2/kerch/utils/tensor.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      452 2022-11-28 17:11:48.000000 kerch-0.2.2/kerch/utils/type.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.345934 kerch-0.2.2/kerch.egg-info/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     6409 2022-11-30 13:09:38.000000 kerch-0.2.2/kerch.egg-info/PKG-INFO
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2722 2022-11-30 13:09:38.000000 kerch-0.2.2/kerch.egg-info/SOURCES.txt
--rw-r--r--   0 hdeplaen (23298) sista     (1300)        1 2022-11-30 13:09:38.000000 kerch-0.2.2/kerch.egg-info/dependency_links.txt
--rw-r--r--   0 hdeplaen (23298) sista     (1300)       61 2022-11-30 13:09:38.000000 kerch-0.2.2/kerch.egg-info/requires.txt
--rw-r--r--   0 hdeplaen (23298) sista     (1300)        6 2022-11-30 13:09:38.000000 kerch-0.2.2/kerch.egg-info/top_level.txt
--rw-r--r--   0 hdeplaen (23298) sista     (1300)       38 2022-11-30 13:09:38.365934 kerch-0.2.2/setup.cfg
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2216 2022-11-24 14:19:01.000000 kerch-0.2.2/setup.py
-drwxr-xr-x   0 hdeplaen (23298) sista     (1300)        0 2022-11-30 13:09:38.364934 kerch-0.2.2/test/
--rw-r--r--   0 hdeplaen (23298) sista     (1300)      331 2022-11-24 14:03:27.000000 kerch-0.2.2/test/test_all.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     6100 2022-11-24 14:03:27.000000 kerch-0.2.2/test/test_kernel.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     4034 2022-11-24 16:19:29.000000 kerch-0.2.2/test/test_kpca.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     2786 2022-11-24 16:34:50.000000 kerch-0.2.2/test/test_lssvm.py
--rw-r--r--   0 hdeplaen (23298) sista     (1300)     5228 2022-11-24 14:03:27.000000 kerch-0.2.2/test/test_mvkpca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:23.526994 kerch-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-23 19:14:19.000000 kerch-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 19:14:19.000000 kerch-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-05-23 19:14:23.526994 kerch-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-23 19:14:19.000000 kerch-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:23.526994 kerch-0.3.1/kerch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-23 19:14:19.000000 kerch-0.3.1/kerch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-23 19:14:19.000000 kerch-0.3.1/kerch/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-23 19:14:19.000000 kerch-0.3.1/kerch/_dataholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-23 19:14:19.000000 kerch-0.3.1/kerch/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-23 19:14:19.000000 kerch-0.3.1/kerch/_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-23 19:14:19.000000 kerch-0.3.1/kerch/_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-23 19:14:19.000000 kerch-0.3.1/kerch/_stochastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:14:23.526994 kerch-0.3.1/kerch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-05-23 19:14:23.000000 kerch-0.3.1/kerch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-23 19:14:23.000000 kerch-0.3.1/kerch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:14:23.000000 kerch-0.3.1/kerch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 19:14:23.000000 kerch-0.3.1/kerch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 19:14:23.000000 kerch-0.3.1/kerch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-23 19:14:19.000000 kerch-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:14:23.526994 kerch-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 19:14:20.000000 kerch-0.3.1/setup.py
```

### Comparing `kerch-0.2.2/README.md` & `kerch-0.3.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Kerch
-[![PyPI version](https://badge.fury.io/py/kerch.svg)](https://badge.fury.io/py/kerch)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://img.shields.io/pypi/v/kerch
+)](https://pypi.org/project/kerch/)
+[![PyPi downloads](https://img.shields.io/pypi/dw/kerch
+)](https://pypi.org/project/kerch/)
+[![License: LGPL-3.0](https://img.shields.io/github/license/hdeplaen/kerch
+)](https://www.gnu.org/licenses/lgpl-3.0.html)
+[![Documentation Status](https://readthedocs.org/projects/kerch/badge/?version=latest
+)](https://kerch.readthedocs.io/en/latest/?badge=latest)
+[![Size of the repository](https://img.shields.io/github/repo-size/hdeplaen/kerch
+)](https://github.com/hdeplaen/kerch)
+[![Total number of commits](https://img.shields.io/github/commit-activity/t/hdeplaen/kerch
+)](https://github.com/hdeplaen/kerch/commits/master/)
+
 
 Kerch is a Python package meant for various kernel methods, and in particular Deep Restricted Kernel Machines. You can natively perform SVMs, LS-SVMs, (K)PCA with various kernels, automatic centering, out-of-sample, etc.
 
-The package is built on PyTorch and supports GPU acceleration.
+The package is built upon PyTorch and supports GPU acceleration.
 
 <!-- toc -->
 
 * [Examples](#examples)
   - [LS-SVM](#training-and-plotting-an-ls-svm)
 * [Installation](#installation)
   - [PIP](#pip)
@@ -19,22 +30,23 @@
 
 ## Examples
 
 
 ### Training and plotting an LS-SVM
 
 This is done by first instantiating a model, setting its dataset, searching for the hyperparameters, fitting with those 
-parameters and plotting. The implementation can be found [here](examples/lssvm-tuning.py).
+parameters and plotting. The implementation can be found [here](research/misc/lssvm-tuning.py).
 
 ```python
-mdl = kerch.model.LSSVM(type="rbf",                 # kernel type
+import kerch                                        # importation is fast as the modules are only loaded when called
+mdl = kerch.model.LSSVM(type="rbf",                 # kernel name
                      representation="dual")         # initiate model
-mdl.set_data_prop(data=data,                        # data
+mdl.set_data_prop(data=data,                        # value
                   labels=labels,                    # corresponding labels
-                  proportions=[1, 0, 0])            # initiate dataset
+                  proportions=[1, 0, 0])            # initiate data
 mdl.hyperopt({"gamma", "sigma"},                    # define which parameters to tune
              max_evals=500,                         # define how many trials
              k=10)                                  # 10-fold cross-validation
 mdl.fit()                                           # fit the optimal parameters found
 kerch.plot.plot_model(mdl)                          # plot the model using the built-in method
 
 ```
@@ -43,24 +55,25 @@
 
 
 ### Out-of-sample kernels with normalization and centering
 The factory class alows for the fast instantiation of various implemented kernels. Centering and normalization are 
 options to choose from and the out-of-sample will also satisfy these properties, based on statistics relative ti the 
 sample. You can easily use numpy arrays ore even python builtins such as `range()`. An implementation can be found 
 [here](examples/kernel.py)
+
 ```python
-sample = np.sin(np.arange(0,15) / np.pi) + .1
-oos = np.sin(np.arange(15,30) / np.pi) + .1
+sample = np.sin(np.arange(0, 15) / np.pi) + .1
+oos = np.sin(np.arange(15, 30) / np.pi) + .1
 
 k = kerch.kernel.factory(type="polynomial", sample=sample, center=True, normalize=True)
 
-k.K   # = k.k()
-k.k(y=oos)
-k.k(x=oos)
-k.k(x=oos, y=oos)
+k.K  # = k1.k1()
+k.k1(y=oos)
+k.k1(x=oos)
+k.k1(x=oos, y=oos)
 
 ```
 
 ![A centered and normalized kernel with out-of-sample parts](docs/_build/html/examples-2.png)
 
 
 ## Installation
@@ -84,8 +97,8 @@
 * [ESAT-STADIUS](https://www.esat.kuleuven.be/stadius/): KU Leuven, Department of Electrical Engineering (ESAT), STADIUS Center for
     Dynamical Systems, Signal Processing and Data Analytics.
 
 ## Contributors
 The contributors and acknowledgements can be found in the [CONRIBUTORS](CONTRIBUTORS) file.
 
 ## License
-Kerch has a MIT license, as found in the [LICENSE](LICENSE) file.
+Kerch has a LGPL-3.0 license, as found in the [LICENSE](LICENSE) file.
```

### Comparing `kerch-0.2.2/kerch/_dataholder.py` & `kerch-0.3.1/kerch/_dataholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,24 +68,24 @@
     def _get_fold(self, prop:float=.2):
         return _DataHolder._split_data_two(self._training_data, self._training_labels, prop=prop)
 
     def _get_default_data(self, data=None, labels=None):
         if data is None:
             data = self._training_data
             labels = self._training_labels
-        elif labels is None: # if labels is None and not data
+        elif labels is None: # if labels is None and not value
             raise NotImplementedError # reconstruction error for example in KPCA (still see how to implement it neatly).
         return data, labels
 
     ####################################################################################################################
 
     @staticmethod
     def _split_data(data, labels=None, props=None):
         r"""
-        Splits the data in multiple random datasets based on props.
+        Splits the value in multiple random datasets based on props.
         """
         if props is None:
             return data, labels
 
         n = data.shape[0]
         perm = np.random.permutation(n)
         data = data[perm]
```

### Comparing `kerch-0.2.2/kerch/_logger.py` & `kerch-0.3.1/kerch/_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 
 _kerch_format = logging.Formatter(_LOGGING_FORMAT)
 _kerch_handler = logging.StreamHandler()
 _kerch_handler.setFormatter(_kerch_format)
 
 
 class _Logger(metaclass=ABCMeta):
+    r"""
+    :param log_level: The logging level of this specific instance. If None, it will be the default logging level set
+        for the toolbox., defaults to None.
+    :type log_level: str or int
+    """
     @utils.kwargs_decorator({
         "log_level": None,
         "name": None
     })
     def __init__(self, *args, **kwargs):
         self._name = kwargs["name"]
         class_name = self.__class__.__name__
@@ -35,19 +40,19 @@
         self._log = logging.getLogger(name=log_name)
         self._log.addHandler(_kerch_handler)
         self.set_log_level(kwargs["log_level"])
 
     def set_log_level(self, level: int = None) -> int:
         r"""
         Sets a specific log Level to this object. It serves as a way to use specific log Level for a specific class,
-        different than the current general KerPy log Level.
+        different than the current general kerch log Level.
 
-        :param level: If the value is ``None``, the current general KerPy log Level will be used (WARNING if not
+        :param level: If the value is ``None``, the current general kerch log Level will be used (WARNING if not
             specified otherwise)., defaults to ``None``.
-        :param type: int, optional
+        :param name: int, optional
         """
         if level is None:
             level = _GLOBALS["LOG_LEVEL"]
         self._log.setLevel(level)
         return level
 
     def get_log_level(self) -> int:
```

### Comparing `kerch-0.2.2/kerch/_module.py` & `kerch-0.3.1/kerch/_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 """
 
 import torch
 from typing import Iterator
 from abc import ABCMeta, abstractmethod
 
 from ._logger import _Logger
-from .utils import capitalize_only_first
+from .utils import capitalize_only_first, extend_docstring
 
 
+@extend_docstring(_Logger)
 class _Module(_Logger,
               torch.nn.Module,
               object,
               metaclass=ABCMeta):
     @abstractmethod
     def __init__(self, *args, **kwargs):
         # for some obscure reason, calling the super init does not lead to the call of both classes.
@@ -49,14 +50,14 @@
                 if isinstance(module, _Module):
                     yield from module._slow_parameters(recurse)
 
     def manifold_parameters(self, recurse=True, type='euclidean') -> Iterator[torch.nn.Parameter]:
         switcher = {'euclidean': self._euclidean_parameters,
                     'stiefel': self._stiefel_parameters,
                     'slow': self._slow_parameters}
-        gen = switcher.get(type, 'Invalid manifold type.')
+        gen = switcher.get(type, 'Invalid manifold name.')
 
         memo = set()
         for p in gen(recurse=recurse):
             if p not in memo:
                 memo.add(p)
                 yield p
```

### Comparing `kerch-0.2.2/kerch/_sample.py` & `kerch-0.3.1/kerch/_sample.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 Allows for a sample set manager, with stochastic support.
 """
 
 import torch
 
 from abc import ABCMeta, abstractmethod
 from torch import Tensor
-import traceback
+from typing import Union
 
 from . import utils
 from ._cache import _Cache
 from ._logger import _Logger
 from ._stochastic import _Stochastic
-
+from .projections import ProjectionTree
 
 @utils.extend_docstring(_Stochastic)
 class _Sample(_Stochastic,  # manager stochastic indices
               _Cache,  # creates a transportable cache (e.g. for GPU)
               _Logger,  # allows logging actions and errors
               metaclass=ABCMeta):
     r"""
@@ -39,39 +39,44 @@
     :param prop_sample: Instead of giving indices, specifying a proportion of the original sample set is also
         possible. The indices will be uniformly randomly chosen without replacement. The value must be chosen
         such that :math:`0 <` `prop_stochastic` :math:`\leq 1`. All indices are considered if both `idx_stochastic` and
         `prop_stochastic` are `None`., defaults to `None`.
 
     :type idx_sample: int[], optional
     :type idx_sample: float, optional
+
+    :param sample_projection: TODO
+    :type sample_projection: List[str]
     """
 
     @abstractmethod
     @utils.kwargs_decorator({
         "sample": None,
         "sample_trainable": False,
         "num_sample": None,
         "dim_input": None,
         "idx_sample": None,
-        "prop_sample": None})
+        "prop_sample": None,
+        "sample_projections": []})
     def __init__(self, **kwargs):
         super(_Sample, self).__init__(**kwargs)
 
         sample = kwargs["sample"]
         if sample is not None:
             sample = utils.castf(sample)
             self._num_total, self._dim_input = sample.shape
         else:
             self._dim_input = kwargs["dim_input"]
             self._num_total = kwargs["num_sample"]
 
         self._sample = torch.nn.Parameter(torch.empty((0, 0)))
         self._sample_trainable = kwargs["sample_trainable"]
-        
+
         self.init_sample(sample, idx_sample=kwargs["idx_sample"], prop_sample=kwargs["prop_sample"])
+        self._default_sample_projections = kwargs["sample_projections"]
 
     @property
     def dim_input(self) -> int:
         r"""
         Dimension of each datapoint.
         """
         return self._dim_input
@@ -99,23 +104,23 @@
         if self._empty_sample:
             return 0
         return self._num_total
 
     @num_sample.setter
     def num_sample(self, val: int):
         assert self._num_total is None, "Cannot set the number of sample points after initialization if the " \
-                                         "sample dataset. Use init_sample() instead."
+                                        "sample dataset. Use init_sample() instead."
         self._num_total = val
         if self._dim_input is not None:
             self.init_sample()
 
     @property
     def sample(self) -> torch.nn.Parameter:
         r"""
-        Sample dataset.
+        Raw sample before any projectionation.
         """
         return self._sample
 
     @sample.setter
     def sample(self, val):
         assert val is not None, "Cannot assign the sample to None. Please use init_sample() if you want to " \
                                 "re-initialize it."
@@ -135,26 +140,30 @@
 
     @property
     def current_sample(self) -> Tensor:
         r"""
         Returns the sample that is currently used in the computations and for the normalizing and centering statistics
         if relevant.
         """
+        return self.sample_projections.projected_sample
+
+    @property
+    def current_sample_unprojectioned(self) -> Tensor:
         return self._sample[self.idx, :]
 
     def init_sample(self, sample=None, idx_sample=None, prop_sample=None):
         r"""
         Initializes the sample set (and the stochastic indices).
 
         :param sample: Sample points used for the various computations. When an out-of-sample computation is asked, it
             will be given relative to these samples. In case of overwriting a current sample, `num_sample` and
             `dim_input` are also overwritten. If `None` is specified, the sample dataset will be initialized according
             to `num_sample` and `dim_input` specified during the construction. If a previous sample set has been used,
             it will keep the same dimension by consequence. A last case occurs when `sample` is of the class
-            `torch.nn.Parameter`: the sample will then use those values and they can thus be shared with the module
+            `torch.nn.Parameter`: the sample will then use those values, and they can thus be shared with the module
             calling this method., defaults to `None`
         :type sample: Tensor, optional
         :param idx_sample: Initializes the indices of the samples to be updated. All indices are considered if both
             `idx_sample` and `prop_sample` are `None`., defaults to `None`
         :type idx_sample: int[], optional
         :param prop_sample: Instead of giving indices, specifying a proportion of the original sample set is also
             possible. The indices will be uniformly randomly chosen without replacement. The value must be chosen
@@ -169,30 +178,30 @@
                 self._log.info(
                     'The sample cannot be initialized because no sample dataset has been provided nor the '
                     'sample dimensions have been initialized yet.')
                 return
             self._sample = torch.nn.Parameter(
                 torch.nn.init.orthogonal_(torch.empty((self._num_total, self._dim_input),
                                                       dtype=utils.FTYPE,
-                                                      device=self._sample.device), ),
+                                                      device=self._sample.device)),
                 requires_grad=self._sample_trainable)
         elif isinstance(sample, torch.nn.Parameter):
             self._log.debug("Using existing sample defined as an external parameter.")
             self._num_total, self._dim_input = sample.shape
             self._sample_trainable = sample.requires_grad
             self._sample = sample
         else:
             self._log.debug("Assigning new sample points based on the given values.")
             self._num_total, self._dim_input = sample.shape
             self._sample = torch.nn.Parameter(sample.data,
                                               requires_grad=self._sample_trainable)
 
         for sample_module in self.children():
             if isinstance(sample_module, _Sample):
-                sample_module.init_sample(self.sample)
+                sample_module.init_sample(self.current_sample)
 
         self.stochastic(idx=idx_sample, prop=prop_sample)
 
     def update_sample(self, sample_values, idx_sample=None):
         r"""
         Updates the sample set. In contradiction to `init_samples`, this only updates the values of the sample and sets
         the gradients of the updated values to zero if relevant.
@@ -205,15 +214,15 @@
         """
 
         if self._empty_sample:
             self._log.warning('Cannot update the sample values of a None sample dataset.')
             return
 
         sample_values = utils.castf(sample_values, dev=self._sample.device)
-        self._reset()
+        self._reset_cache()
 
         # use all indices if unspecified
         if idx_sample is None:
             idx_sample = self._all_idx
 
         # check consistency of indices
         assert len(idx_sample) == sample_values.shape[0], f"Number of sample values ({sample_values.shape[0]}) and " \
@@ -224,9 +233,41 @@
 
         # zeroing relevant gradient if relevant
         if self._sample_trainable:
             self._sample.grad.data[idx_sample, :].zero_()
 
     def _euclidean_parameters(self, recurse=True):
         if not self._empty_sample:
-            yield self.sample
+            yield self._sample
         yield from super(_Sample, self)._euclidean_parameters(recurse)
+
+    @property
+    def sample_projections(self) -> ProjectionTree:
+        r"""
+        Default projections used by the sample.
+        """
+        return self._sample_projections
+
+    @property
+    def _sample_projections(self) -> ProjectionTree:
+        def fun():
+            return ProjectionTree(explicit=True,
+                                  sample=self._sample[self.idx, :],
+                                  default_projections=self._default_sample_projections,
+                                  cache_level=self._cache_level)
+        return self._get("sample_projections", "oblivious", fun)
+
+    def project_sample(self, data) -> Union[Tensor, None]:
+        r"""
+        Apply to value the same projections as on the sample.
+        """
+        if data is None:
+            return None
+        return self.sample_projections.apply(data)
+
+    def projection_sample_revert(self, data) -> Tensor:
+        r"""
+        Get back the original value from a projected value, by using the same projections as the sample,
+        but in reverse. This is not always feasible, depending on the projections used (normalizations are
+        typically not invertible as they are projections which are not bijective).
+        """
+        return self.sample_projections.revert(data)
```

### Comparing `kerch-0.2.2/kerch/_stochastic.py` & `kerch-0.3.1/kerch/_stochastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 from abc import ABCMeta, abstractmethod
 from torch import Tensor
 
 from . import utils
 from ._cache import _Cache
 from ._logger import _Logger
 
+class _StochasticElement():
+    pass
 
+
+@utils.extend_docstring(_Cache)
 class _Stochastic(_Cache,  # creates a transportable cache (e.g. for GPU)
                   metaclass=ABCMeta):
     @abstractmethod
     def __init__(self, *args, **kwargs):
         super(_Stochastic, self).__init__(*args, **kwargs)
         self._num_total = None
         self._idx_stochastic = None
@@ -71,18 +75,18 @@
         original sample set. This is also the default behavior if this function is never called, nor the parameters
         specified during initialization.
 
         .. note::
             Both `idx_stochastic` and `prop_stochastic` cannot be filled together as conflict would arise.
         """
         if self._num_total is None:
-            self._log.info("Setting stochastic indices cannot work before any data or dimensions have been fed.")
+            self._log.info("Setting stochastic indices cannot work before any value or dimensions have been fed.")
             return
 
-        self._reset()
+        self._reset_cache()
         assert idx is None or prop is None, "Both idx_stochastic and prop_stochastic are not None. " \
                                                           "Please choose one non-None parameter only."
 
         if idx is not None:
             self._log.debug("Using the provided indices for stochasticity.")
             self._idx_stochastic = idx
         elif prop is not None:
```

