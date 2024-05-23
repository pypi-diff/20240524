# Comparing `tmp/stpredict-0.0.8.tar.gz` & `tmp/stpredict-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stpredict-0.0.8.tar", last modified: Thu Oct 20 17:23:06 2022, max compression
+gzip compressed data, was "stpredict-0.0.9.tar", last modified: Thu May 23 21:59:53 2024, max compression
```

## Comparing `stpredict-0.0.8.tar` & `stpredict-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxrwxrwx   0        0        0        0 2022-10-20 17:23:06.958128 stpredict-0.0.8/
--rw-rw-rw-   0        0        0     1091 2021-07-27 12:08:22.000000 stpredict-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       32 2022-09-26 15:18:24.000000 stpredict-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    17214 2022-10-20 17:23:06.958128 stpredict-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    16485 2022-10-20 14:06:20.000000 stpredict-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2021-07-27 11:18:15.000000 stpredict-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1009 2022-10-20 17:23:06.958128 stpredict-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-20 17:23:06.825827 stpredict-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-10-20 17:23:06.916590 stpredict-0.0.8/src/stpredict/
--rw-rw-rw-   0        0        0     6166 2022-10-02 19:00:17.000000 stpredict-0.0.8/src/stpredict/__init__.py
--rw-rw-rw-   0        0        0     9088 2022-01-10 19:23:20.000000 stpredict-0.0.8/src/stpredict/apply_performance_mode.py
--rw-rw-rw-   0        0        0     1900 2022-02-03 19:34:40.000000 stpredict-0.0.8/src/stpredict/configurations.py
-drwxrwxrwx   0        0        0        0 2022-10-20 17:23:06.955377 stpredict-0.0.8/src/stpredict/data/
--rw-rw-rw-   0        0        0    92700 2022-09-29 12:51:38.000000 stpredict-0.0.8/src/stpredict/data/USA_COVID_19_data.csv
--rw-rw-rw-   0        0        0    42262 2022-09-30 22:29:42.000000 stpredict-0.0.8/src/stpredict/data/earthquake_data.csv
--rw-rw-rw-   0        0        0      928 2021-08-05 21:08:08.000000 stpredict-0.0.8/src/stpredict/get_future_data.py
--rw-rw-rw-   0        0        0     6563 2022-01-10 16:05:46.000000 stpredict-0.0.8/src/stpredict/get_normal_target.py
--rw-rw-rw-   0        0        0     1170 2021-08-05 21:09:40.000000 stpredict-0.0.8/src/stpredict/get_target_quantities.py
--rw-rw-rw-   0        0        0     5214 2021-08-05 21:10:18.000000 stpredict-0.0.8/src/stpredict/get_target_temporal_ids.py
--rw-rw-rw-   0        0        0     4109 2022-01-10 16:04:02.000000 stpredict-0.0.8/src/stpredict/get_trivial_values.py
--rw-rw-rw-   0        0        0    19299 2022-02-03 20:39:33.000000 stpredict-0.0.8/src/stpredict/models.py
--rw-rw-rw-   0        0        0    24127 2022-02-14 15:43:23.000000 stpredict-0.0.8/src/stpredict/one_by_one.py
--rw-rw-rw-   0        0        0    10521 2022-02-03 19:34:11.000000 stpredict-0.0.8/src/stpredict/performance.py
--rw-rw-rw-   0        0        0    29618 2022-02-14 10:45:41.000000 stpredict-0.0.8/src/stpredict/performance_summary.py
--rw-rw-rw-   0        0        0    11556 2022-02-14 14:11:01.000000 stpredict-0.0.8/src/stpredict/plot_prediction.py
--rw-rw-rw-   0        0        0      443 2022-01-06 19:52:16.000000 stpredict-0.0.8/src/stpredict/predict.py
--rw-rw-rw-   0        0        0     4173 2022-01-10 20:31:44.000000 stpredict-0.0.8/src/stpredict/predict_func.py
--rw-rw-rw-   0        0        0    12631 2021-08-15 11:49:36.000000 stpredict-0.0.8/src/stpredict/predict_future.py
--rw-rw-rw-   0        0        0   118249 2022-09-29 21:23:30.000000 stpredict-0.0.8/src/stpredict/preprocess.py
--rw-rw-rw-   0        0        0     6292 2022-01-13 12:38:57.000000 stpredict-0.0.8/src/stpredict/rank_covariates.py
--rw-rw-rw-   0        0        0     5098 2022-01-13 12:32:42.000000 stpredict-0.0.8/src/stpredict/rank_features.py
--rw-rw-rw-   0        0        0     4425 2021-08-05 21:28:12.000000 stpredict-0.0.8/src/stpredict/scaling.py
--rw-rw-rw-   0        0        0     1833 2022-10-01 22:30:29.000000 stpredict-0.0.8/src/stpredict/select_features.py
--rw-rw-rw-   0        0        0     8776 2021-08-05 21:33:34.000000 stpredict-0.0.8/src/stpredict/split_data.py
--rw-rw-rw-   0        0        0    18717 2022-02-03 19:38:50.000000 stpredict-0.0.8/src/stpredict/train_evaluate.py
--rw-rw-rw-   0        0        0    22947 2022-02-14 17:19:44.000000 stpredict-0.0.8/src/stpredict/train_test.py
--rw-rw-rw-   0        0        0   106849 2022-02-10 12:04:44.000000 stpredict-0.0.8/src/stpredict/train_validate.py
--rw-rw-rw-   0        0        0    23575 2022-02-14 15:37:26.000000 stpredict-0.0.8/src/stpredict/whole_as_one.py
-drwxrwxrwx   0        0        0        0 2022-10-20 17:23:06.947009 stpredict-0.0.8/src/stpredict.egg-info/
--rw-rw-rw-   0        0        0    17214 2022-10-20 17:23:06.000000 stpredict-0.0.8/src/stpredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2022-10-20 17:23:06.000000 stpredict-0.0.8/src/stpredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-20 17:23:06.000000 stpredict-0.0.8/src/stpredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2022-10-20 17:23:06.000000 stpredict-0.0.8/src/stpredict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-10-20 17:23:06.000000 stpredict-0.0.8/src/stpredict.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 21:59:52.936907 stpredict-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2021-07-27 12:08:22.000000 stpredict-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       32 2022-09-26 15:18:24.000000 stpredict-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    17312 2024-05-23 21:59:52.932634 stpredict-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    16485 2022-10-20 14:06:20.000000 stpredict-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-07-27 11:18:15.000000 stpredict-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1028 2024-05-23 21:59:52.982142 stpredict-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 21:59:52.359726 stpredict-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 21:59:52.692409 stpredict-0.0.9/src/stpredict/
+-rw-rw-rw-   0        0        0     6166 2023-09-18 14:54:20.000000 stpredict-0.0.9/src/stpredict/__init__.py
+-rw-rw-rw-   0        0        0     9088 2023-09-18 14:54:20.000000 stpredict-0.0.9/src/stpredict/apply_performance_mode.py
+-rw-rw-rw-   0        0        0     1909 2023-09-19 19:04:52.000000 stpredict-0.0.9/src/stpredict/configurations.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:59:52.874944 stpredict-0.0.9/src/stpredict/data/
+-rw-rw-rw-   0        0        0    92700 2022-09-29 12:51:38.000000 stpredict-0.0.9/src/stpredict/data/USA_COVID_19_data.csv
+-rw-rw-rw-   0        0        0    42262 2022-09-30 22:29:42.000000 stpredict-0.0.9/src/stpredict/data/earthquake_data.csv
+-rw-rw-rw-   0        0        0      928 2023-09-18 14:54:20.000000 stpredict-0.0.9/src/stpredict/get_future_data.py
+-rw-rw-rw-   0        0        0     5482 2023-09-30 19:19:54.000000 stpredict-0.0.9/src/stpredict/get_map.py
+-rw-rw-rw-   0        0        0     6586 2023-09-18 17:28:18.000000 stpredict-0.0.9/src/stpredict/get_normal_target.py
+-rw-rw-rw-   0        0        0     1170 2023-09-18 14:54:20.000000 stpredict-0.0.9/src/stpredict/get_target_quantities.py
+-rw-rw-rw-   0        0        0     5214 2023-09-18 14:54:22.000000 stpredict-0.0.9/src/stpredict/get_target_temporal_ids.py
+-rw-rw-rw-   0        0        0     4109 2023-09-18 14:54:23.000000 stpredict-0.0.9/src/stpredict/get_trivial_values.py
+-rw-rw-rw-   0        0        0    34834 2024-05-23 21:02:25.000000 stpredict-0.0.9/src/stpredict/models.py
+-rw-rw-rw-   0        0        0    24160 2023-09-26 19:59:31.000000 stpredict-0.0.9/src/stpredict/one_by_one.py
+-rw-rw-rw-   0        0        0    10635 2023-09-26 19:53:26.000000 stpredict-0.0.9/src/stpredict/performance.py
+-rw-rw-rw-   0        0        0    30329 2023-09-19 20:21:03.000000 stpredict-0.0.9/src/stpredict/performance_summary.py
+-rw-rw-rw-   0        0        0    11932 2023-09-19 21:11:57.000000 stpredict-0.0.9/src/stpredict/plot_prediction.py
+-rw-rw-rw-   0        0        0      443 2023-09-18 14:54:23.000000 stpredict-0.0.9/src/stpredict/predict.py
+-rw-rw-rw-   0        0        0     4173 2023-09-18 14:54:23.000000 stpredict-0.0.9/src/stpredict/predict_func.py
+-rw-rw-rw-   0        0        0    12637 2023-09-26 15:55:49.000000 stpredict-0.0.9/src/stpredict/predict_future.py
+-rw-rw-rw-   0        0        0   134666 2024-05-23 11:29:06.000000 stpredict-0.0.9/src/stpredict/preprocess.py
+-rw-rw-rw-   0        0        0     6292 2023-09-18 14:54:27.000000 stpredict-0.0.9/src/stpredict/rank_covariates.py
+-rw-rw-rw-   0        0        0     5098 2023-09-18 14:54:26.000000 stpredict-0.0.9/src/stpredict/rank_features.py
+-rw-rw-rw-   0        0        0     4425 2023-09-18 14:54:26.000000 stpredict-0.0.9/src/stpredict/scaling.py
+-rw-rw-rw-   0        0        0     1833 2023-09-18 14:54:26.000000 stpredict-0.0.9/src/stpredict/select_features.py
+-rw-rw-rw-   0        0        0    17674 2023-09-26 20:15:49.000000 stpredict-0.0.9/src/stpredict/sgcrf.py
+-rw-rw-rw-   0        0        0     8776 2023-09-18 14:54:26.000000 stpredict-0.0.9/src/stpredict/split_data.py
+-rw-rw-rw-   0        0        0    20888 2023-09-26 21:31:44.000000 stpredict-0.0.9/src/stpredict/train_evaluate.py
+-rw-rw-rw-   0        0        0    22968 2023-09-26 20:02:28.000000 stpredict-0.0.9/src/stpredict/train_test.py
+-rw-rw-rw-   0        0        0   107676 2024-01-25 23:31:14.000000 stpredict-0.0.9/src/stpredict/train_validate.py
+-rw-rw-rw-   0        0        0    23608 2023-09-26 20:00:53.000000 stpredict-0.0.9/src/stpredict/whole_as_one.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:59:52.926013 stpredict-0.0.9/src/stpredict.egg-info/
+-rw-rw-rw-   0        0        0    17312 2024-05-23 21:59:52.000000 stpredict-0.0.9/src/stpredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1233 2024-05-23 21:59:52.000000 stpredict-0.0.9/src/stpredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:59:52.000000 stpredict-0.0.9/src/stpredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-23 21:59:52.000000 stpredict-0.0.9/src/stpredict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 21:59:52.000000 stpredict-0.0.9/src/stpredict.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 21:59:52.909237 stpredict-0.0.9/tests/
+-rw-rw-rw-   0        0        0    15673 2024-05-23 21:09:44.000000 stpredict-0.0.9/tests/test_predict.py
+-rw-rw-rw-   0        0        0     5343 2022-10-20 06:30:02.000000 stpredict-0.0.9/tests/test_preprocess.py
```

### Comparing `stpredict-0.0.8/LICENSE` & `stpredict-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/PKG-INFO` & `stpredict-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: stpredict
-Version: 0.0.8
-Summary: Spatio-temporal prediction package
-Home-page: https://github.com/network-and-Data-Science-IUT/stpredict
-Author: Arash Mari Oriyad, Maryam Meghdadi, Mahdi Naderi, Arezoo Haratian
-Author-email: arashmarioriyad@gmail.com, arezo.h1371@yahoo.com
-Maintainer: cndalab
-Maintainer-email: cndalab.iut@gmail.com, pramazi@brocku.ca, arashmarioriyad@gmail.com, arezo.h1371@yahoo.com
-Project-URL: Documentation, https://stpredict.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 STPredict package
 =================
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stpredict?logo=python)
 ![Read the Docs](https://img.shields.io/readthedocs/stpredict?logo=readthedocs)
 ![GitHub last commit](https://img.shields.io/github/last-commit/network-and-Data-Science-IUT/stpredict?color=orange&logo=github)
```

### Comparing `stpredict-0.0.8/README.md` & `stpredict-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: stpredict
+Version: 0.0.9
+Summary: Spatio-temporal prediction package
+Home-page: https://github.com/network-and-Data-Science-IUT/stpredict
+Author: Arash Mari Oriyad, Maryam Meghdadi, Mahdi Naderi, Arezoo Haratian
+Author-email: arashmarioriyad@gmail.com, arezo.h1371@yahoo.com
+Maintainer: cndalab
+Maintainer-email: cndalab.iut@gmail.com, pramazi@brocku.ca, arashmarioriyad@gmail.com, arezo.h1371@yahoo.com
+Project-URL: Documentation, https://stpredict.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas<=1.1.5
+Requires-Dist: scikit-learn>=0.24
+Requires-Dist: scikeras>=0.13.0
+
 
 STPredict package
 =================
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stpredict?logo=python)
 ![Read the Docs](https://img.shields.io/readthedocs/stpredict?logo=readthedocs)
 ![GitHub last commit](https://img.shields.io/github/last-commit/network-and-Data-Science-IUT/stpredict?color=orange&logo=github)
```

### Comparing `stpredict-0.0.8/setup.cfg` & `stpredict-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7470 7265 6469 6374 0d0a 7665   = stpredict..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 380d 0a61  rsion = 0.0.8..a
+00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
 00000030: 7574 686f 7220 3d20 4172 6173 6820 4d61  uthor = Arash Ma
 00000040: 7269 204f 7269 7961 642c 204d 6172 7961  ri Oriyad, Marya
 00000050: 6d20 4d65 6768 6461 6469 2c20 4d61 6864  m Meghdadi, Mahd
 00000060: 6920 4e61 6465 7269 2c20 4172 657a 6f6f  i Naderi, Arezoo
 00000070: 2048 6172 6174 6961 6e0d 0a61 7574 686f   Haratian..autho
 00000080: 725f 656d 6169 6c20 3d20 6172 6173 686d  r_email = arashm
 00000090: 6172 696f 7269 7961 6440 676d 6169 6c2e  arioriyad@gmail.
@@ -46,19 +46,20 @@
 000002d0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
 000002e0: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
 000002f0: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
 00000300: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
 00000310: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
 00000320: 7320 3d20 0d0a 0970 616e 6461 733c 3d31  s = ...pandas<=1
 00000330: 2e31 2e35 0d0a 0973 6369 6b69 742d 6c65  .1.5...scikit-le
-00000340: 6172 6e3e 3d30 2e32 340d 0a69 6e63 6c75  arn>=0.24..inclu
-00000350: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-00000360: 3d20 5472 7565 0d0a 0d0a 5b6f 7074 696f  = True....[optio
-00000370: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000380: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
-00000390: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000003a0: 6765 5f64 6174 615d 0d0a 7374 7072 6564  ge_data]..stpred
-000003b0: 6963 742e 6461 7461 203d 200d 0a09 2a2e  ict.data = ...*.
-000003c0: 6373 760d 0a0d 0a5b 6567 675f 696e 666f  csv....[egg_info
-000003d0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000003e0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000003f0: 0a                                       .
+00000340: 6172 6e3e 3d30 2e32 340d 0a09 7363 696b  arn>=0.24...scik
+00000350: 6572 6173 3e3d 302e 3133 2e30 0d0a 696e  eras>=0.13.0..in
+00000360: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000370: 7461 203d 2054 7275 650d 0a0d 0a5b 6f70  ta = True....[op
+00000380: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000390: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+000003a0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  c....[options.pa
+000003b0: 636b 6167 655f 6461 7461 5d0d 0a73 7470  ckage_data]..stp
+000003c0: 7265 6469 6374 2e64 6174 6120 3d20 0d0a  redict.data = ..
+000003d0: 092a 2e63 7376 0d0a 0d0a 5b65 6767 5f69  .*.csv....[egg_i
+000003e0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000003f0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000400: 0d0a 0d0a                                ....
```

### Comparing `stpredict-0.0.8/src/stpredict/__init__.py` & `stpredict-0.0.9/src/stpredict/__init__.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/apply_performance_mode.py` & `stpredict-0.0.9/src/stpredict/apply_performance_mode.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/configurations.py` & `stpredict-0.0.9/src/stpredict/configurations.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 TARGET_MODES = ['normal', 'cumulative', 'differential', 'moving_average']
 
 RANKING_METHODS = ['mRMR', 'correlation', 'variance']
 
 FEATURE_SELECTION_TYPES = ['covariate', 'feature']
 
-PRE_DEFINED_MODELS = ['nn', 'knn', 'glm', 'gbm']
+PRE_DEFINED_MODELS = ['nn', 'knn', 'glm', 'gbm', 'sgcrf']
 
 MODEL_TYPES = ['regression', 'classification']
 
 PERFORMANCE_MEASURES = ['MAE', 'MAPE', 'MASE', 'MSE', 'R2_score', 'AIC', 'BIC', 'likelihood', 'AUC', 'AUPR']
 
 REGRESSION_PERFORMANCE_MEASURES = ['MAE', 'MAPE', 'MASE', 'MSE', 'R2_score']
```

### Comparing `stpredict-0.0.8/src/stpredict/data/USA_COVID_19_data.csv` & `stpredict-0.0.9/src/stpredict/data/USA_COVID_19_data.csv`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/data/earthquake_data.csv` & `stpredict-0.0.9/src/stpredict/data/earthquake_data.csv`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/get_future_data.py` & `stpredict-0.0.9/src/stpredict/get_future_data.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/get_normal_target.py` & `stpredict-0.0.9/src/stpredict/get_normal_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return training_target, test_target, training_prediction, test_prediction
 
     training_target.loc[:, ('type')] = 1
     test_target.loc[:, ('type')] = 2
     
     training_dates = list(training_target['temporal id'].unique())
     test_dates = list(test_target['temporal id'].unique())
-    data = training_target.append(test_target)
+    data = pd.concat([training_target,test_target],ignore_index=True)
     
     if same_train_test == True:
         test_dates = []
         test_prediction = []
         data = training_target
     
     # if target mode is cumulative we need to return the target variable to its original state
```

### Comparing `stpredict-0.0.8/src/stpredict/get_target_quantities.py` & `stpredict-0.0.9/src/stpredict/get_target_quantities.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/get_target_temporal_ids.py` & `stpredict-0.0.9/src/stpredict/get_target_temporal_ids.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/get_trivial_values.py` & `stpredict-0.0.9/src/stpredict/get_trivial_values.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/one_by_one.py` & `stpredict-0.0.9/src/stpredict/one_by_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,15 @@
             print("Warning: The input 'performance_mode' is set to 'normal' according to model_type=classification'.")
         if target_scaler is not None:
             target_scaler = None
             print("Warning: The input 'target_scaler' is set to None according to model_type=classification'.")
         target_column_name = list(filter(lambda x: x.startswith('Target'), data[0].columns.values))[0]
         labels = data[0].loc[:, target_column_name].unique().tolist()
         labels = [label for label in labels if not (label is None or str(label) == 'nan')]
+        labels = sorted(labels)
         if len(labels) < 2:
             raise Exception("Error: The labels length must be at least two.")
     else:
         if not set(performance_measures) <= set(REGRESSION_PERFORMANCE_MEASURES):
             raise Exception("Error: The input 'performance_measures' is not valid according to 'model_type=regression'.")
     
     if performance_benchmark not in performance_measures:
```

### Comparing `stpredict-0.0.8/src/stpredict/performance.py` & `stpredict-0.0.9/src/stpredict/performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,21 @@
     
     return prediction_mae/trivial_mae
 
 # ROC AUC for binary and multiclass classification
 def auc(true_values, y_score, labels=None):
     # detecting how many classes the classification problem have
     number_of_classes = len(labels)
-
+    
+    
     if number_of_classes == 1 or number_of_classes == 2:    # binary classification
+        true_values_binary = np.where(true_values == labels[0], np.full(true_values.shape, 0), np.full(true_values.shape, 1))
         auc = metrics.roc_auc_score(
-            y_true=true_values, 
-            y_score=y_score[:, 1], 
-            labels=labels
+            y_true=true_values_binary, 
+            y_score=y_score[:, 1]
         )
 
         # # Data to plot roc curve
         # false_positive_rate, true_positive_rate, _ = metrics.roc_curve(true_values, y_score[:, 1])
         
         # # plot roc curve
         # plt.figure(dpi=100)
```

### Comparing `stpredict-0.0.8/src/stpredict/performance_summary.py` & `stpredict-0.0.9/src/stpredict/performance_summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,618 +1,618 @@
-import warnings
-
-with warnings.catch_warnings():
-    warnings.simplefilter("ignore")
-    import numpy as np
-    import pandas as pd
-    import matplotlib.pyplot as plt
-    from os import listdir
-    from os.path import isfile, join, exists
-    import datetime
-    from datetime import timedelta
-    from dateutil.relativedelta import relativedelta
-    import random
-    import sys
-    import os
-    import matplotlib as mpl
-    from matplotlib.backends.backend_pdf import PdfPages
-    import matplotlib.patches as mpatches
-    from matplotlib import colors as mcolors
-    import matplotlib.ticker as ticker
-
-warnings.filterwarnings("ignore")
-
-
-# merge the cells in matplotlib table
-def mergecells(table, cells, selected_text = 'L'):
-    if len(cells)<=1:
-        return
-    cells_array = [np.asarray(c) for c in cells]
-    h = np.array([cells_array[i+1][0] - cells_array[i][0] for i in range(len(cells_array) - 1)])
-    v = np.array([cells_array[i+1][1] - cells_array[i][1] for i in range(len(cells_array) - 1)])
-    bold = False
-
-    # if it's a horizontal merge, all values for `h` are 0
-    if not np.any(h):
-        # sort by horizontal coord
-        cells = np.array(sorted(list(cells), key=lambda v: v[1]))
-        edges = ['BTL'] + ['BT' for i in range(len(cells) - 2)] + ['BTR']
-    elif not np.any(v):
-        cells = np.array(sorted(list(cells), key=lambda h: h[0]))
-        edges = ['TRL'] + ['RL' for i in range(len(cells) - 2)] + ['BRL']
-    else:
-        raise ValueError("Only horizontal and vertical merges allowed")
-
-    for cell, e in zip(cells, edges):
-        table[cell[0], cell[1]].visible_edges = e
-        
-    txts = [table[cell[0], cell[1]].get_text() for cell in cells]
-    tpos = [np.array(t.get_position()) for t in txts]
-    
-    if any([txt.get_weight() == 'bold' for txt in txts]):
-        bold = True
-        
-    if selected_text == 'L':
-        # transpose the text of the left cell
-        trans = (tpos[-1] - tpos[0])/2
-        # didn't had to check for ha because I only want ha='center'
-        txts[0].set_transform(mpl.transforms.Affine2D().translate(*trans))
-        if bold == True:
-            txts[0].set_weight('bold')
-        for txt in txts[1:]:
-            txt.set_visible(False)
-        
-    elif selected_text == 'R':
-        # transpose the text of the right cell
-        trans = (tpos[0] - tpos[-1])/2
-        # didn't had to check for ha because I only want ha='center'
-        txts[-1].set_transform(mpl.transforms.Affine2D().translate(*trans))
-        if bold == True:
-            txts[-1].set_weight('bold')
-        for txt in txts[:-1]:
-            txt.set_visible(False)
-        
-# find the consecutive cells with same values and merge them
-def merge_same_values(row_number,column,offset,the_table):
-    values = [the_table.get_celld()[(i,column)].get_text().get_text() for i in range(offset,row_number+1)]
-    current_value = values[0]
-    merge_list = []
-    for index,value in enumerate(values):
-        # model name of test points must not be merged with previous rows
-        if column == 2 and (the_table.get_celld()[(index+offset,1)].get_text().get_text() == 'Test'):
-            mergecells(the_table, merge_list)
-            if index+offset+1 < row_number:
-                current_value = the_table.get_celld()[(index+offset+1,column)].get_text().get_text()
-                merge_list = []
-            
-        elif value == current_value:
-            merge_list = merge_list+[(index+offset,column)]
-                
-        else:
-            current_value = value
-            mergecells(the_table, merge_list)
-            merge_list = [(index+offset,column)]
-            
-    mergecells(the_table, merge_list)
-    return the_table
-
-# find the consecutive cells with same values and colours them with the same color
-def color_same_values(row_number,column_number,column,offset,the_table,color_dict):
-    
-    colors = ['#008e99','#424242','#ba4c4d','#858585','#acc269','#7255b2']
-    
-    # find cells with same text
-    values = [the_table.get_celld()[(i,column)].get_text().get_text() for i in range(offset,row_number+1)]
-    models = np.unique(values)
-    if len(models) == 1 :
-        color_dict = {models[0]:'#000000'}
-        
-    current_value = values[0]
-    for index,value in enumerate(values):
-        if value == current_value:
-            for col in range(column,column_number):
-                the_table.get_celld()[(index+offset,col)].get_text().set_color(color_dict[value])
-        else:
-            current_value = value
-            for col in range(column,column_number):
-                the_table.get_celld()[(index+offset,col)].get_text().set_color(color_dict[value])
-            
-    return the_table
-
-# prepare input df by counting features and rounding performance values
-def prepare_df(df,base_columns,measure_names,performance_benchmark,test_type,plot_type):
-    
-    if test_type == 'whole-as-one':
-        unique_columns = ['model name', 'history length']
-    if test_type == 'one-by-one':
-        unique_columns = ['Test point','model name','history length']
-        
-    df['feature or covariate set'] = df['feature or covariate set'].apply(lambda x:len(x.split(',')))
-    if performance_benchmark in ['MAE', 'MAPE', 'MASE', 'MSE', 'AIC', 'BIC', 'likelihood']:
-        optimum_performance_df = df.groupby(unique_columns)[[performance_benchmark]].min().reset_index().rename(columns = {performance_benchmark:'best '+performance_benchmark})
-    else:
-        optimum_performance_df = df.groupby(unique_columns)[[performance_benchmark]].max().reset_index().rename(columns = {performance_benchmark:'best '+performance_benchmark})
-    df = pd.merge(df,optimum_performance_df)
-    df = df[df[performance_benchmark] == df['best '+performance_benchmark]].drop_duplicates(subset = unique_columns)
-    df = df[base_columns + measure_names]
-        
-    return df
-
-def table_add(table, df, best_loc, measure_names, performance_benchmark, best_loc_flag):
-    
-    if best_loc_flag == True:
-        df = df.reset_index(drop = True)
-        df[performance_benchmark] = df[performance_benchmark].astype(float)
-        
-        if performance_benchmark in ['MAE', 'MAPE', 'MASE', 'MSE', 'AIC', 'BIC', 'likelihood']:
-            optimum_performance = df[performance_benchmark].min()
-        else:
-            optimum_performance = df[performance_benchmark].max()
-            
-        df_best_loc = list(df[df[performance_benchmark] == optimum_performance].index)[-1]
-        best_loc = best_loc + [df_best_loc + len(table)+1]
-    
-    for measure in measure_names:
-        df[measure] = df[measure].apply(lambda x:np.round(x,2))
-        df.loc[df[measure]>99999,measure] = df.loc[df[measure]>99999,measure].apply(lambda x:'{:.2E}'.format(x))
-    table = table + df.values.tolist()
-    
-    return table, best_loc
-
-# make tables and save into pdf
-def plot_table(train_df,validation_df,test_df,test_type,performance_benchmark,test_point_number):
-    
-    if test_type == 'whole-as-one':
-        base_columns = ['Dataset', 'model name', 'history length', 'feature or covariate set']
-    if test_type == 'one-by-one':
-        base_columns = ['Test point', 'Dataset', 'model name', 'history length', 'feature or covariate set']
-    measure_names = list(filter(lambda x: x not in base_columns, test_df.columns))
-    models_number = len(train_df['model name'].unique())
-    max_history = len(train_df['history length'].unique())
-    
-    models = train_df['model name'].unique()
-    colors = ['#008e99','#424242','#ba4c4d','#858585','#acc269','#7255b2']
-    color_list = colors * ((len(models)//6)+1) 
-    color_dict = {model:color_list[i] for i , model in enumerate(models)}
-
-    test_df = prepare_df(test_df,base_columns,measure_names,performance_benchmark,test_type,'table')
-    train_df = prepare_df(train_df,base_columns,measure_names,performance_benchmark,test_type,'table')
-    if validation_df is not None:
-        validation_df = prepare_df(validation_df,base_columns,measure_names,performance_benchmark,test_type,'table')
-    
-    # the location of best obtained results for each set, in the table 
-    best_loc = []
-    table = []
-    
-    if test_type == 'whole-as-one':
-        table, best_loc = table_add(table, test_df, best_loc, measure_names, performance_benchmark, True)
-        if validation_df is not None:
-            table, best_loc = table_add(table, validation_df, best_loc, measure_names, performance_benchmark, True)
-        table, best_loc = table_add(table, train_df, best_loc, measure_names, performance_benchmark, True)
-        colWidths = [0.15, 0.15, 0.17, 0.15] + [0.15]*len(measure_names)
-        for index,measure_name in enumerate(measure_names):
-            if measure_name in ['R2_score', 'likelihood']:
-                colWidths[index+4] = 0.17
-        row_number = len(table)
-
-    if test_type == 'one-by-one':
-        table, best_loc = table_add(table, test_df[test_df['Test point'] == 'All test points'], best_loc, measure_names, performance_benchmark, False)
-        table = table + [['1','Test','Model','History length','#Features'] + measure_names]
-        for test_point in range(1,test_point_number+1):
-            table, best_loc = table_add(table, test_df[test_df['Test point'] == str(test_point)], best_loc, measure_names, performance_benchmark, True)
-            if validation_df is not None:
-                table, best_loc = table_add(table, validation_df[validation_df['Test point'] == str(test_point)], best_loc, measure_names, performance_benchmark, True)
-            table, best_loc = table_add(table, train_df[train_df['Test point'] == str(test_point)], best_loc, measure_names, performance_benchmark, True)
-        colWidths = [0.15, 0.15, 0.15, 0.17, 0.15] + [0.15]*len(measure_names)
-        for index,measure_name in enumerate(measure_names):
-            if measure_name in ['R2_score', 'likelihood']:
-                colWidths[index+5] = 0.17
-        headerColWidths = [0.15, 0.15] + [np.sum(colWidths[2:])/len(measure_names)]*len(measure_names)
-        row_number = len(table)
-        
-    
-    # calculate number of pages needed
-    npages = row_number // 300
-    if row_number % 300 > 0:
-        npages += 1
-    
-
-    pdf = PdfPages('./plots/performance summary.pdf')
-    
-    for page in range(npages):
-        fig = plt.figure()
-        plt.tight_layout()
-        ax = fig.gca()
-        ax.axis('tight')
-        ax.axis('off')
-        temp_table = table[page*300:(page+1)*300]
-        page_best_locs = [index - (page*300) for index in best_loc if index in range(page*300,(page+1)*300)]
-        
-        ylim = 0.08278145695364238*(len(temp_table))
-        xlim = np.sum(colWidths) + 0.7
-        bbox = (0,0,xlim,ylim)
-        
-        if test_type == 'whole-as-one':
-            colLabels = ['Dataset','Model','History length','#Features'] + measure_names
-
-        
-        if test_type == 'one-by-one' and page == 0:
-            colLabels = ['Test point', 'Dataset','','',''] + measure_names
-        elif test_type == 'one-by-one' and page > 0:
-            colLabels = ['Test point', 'Dataset','Model','History length','#Features'] + measure_names
-        
-        
-        if test_type == 'one-by-one' and page == 0:
-            # make a table to represent header and test set results with different column number
-            headerdata = [[temp_table[0][i] for i in [0,1]+[i+5 for i in range(len(measure_names))]]] + [['']*len(headerColWidths)]*(len(temp_table)-1)
-            headertable = ax.table(cellText=headerdata, colLabels=['Test point', 'Dataset'] + measure_names, 
-                                   colWidths=headerColWidths, loc='center', colColours = ['lightgray']*len(headerColWidths),
-                                   cellLoc='center', edges = 'open', bbox = bbox)
-            for i in range(len(headerColWidths)):
-                headertable.get_celld()[(0,i)].visible_edges = 'closed'
-                headertable.get_celld()[(0,i)].set_text_props(weight='bold')
-                headertable.get_celld()[(1,i)].visible_edges = 'closed'
-            headertable.auto_set_font_size(False)
-            headertable.set_fontsize(9)
-            headertable.scale(1.5, 1.5)
-            fig.canvas.draw()
-        
-        
-        the_table = ax.table(cellText=temp_table, colLabels=colLabels, colWidths=colWidths, loc='center', cellLoc='center', bbox = bbox)
-        the_table.auto_set_font_size(False)
-        the_table.set_fontsize(9)
-        the_table.scale(1.5, 1.5)
-        fig.canvas.draw()
-
-        if test_type == 'whole-as-one':
-            
-            for i in range(1,len(colLabels)):
-                for j in page_best_locs:
-                    the_table.get_celld()[(j,i)].set_text_props(weight='bold')
-                    
-            # merge the cells containing dataset name in first column
-            offset = 2 if page == 0 else 1
-            the_table = merge_same_values(row_number = len(temp_table),
-                                  column = 0, offset = offset, the_table = the_table)
-            # merge the cells containing model name in second column 
-            offset = 2 if page == 0 else 1
-            the_table = color_same_values(row_number = len(temp_table), column_number = len(colLabels),
-                                  column = 1, offset = offset, the_table = the_table, color_dict = color_dict)
-            the_table = merge_same_values(row_number = len(temp_table),
-                                  column = 1, offset = offset, the_table = the_table)
-            
-            
-        if test_type == 'one-by-one':
-            
-            for i in range(2,len(colLabels)):
-                for j in page_best_locs:
-                    the_table.get_celld()[(j,i)].set_text_props(weight='bold')
-                    
-            # merge the cells containing test point number in first column
-            offset = 2 if page == 0 else 1
-            the_table = merge_same_values(row_number = len(temp_table),
-                                          column = 0, offset = offset, the_table = the_table)
-            # merge the cells containing dataset name in second column
-            the_table = merge_same_values(row_number = len(temp_table),
-                                          column = 1, offset = offset, the_table = the_table)
-            # merge the cells containing model name in third column
-            offset = 3 if page == 0 else 1
-            the_table = color_same_values(row_number = len(temp_table), column_number = len(colLabels),
-                                  column = 2, offset = offset, the_table = the_table, color_dict = color_dict)
-            the_table = merge_same_values(row_number = len(temp_table),
-                                          column = 2, offset = offset, the_table = the_table)
-        
-        # colour header
-        for i in range(len(colLabels)):
-            the_table.get_celld()[(0,i)].set_facecolor('lightgray')
-            the_table.get_celld()[(0,i)].set_text_props(weight='bold')
-            
-            if (page == 0) and (test_type == 'one-by-one' and i>1):
-                the_table.get_celld()[(2,i)].set_facecolor('lightgray')#'#40466e'
-                the_table.get_celld()[(2,i)].set_text_props(weight='bold')#, color='w')
-                
-        
-        
-        # set the_table header invisible to make header table visible
-        if test_type == 'one-by-one' and page == 0:
-            for i in range(len(colLabels)):
-                the_table.get_celld()[(0,i)].set_alpha(0)
-                the_table.get_celld()[(1,i)].set_alpha(0)
-                if i>=2:
-                    the_table.get_celld()[(0,i)].get_text().set_visible(False)
-                    the_table.get_celld()[(1,i)].get_text().set_visible(False)
-                
-            
-        
-        pdf.savefig(fig , dpi=300, bbox_inches='tight', pad_inches=1)
-        plt.close()
-
-    pdf.close()
-    
-# make barplots and save into pdf
-
-def plot_bar(train_df,validation_df,test_type,performance_benchmark,test_point_number):
-    
-    if test_type == 'whole-as-one':
-        base_columns = ['Dataset', 'model name', 'history length', 'feature or covariate set']
-    if test_type == 'one-by-one':
-        base_columns = ['Test point', 'Dataset', 'model name', 'history length', 'feature or covariate set']
-    measure_names = list(filter(lambda x: x not in base_columns, train_df.columns))
-    models = train_df['model name'].unique()
-    models_number = len(models)
-    max_history = len(train_df['history length'].unique())
-    
-    colors = ['#008e99','#424242','#ba4c4d','#858585','#acc269','#7255b2']
-    color_list = colors * ((len(models)//6)+1) 
-    color_dict = {model:color_list[i] for i , model in enumerate(models)}
-        
-    train_df = prepare_df(train_df,base_columns,measure_names,performance_benchmark,test_type,'bar')
-    if validation_df is not None:
-        validation_df = prepare_df(validation_df,base_columns,measure_names,performance_benchmark,test_type,'bar')
-    
-    if test_type == 'whole-as-one':
-        test_point_number = 1
-    
-    models_per_plot = 6
-    # calculate number of pages needed
-    npages = models_number // (models_per_plot*5)
-    if models_number % (models_per_plot*5) > 0:
-        npages += 1
-    
-    barWidth = 0.015 if validation_df is not None else 0.030
-    pos = 0.195*np.arange(max_history)
-    
-        
-    # initialize pdf
-    pdf = PdfPages('./plots/performance bar plots.pdf')
-    
-    for test_point in range(1,test_point_number+1):
-        
-        mpl.rcParams.update({'font.size': 12})
-        
-        for page in range(npages):
-            
-            current_models = train_df['model name'].unique()[page*5*models_per_plot:(page+1)*5*models_per_plot]
-            num_subplots = (len(current_models)//models_per_plot)+int()
-            if len(current_models)%models_per_plot > 0:
-                num_subplots += 1
-                
-            fig, axes = plt.subplots(num_subplots,1)
-            if num_subplots == 1:
-                axes = np.array([axes])
-            
-            if test_type == 'one-by-one':
-                plt.suptitle('Test point number {0}'.format(test_point), fontweight='bold', fontsize='16', y=1.05)
-                
-            for subplot in range(num_subplots):
-                
-                subplot_models = current_models[subplot*models_per_plot:(subplot+1)*models_per_plot]
-                ax = axes[subplot]
-                ax.grid(axis = 'y', linestyle = '--')
-                ax.set_axisbelow(True)
-                log_flag = False
-                    
-                for index,model in enumerate(subplot_models):
-
-                    # Set position of bar on X axis
-                    if validation_df is not None:
-                        current_train_pos=[x + (2*index)*barWidth for x in pos]
-                        current_validation_pos=[x + (2*index+1)*barWidth for x in pos]
-                    else:
-                        current_train_pos=[x + index*barWidth for x in pos]
-
-                    if test_type == 'whole-as-one':
-                        train_performance = list(train_df.loc[train_df['model name'] == model,performance_benchmark])
-                        if validation_df is not None:
-                            validation_performance = list(validation_df.loc[validation_df['model name'] == model,performance_benchmark])
-
-                    if test_type == 'one-by-one':
-                        train_performance = list(train_df.loc[(train_df['Test point'] == test_point)&(train_df['model name'] == model),performance_benchmark])
-                        if validation_df is not None:
-                            validation_performance = list(validation_df.loc[(validation_df['Test point'] == test_point)&(validation_df['model name'] == model),performance_benchmark])
-                    
-                    if validation_df is not None:
-                        performance_list = list(train_performance)+list(validation_performance)
-                    else:
-                        performance_list = list(train_performance)
-                    if max(performance_list)-min(performance_list)>10000 and min(performance_list)>=0:
-                        log_flag = True
-
-                    # Make the plot
-                    if validation_df is not None:
-                        ax.bar(current_train_pos, train_performance, color=color_dict[model], width=barWidth, edgecolor='white',hatch='//////')
-                        ax.bar(current_validation_pos, validation_performance, color=color_dict[model], width=barWidth, edgecolor='white', label=model)
-                    else:
-                        ax.bar(current_train_pos, train_performance, color=color_dict[model], width=barWidth, edgecolor='white', label=model)
-                    
-
-                ax.set_ylabel(performance_benchmark,fontweight='bold')
-                if validation_df is not None:
-                    ax.set_xticks(ticks = [r + (len(subplot_models)-0.5)*barWidth for r in pos])
-                else:
-                    ax.set_xticks(ticks = [r + ((len(subplot_models)/2)-0.5)*barWidth for r in pos])
-                ax.set_xticklabels(labels = [str(history) for history in range (1,max_history+1)])
-                if validation_df is not None:
-                    ax.set_title('The predictive models performance', fontweight='bold')
-                else:
-                    ax.set_title('The predictive models performance on\nthe training dataset', fontweight='bold')
-                    
-                if subplot == 0 and validation_df is not None:
-                    train_patch = mpatches.Patch(edgecolor='gray', facecolor='w', label='Training', hatch='//////')
-                    validation_patch = mpatches.Patch(color='gray', label='Validation')
-                    leg1 = ax.legend(handles=[train_patch,validation_patch], loc='upper left', bbox_to_anchor=(1, 1))
-                    ax.add_artist(leg1)
-
-                # Create legend & Show graphic
-                ax.legend(loc='lower left', bbox_to_anchor=(1, 0))
-                
-                
-                y_min = min(ax.get_yticks())
-                y_max = max(ax.get_yticks())
-                if y_max - y_min <= 1:
-                    step = 0.1
-                    ax.set_yticks(np.arange(y_min, y_max, step))
-                else:
-                    step = (y_max-y_min)/10
-                    ax.set_yticks(np.arange(y_min, y_max, step))
-                    
-                if log_flag == True:
-                    ax.set_yscale('log')
-                
-            
-            plt.xlabel('History Length', fontweight='bold')
-            if max_history>5:
-                plt.gcf().set_size_inches(plt.gcf().get_size_inches()[0]*(max_history/5), plt.gcf().get_size_inches()[1]*num_subplots)
-            else:
-                plt.gcf().set_size_inches(plt.gcf().get_size_inches()[0]*(1.5), plt.gcf().get_size_inches()[1]*num_subplots)
-                
-            plt.tight_layout()
-            pdf.savefig(fig , dpi=300, bbox_inches='tight', pad_inches=1)
-            plt.close()
-            
-    pdf.close()
-
-# save summary of performance reports
-
-def performance_summary(forecast_horizon,test_type,performance_benchmark):
-    
-    validation_dir = './performance/validation process/'
-    testing_dir = './performance/test process/'
-    if not exists('./plots/'):
-        os.makedirs('./plots/')
-
-
-    path = validation_dir
-    files = [f for f in listdir(path) if isfile(join(path, f))]
-    prefix = 'training performance report forecast horizon = {0}, test-point #'.format(forecast_horizon)
-    files = [file for file in files if file.startswith(prefix)]
-    file_test_points = [int(file.split('test-point #')[1][:-4]) for file in files]
-    file_test_points.sort()
-
-    if test_type == 'whole-as-one':
-        
-        test_csv_file = testing_dir + 'test performance report forecast horizon = {0}.csv'.format(forecast_horizon)
-        train_csv_file = validation_dir + 'training performance report forecast horizon = {0}.csv'.format(forecast_horizon)
-        validation_csv_file = validation_dir + 'validation performance report forecast horizon = {0}.csv'.format(forecast_horizon)
-
-        test_df = pd.read_csv(test_csv_file)
-        test_df.insert(0, 'Dataset', 'Test')
-
-        train_df = pd.read_csv(train_csv_file)
-        train_df.insert(0, 'Dataset', 'Training')
-        
-        if exists(validation_csv_file):
-            validation_df = pd.read_csv(validation_csv_file)
-            validation_df.insert(0, 'Dataset', 'Validation')
-        else:
-            validation_df = None
-        
-        try:
-            plot_table(train_df,validation_df,test_df,test_type,performance_benchmark,None)
-        except Exception:
-            print('There is a problem in creating the results table.')
-
-    elif test_type == 'one-by-one':
-
-        test_point_number = len(file_test_points)    
-        test_df = pd.read_csv(testing_dir + 'test performance report forecast horizon = {0}.csv'.format(forecast_horizon))
-        test_df = test_df.rename(columns = {'test point':'Test point'})
-        test_df.insert(1, 'Dataset', 'Test')
-
-
-        train_df = pd.DataFrame()
-        validation_df = pd.DataFrame()
-        for test_point in range(1,test_point_number+1):
-
-            tp_number = file_test_points[test_point-1]
-            
-            train_csv_file = validation_dir + 'training performance report forecast horizon = {0}, test-point #{1}.csv'.format(forecast_horizon,tp_number)
-            validation_csv_file = validation_dir + 'validation performance report forecast horizon = {0}, test-point #{1}.csv'.format(forecast_horizon,tp_number)
-
-            temp_train_df = pd.read_csv(train_csv_file)
-            temp_train_df.insert(0, 'Test point', str(test_point))
-            temp_train_df.insert(1, 'Dataset', 'Training')
-            train_df = train_df.append(temp_train_df)
-            
-            if exists(validation_csv_file):
-                temp_validation_df = pd.read_csv(validation_csv_file)
-                temp_validation_df.insert(0, 'Test point', str(test_point))
-                temp_validation_df.insert(1, 'Dataset', 'Validation')
-                validation_df = validation_df.append(temp_validation_df)
-            else:
-                validation_df = None
-
-        try:
-            plot_table(train_df,validation_df,test_df,test_type,performance_benchmark,test_point_number)
-        except Exception:
-            print('There is a problem in creating the results table.')
-        
-
-
-# plot the performance bars for training and validation
-def performance_bar_plot(forecast_horizon,test_type,performance_benchmark):
-
-    validation_dir = './performance/validation process/'
-    testing_dir = './performance/test process/'
-    if not exists('./plots/'):
-        os.makedirs('./plots/')
-
-    path = validation_dir
-    files = [f for f in listdir(path) if isfile(join(path, f))]
-    prefix = 'training performance report forecast horizon = {0}, test-point #'.format(forecast_horizon)
-    files = [file for file in files if file.startswith(prefix)]
-    file_test_points = [int(file.split('test-point #')[1][:-4]) for file in files]
-    file_test_points.sort()
-
-    if test_type == 'whole-as-one':
-        
-        train_csv_file = validation_dir + 'training performance report forecast horizon = {0}.csv'.format(forecast_horizon)
-        validation_csv_file = validation_dir + 'validation performance report forecast horizon = {0}.csv'.format(forecast_horizon)
-        
-        train_df = pd.read_csv(train_csv_file)
-        train_df.insert(0, 'Dataset', 'Training')
-        
-        if exists(validation_csv_file):
-            validation_df = pd.read_csv(validation_csv_file)
-            validation_df.insert(0, 'Dataset', 'Validation')
-        else: 
-            validation_df = None
-            
-        try:
-            plot_bar(train_df,validation_df,test_type,performance_benchmark,None)
-        except Exception:
-            print('There is a problem in plotting the results.')
-
-    elif test_type == 'one-by-one':
-
-        test_point_number = len(file_test_points)    
-        test_df = pd.read_csv(testing_dir + 'test performance report forecast horizon = {0}.csv'.format(forecast_horizon))
-        test_df.insert(0, 'Test point', 'Overall')
-        test_df.insert(1, 'Dataset', 'Test')
-
-
-        train_df = pd.DataFrame()
-        validation_df = pd.DataFrame()
-        for test_point in range(1,test_point_number+1):
-            
-            tp_number = file_test_points[test_point-1]
-            
-            train_csv_file = validation_dir + 'training performance report forecast horizon = {0}, test-point #{1}.csv'.format(forecast_horizon,tp_number)
-            validation_csv_file = validation_dir + 'validation performance report forecast horizon = {0}, test-point #{1}.csv'.format(forecast_horizon,tp_number)
-
-            temp_train_df = pd.read_csv(train_csv_file)
-            temp_train_df.insert(0, 'Test point', test_point)
-            temp_train_df.insert(1, 'Dataset', 'Training')
-            train_df = train_df.append(temp_train_df)
-            
-            if exists(validation_csv_file):
-                temp_validation_df = pd.read_csv(validation_csv_file)
-                temp_validation_df.insert(0, 'Test point', test_point)
-                temp_validation_df.insert(1, 'Dataset', 'Validation')
-                validation_df = validation_df.append(temp_validation_df)
-            else:
-                validation_df = None
-
-        try:
-            plot_bar(train_df,validation_df,test_type,performance_benchmark,test_point_number)
-        except Exception:
+import warnings
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    import numpy as np
+    import pandas as pd
+    import matplotlib.pyplot as plt
+    from os import listdir
+    from os.path import isfile, join, exists
+    import datetime
+    from datetime import timedelta
+    from dateutil.relativedelta import relativedelta
+    import random
+    import sys
+    import os
+    import matplotlib as mpl
+    from matplotlib.backends.backend_pdf import PdfPages
+    import matplotlib.patches as mpatches
+    from matplotlib import colors as mcolors
+    import matplotlib.ticker as ticker
+
+warnings.filterwarnings("ignore")
+
+
+# merge the cells in matplotlib table
+def mergecells(table, cells, selected_text = 'L'):
+    if len(cells)<=1:
+        return
+    cells_array = [np.asarray(c) for c in cells]
+    h = np.array([cells_array[i+1][0] - cells_array[i][0] for i in range(len(cells_array) - 1)])
+    v = np.array([cells_array[i+1][1] - cells_array[i][1] for i in range(len(cells_array) - 1)])
+    bold = False
+
+    # if it's a horizontal merge, all values for `h` are 0
+    if not np.any(h):
+        # sort by horizontal coord
+        cells = np.array(sorted(list(cells), key=lambda v: v[1]))
+        edges = ['BTL'] + ['BT' for i in range(len(cells) - 2)] + ['BTR']
+    elif not np.any(v):
+        cells = np.array(sorted(list(cells), key=lambda h: h[0]))
+        edges = ['TRL'] + ['RL' for i in range(len(cells) - 2)] + ['BRL']
+    else:
+        raise ValueError("Only horizontal and vertical merges allowed")
+
+    for cell, e in zip(cells, edges):
+        table[cell[0], cell[1]].visible_edges = e
+        
+    txts = [table[cell[0], cell[1]].get_text() for cell in cells]
+    tpos = [np.array(t.get_position()) for t in txts]
+    
+    if any([txt.get_weight() == 'bold' for txt in txts]):
+        bold = True
+        
+    if selected_text == 'L':
+        # transpose the text of the left cell
+        trans = (tpos[-1] - tpos[0])/2
+        # didn't had to check for ha because I only want ha='center'
+        txts[0].set_transform(mpl.transforms.Affine2D().translate(*trans))
+        if bold == True:
+            txts[0].set_weight('bold')
+        for txt in txts[1:]:
+            txt.set_visible(False)
+        
+    elif selected_text == 'R':
+        # transpose the text of the right cell
+        trans = (tpos[0] - tpos[-1])/2
+        # didn't had to check for ha because I only want ha='center'
+        txts[-1].set_transform(mpl.transforms.Affine2D().translate(*trans))
+        if bold == True:
+            txts[-1].set_weight('bold')
+        for txt in txts[:-1]:
+            txt.set_visible(False)
+        
+# find the consecutive cells with same values and merge them
+def merge_same_values(row_number,column,offset,the_table):
+    values = [the_table.get_celld()[(i,column)].get_text().get_text() for i in range(offset,row_number+1)]
+    current_value = values[0]
+    merge_list = []
+    for index,value in enumerate(values):
+        # model name of test points must not be merged with previous rows
+        if column == 2 and (the_table.get_celld()[(index+offset,1)].get_text().get_text() == 'Test'):
+            mergecells(the_table, merge_list)
+            if index+offset+1 < row_number:
+                current_value = the_table.get_celld()[(index+offset+1,column)].get_text().get_text()
+                merge_list = []
+            
+        elif value == current_value:
+            merge_list = merge_list+[(index+offset,column)]
+                
+        else:
+            current_value = value
+            mergecells(the_table, merge_list)
+            merge_list = [(index+offset,column)]
+            
+    mergecells(the_table, merge_list)
+    return the_table
+
+# find the consecutive cells with same values and colours them with the same color
+def color_same_values(row_number,column_number,column,offset,the_table,color_dict):
+    
+    colors = ['#008e99','#424242','#ba4c4d','#858585','#acc269','#7255b2']
+    
+    # find cells with same text
+    values = [the_table.get_celld()[(i,column)].get_text().get_text() for i in range(offset,row_number+1)]
+    models = np.unique(values)
+    if len(models) == 1 :
+        color_dict = {models[0]:'#000000'}
+        
+    current_value = values[0]
+    for index,value in enumerate(values):
+        if value == current_value:
+            for col in range(column,column_number):
+                the_table.get_celld()[(index+offset,col)].get_text().set_color(color_dict[value])
+        else:
+            current_value = value
+            for col in range(column,column_number):
+                the_table.get_celld()[(index+offset,col)].get_text().set_color(color_dict[value])
+            
+    return the_table
+
+# prepare input df by counting features and rounding performance values
+def prepare_df(df,base_columns,measure_names,performance_benchmark,test_type,plot_type):
+    
+    if test_type == 'whole-as-one':
+        unique_columns = ['model name', 'history length']
+    if test_type == 'one-by-one':
+        unique_columns = ['Test point','model name','history length']
+        
+    df['feature or covariate set'] = df['feature or covariate set'].apply(lambda x:len(x.split(',')))
+    if performance_benchmark in ['MAE', 'MAPE', 'MASE', 'MSE', 'AIC', 'BIC', 'likelihood']:
+        optimum_performance_df = df.groupby(unique_columns)[[performance_benchmark]].min().reset_index().rename(columns = {performance_benchmark:'best '+performance_benchmark})
+    else:
+        optimum_performance_df = df.groupby(unique_columns)[[performance_benchmark]].max().reset_index().rename(columns = {performance_benchmark:'best '+performance_benchmark})
+    df = pd.merge(df,optimum_performance_df)
+    df = df[df[performance_benchmark] == df['best '+performance_benchmark]].drop_duplicates(subset = unique_columns)
+    df = df[base_columns + measure_names]
+        
+    return df
+
+def table_add(table, df, best_loc, measure_names, performance_benchmark, best_loc_flag):
+    
+    if best_loc_flag == True:
+        df = df.reset_index(drop = True)
+        df[performance_benchmark] = df[performance_benchmark].astype(float)
+        
+        if performance_benchmark in ['MAE', 'MAPE', 'MASE', 'MSE', 'AIC', 'BIC', 'likelihood']:
+            optimum_performance = df[performance_benchmark].min()
+        else:
+            optimum_performance = df[performance_benchmark].max()
+            
+        df_best_loc = list(df[df[performance_benchmark] == optimum_performance].index)[-1]
+        best_loc = best_loc + [df_best_loc + len(table)+1]
+    
+    for measure in measure_names:
+        df[measure] = df[measure].apply(lambda x:np.round(x,2))
+        df.loc[df[measure]>99999,measure] = df.loc[df[measure]>99999,measure].apply(lambda x:'{:.2E}'.format(x))
+    table = table + df.values.tolist()
+    
+    return table, best_loc
+
+# make tables and save into pdf
+def plot_table(train_df,validation_df,test_df,test_type,performance_benchmark,test_point_number):
+    
+    if test_type == 'whole-as-one':
+        base_columns = ['Dataset', 'model name', 'history length', 'feature or covariate set']
+    if test_type == 'one-by-one':
+        base_columns = ['Test point', 'Dataset', 'model name', 'history length', 'feature or covariate set']
+    measure_names = list(filter(lambda x: x not in base_columns, test_df.columns))
+    models_number = len(train_df['model name'].unique())
+    max_history = len(train_df['history length'].unique())
+    
+    models = train_df['model name'].unique()
+    colors = ['#008e99','#424242','#ba4c4d','#858585','#acc269','#7255b2']
+    color_list = colors * ((len(models)//6)+1) 
+    color_dict = {model:color_list[i] for i , model in enumerate(models)}
+
+    test_df = prepare_df(test_df,base_columns,measure_names,performance_benchmark,test_type,'table')
+    train_df = prepare_df(train_df,base_columns,measure_names,performance_benchmark,test_type,'table')
+    if validation_df is not None:
+        validation_df = prepare_df(validation_df,base_columns,measure_names,performance_benchmark,test_type,'table')
+    
+    # the location of best obtained results for each set, in the table 
+    best_loc = []
+    table = []
+    
+    if test_type == 'whole-as-one':
+        table, best_loc = table_add(table, test_df, best_loc, measure_names, performance_benchmark, True)
+        if validation_df is not None:
+            table, best_loc = table_add(table, validation_df, best_loc, measure_names, performance_benchmark, True)
+        table, best_loc = table_add(table, train_df, best_loc, measure_names, performance_benchmark, True)
+        colWidths = [0.15, 0.15, 0.17, 0.15] + [0.15]*len(measure_names)
+        for index,measure_name in enumerate(measure_names):
+            if measure_name in ['R2_score', 'likelihood']:
+                colWidths[index+4] = 0.17
+        row_number = len(table)
+
+    if test_type == 'one-by-one':
+        table, best_loc = table_add(table, test_df[test_df['Test point'] == 'All test points'], best_loc, measure_names, performance_benchmark, False)
+        table = table + [['1','Test','Model','History length','#Features'] + measure_names]
+        for test_point in range(1,test_point_number+1):
+            table, best_loc = table_add(table, test_df[test_df['Test point'] == str(test_point)], best_loc, measure_names, performance_benchmark, True)
+            if validation_df is not None:
+                table, best_loc = table_add(table, validation_df[validation_df['Test point'] == str(test_point)], best_loc, measure_names, performance_benchmark, True)
+            table, best_loc = table_add(table, train_df[train_df['Test point'] == str(test_point)], best_loc, measure_names, performance_benchmark, True)
+        colWidths = [0.15, 0.15, 0.15, 0.17, 0.15] + [0.15]*len(measure_names)
+        for index,measure_name in enumerate(measure_names):
+            if measure_name in ['R2_score', 'likelihood']:
+                colWidths[index+5] = 0.17
+        headerColWidths = [0.15, 0.15] + [np.sum(colWidths[2:])/len(measure_names)]*len(measure_names)
+        row_number = len(table)
+        
+    
+    # calculate number of pages needed
+    npages = row_number // 300
+    if row_number % 300 > 0:
+        npages += 1
+    
+
+    pdf = PdfPages('./plots/performance summary.pdf')
+    
+    for page in range(npages):
+        fig = plt.figure()
+        plt.tight_layout()
+        ax = fig.gca()
+        ax.axis('tight')
+        ax.axis('off')
+        temp_table = table[page*300:(page+1)*300]
+        page_best_locs = [index - (page*300) for index in best_loc if index in range(page*300,(page+1)*300)]
+        
+        ylim = 0.08278145695364238*(len(temp_table))
+        xlim = np.sum(colWidths) + 0.7
+        bbox = (0,0,xlim,ylim)
+        
+        if test_type == 'whole-as-one':
+            colLabels = ['Dataset','Model','History length','#Features'] + measure_names
+
+        
+        if test_type == 'one-by-one' and page == 0:
+            colLabels = ['Test point', 'Dataset','','',''] + measure_names
+        elif test_type == 'one-by-one' and page > 0:
+            colLabels = ['Test point', 'Dataset','Model','History length','#Features'] + measure_names
+        
+        
+        if test_type == 'one-by-one' and page == 0:
+            # make a table to represent header and test set results with different column number
+            headerdata = [[temp_table[0][i] for i in [0,1]+[i+5 for i in range(len(measure_names))]]] + [['']*len(headerColWidths)]*(len(temp_table)-1)
+            headertable = ax.table(cellText=headerdata, colLabels=['Test point', 'Dataset'] + measure_names, 
+                                   colWidths=headerColWidths, loc='center', colColours = ['lightgray']*len(headerColWidths),
+                                   cellLoc='center', edges = 'open', bbox = bbox)
+            for i in range(len(headerColWidths)):
+                headertable.get_celld()[(0,i)].visible_edges = 'closed'
+                headertable.get_celld()[(0,i)].set_text_props(weight='bold')
+                headertable.get_celld()[(1,i)].visible_edges = 'closed'
+            headertable.auto_set_font_size(False)
+            headertable.set_fontsize(9)
+            headertable.scale(1.5, 1.5)
+            fig.canvas.draw()
+        
+        
+        the_table = ax.table(cellText=temp_table, colLabels=colLabels, colWidths=colWidths, loc='center', cellLoc='center', bbox = bbox)
+        the_table.auto_set_font_size(False)
+        the_table.set_fontsize(9)
+        the_table.scale(1.5, 1.5)
+        fig.canvas.draw()
+
+        if test_type == 'whole-as-one':
+            
+            for i in range(1,len(colLabels)):
+                for j in page_best_locs:
+                    the_table.get_celld()[(j,i)].set_text_props(weight='bold')
+                    
+            # merge the cells containing dataset name in first column
+            offset = 2 if page == 0 else 1
+            the_table = merge_same_values(row_number = len(temp_table),
+                                  column = 0, offset = offset, the_table = the_table)
+            # merge the cells containing model name in second column 
+            offset = 2 if page == 0 else 1
+            the_table = color_same_values(row_number = len(temp_table), column_number = len(colLabels),
+                                  column = 1, offset = offset, the_table = the_table, color_dict = color_dict)
+            the_table = merge_same_values(row_number = len(temp_table),
+                                  column = 1, offset = offset, the_table = the_table)
+            
+            
+        if test_type == 'one-by-one':
+            
+            for i in range(2,len(colLabels)):
+                for j in page_best_locs:
+                    the_table.get_celld()[(j,i)].set_text_props(weight='bold')
+                    
+            # merge the cells containing test point number in first column
+            offset = 2 if page == 0 else 1
+            the_table = merge_same_values(row_number = len(temp_table),
+                                          column = 0, offset = offset, the_table = the_table)
+            # merge the cells containing dataset name in second column
+            the_table = merge_same_values(row_number = len(temp_table),
+                                          column = 1, offset = offset, the_table = the_table)
+            # merge the cells containing model name in third column
+            offset = 3 if page == 0 else 1
+            the_table = color_same_values(row_number = len(temp_table), column_number = len(colLabels),
+                                  column = 2, offset = offset, the_table = the_table, color_dict = color_dict)
+            the_table = merge_same_values(row_number = len(temp_table),
+                                          column = 2, offset = offset, the_table = the_table)
+        
+        # colour header
+        for i in range(len(colLabels)):
+            the_table.get_celld()[(0,i)].set_facecolor('lightgray')
+            the_table.get_celld()[(0,i)].set_text_props(weight='bold')
+            
+            if (page == 0) and (test_type == 'one-by-one' and i>1):
+                the_table.get_celld()[(2,i)].set_facecolor('lightgray')#'#40466e'
+                the_table.get_celld()[(2,i)].set_text_props(weight='bold')#, color='w')
+                
+        
+        
+        # set the_table header invisible to make header table visible
+        if test_type == 'one-by-one' and page == 0:
+            for i in range(len(colLabels)):
+                the_table.get_celld()[(0,i)].set_alpha(0)
+                the_table.get_celld()[(1,i)].set_alpha(0)
+                if i>=2:
+                    the_table.get_celld()[(0,i)].get_text().set_visible(False)
+                    the_table.get_celld()[(1,i)].get_text().set_visible(False)
+                
+            
+        
+        pdf.savefig(fig , dpi=300, bbox_inches='tight', pad_inches=1)
+        plt.close()
+
+    pdf.close()
+    
+# make barplots and save into pdf
+
+def plot_bar(train_df,validation_df,test_type,performance_benchmark,test_point_number):
+    
+    if test_type == 'whole-as-one':
+        base_columns = ['Dataset', 'model name', 'history length', 'feature or covariate set']
+    if test_type == 'one-by-one':
+        base_columns = ['Test point', 'Dataset', 'model name', 'history length', 'feature or covariate set']
+    measure_names = list(filter(lambda x: x not in base_columns, train_df.columns))
+    models = train_df['model name'].unique()
+    models_number = len(models)
+    max_history = len(train_df['history length'].unique())
+    
+    colors = ['#008e99','#424242','#ba4c4d','#858585','#acc269','#7255b2']
+    color_list = colors * ((len(models)//6)+1) 
+    color_dict = {model:color_list[i] for i , model in enumerate(models)}
+        
+    train_df = prepare_df(train_df,base_columns,measure_names,performance_benchmark,test_type,'bar')
+    if validation_df is not None:
+        validation_df = prepare_df(validation_df,base_columns,measure_names,performance_benchmark,test_type,'bar')
+    
+    if test_type == 'whole-as-one':
+        test_point_number = 1
+    
+    models_per_plot = 6
+    # calculate number of pages needed
+    npages = models_number // (models_per_plot*5)
+    if models_number % (models_per_plot*5) > 0:
+        npages += 1
+    
+    barWidth = 0.015 if validation_df is not None else 0.030
+    pos = 0.195*np.arange(max_history)
+    
+        
+    # initialize pdf
+    pdf = PdfPages('./plots/performance bar plots.pdf')
+    
+    for test_point in range(1,test_point_number+1):
+        
+        mpl.rcParams.update({'font.size': 12})
+        
+        for page in range(npages):
+            
+            current_models = train_df['model name'].unique()[page*5*models_per_plot:(page+1)*5*models_per_plot]
+            num_subplots = (len(current_models)//models_per_plot)+int()
+            if len(current_models)%models_per_plot > 0:
+                num_subplots += 1
+                
+            fig, axes = plt.subplots(num_subplots,1)
+            if num_subplots == 1:
+                axes = np.array([axes])
+            
+            if test_type == 'one-by-one':
+                plt.suptitle('Test point number {0}'.format(test_point), fontweight='bold', fontsize='16', y=1.05)
+                
+            for subplot in range(num_subplots):
+                
+                subplot_models = current_models[subplot*models_per_plot:(subplot+1)*models_per_plot]
+                ax = axes[subplot]
+                ax.grid(axis = 'y', linestyle = '--')
+                ax.set_axisbelow(True)
+                log_flag = False
+                    
+                for index,model in enumerate(subplot_models):
+
+                    # Set position of bar on X axis
+                    if validation_df is not None:
+                        current_train_pos=[x + (2*index)*barWidth for x in pos]
+                        current_validation_pos=[x + (2*index+1)*barWidth for x in pos]
+                    else:
+                        current_train_pos=[x + index*barWidth for x in pos]
+
+                    if test_type == 'whole-as-one':
+                        train_performance = list(train_df.loc[train_df['model name'] == model,performance_benchmark])
+                        if validation_df is not None:
+                            validation_performance = list(validation_df.loc[validation_df['model name'] == model,performance_benchmark])
+
+                    if test_type == 'one-by-one':
+                        train_performance = list(train_df.loc[(train_df['Test point'] == test_point)&(train_df['model name'] == model),performance_benchmark])
+                        if validation_df is not None:
+                            validation_performance = list(validation_df.loc[(validation_df['Test point'] == test_point)&(validation_df['model name'] == model),performance_benchmark])
+                    
+                    if validation_df is not None:
+                        performance_list = list(train_performance)+list(validation_performance)
+                    else:
+                        performance_list = list(train_performance)
+                    if max(performance_list)-min(performance_list)>10000 and min(performance_list)>=0:
+                        log_flag = True
+
+                    # Make the plot
+                    if validation_df is not None:
+                        ax.bar(current_train_pos, train_performance, color=color_dict[model], width=barWidth, edgecolor='white',hatch='//////')
+                        ax.bar(current_validation_pos, validation_performance, color=color_dict[model], width=barWidth, edgecolor='white', label=model)
+                    else:
+                        ax.bar(current_train_pos, train_performance, color=color_dict[model], width=barWidth, edgecolor='white', label=model)
+                    
+
+                ax.set_ylabel(performance_benchmark,fontweight='bold')
+                if validation_df is not None:
+                    ax.set_xticks(ticks = [r + (len(subplot_models)-0.5)*barWidth for r in pos])
+                else:
+                    ax.set_xticks(ticks = [r + ((len(subplot_models)/2)-0.5)*barWidth for r in pos])
+                ax.set_xticklabels(labels = [str(history) for history in range (1,max_history+1)])
+                if validation_df is not None:
+                    ax.set_title('The predictive models performance', fontweight='bold')
+                else:
+                    ax.set_title('The predictive models performance on\nthe training dataset', fontweight='bold')
+                    
+                if subplot == 0 and validation_df is not None:
+                    train_patch = mpatches.Patch(edgecolor='gray', facecolor='w', label='Training', hatch='//////')
+                    validation_patch = mpatches.Patch(color='gray', label='Validation')
+                    leg1 = ax.legend(handles=[train_patch,validation_patch], loc='upper left', bbox_to_anchor=(1, 1))
+                    ax.add_artist(leg1)
+
+                # Create legend & Show graphic
+                ax.legend(loc='lower left', bbox_to_anchor=(1, 0))
+                
+                
+                y_min = min(ax.get_yticks())
+                y_max = max(ax.get_yticks())
+                if y_max - y_min <= 1:
+                    step = 0.1
+                    ax.set_yticks(np.arange(y_min, y_max, step))
+                else:
+                    step = (y_max-y_min)/10
+                    ax.set_yticks(np.arange(y_min, y_max, step))
+                    
+                if log_flag == True:
+                    ax.set_yscale('log')
+                
+            
+            plt.xlabel('History Length', fontweight='bold')
+            if max_history>5:
+                plt.gcf().set_size_inches(plt.gcf().get_size_inches()[0]*(max_history/5), plt.gcf().get_size_inches()[1]*num_subplots)
+            else:
+                plt.gcf().set_size_inches(plt.gcf().get_size_inches()[0]*(1.5), plt.gcf().get_size_inches()[1]*num_subplots)
+                
+            plt.tight_layout()
+            pdf.savefig(fig , dpi=300, bbox_inches='tight', pad_inches=1)
+            plt.close()
+            
+    pdf.close()
+
+# save summary of performance reports
+
+def performance_summary(forecast_horizon,test_type,performance_benchmark):
+    
+    validation_dir = './performance/validation process/'
+    testing_dir = './performance/test process/'
+    if not exists('./plots/'):
+        os.makedirs('./plots/')
+
+
+    path = validation_dir
+    files = [f for f in listdir(path) if isfile(join(path, f))]
+    prefix = 'training performance report forecast horizon = {0}, test-point #'.format(forecast_horizon)
+    files = [file for file in files if file.startswith(prefix)]
+    file_test_points = [int(file.split('test-point #')[1][:-4]) for file in files]
+    file_test_points.sort()
+
+    if test_type == 'whole-as-one':
+        
+        test_csv_file = testing_dir + 'test performance report forecast horizon = {0}.csv'.format(forecast_horizon)
+        train_csv_file = validation_dir + 'training performance report forecast horizon = {0}.csv'.format(forecast_horizon)
+        validation_csv_file = validation_dir + 'validation performance report forecast horizon = {0}.csv'.format(forecast_horizon)
+
+        test_df = pd.read_csv(test_csv_file)
+        test_df.insert(0, 'Dataset', 'Test')
+
+        train_df = pd.read_csv(train_csv_file)
+        train_df.insert(0, 'Dataset', 'Training')
+        
+        if exists(validation_csv_file):
+            validation_df = pd.read_csv(validation_csv_file)
+            validation_df.insert(0, 'Dataset', 'Validation')
+        else:
+            validation_df = None
+        
+        try:
+            plot_table(train_df,validation_df,test_df,test_type,performance_benchmark,None)
+        except Exception:
+            print('There is a problem in creating the results table.')
+
+    elif test_type == 'one-by-one':
+
+        test_point_number = len(file_test_points)    
+        test_df = pd.read_csv(testing_dir + 'test performance report forecast horizon = {0}.csv'.format(forecast_horizon))
+        test_df = test_df.rename(columns = {'test point':'Test point'})
+        test_df.insert(1, 'Dataset', 'Test')
+
+
+        train_df = pd.DataFrame()
+        validation_df = pd.DataFrame()
+        for test_point in range(1,test_point_number+1):
+
+            tp_number = file_test_points[test_point-1]
+            
+            train_csv_file = validation_dir + 'training performance report forecast horizon = {0}, test-point #{1}.csv'.format(forecast_horizon,tp_number)
+            validation_csv_file = validation_dir + 'validation performance report forecast horizon = {0}, test-point #{1}.csv'.format(forecast_horizon,tp_number)
+
+            temp_train_df = pd.read_csv(train_csv_file)
+            temp_train_df.insert(0, 'Test point', str(test_point))
+            temp_train_df.insert(1, 'Dataset', 'Training')
+            train_df = pd.concat([train_df,temp_train_df], ignore_index=True)
+            
+            if exists(validation_csv_file):
+                temp_validation_df = pd.read_csv(validation_csv_file)
+                temp_validation_df.insert(0, 'Test point', str(test_point))
+                temp_validation_df.insert(1, 'Dataset', 'Validation')
+                validation_df = pd.concat([validation_df,temp_validation_df], ignore_index=True)
+            else:
+                validation_df = None
+
+        try:
+            plot_table(train_df,validation_df,test_df,test_type,performance_benchmark,test_point_number)
+        except Exception:
+            print('There is a problem in creating the results table.')
+        
+
+
+# plot the performance bars for training and validation
+def performance_bar_plot(forecast_horizon,test_type,performance_benchmark):
+
+    validation_dir = './performance/validation process/'
+    testing_dir = './performance/test process/'
+    if not exists('./plots/'):
+        os.makedirs('./plots/')
+
+    path = validation_dir
+    files = [f for f in listdir(path) if isfile(join(path, f))]
+    prefix = 'training performance report forecast horizon = {0}, test-point #'.format(forecast_horizon)
+    files = [file for file in files if file.startswith(prefix)]
+    file_test_points = [int(file.split('test-point #')[1][:-4]) for file in files]
+    file_test_points.sort()
+
+    if test_type == 'whole-as-one':
+        
+        train_csv_file = validation_dir + 'training performance report forecast horizon = {0}.csv'.format(forecast_horizon)
+        validation_csv_file = validation_dir + 'validation performance report forecast horizon = {0}.csv'.format(forecast_horizon)
+        
+        train_df = pd.read_csv(train_csv_file)
+        train_df.insert(0, 'Dataset', 'Training')
+        
+        if exists(validation_csv_file):
+            validation_df = pd.read_csv(validation_csv_file)
+            validation_df.insert(0, 'Dataset', 'Validation')
+        else: 
+            validation_df = None
+            
+        try:
+            plot_bar(train_df,validation_df,test_type,performance_benchmark,None)
+        except Exception:
+            print('There is a problem in plotting the results.')
+
+    elif test_type == 'one-by-one':
+
+        test_point_number = len(file_test_points)    
+        test_df = pd.read_csv(testing_dir + 'test performance report forecast horizon = {0}.csv'.format(forecast_horizon))
+        test_df.insert(0, 'Test point', 'Overall')
+        test_df.insert(1, 'Dataset', 'Test')
+
+
+        train_df = pd.DataFrame()
+        validation_df = pd.DataFrame()
+        for test_point in range(1,test_point_number+1):
+            
+            tp_number = file_test_points[test_point-1]
+            
+            train_csv_file = validation_dir + 'training performance report forecast horizon = {0}, test-point #{1}.csv'.format(forecast_horizon,tp_number)
+            validation_csv_file = validation_dir + 'validation performance report forecast horizon = {0}, test-point #{1}.csv'.format(forecast_horizon,tp_number)
+
+            temp_train_df = pd.read_csv(train_csv_file)
+            temp_train_df.insert(0, 'Test point', test_point)
+            temp_train_df.insert(1, 'Dataset', 'Training')
+            train_df = pd.concat([train_df,temp_train_df],ignore_index=True)
+            
+            if exists(validation_csv_file):
+                temp_validation_df = pd.read_csv(validation_csv_file)
+                temp_validation_df.insert(0, 'Test point', test_point)
+                temp_validation_df.insert(1, 'Dataset', 'Validation')
+                validation_df = pd.concat([validation_df,temp_validation_df],ignore_index=True)
+            else:
+                validation_df = None
+
+        try:
+            plot_bar(train_df,validation_df,test_type,performance_benchmark,test_point_number)
+        except Exception:
             print('There is a problem in plotting the results.')
```

### Comparing `stpredict-0.0.8/src/stpredict/plot_prediction.py` & `stpredict-0.0.9/src/stpredict/plot_prediction.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,24 +139,26 @@
                 validation_df = validation_df[validation_df['model name'] == selected_model]
                 validation_df = validation_df.assign(sort = 'validation')
             else: 
                 validation_df = pd.DataFrame(columns = train_df.columns)
             gap_df = data.rename(columns = {'Normal target':'real'})
             gap_df = gap_df.assign(prediction = np.NaN)
             gap_df = gap_df.assign(sort = 'gap')
-            gap_df = gap_df[(gap_df['temporal id'] < test_df['temporal id'].min()) & (gap_df['temporal id'] > train_df.append(validation_df)['temporal id'].max())]
-            all_df = train_df[needed_columns].append(validation_df[needed_columns]).append(gap_df[needed_columns]).append(test_df[needed_columns])
+            gap_df = gap_df[(gap_df['temporal id'] < test_df['temporal id'].min()) & (gap_df['temporal id'] > pd.concat([train_df,validation_df],ignore_index = True)['temporal id'].max())]
+            all_df = pd.concat([train_df[needed_columns],validation_df[needed_columns]],ignore_index = True)
+            all_df = pd.concat([all_df,gap_df[needed_columns]],ignore_index = True)
+            all_df = pd.concat([all_df,test_df[needed_columns]],ignore_index = True)
             
         elif plot_type == 'future':
             future_df = pd.read_csv(future_csv_file)
             future_df = future_df.assign(sort = 'future')
             train_df = data.rename(columns = {'Normal target':'real'})
             train_df = train_df.assign(prediction = np.NaN)
             train_df = train_df.assign(sort = 'train')
-            all_df = train_df[needed_columns].append(future_df[needed_columns])
+            all_df = pd.concat([train_df[needed_columns],future_df[needed_columns]],ignore_index = True)
         
         try:
             create_plot(df = all_df, forecast_horizon = forecast_horizon, granularity = granularity, spatial_ids = spatial_ids, 
                         save_address = './plots/', plot_type = plot_type, test_point = None)
         except Exception as e:
             raise Exception('There is a problem in plotting predictions:\n'+str(e))
 
@@ -186,30 +188,32 @@
                     validation_df = validation_df[validation_df['model name'] == selected_model]
                     validation_df = validation_df.assign(sort = 'validation')
                 else: 
                     validation_df = pd.DataFrame(columns = train_df.columns)
                 gap_df = data.rename(columns = {'Normal target':'real'})
                 gap_df = gap_df.assign(prediction = np.NaN)
                 gap_df = gap_df.assign(sort = 'gap')
-                gap_df = gap_df[(gap_df['temporal id'] < test_df['temporal id'].min()) & (gap_df['temporal id'] > train_df.append(validation_df)['temporal id'].max())]
-                all_df = train_df[needed_columns].append(validation_df[needed_columns]).append(gap_df[needed_columns]).append(test_df[needed_columns])
+                gap_df = gap_df[(gap_df['temporal id'] < test_df['temporal id'].min()) & (gap_df['temporal id'] > pd.concat([train_df,validation_df],ignore_index = True)['temporal id'].max())]
+                all_df = pd.concat([train_df[needed_columns],validation_df[needed_columns]],ignore_index = True)
+                all_df = pd.concat([all_df,gap_df[needed_columns]],ignore_index = True)
+                all_df = pd.concat([all_df,test_df[needed_columns]],ignore_index = True)
 
                 try:
                     create_plot(df = all_df, forecast_horizon = forecast_horizon, granularity = granularity, spatial_ids = spatial_ids, 
                                 save_address = './plots/', plot_type = plot_type, test_point = test_point)
                 except Exception as e:
                     print('There is a problem in plotting predictions.')
         
         elif plot_type == 'future':
             
             future_df = pd.read_csv(future_dir + 'future prediction forecast horizon = {0}.csv'.format(forecast_horizon))
             future_df = future_df.assign(sort = 'future')
             train_df = data.rename(columns = {'Normal target':'real'})
             train_df = train_df.assign(prediction = np.NaN)
             train_df = train_df.assign(sort = 'train')
-            all_df = train_df[needed_columns].append(future_df[needed_columns])
+            all_df = pd.concat([train_df[needed_columns], future_df[needed_columns]], ignore_index = True)
         
             try:
                 create_plot(df = all_df, forecast_horizon = forecast_horizon, granularity = granularity, spatial_ids = spatial_ids, 
                             save_address = './plots/', plot_type = plot_type, test_point = None)
             except Exception:
                 print('There is a problem in plotting predictions.')
```

### Comparing `stpredict-0.0.8/src/stpredict/predict_func.py` & `stpredict-0.0.9/src/stpredict/predict_func.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/predict_future.py` & `stpredict-0.0.9/src/stpredict/predict_future.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     
     # find labels for classification problem
     if labels == None:
         if model_type == 'regression':    # just an empty list
             labels = []
         elif model_type == 'classification':    # unique values in 'Target' column of data
             labels = training_data.Target.unique()
-            labels.sort()
+    labels.sort()
             
     training_data = select_features(data=training_data.copy(),
                                     ordered_covariates_or_features=feature_or_covariate_set)
     testing_data = select_features(data=testing_data.copy(),
                                    ordered_covariates_or_features=feature_or_covariate_set)
 
     futuristic_features = [column_name
@@ -162,19 +162,20 @@
                      "some futuristic features have null values in the input 'future_data'.")
 
     scaled_training_data, scaled_testing_data = data_scaling(train_data=training_data.copy(),
                                                              test_data=testing_data.copy(),
                                                              feature_scaler=feature_scaler,
                                                              target_scaler=target_scaler)
 
-    scaled_training_data.drop(NON_FEATURE_COLUMNS_NAMES, axis=1, inplace=True)
+    # scaled_training_data.drop(NON_FEATURE_COLUMNS_NAMES, axis=1, inplace=True)
     scaled_training_data.drop(NORMAL_TARGET_COLUMN_NAME, axis=1, inplace=True)
-    scaled_testing_data.drop(NON_FEATURE_COLUMNS_NAMES, axis=1, inplace=True)
+    # scaled_testing_data.drop(NON_FEATURE_COLUMNS_NAMES, axis=1, inplace=True)
     scaled_testing_data.drop(NORMAL_TARGET_COLUMN_NAME, axis=1, inplace=True)
-
+    
+    
     scaled_training_predictions, scaled_testing_predictions, trained_model = \
         train_evaluate(training_data=scaled_training_data,
                        validation_data=scaled_testing_data,
                        model_type=model_type,
                        model=model,
                        model_parameters=model_parameters,
                        labels=labels,
```

### Comparing `stpredict-0.0.8/src/stpredict/preprocess.py` & `stpredict-0.0.9/src/stpredict/preprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,2068 +1,2369 @@
-import warnings
-
-with warnings.catch_warnings():
-    warnings.simplefilter("ignore")
-    import pandas as pd
-    import numpy as np
-    import sys
-    import datetime
-    from sklearn.impute import KNNImputer
-    import matplotlib.pyplot as plt
-    import calendar
-
-
-###################### renaming the columns to formal format
-
-def rename_columns(data,column_identifier, mode = 'formalize', keep_target = False):
-        
-    if type(column_identifier) == dict:
-        if any([key not in list(column_identifier.keys()) for key in ['target','temporal covariates']]):
-            raise ValueError("The target and temporal covariates are not specified in column_identifier.")
-        if mode == 'formalize':
-            for key, value in column_identifier.items():
-                if key not in ['temporal covariates','spatial covariates']:
-                    if (key == 'target') and (value in column_identifier['temporal covariates']) and (value in data.columns):
-                        if 'target' not in data.columns:
-                            data.loc[:,('target')] = list(data[value])
-                    else:
-                        data.rename(columns = {value:key}, inplace = True)
-        elif mode == 'deformalize':
-            for key, value in column_identifier.items():
-                if key not in ['temporal covariates','spatial covariates']:
-                    if (key == 'target') and (value in column_identifier['temporal covariates']) and (value in data.columns):
-                        if keep_target == False:
-                          data = data.drop(['target'],axis = 1)
-                    else:
-                        data.rename(columns = {key:value}, inplace = True)
-            
-    elif column_identifier is not None:
-        raise TypeError("The column_identifier must be of type dict")
-
-    return data
-
-###################### check validity of input data
-
-def check_validity(data, input_name = 'temporal_data', data_type = 'temporal', column_identifier = None): 
-# data argument could accept temporal_data, full_data, spatial_data, spatial_scale_table or future_data_table
-# the type will be determined based on data_type argument and the input_name argument will
-# be used to produce more clear warning errors
-
-    if 'spatial id level 1' not in data.columns:
-        if data_type != 'spatial_scales':
-            raise Exception("The input {0} has no spatial id column, and the name of this column is not specified in the column_identifier.\nmissing column: 'spatial id level 1'".format(input_name))
-        else:
-            raise Exception("The input {0} has no spatial id column.\nmissing column: 'spatial id level 1'".format(input_name))
-    
-    else:
-        # check for null values
-        for i in range(1,200):
-            column_name = 'spatial id level ' + str(i)
-            if column_name in data.columns:
-                if data[column_name].isnull().values.any():
-                    raise ValueError('spatial id must have value for all instances but spatial id level '+str(i)+' in {0} includes NULL values'.format(input_name))
-            else: break
-
-    if data_type in ['temporal','full']:
-        
-        if 'temporal id' in data.columns: # integrated temporal id format
-            temporal_identifier_column_name = 'temporal id'
-            if data[temporal_identifier_column_name].isnull().values.any():
-                    raise ValueError('temporal id must have value for all instances but temporal id column in {0} includes NULL values'.format(input_name))
-
-        elif 'temporal id level 1' in data.columns: # non-integrated temporal id format
-            data = add_dummy_integrated_temporal_id(data.copy())
-            temporal_identifier_column_name = 'dummy temporal id'
-        else:
-            raise Exception("The input {0} has no temporal id column, and the name of this column is not specified in the column_identifier.\nmissing column: 'temporal id' or 'temporal id level 1'".format(input_name))
-            
-        data = data.drop_duplicates(subset = ['spatial id level 1',temporal_identifier_column_name]).copy()
-
-        if len(data) != len(data['spatial id level 1'].unique())* len(data[temporal_identifier_column_name].unique()):
-            raise ValueError("The input {0} has different number of temporal units recorded for each spatial unit".format(input_name))
-        if 'dummy temporal id' in data.columns:
-            data.drop(['dummy temporal id'], axis = 1, inplace = True)
-            
-    if column_identifier is None:
-        numerical_columns = list(filter(lambda x: x.startswith(('temporal covariate','spatial covariate','target')),data.columns))
-    elif all([key in list(column_identifier.keys()) for key in ['target','spatial covariates','temporal covariates']]):
-        numerical_columns = list(filter(lambda x: x in(['target']+column_identifier['spatial covariates']+column_identifier['temporal covariates']),data.columns))
-    elif all([key in list(column_identifier.keys()) for key in ['target','temporal covariates']]):
-        numerical_columns = list(filter(lambda x: x in(['target']+column_identifier['temporal covariates']),data.columns))
-    else:
-        raise ValueError("The target and temporal covariates are not specified in column_identifier.")
-        
-    for covar in numerical_columns:
-        try:
-            data[covar].astype(float)
-        except (ValueError, TypeError):
-            raise ValueError("The covariates and target variable must include only numerical values. But non-numerical values are recorded for the {0}".format(covar))
-    return
-            
-############################ rename the columns of final historical data
-
-def recorrect_hist_data(data, augmentation, granularity, target_mode, target_granularity):
-    
-    # name of target mode
-    target_column_name = 'Target'
-    if augmentation == True:
-        target_column_name = 'Target (augmented with {0} units)'.format(granularity)
-        data = data.rename(columns={'Target':target_column_name})
-
-    if target_mode in ['differential', 'cumulative', 'normal']:
-        data = data.rename(columns={target_column_name:'{0} ({1})'.format(target_column_name, target_mode)})
-        target_column_name = '{0} ({1})'.format(target_column_name, target_mode)
-
-    if target_mode == 'moving average':
-        data = data.rename(columns={target_column_name:'{0} (moving average on {1} units)'.format(target_column_name, target_granularity)})
-        target_column_name = '{0} (moving average on {1} units)'.format(target_column_name, target_granularity)
-
-    data = data.rename(columns={target_column_name:target_column_name.replace(') (',' - ')})
-    
-    return data
-
-############################ adding or separating the values of futuristic covariates (future_data_table) to the data
-
-def current_future(data, future_data_table, futuristic_covariates, column_identifier , mode):
-    '''
-    mode = 'split' or 'add'
-    '''
-    if futuristic_covariates == None:
-        return data, None, []
-    
-    futuristic_covariate_list = list(futuristic_covariates.keys())
-
-    data = rename_columns(data.copy(), column_identifier)
-    check_validity(data.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier)
-    
-    if column_identifier is None:
-        spatial_covariates = list(filter(lambda x:x.startswith('spatial covariate'), data.columns))
-        temporal_covariates = list(filter(lambda x:x.startswith('temporal covariate'), data.columns))
-    else:
-        if 'spatial covariates' in column_identifier.keys():
-            spatial_covariates = [item for item in list(column_identifier['spatial covariates']) if item in data.columns]
-        else: spatial_covariates = []
-        temporal_covariates = [item for item in list(column_identifier['temporal covariates']) if item in data.columns]
-        
-    id_columns = list(filter(lambda x: x.startswith(('spatial id','temporal id')),data.columns))
-    spatial_id_columns = list(filter(lambda x: x.startswith(('spatial id')),data.columns))
-    temporal_id_columns = list(filter(lambda x: x.startswith(('temporal id')),data.columns))
-    target_columns = ['target']
-    if 'Normal target' in data.columns:
-        target_columns = target_columns + ['Normal target']
-    
-    spatial_data = None
-    temporal_data = data[id_columns + temporal_covariates + target_columns]
-    if len(spatial_covariates) > 0:
-        # if input 'data' is full data, data on spatial covariates is saved to add to the data at the end of the process
-        if len(list(set(spatial_covariates) - set(data.columns))) == 0 :
-            spatial_data = data[spatial_id_columns + spatial_covariates].drop_duplicates(subset = spatial_id_columns)
-    
-    
-    if future_data_table is not None:
-        future_data_table = rename_columns(future_data_table.copy(), column_identifier)
-        check_validity(future_data_table.copy(), input_name = 'future_data_table',
-                       data_type = 'temporal', column_identifier = column_identifier)
-        
-        for col in id_columns:
-            if col not in future_data_table.columns :
-                raise ValueError("The temporal and spatial id columns must be identical in the future_data_table and the input data.")
-        
-        extra_columns = (set(future_data_table.columns)-set(id_columns)-set(futuristic_covariate_list))
-        if len(extra_columns) > 0: print("\nWarning: some of the columns in the future_data_table are not in the futuristic_covariates and will be ignored.")
-        unspecified_columns = (set(futuristic_covariate_list)-(set(future_data_table.columns)-set(id_columns)))
-        if len(unspecified_columns) > 0:raise Exception("Some of the futuristic covariates in the futuristic_covariates dict are not included in the future_data_table.")
-        
-    if 'temporal id' in temporal_data.columns:
-        temporal_identifier_column_name = 'temporal id'
-        non_futuristic_covariates = list(set(temporal_data.columns) - set(futuristic_covariate_list + spatial_id_columns + ['temporal id']))
-
-
-    else: # non-integrated temporal id format
-        for level in range(1,200):
-            if 'temporal id level ' + str(level) in temporal_data.columns:
-                smallest_temporal_level = level
-                break
-        temporal_data = add_dummy_integrated_temporal_id(temporal_data.copy(), start_level = smallest_temporal_level)
-        if future_data_table is not None:
-            future_data_table = add_dummy_integrated_temporal_id(future_data_table.copy(), start_level = smallest_temporal_level)
-        temporal_identifier_column_name = 'dummy temporal id'
-        non_futuristic_covariates = list(set(temporal_data.columns) - set(futuristic_covariate_list + spatial_id_columns + ['dummy temporal id'] + temporal_id_columns))
-
-
-    if mode == 'split':
-        
-        temporal_data = temporal_data.drop_duplicates(subset = ['spatial id level 1', temporal_identifier_column_name]).copy()
-        temporal_data = temporal_data.sort_values(by = [temporal_identifier_column_name,'spatial id level 1'])
-
-        temporal_data['...'] = list(range(len(temporal_data))) # add an unique id to the data frame
-
-        current_data = temporal_data.dropna(subset = non_futuristic_covariates, how='all')
-        current_data_index = list(current_data['...'])
-        future_data = temporal_data[~(temporal_data['...'].isin(current_data_index))]
-        temp = future_data.groupby([temporal_identifier_column_name]).count()
-        
-        # remove dates which is not compeletly missed the non_futuristic_covariates (are not related to the future data)
-        total_number_of_spatial_ids = temp['spatial id level 1'].max()
-        incomplete_dates = temp[temp['spatial id level 1'] < total_number_of_spatial_ids].index
-
-        future_data = future_data[~(future_data[temporal_identifier_column_name].isin(incomplete_dates))]
-        current_data = temporal_data[~(temporal_data['...'].isin(future_data['...']))]
-        
-        futuristic_temporal_units = list(future_data[temporal_identifier_column_name].unique())
-        future_data_table_columns = id_columns + futuristic_covariate_list
-        future_data_table = future_data[future_data_table_columns]
-
-        if 'dummy temporal id' in current_data.columns:
-            current_data = current_data.drop(['dummy temporal id','...'], axis = 1)
-        else:
-            current_data = current_data.drop(['...'], axis = 1)
-        
-        if len(future_data_table) == 0 :
-            future_data_table = None
-        
-        if spatial_data is not None:
-            current_data = pd.merge(current_data, spatial_data, on = 'spatial id level 1', how = 'left')
-        
-        return current_data, future_data_table, futuristic_temporal_units
-        
-    if mode == 'add':
-        for col in non_futuristic_covariates:
-            future_data_table.loc[:,(col)] = np.NaN
-        future_data_table = future_data_table[list(temporal_data.columns)]
-        
-        future_data_table = future_data_table[future_data_table['spatial id level 1'].isin(temporal_data['spatial id level 1'].unique())]
-        
-        future_data_table = future_data_table[future_data_table[temporal_identifier_column_name]>max(temporal_data[temporal_identifier_column_name])]
-        
-        temporal_data = temporal_data.append(future_data_table)
-        
-        temporal_data.sort_values(by = [temporal_identifier_column_name, 'spatial id level 1'])
-        if 'dummy temporal id' in temporal_data.columns:
-            temporal_data = temporal_data.drop(['dummy temporal id'], axis = 1)
-            
-        futuristic_temporal_units = list(future_data_table[temporal_identifier_column_name].unique())
-        
-        if spatial_data is not None:
-            data = pd.merge(temporal_data, spatial_data, on = 'spatial id level 1', how = 'left')
-        else: data = temporal_data
-            
-        return data, None, futuristic_temporal_units
-
-        
-############################ filling up the future temporal units null values with inf to recognize them later
-    
-def fill_future_nulls(data, futuristic_temporal_units):
-        if 'temporal id' in data.columns:
-            temporal_identifier_column_name = 'temporal id'
-        else:
-            for level in range(1,200):
-                if 'temporal id level ' + str(level) in data.columns:
-                    smallest_temporal_level = level
-                    break
-            data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
-            temporal_identifier_column_name = 'dummy temporal id'
-        current_data = data[~(data[temporal_identifier_column_name].isin(futuristic_temporal_units))]
-        future_data = data[data[temporal_identifier_column_name].isin(futuristic_temporal_units)]
-        future_data = future_data.fillna(np.inf)
-        data = current_data.append(future_data)
-        return data
-        
-############################ adding an integrated teporal id to the data for non integrated temporal id format
-
-
-# Integrating the temporal id columns with the scale levels greater than 'start_level',
-# to obtain a single temporal id which is unique for each unit of the temporal scale level 'start_level'
-def add_dummy_integrated_temporal_id(temporal_data, start_level = 1):
-    
-    temporal_data_columns = temporal_data.columns
-    
-    valid_temporal_id_levels = ['temporal id level ' + str(start_level)] # sequense of temporal levels without gap
-    greatest_temporal_level = start_level
-
-    # determine the greatest temporal scale level and valid temporal id levels
-    for i in range(start_level+1,200):
-        
-        if 'temporal id level '+str(i) in temporal_data_columns:
-            greatest_temporal_level += 1
-            valid_temporal_id_levels.append('temporal id level '+str(i))
-            
-            # check for null values
-            if temporal_data['temporal id level '+str(i)].isnull().values.any():
-                raise ValueError('temporal id must have value for all instances but temporal id level '+str(i)+' includes NULL values')
-        else:
-            break
-            
-    # remove invalid temporal id levels from data
-    all_temporal_id_levels = list(filter(lambda x: x.startswith('temporal id level '), temporal_data.columns))
-    invalid_temporal_id_levels = list(set(all_temporal_id_levels)-set(valid_temporal_id_levels))
-    if len(invalid_temporal_id_levels) > 0:
-        temporal_data.drop(invalid_temporal_id_levels, axis = 1, inplace = True)
-        if start_level>1:
-            smaller_temporal_id_levels = ['temporal id level '+str(i) for i in range(1,start_level)]
-            invalid_temporal_id_levels = list (set(invalid_temporal_id_levels)-set(smaller_temporal_id_levels))
-            if len(invalid_temporal_id_levels) > 0:
-                print('\nWarning: There is a gap in the sequence of temporal scale levels recorded in the data.\nIds for temporal scale levels greater than {0} are ignored.\n'.format(greatest_temporal_level))
-    
-    # construct the integrated (sortable) temporal id
-    temporal_data.loc[:,('dummy temporal id')] = temporal_data['temporal id level ' + str(greatest_temporal_level)]
-
-    if greatest_temporal_level > 1:
-        for level in range(start_level,greatest_temporal_level)[::-1]:
-            temporal_data.loc[:,('dummy temporal id')] = temporal_data['dummy temporal id'].astype(str) + '/' + temporal_data['temporal id level ' + str(level)].astype(str)
-    
-    return temporal_data
-
-
-############################ adding secondary spatial scale id's to data
-
-def add_spatial_ids(data,spatial_scale_table):
-    
-    
-    # to use the spatial scale mapping in the spatial_scale_table
-    # first the existing secondary spatial scale levels are removed from the data
-    extra_spatial_ids = list(filter(lambda x: x.startswith('spatial id level '), data.columns))
-    extra_spatial_ids.remove('spatial id level 1')
-    data.drop(extra_spatial_ids, axis = 1, inplace = True)
-
-    # check spatial_scale_table to have information of all the units in the spatial scale level 1
-    intersection = list(set(data['spatial id level 1'].unique()) & set(spatial_scale_table['spatial id level 1'].unique()))
-    if len(intersection) < len(data['spatial id level 1'].unique()):
-        raise ValueError('The ids of some units in the spatial scale level 1 are missed in the spatial_scales_table.')
-
-    spatial_scale_levels = ['spatial id level 1']
-    for i in range(2,200):
-        column_name = 'spatial id level ' + str(i)
-        if column_name in spatial_scale_table.columns:
-            spatial_scale_levels.append(column_name)
-        else: break
-
-    data = pd.merge(data,spatial_scale_table[spatial_scale_levels], how = 'left', on= 'spatial id level 1')
-
-    return data
-
-
-############################ transform temporal ids in the data frame to the time stamp format
-
-def create_time_stamp(data, time_format, required_suffix):
-    try:
-        data.loc[:,('temporal id')] = data['temporal id'].astype(str) + required_suffix
-        data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x:datetime.datetime.strptime(x,time_format))
-    except ValueError:
-        raise ValueError("temporal id values doesn't match any supported integrated format for temporal id.\n")
-    return data
-
-############################ find the scale of temporal ids and transform to the time stamp format
-
-def check_integrated_temporal_id(temporal_data):
-        
-    list_of_supported_formats_string_length = [4,7,10,13,16,19]
-    temporal_data = temporal_data.sort_values(by = ['spatial id level 1','temporal id']).copy()
-    temporal_id_instance = str(temporal_data['temporal id'].iloc[0])
-    
-    if len(temporal_id_instance) not in list_of_supported_formats_string_length:
-        raise ValueError("temporal id values doesn't match any supported integrated format for temporal id.\n")
-    
-    # find the scale
-    if len(temporal_id_instance) == 4:
-        scale = 'year'
-        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d', '/01/01')
-            
-    elif len(temporal_id_instance) == 7:
-        scale = 'month'
-        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d', '/01')
-        
-    elif len(temporal_id_instance) == 10:
-        
-        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d', '')
-        
-        first_temporal_id_instance = temporal_data['temporal id'].iloc[0]
-        second_temporal_id_instance = temporal_data['temporal id'].iloc[1]
-        
-        delta = second_temporal_id_instance - first_temporal_id_instance
-        if delta.days == 1:
-            scale = 'day'
-        elif delta.days == 7:
-            scale = 'week'
-        else:
-            raise ValueError("temporal ids with format YYYY/MM/DD must be daily or weekly, but two consecutive id's of input data have a difference of {0} days.\n".format(delta.days))
-    
-    elif len(temporal_id_instance) == 13:
-        scale = 'hour'
-        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d %H:%M:%S', ':00:00')
-
-    elif len(temporal_id_instance) == 16:
-        scale = 'min'
-        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d %H:%M:%S', ':00')
-            
-    elif len(temporal_id_instance) == 19:
-        scale = 'sec'
-        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d %H:%M:%S', '')
-    
-    return temporal_data, scale
-            
-############################ find the number of smaller scale units in each bigger scale unit
-
-def find_granularity(data, temporal_scale_level):
-    
-    if (type(temporal_scale_level) != int) and (temporal_scale_level is not None):
-        raise TypeError("The temporal_scale_level must be of type int.\n")
-    
-    
-    ###################################### integrated temporal id format ################################
-    
-    if 'temporal id' in data.columns:
-    
-        scale_level_dict = {'sec':1, 'min':2, 'hour':3, 'day':4, 'week':5, 'month':6, 'year':7}
-        scale_format = {'sec':'%Y/%m/%d %H:%M:%S', 'min':'%Y/%m/%d %H:%M', 'hour':'%Y/%m/%d %H', 'day':'%Y/%m/%d', 'week':'%Y/%m/%d', 'month':'%Y/%m', 'year':'%Y'}
-        scale_second_units_number = {'sec':1, 'min':60, 'hour':3600, 'day':24*3600, 'week':7*24*3600, 'month':30*24*3600, 'year':365*24*3600}
-
-        data = data.drop_duplicates(subset = ['spatial id level 1','temporal id']).copy()
-
-        # determining input data temporal scale and transforming temporal id's to timestamp
-        data , scale = check_integrated_temporal_id(data.copy())
-        
-        # in moving average target mode the temporal_scale_level is the next level of current level and must be detected
-        # based on current level
-        if temporal_scale_level is None:
-            temporal_scale_level = 2
-            desired_temporal_scale_level = scale_level_dict[scale] + temporal_scale_level - 1
-            if desired_temporal_scale_level > 7:
-                raise exception("The temporal scale level of the data is {0}. Thus the 'moving average' target_mode couldn't be applied cause the temporal scale bigger than {0} is ambiguous.\n".format(scale))
-
-
-        # determine the numerical desired temporal scale level based on the input data
-        # temporal scale and user specified temporal_scale_level
-        desired_temporal_scale_level = scale_level_dict[scale] + temporal_scale_level - 1
-        if desired_temporal_scale_level > 7:
-            raise Exception('The first temporal scale level recorded in the data is {0}. So the temporal scale level {1} is out of the supported range of temporal scale levels: second, minute, hour, day, week, month, year'.format(scale,temporal_scale_level))
-
-        # get the nominal form of desired temporal scale level
-        desired_temporal_scale = list(scale_level_dict.keys())[list(scale_level_dict.values()).index(desired_temporal_scale_level)]
-        
-        # get number of smaller temporal units in each bigger temporal unit
-        granularity = scale_second_units_number[desired_temporal_scale]//scale_second_units_number[scale]
-        
-    ###################################### non_integrated temporal id format ################################
-        
-    if 'temporal id level 1' in data.columns: 
-        
-        # if function is called for getting granularity of moving average target mode, the temporal_scale_level
-        # is the next level of current level and must be detected based on current level
-        if temporal_scale_level is None:
-            for level in range(1,200):
-                if 'temporal id level ' + str(level) in data.columns:
-                    smallest_temporal_level = level
-                    break
-            temporal_scale_level = smallest_temporal_level + 1
-            desired_scale_column_name = 'temporal id level ' + str(temporal_scale_level)
-            if desired_scale_column_name not in data.columns:
-                raise ValueError("The next bigger temporal scale after data current temporal scale (temporal scale level {0}) isn't included in the data or is located after a gap in the temporal scale levels sequence and is therefore ignored.\n".format(smallest_temporal_level))
-            
-        else:
-            smallest_temporal_level = 1
-            desired_scale_column_name = 'temporal id level ' + str(temporal_scale_level)
-            if desired_scale_column_name not in data.columns:
-                raise ValueError("temporal_scale_level {0} is not in the time scale levels recorded in the data or is located after a gap in the temporal scale levels sequence and is therefore ignored. ".format(temporal_scale_level))
-
-            
-        # next 2 line removes the duplicate data samples having same spatial and temporal id's.
-        data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
-        data = data.drop_duplicates(subset = ['spatial id level 1','dummy temporal id']).copy()
-
-        
-        # get number of smaller temporal units in each bigger temporal unit
-        granularity = data.groupby(['spatial id level 1',desired_scale_column_name]).count()['dummy temporal id'].max()
-
-
-    return granularity
-
-############################ preprocessing the input data and split it to temporal and spatial data
-
-def prepare_data(data, column_identifier):
-    
-    # initialize
-    spatial_data = None
-    temporal_data = None
-    
-    if type(data) != dict :
-
-        if type(data) == str :
-            try:
-                data = pd.read_csv(data)
-            except FileNotFoundError:
-                raise FileNotFoundError("File '{0}' does not exist.\n".format(data))
-        elif type(data) != pd.DataFrame :
-            raise TypeError("The input data must be of type DataFrame, string, or a dict containing temporal and spatial DataFrames or addresses.\n")
-        data = rename_columns(data.copy(), column_identifier)
-
-        check_validity(data.copy(), input_name = 'data', data_type = 'full',
-                       column_identifier = column_identifier)
-
-        ##### split data to temporal and spatial data
-
-        spatial_columns = []
-        temporal_columns = []
-
-        # if type of each column is specified in column_identifier
-        if column_identifier is not None:
-            temporal_columns = list(filter(lambda x: x.startswith(('temporal id', 'spatial id','target')), data.columns)) + [item for item in column_identifier['temporal covariates'] if item in data.columns]
-            temporal_data = data[temporal_columns]
-            # if data includes spatial covariates
-            if 'spatial covariates' in column_identifier.keys():
-                spatial_columns = list(filter(lambda x: x.startswith('spatial id'), data.columns)) + [item for item in column_identifier['spatial covariates'] if item in data.columns]
-                spatial_data = data[spatial_columns].drop_duplicates(subset = ['spatial id level 1']).copy()
-
-        # if type of columns are clear based on column name
-        else:
-            temporal_columns = list(filter(lambda x: x.startswith(('temporal id', 'spatial id','temporal covariate','target')), data.columns))
-            temporal_data = data[temporal_columns]
-            # if data includes spatial covariates
-            if len(list(filter(lambda x: x.startswith('spatial covariate'), data.columns))) > 0 :
-                spatial_columns = list(filter(lambda x: x.startswith('spatial id','spatial covariate'), data.columns))
-                spatial_data = data[spatial_columns].drop_duplicates(subset = ['spatial id level 1']).copy()
-
-
-        data_extra_columns = list(set(data.columns)-set(spatial_columns+temporal_columns))
-
-        if len(data_extra_columns) > 0:
-            print("\nWarning: Input data column names must match one of the formats:\n{'temporal id', 'temporal id level x', 'spatial id', 'spatial id level x', 'temporal covariate x', 'spatial covariate x', 'target'},")
-            print("or be specified in the column_identifier, but the names of some of the columns do not match any of the supported formats and are not mentioned in the column_identifier:\n{0}\nThese columns will be ignored.\n".format(data_extra_columns))
-
-
-    elif type(data) == dict:
-        if 'temporal_data' in data.keys():
-
-            if type(data['temporal_data']) == str:
-                try:
-                    temporal_data = pd.read_csv(data['temporal_data'])
-                except FileNotFoundError:
-                    raise FileNotFoundError("File '{0}' does not exist.\n".format(data['temporal_data']))
-
-            elif type(data['temporal_data']) == pd.DataFrame:
-                temporal_data = data['temporal_data']
-            else:
-                raise valueError("The value of the 'temporal id' key in the data dictionary must be a DataFrame or the address of temporal data.\n")
-            temporal_data = rename_columns(temporal_data.copy(), column_identifier)
-            check_validity(temporal_data.copy(), input_name = 'temporal_data', 
-                           data_type = 'temporal', column_identifier = column_identifier)
-
-            if column_identifier is not None:
-                if 'temporal covariates' in column_identifier.keys():
-                    temporal_data_extra_columns = list(set(filter(lambda x: not x.startswith(('temporal id','spatial id','target')), temporal_data.columns)) - set(column_identifier['temporal covariates']))
-            else:
-                temporal_data_extra_columns = list(filter(lambda x: not x.startswith('temporal id','spatial id','temporal covariate','target'), temporal_data.columns))
-
-            if len(temporal_data_extra_columns) > 0:
-                print("\nWarning: Input temporal_data column names must match one of the formats:\n{'temporal id', 'temporal id level x', 'spatial id', 'spatial id level x', 'temporal covariate x', 'target'}")
-                print("or be specified in the column_identifier,but the names of some of the columns do not match any of the supported formats and are not mentioned in the column_identifier:\n{0}\nThese columns will be ignored.\n".format(temporal_data_extra_columns))
-            temporal_data.drop(temporal_data_extra_columns, axis = 1, inplace = True)
-
-        else:
-            raise Exception("The data on temporal covariates and target variable must be passed to the function using data argument and as a DataFrame, Data address or value of 'temporal_data' key in the dictionary of data. But none is passed.\n")
-
-
-        if ('spatial_data' in data.keys()) and (data['spatial_data'] is not None):
-
-            if type(data['spatial_data']) == str:
-                try:
-                    spatial_data = pd.read_csv(data['spatial_data'])
-                except FileNotFoundError:
-                    raise FileNotFoundError("File '{0}' does not exist.\n".format(data['spatial_data']))
-
-            elif type(data['spatial_data']) == pd.DataFrame:
-                spatial_data = data['spatial_data']
-            else:
-                raise ValueError("The value of the 'spatial id' key in the data dictionary must be a DataFrame or the address of spatial data.\n")
-
-            spatial_data = rename_columns(spatial_data.copy(), column_identifier)
-            check_validity(spatial_data.copy(), input_name = 'spatial_data',
-                           data_type = 'spatial', column_identifier = column_identifier)
-            spatial_data = spatial_data.drop_duplicates(subset = ['spatial id level 1']).copy()
-
-            if column_identifier is not None:
-                if 'spatial covariates' in column_identifier.keys():
-                    spatial_data_extra_columns = list(set(filter(lambda x: not x.startswith('spatial id'), spatial_data.columns)) - set(column_identifier['spatial covariates']))
-            else:
-                spatial_data_extra_columns = list(filter(lambda x: not x.startswith(('spatial id','spatial covariate')), spatial_data.columns))
-
-            if len(spatial_data_extra_columns) > 0:
-                print("\nWarning: Input spatial_data column names must match one of the formats:\n{'spatial id', 'spatial id level x', 'spatial covariate x'}")
-                print("or be specified in the column_identifier,but the names of some of the columns do not match any of the supported formats and are not mentioned in the column_identifier:\n{0}\nThis columns will be ignored.\n".format(spatial_data_extra_columns))
-            spatial_data.drop(spatial_data_extra_columns, axis = 1, inplace = True)
-            
-    return temporal_data, spatial_data
-
-
-#############################################################################################
-############################  imputing the tepmoral data ####################################
-#############################################################################################
-
-def impute(data, column_identifier = None, verbose = 0):
-    
-    if type(data) == str:
-        data = pd.read_csv(data)
-    
-    data = rename_columns(data.copy(), column_identifier)
-        
-    check_validity(data.copy(), input_name = 'data', data_type = 'temporal',
-                   column_identifier = column_identifier)
-    
-    if 'temporal id' in data.columns:
-        temporal_identifier_column_name = 'temporal id'
-        
-    elif 'temporal id level 1' in data.columns: # non-integrated temporal id format
-        # first integrated format for temporal id must constructed
-        data = add_dummy_integrated_temporal_id(data.copy())
-        temporal_identifier_column_name = 'dummy temporal id'
-
-    data = data.drop_duplicates(subset = ['spatial id level 1', temporal_identifier_column_name]).copy()
-        
-    covariate_names = list(filter(lambda x: not x.startswith(('temporal id', 'spatial id', 'dummy temporal id')), data.columns))
-    
-    if 'target' in data.columns:
-        if data['target'].isnull().values.any():
-            if verbose > 0: print("\nWarning: The target variable includes missing values. This values will be imputed.\n")
-            
-    spatial_units_observed_value_count = data.groupby('spatial id level 1').count()
-    temporal_units_observed_value_count = data.groupby(temporal_identifier_column_name).count()
-    
-    
-    
-    for covar in covariate_names:
-        spatial_units_with_all_nulls=spatial_units_observed_value_count[spatial_units_observed_value_count[covar]==0].index
-        temporal_units_with_all_nulls=temporal_units_observed_value_count[temporal_units_observed_value_count[covar]==0].index
-        
-        # check if covariate has no value for an temporal unit
-        if len(temporal_units_with_all_nulls) > 0:
-            raise ValueError("The input data has no value for {0}, in some temporal units.\nThe covariates must have value for at least one spatial unit in each temporal units recorded in the data".format(covar))
-        
-        data = data.drop_duplicates(subset = ['spatial id level 1',temporal_identifier_column_name]).copy()
-        
-        # create data frame with each row representing a spatial unit and each column representing a temporal unit 
-        temp = data.pivot(index='spatial id level 1', columns=temporal_identifier_column_name, values=covar)
-        
-        # impute missing values using KNN imputation
-        X = np.array(temp)
-        imputer = KNNImputer(n_neighbors=5)
-        imp=imputer.fit_transform(X)
-        imp=pd.DataFrame(imp, index = temp.index, columns = temp.columns)
-        
-        # reshape imputed values of covariate into one column
-        imp = pd.melt(imp.reset_index(), id_vars='spatial id level 1', value_vars=list(imp.columns),
-                     var_name=temporal_identifier_column_name, value_name=covar)
-        
-        # add the imputed values back to the data set
-        data.drop([covar], axis = 1, inplace = True)
-        data = pd.merge(data, imp, how = 'left')
-        
-        # remove the imputed values for the spatial units with no observed values
-        data.loc[data['spatial id level 1'].isin(spatial_units_with_all_nulls),covar]=np.NaN
-        if len(spatial_units_with_all_nulls)>0:
-            if verbose == 2:
-                print('\nWarning: Following spatial units has no recorded values for {0} and therefore will be removed from the data:\n{1}\n'.format(covar,list(spatial_units_with_all_nulls)))
-            elif verbose == 1:
-                print('\nWarning: The number of {0} spatial units has no recorded values for {1} and therefore will be removed from the data\n.'.format(len(list(spatial_units_with_all_nulls)),covar))
-    
-    # remove temporarily added column
-    if 'dummy temporal id' in data.columns: data.drop(['dummy temporal id'], axis = 1, inplace = True)
-    
-    # produce warning for removed spatial units
-    number_of_spatial_units = len(data['spatial id level 1'].unique())
-    imputed_data = data.dropna()
-    number_of_removed_spatial_units = number_of_spatial_units - len(imputed_data['spatial id level 1'].unique())
-    
-    if number_of_removed_spatial_units == number_of_spatial_units:
-        raise Exception("All the spatial units have no value for at least one temporal covariate and are removed from the data. Therefore, no spatial unit remains to make a prediction.\n")
-    elif number_of_removed_spatial_units > 0:
-        if verbose == 0:
-            print('\nWarning: The number of {0} spatial units has no value for at least one temporal covariate and are removed from the data.\n'.format(number_of_removed_spatial_units))
-    
-    imputed_data = rename_columns(imputed_data.copy(), column_identifier, 'deformalize')
-    
-    return imputed_data
-
-#################################################################################################
-############################  transforming the spatial scale ####################################
-#################################################################################################
-
-def spatial_scale_transform(data, data_type, spatial_scale_table = None, spatial_scale_level = 2, aggregation_mode = 'mean', column_identifier = None, verbose = 0):
-    
-    # initializing list of covariates with sum or mean aggregation modes
-    mean_covariates = []
-    sum_covariates = []
-    
-    desired_scale_column_name = 'spatial id level ' + str(spatial_scale_level)
-    base_columns = [desired_scale_column_name]
-    
-    if type(data) == str:
-        data = pd.read_csv(data)
-    data = rename_columns(data.copy(), column_identifier)
-    
-    check_validity(data.copy(), input_name = 'data', data_type = data_type, column_identifier = column_identifier)
-    if spatial_scale_table is not None:
-        if type(spatial_scale_table) == str:
-            spatial_scale_table = pd.read_csv(spatial_scale_table)
-        spatial_scale_table = rename_columns(spatial_scale_table.copy(), column_identifier)
-        check_validity(spatial_scale_table.copy(), input_name = 'spatial_scale_table',
-                       data_type = 'spatial_scales', column_identifier = column_identifier)
-        # drop duplicate is needed ????
-        data = add_spatial_ids(data.copy(),spatial_scale_table)
-
-    if desired_scale_column_name not in data.columns:
-        raise ValueError("spatial_scale_level {0} isn't in the spatial scale levels included in the data.\n".format(spatial_scale_level))
-
-
-    if data_type == 'temporal':
-
-        if 'temporal id' in data.columns: # integrated temporal id format
-            temporal_identifier_column_name = 'temporal id'
-
-        elif 'temporal id level 1' in data.columns: # non-integrated temporal id format
-            # first integrated format for temporal id must constructed
-            data = add_dummy_integrated_temporal_id(data.copy())
-            temporal_identifier_column_name = 'dummy temporal id'
-
-            non_integrated_temporal_levels = list(filter(lambda x: x.startswith('temporal id level '), data.columns))
-            temporal_levels_data_frame = data[non_integrated_temporal_levels + ['dummy temporal id']]
-            data.drop(non_integrated_temporal_levels, axis = 1, inplace = True)
-
-        base_columns.append(temporal_identifier_column_name)
-        data = data.drop_duplicates(subset = ['spatial id level 1',temporal_identifier_column_name]).copy()
-
-    else:
-        data = data.drop_duplicates(subset = ['spatial id level 1']).copy()
-
-
-    # removing spatial id columns except for desired spatial scale ids
-    extra_spatial_ids = list(filter(lambda x: x.startswith('spatial id '), data.columns))
-    extra_spatial_ids.remove(desired_scale_column_name)
-    data.drop(extra_spatial_ids, axis = 1, inplace = True)
-
-    covariate_names = list(filter(lambda x: not x.startswith(('temporal id','spatial id','dummy temporal id')), data.columns))
-
-
-    if aggregation_mode == 'mean':
-        mean_covariates = covariate_names.copy()
-    elif aggregation_mode == 'sum':
-        sum_covariates = covariate_names.copy()
-    elif type(aggregation_mode) == dict:
-        extra_covariates_listed = list(set(aggregation_mode.keys())-set(covariate_names))
-        if len(extra_covariates_listed) > 0:
-            aggregation_mode = {covar:operator for covar,operator in aggregation_mode.items() if covar in covariate_names}
-            if verbose == 1:
-                print("\nWarning : Some of the covariates specified in aggregation_mode are not exist in the data.\n")
-            if verbose == 2:
-                print("\nWarning : Some of the covariates specified in aggregation_mode are not exist in the data:\n{0}\n".format(extra_covariates_listed))
-        mean_covariates = [covar for covar,operator in aggregation_mode.items() if operator == 'mean']
-        sum_covariates = [covar for covar,operator in aggregation_mode.items() if operator == 'sum']
-    else:
-        raise ValueError("aggregation_mode must be 'sum' or 'mean' or a dictionary with covariates name as the keys and 'sum' or 'mean' as the values")
-
-    unspecified_covariates = list(set(covariate_names)-set(mean_covariates + sum_covariates))
-    if len(unspecified_covariates)>0:
-        if verbose < 2:
-            print("\nWarning : The aggregation_mode is not specified for some of the covariates.\nThe mean operator will be used to aggregate these covariates' values.\n")
-        if verbose == 2:
-            print("\nWarning : The aggregation_mode is not specified for some of the covariates:\n{0}\nThe mean operator will be used to aggregate these covariates' values.\n".format(unspecified_covariates))
-        mean_covariates = mean_covariates + unspecified_covariates
-
-    if len(mean_covariates)>0:
-        mean_covariates+=base_columns
-        mean_data = data.copy()[mean_covariates]
-        mean_data = mean_data.groupby(base_columns).mean()
-        mean_data = mean_data.reset_index()
-
-    if len(sum_covariates)>0:
-        sum_covariates+=base_columns
-        sum_data = data.copy()[sum_covariates]
-        sum_data = sum_data.groupby(base_columns).sum(min_count=1)
-        sum_data = sum_data.reset_index()
-
-    if len(mean_covariates)>0 and len(sum_covariates)>0:
-        data = pd.merge(mean_data,sum_data,on=base_columns)
-    elif len(mean_covariates)>0:
-        data = mean_data
-    elif len(sum_covariates)>0:
-        data = sum_data
-    
-    if 'dummy temporal id' in data.columns:
-        data = pd.merge(temporal_levels_data_frame.drop_duplicates(), data, on = ['dummy temporal id']).drop_duplicates().copy()
-        data.drop(['dummy temporal id'], axis=1, inplace = True)
-        ordered_columns = [desired_scale_column_name]+list(temporal_levels_data_frame.columns.drop(['dummy temporal id']))+covariate_names
-    elif 'temporal id' in data.columns:
-        ordered_columns = [desired_scale_column_name,'temporal id']+covariate_names
-    else:
-        ordered_columns = [desired_scale_column_name]+covariate_names
-        
-    data = data.copy()[ordered_columns]
-    
-    data = rename_columns(data.copy(), column_identifier, 'deformalize')
-                  
-    return data
-
-##############################################################################################
-############################  transforming temporal scale ####################################
-##############################################################################################
-
-def temporal_scale_transform(data, column_identifier = None, temporal_scale_level = 2, augmentation = False, verbose = 0):
-    
-    if type(data) == str:
-        data = pd.read_csv(data)
-    data = rename_columns(data.copy(), column_identifier)
-    check_validity(data.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier)
-    
-    if type(temporal_scale_level) != int:
-        raise TypeError("The temporal_scale_level must be of type int.\n")
-        
-    if temporal_scale_level == 1:
-        if verbose > 0: print ('The temporal_scale_level = 1 is interpreted to no temporal transformation')
-        return data
-    
-    # Next 4 lines save the secondary spatial scale levels information in a data frame to be added to the transformed data
-    secondary_spatial_levels = list(filter(lambda x: x.startswith('spatial id level '), data.columns))
-    spatial_levels_data_frame = data[secondary_spatial_levels].drop_duplicates().copy()
-    secondary_spatial_levels.remove('spatial id level 1')
-    data.drop(secondary_spatial_levels, axis = 1, inplace = True)
-    
-    ###################################### integrated temporal id format ################################
-    
-    if 'temporal id' in data.columns:
-    
-        scale_level_dict = {'sec':1, 'min':2, 'hour':3, 'day':4, 'week':5, 'month':6, 'year':7}
-        scale_format = {'sec':'%Y/%m/%d %H:%M:%S', 'min':'%Y/%m/%d %H:%M', 'hour':'%Y/%m/%d %H', 'day':'%Y/%m/%d', 'week':'%Y/%m/%d', 'month':'%Y/%m', 'year':'%Y'}
-        scale_second_units_number = {'sec':1, 'min':60, 'hour':3600, 'day':24*3600, 'week':7*24*3600, 'month':30*24*3600, 'year':365*24*3600}
-
-        data = data.drop_duplicates(subset = ['spatial id level 1','temporal id']).copy()
-
-        # determining input data temporal scale and transforming temporal id's to timestamp
-        data , scale = check_integrated_temporal_id(data.copy())
-
-        # determine the numerical desired temporal scale level based on the input data
-        # temporal scale and user specified temporal_scale_level
-        desired_temporal_scale_level = scale_level_dict[scale] + temporal_scale_level - 1
-        if desired_temporal_scale_level > 7:
-            raise Exception('The first temporal scale level recorded in the data is {0}. So the temporal scale level {1} is out of the supported range of temporal scale levels: second, minute, hour, day, week, month, year'.format(scale,temporal_scale_level))
-
-        # get the nominal form of desired temporal scale level
-        desired_temporal_scale = list(scale_level_dict.keys())[list(scale_level_dict.values()).index(desired_temporal_scale_level)]
-        if verbose > 0 : print("\nTransformation of data to the temporal scale of the {0} is running.\n".format(desired_temporal_scale))
-            
-        # get number of smaller temporal units in each bigger temporal unit
-        granularity = scale_second_units_number[desired_temporal_scale]//scale_second_units_number[scale]
-        
-        number_of_temporal_units=len(data['temporal id'].unique())
-        number_of_spatial_units=len(data['spatial id level 1'].unique())
-        
-        if augmentation == False:
-
-            # For the temporal scale of the week, each date must be replaced with the date of the first day
-            # of the corresponding week
-            if desired_temporal_scale == 'week' :
-                data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x : x - datetime.timedelta(days=x.weekday()))
-
-            data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x : datetime.datetime.strftime(x,scale_format[desired_temporal_scale]))
-            
-            # remove the data of the smaller scale temporal units in beggining and
-            # ending of data which does'nt make up a complete bigger tempral scale unit
-            max_temporal_id = max(data['temporal id'])
-            min_temporal_id = min(data['temporal id'])
-            if len(data[data['temporal id'] == max_temporal_id])<number_of_spatial_units*granularity:
-                data = data[data['temporal id'] != max_temporal_id]
-            if len(data[data['temporal id'] == min_temporal_id])<number_of_spatial_units*granularity:
-                data = data[data['temporal id'] != min_temporal_id]
-            
-            base_columns = ['temporal id', 'spatial id level 1']
-            data = data.groupby(base_columns).mean()
-            data = data.reset_index()
-
-        if augmentation == True:
-
-            data = data.sort_values(by = ['temporal id' , 'spatial id level 1']).copy()
-            data.reset_index(drop = True, inplace = True)
-
-            transformed_data = pd.DataFrame(columns = data.columns)
-
-            while number_of_temporal_units >= granularity:
-                bigger_scale_unit_data = data.copy().tail(number_of_spatial_units*granularity) 
-                current_temporal_id = data.copy().tail(1)['temporal id'].values[0]
-
-                # average of covariates and target values on last bigger temporal scale unit for all spatial scale units
-                bigger_scale_unit_data_average = bigger_scale_unit_data.groupby(['spatial id level 1']).mean().reset_index()
-                bigger_scale_unit_data_average.loc[:,('temporal id')] = current_temporal_id
-
-                transformed_data = transformed_data.append(bigger_scale_unit_data_average)
-                # remove last smaller temporal scale unit for all spatial units from base data
-                data = data.iloc[:-(number_of_spatial_units),:]
-                number_of_temporal_units = number_of_temporal_units - 1
-
-            data = transformed_data.copy()
-            data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x : datetime.datetime.strftime(x,scale_format[scale]))
-
-        data = data.sort_values(by=['spatial id level 1','temporal id']).copy()
-    
-    ###################################### non_integrated temporal id format ################################
-        
-    if 'temporal id level 1' in data.columns: 
-    
-        # next 2 line removes the duplicate data samples having same spatial and temporal id's.
-        data = add_dummy_integrated_temporal_id(data.copy(), start_level = 1)
-        data = data.drop_duplicates(subset = ['spatial id level 1','dummy temporal id']).copy()
-
-        desired_scale_column_name = 'temporal id level ' + str(temporal_scale_level)
-        if desired_scale_column_name not in data.columns:
-            raise ValueError("temporal_scale_level {0} is not in the temporal scale levels recorded in the data or is located after a gap in the temporal scale levels sequence and is therefore ignored. ".format(temporal_scale_level))
-        elif verbose > 0 :
-            if column_identifier is not None:
-                print("\nTransformation of data to the temporal scale of the {0} is running.\n".format(column_identifier[desired_scale_column_name]))
-            else:
-                print("\nTransformation of data to the temporal scale of the {0} is running.\n".format(desired_scale_column_name))
-        
-        if augmentation == False :
-
-            # remove dummy temporal id which is based on level 1 to add dummy temporal id based on 'temporal_scale_level'
-            data.drop(['dummy temporal id'], axis = 1, inplace = True)
-            data = add_dummy_integrated_temporal_id(data.copy(), start_level = temporal_scale_level)
-
-            secondary_temporal_levels = list(filter(lambda x: x.startswith('temporal id level '), data.columns))
-            temporal_levels_data_frame = data[secondary_temporal_levels + ['dummy temporal id']]
-            data.drop(secondary_temporal_levels, axis = 1, inplace = True)
-
-            base_columns = ['dummy temporal id', 'spatial id level 1']
-
-            data = data.groupby(base_columns).mean()
-            data = data.reset_index()
-            data = pd.merge(temporal_levels_data_frame.drop_duplicates(), data, on = 'dummy temporal id', how = 'right').drop_duplicates().copy()
-            # sorting columns
-            data_columns = list(data.columns).copy()
-            data_columns.remove('dummy temporal id')
-            data = data[['dummy temporal id']+data_columns]
-
-
-        elif augmentation == True :
-
-            # get number of smaller temporal units in each bigger temporal unit
-            granularity = data.groupby(['spatial id level 1',desired_scale_column_name]).count()['dummy temporal id'].max()
-
-            secondary_temporal_levels = list(filter(lambda x: x.startswith('temporal id level '), data.columns))
-            temporal_levels_data_frame = data[secondary_temporal_levels + ['dummy temporal id']]
-            data.drop(secondary_temporal_levels, axis = 1, inplace = True)
-
-            data = data.sort_values(by = ['dummy temporal id' , 'spatial id level 1']).copy()
-            data.reset_index(drop = True, inplace = True)
-            number_of_temporal_units=len(data['dummy temporal id'].unique())
-            number_of_spatial_units=len(data['spatial id level 1'].unique())
-
-            transformed_data = pd.DataFrame(columns = data.columns)
-
-            while number_of_temporal_units >= granularity:
-                bigger_scale_unit_data = data.copy().tail(number_of_spatial_units*granularity) 
-                current_temporal_id = data.copy().tail(1)['dummy temporal id'].values[0]
-
-                # average of covariates and target values on last bigger temporal scale unit for all spatial scale units
-                bigger_scale_unit_data_average = bigger_scale_unit_data.groupby(['spatial id level 1']).mean().reset_index()
-                bigger_scale_unit_data_average.loc[:,('dummy temporal id')] = current_temporal_id
-                
-
-                transformed_data = transformed_data.append(bigger_scale_unit_data_average)
-                data = data.iloc[:-(number_of_spatial_units),:]# remove last smaller temporal scale unit for all spatial units from base data
-                number_of_temporal_units = number_of_temporal_units - 1
-
-            data = transformed_data.copy()
-
-            data = pd.merge(temporal_levels_data_frame.drop_duplicates(), data, on = 'dummy temporal id', how = 'right').drop_duplicates().copy()
-
-        data = data.sort_values(by=['spatial id level 1','dummy temporal id']).copy()
-        data.drop(['dummy temporal id'] ,axis = 1 , inplace = True)
-
-        
-    # add secondary spatial scale levels back to data
-    data = pd.merge(spatial_levels_data_frame.drop_duplicates(), data, on = 'spatial id level 1', how = 'right').drop_duplicates().copy()
-    
-    # sorting columns
-    data_columns = list(data.columns).copy()
-    data_columns.remove('spatial id level 1')
-    data = data[['spatial id level 1']+data_columns]
-    
-    if column_identifier is not None:
-        if 'temporal id' in data.columns: # integrated temporal_id format
-            data = rename_columns(data, {key:value for key,value in column_identifier.items() if key != 'temporal id'}, 'deformalize')
-        else: # non_integrated temporal_id format
-            data = rename_columns(data, column_identifier, 'deformalize')
-            
-    if len(data)<1:
-        raise Exception("The number of recorded units in the data with the specified temporal scale level is less than one.")
-    
-    return data
-
-######################################################################################
-############################  target modification ####################################
-######################################################################################
-
-# modifying target to the cumulative or differential or moving average mode
-
-def target_modification(data, target_mode, column_identifier = None, verbose = 0):
-    
-    if type(data) == str:
-        data = pd.read_csv(data)
-    data = rename_columns(data.copy(), column_identifier)
-    
-    check_validity(data.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier)
-    
-    if 'target' not in data.columns:
-        raise ValueError("There is no column named 'target' in the input data, and the corresponding column is not specified in the column_identifier.\n")
-    try:
-        data.loc[:,('target')] = data['target'].astype(float)
-    except ValueError:
-        raise ValueError("The target column includes non-numerical values.\n")
-        
-    if (data['target'].isnull().values.any()) and (target_mode in ['cumulative', 'differential', 'moving average']):
-        print("\nWarning: The target variable column includes Null values and therefore the resulting values of applying {0} target_mode is not valid.\n".format(target_mode))
-        
-    if 'temporal id' in data.columns: # integrated temporal id format
-        temporal_identifier_column_name = 'temporal id'
-    else: # Non_integrated temporal id format
-        for level in range(1,200):
-            if 'temporal id level ' + str(level) in data.columns:
-                smallest_temporal_level = level
-                break
-        data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
-        temporal_identifier_column_name = 'dummy temporal id'
-        
-
-    data = data.drop_duplicates(subset = [temporal_identifier_column_name,'spatial id level 1']).copy()
-    data = data.sort_values(by=[temporal_identifier_column_name,'spatial id level 1']).copy()
-    
-    normal_target_df = data[['spatial id level 1', temporal_identifier_column_name, 'target']].rename(columns = {'target':'Normal target'})
-    
-    ######################################################################### cumulative
-    
-    if target_mode == 'cumulative':
-        temporal_ids = data[temporal_identifier_column_name].unique()
-        for i in range(len(temporal_ids)-1): 
-            data.loc[data[temporal_identifier_column_name]==temporal_ids[i+1],'target']=\
-            list(np.array(data.loc[data[temporal_identifier_column_name]==temporal_ids[i+1],'target'])+\
-                  np.array(data.loc[data[temporal_identifier_column_name]==temporal_ids[i],'target']))
-        
-                
-    ######################################################################### differential
-
-    elif target_mode == 'differential': # make target differential
-        reverse_temporal_ids = data[temporal_identifier_column_name].unique()[::-1]
-        for i in range(len(reverse_temporal_ids)):
-            temprl_unit = reverse_temporal_ids[i]
-            past_temprl_unit = reverse_temporal_ids[i+1]
-            data.loc[data[temporal_identifier_column_name] == temprl_unit,'target']=\
-            list(np.array(data.loc[data[temporal_identifier_column_name]==temprl_unit,'target'])-\
-                 np.array(data.loc[data[temporal_identifier_column_name]==past_temprl_unit,'target']))
-            if i == len(reverse_temporal_ids)-2:
-                break
-            
-    ######################################################################### moving average
-            
-    elif target_mode == 'moving average':
-        
-        ############### integrated temporal id format
-        if temporal_identifier_column_name == 'temporal id': 
-            
-            scale_level_dict = {'sec':1, 'min':2, 'hour':3, 'day':4, 'week':5, 'month':6, 'year':7}
-            scale_format = {'sec':'%Y/%m/%d %H:%M:%S', 'min':'%Y/%m/%d %H:%M', 'hour':'%Y/%m/%d %H', 'day':'%Y/%m/%d', 'week':'%Y/%m/%d', 'month':'%Y/%m', 'year':'%Y'}
-            scale_second_units_number = {'sec':1, 'min':60, 'hour':3600, 'day':24*3600, 'week':7*24*3600, 'month':30*24*3600, 'year':365*24*3600}
-
-            # determining input data temporal scale and transforming temporal id's to timestamp
-            data , scale = check_integrated_temporal_id(data.copy())
-
-            # determine the numerical level of the next temporal scale after input data
-            # temporal scale for applying moving average on target values
-
-            desired_temporal_scale_level = scale_level_dict[scale] + 1
-            if desired_temporal_scale_level > 7:
-                raise Exception("The temporal scale level of the data is {0}. Thus the 'moving average' target_mode couldn't be applied cause the temporal scale bigger than {0} is ambiguous.\n".format(scale))
-
-             # get the nominal form of desired temporal scale level
-            desired_temporal_scale = list(scale_level_dict.keys())[list(scale_level_dict.values()).index(desired_temporal_scale_level)]
-            
-            if verbose > 0:
-                print("\nThe temporal scale level of the data is {0}, and using 'moving average' target_mode, the target value for each {0} is the average of values in the previous {1} of that {0}.\n".format(scale,desired_temporal_scale))
-
-            # get number of smaller temporal units in each bigger temporal unit
-            granularity = scale_second_units_number[desired_temporal_scale]//scale_second_units_number[scale]
-
-
-            data = data.sort_values(by = ['temporal id' , 'spatial id level 1']).copy()
-            data.reset_index(drop = True, inplace = True)
-            number_of_temporal_units=len(data['temporal id'].unique())
-            number_of_spatial_units=len(data['spatial id level 1'].unique())
-
-            transformed_data = pd.DataFrame(columns = data.columns)
-
-            while number_of_temporal_units >= granularity:
-
-                bigger_scale_unit_data = data.copy().tail(number_of_spatial_units*granularity) 
-                smaller_scale_unit_data = data.copy().tail(number_of_spatial_units)
-
-                # average of target values on last bigger temporal scale unit for all spatial scale units
-                bigger_scale_unit_data_average = bigger_scale_unit_data.groupby(['spatial id level 1']).mean().reset_index()
-                # add averaged target values of last bigger temporal scale unit to the smaller temporal scale unit
-                smaller_scale_unit_data.loc[:,('target')] = bigger_scale_unit_data_average.loc[:,('target')].tolist()
-
-                transformed_data = transformed_data.append(smaller_scale_unit_data)
-                # remove last smaller temporal scale unit for all spatial units from base data
-                data = data.iloc[:-(number_of_spatial_units),:]
-                number_of_temporal_units = number_of_temporal_units - 1
-
-            data = transformed_data.copy()
-            data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x : datetime.datetime.strftime(x,scale_format[scale]))
-            data = data.sort_values(by=['spatial id level 1','temporal id']).copy()
-        
-        ####################### non_integrated temporal id format
-        
-        elif temporal_identifier_column_name == 'dummy temporal id': 
-            
-            desired_scale_column_name = 'temporal id level ' + str(smallest_temporal_level+1)
-            if desired_scale_column_name not in data.columns:
-                raise Exception("The next bigger temporal scale after data current temporal scale (temporal scale level {0}) isn't included in the data or is located after a gap in the temporal scale levels sequence and is therefore ignored.\n".format(smallest_temporal_level))
-                
-            # get number of smaller temporal units in each bigger temporal unit
-            granularity = data.groupby(['spatial id level 1',desired_scale_column_name]).count()['dummy temporal id'].max()
-
-            data = data.sort_values(by = ['dummy temporal id' , 'spatial id level 1']).copy()
-            data.reset_index(drop = True, inplace = True)
-            number_of_temporal_units=len(data['dummy temporal id'].unique())
-            number_of_spatial_units=len(data['spatial id level 1'].unique())
-
-            transformed_data = pd.DataFrame(columns = data.columns)
-
-            while number_of_temporal_units >= granularity:
-
-                bigger_scale_unit_data = data.copy().tail(number_of_spatial_units*granularity) 
-                smaller_scale_unit_data = data.copy().tail(number_of_spatial_units)
-
-                # average of target values on last bigger temporal scale unit for all spatial scale units
-                bigger_scale_unit_data_average = bigger_scale_unit_data.groupby(['spatial id level 1']).mean().reset_index()
-                # add averaged target values of last bigger temporal scale unit to the smaller temporal scale unit
-                smaller_scale_unit_data.loc[:,('target')] = bigger_scale_unit_data_average.loc[:,('target')].tolist()
-
-                transformed_data = transformed_data.append(smaller_scale_unit_data)
-                # remove last smaller temporal scale unit for all spatial units from base data
-                data = data.iloc[:-(number_of_spatial_units),:]
-                number_of_temporal_units = number_of_temporal_units - 1
-
-            data = transformed_data.sort_values(by=['spatial id level 1','dummy temporal id']).copy()
-            
-    elif target_mode == 'normal':
-        data = data
-    else:
-        raise ValueError("The specified target_mode is not recognized. The supported target_modes are:\n{'normal', 'cumulative', 'differential', 'moving average'}")
-    
-    data = pd.merge(data,
-            normal_target_df[normal_target_df[temporal_identifier_column_name].isin(data[temporal_identifier_column_name].unique())],
-            on = ['spatial id level 1', temporal_identifier_column_name], how = 'inner')
-    
-    if 'dummy temporal id' in data.columns:
-        data.drop(['dummy temporal id'], axis = 1, inplace = True)
-    
-    data = rename_columns(data.copy(), column_identifier, 'deformalize', keep_target = True)
-        
-    return data
-
-
-#########################################################################################
-############################  making historical data ####################################
-#########################################################################################
-
-
-def make_historical_data(data, forecast_horizon, history_length = 1, column_identifier = None,
-                         futuristic_covariates = None, future_data_table = None, step = 1, verbose = 0):
-    
-    future_data = True
-    if type(data) != dict :
-        if type(data) == str :
-            try:
-                data = pd.read_csv(data)
-            except FileNotFoundError:
-                raise FileNotFoundError("File '{0}' does not exist.\n".format(data))
-        elif type(data) != pd.DataFrame :
-            raise TypeError("The input data must be of type DataFrame, string, or a dict containing temporal and spatial DataFrames or addresses.\n")
-        data = rename_columns(data.copy(), column_identifier)
-        
-        check_validity(data.copy(), input_name = 'data', data_type = 'full', column_identifier = column_identifier)
-
-    elif type(data) == dict:
-        if 'temporal_data' in data.keys():
-            
-            if type(data['temporal_data']) == str:
-                try:
-                    temporal_data = pd.read_csv(data['temporal_data'])
-                except FileNotFoundError:
-                    raise FileNotFoundError("File '{0}' does not exist.\n".format(data['temporal_data']))
-                    
-            elif type(data['temporal_data']) == pd.DataFrame:
-                temporal_data = data['temporal_data']
-            else:
-                raise ValueError("The value of the 'temporal id' key in the data dictionary must be a DataFrame or the address of temporal data.\n")
-            temporal_data = rename_columns(temporal_data.copy(), column_identifier)
-            check_validity(temporal_data.copy(), input_name = 'temporal_data', 
-                           data_type = 'temporal', column_identifier = column_identifier)
-            
-        else:
-            raise Exception("The data on temporal covariates and target variable must be passed to the function using data argument and as a DataFrame, Data address or value of 'temporal_data' key in the dictionary of data. But none is passed.\n")
-        
-
-        if ('spatial_data' in data.keys()) and (data['spatial_data'] is not None):
-            
-            if type(data['spatial_data']) == str:
-                try:
-                    spatial_data = pd.read_csv(data['spatial_data'])
-                except FileNotFoundError:
-                    raise ("File '{0}' does not exist.\n".format(data['spatial_data']))
-                    
-            elif type(data['spatial_data']) == pd.DataFrame:
-                spatial_data = data['spatial_data']
-            else:
-                raise ValueError("The value of the 'spatial id' key in the data dictionary must be a DataFrame or the address of spatial data.\n")
-            
-            spatial_data = rename_columns(spatial_data.copy(), column_identifier)
-            check_validity(spatial_data.copy(), input_name = 'spatial_data',
-                           data_type = 'spatial', column_identifier = column_identifier)
-            
-            if len(list(set(temporal_data['spatial id level 1'].unique())-set(spatial_data['spatial id level 1'].unique())))>0:
-                print("\nWarning: Some of the spatial units in the temporal_data, are not recorded in the spatial_data. These spatial units will be ignored.\n")
-                temporal_data = temporal_data[temporal_data['spatial id level 1'].isin(spatial_data['spatial id level 1'].unique())]
-                
-            data = pd.merge(temporal_data, spatial_data, on = 'spatial id level 1', how = 'left')
-            
-        else:
-            data = temporal_data.copy()
-    
-    # Non_integrated temporal id format
-    if 'temporal id' not in data.columns: 
-            # find smallest temporal level
-            for level in range(1,200):
-                if 'temporal id level ' + str(level) in data.columns:
-                    smallest_temporal_level = level
-                    break
-            # add integrated temporal id
-            data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
-            # remove discrete temporal id columns
-            extra_temporal_ids = list(filter(lambda x:x.startswith('temporal id level '), data.columns))
-            data.drop(extra_temporal_ids, axis = 1, inplace = True)
-            data.rename(columns = {'dummy temporal id':'temporal id'}, inplace = True)
-            
-            
-    if 'target' not in data.columns:
-        raise ValueError("There is no column named 'target' in input data")
-    
-    if column_identifier is None:
-        spatial_covariates = list(filter(lambda x:x.startswith('spatial covariate'), data.columns))
-        temporal_covariates = list(filter(lambda x:x.startswith('temporal covariate'), data.columns))
-    else:
-        if 'spatial covariates' in column_identifier.keys():
-            spatial_covariates = [item for item in list(column_identifier['spatial covariates']) if item in data.columns]
-        else: spatial_covariates = []
-        temporal_covariates = [item for item in list(column_identifier['temporal covariates']) if item in data.columns]
-        
-    all_covariates = list(filter(lambda x: not x.startswith(('temporal id', 'spatial id', 'target', 'Normal target')), data.columns))
-    extra_columns = list(set(all_covariates)-set(spatial_covariates + temporal_covariates))
-    
-    if len(extra_columns) > 0 :
-        print("\nWarning: Input data column names must match one of the specified formats:\n{'temporal id', 'temporal id level x', 'spatial id', 'spatial id level x', 'temporal covariate x', 'spatial covariate x', 'target'}, or be specified in column_identifier.\n")
-        print("But the names of some of the columns do not match any of the supported formats and is not mentioned in column_identifier:\n{0}\nThis columns will be ignored.\n".format(extra_columns))
-    
-    ######################## check type of future_data_table
-    
-    if type(future_data_table) == str:
-        try:
-            future_data_table = pd.read_csv(future_data_table)
-        except FileNotFoundError:
-            raise ("File '{0}' does not exist.\n".format(future_data_table))
-            
-    elif (type(future_data_table) != pd.DataFrame) and (future_data_table is not None):
-        raise TypeError("The future_data_table must be a data frame or address of the data frame containing the values of futuristic covariates in the future.")
-    
-            
-    ######################## check type and validity of input history_length and futuristic_covariates #####################
-    if type(history_length) == int:
-        if history_length == 0 : history_length = 1
-        history_length_dict = {covar:history_length for covar in temporal_covariates}
-        max_history_length = history_length # maximum history length of all temporal covariates
-        
-    elif type(history_length) == dict:
-        
-        key_list = list(history_length.keys())
-        for item in key_list:
-            if type(item) == tuple:
-                for key in item:
-                    history_length[key] = history_length[item]
-                del history_length[item]
-            
-        extra_hist_covariates = list(set(history_length.keys()) - set(temporal_covariates))
-        
-        if (len(extra_hist_covariates) > 0) and (verbose > 0):
-            print("\nWarning: The following keys in the history_length do not exist in the input data temporal covariates, and thus will be ignored:\n{0}\n".format(extra_hist_covariates))
-        
-        history_length = {key:value for key, value in history_length.items() if key not in extra_hist_covariates}
-        # The history length of 0 is interpreted to no historical values which is same as history length = 1
-        for key, value in history_length.items():
-            if value == 0: history_length[key] = 1
-        
-        history_length_dict = history_length.copy()
-        
-        # if covariate doesnt mentioned in history_length or futuristic_covariates
-        unspecified_history_covariates = list(set(temporal_covariates)-set(history_length_dict.keys()))
-        if (futuristic_covariates is not None) and (type(futuristic_covariates) == dict):
-            unspecified_history_covariates = list(set(unspecified_history_covariates) - set(futuristic_covariates.keys()))
-            
-        if len(unspecified_history_covariates)> 0:
-            print("\nWarning: The history length of some temporal covariates is not specified in history_length:\n{0}\nFor these covariates the history length of 1 will be considered.\n".format(unspecified_history_covariates))
-        for covar in unspecified_history_covariates:
-            history_length_dict[covar] = 1
-        for covar in history_length_dict.keys():
-            if type(history_length_dict[covar]) != int:
-                raise ValueError("The specified history length for each covariate in the history_length dict must be of type int.\n")
-        max_history_length = max(history_length_dict.values())
-        
-    else:
-        raise TypeError("The history_length must be of type int or dict.\n")
-        
-    if futuristic_covariates is not None:
-        if type(futuristic_covariates) == dict:
-            for covar in futuristic_covariates.keys():
-                if (len(futuristic_covariates[covar])!=2) or (futuristic_covariates[covar][1]-futuristic_covariates[covar][0]<0):
-                    raise ValueError("The temporal interval of each futuristic covariate must be specified in futuristic_covariates dict using a list including start and end of the interval as first and second item.\n")
-                elif (type(futuristic_covariates[covar][0])!=int)or(type(futuristic_covariates[covar][1])!=int):
-                    raise ValueError("The start and end point of futuristic covariates temporal interval must be of type int.\n")
-                elif futuristic_covariates[covar][1] > forecast_horizon:
-                    raise ValueError("The end point of futuristic covariates temporal interval must be smaller than forecast_horizon.\n")
-                else:
-                    history_length_dict['future '+covar] = futuristic_covariates[covar][1] - futuristic_covariates[covar][0] + 1
-
-        else:
-            raise TypeError("The futuristic_covariates must be of type dict.\n")
-        
-        key_list = list(futuristic_covariates.keys())
-        for item in key_list:
-            if type(item) == tuple:
-                for key in item:
-                    futuristic_covariates[key] = futuristic_covariates[item]
-                del futuristic_covariates[item]
-            
-        invalid_futuristic_covariates = list(set(futuristic_covariates.keys()) - set(temporal_covariates))
-        
-        if (len(invalid_futuristic_covariates) > 0) and (verbose > 0):
-            print("\nWarning: The following keys in the futuristic_covariates do not exist in the input data temporal covariates, and thus will be ignored:\n{0}\n".format(invalid_futuristic_covariates))
-        
-        futuristic_covariates = {key:value for key, value in futuristic_covariates.items() if key not in invalid_futuristic_covariates}
-        
-    ######################## check type and validity of forecast horizon
-    
-    if type(forecast_horizon) != int:
-        raise TypeError("The forecast_horizon must be of type int.")
-    elif forecast_horizon == 0:
-        forecast_horizon = 1
-    
-    ############## preparing data
-    
-    # adding future values of futuristic covariates to the data
-    if future_data_table is not None:
-        data, future_data_table, futuristic_temporal_units = current_future(data = data.copy(), future_data_table = future_data_table,
-                                                              futuristic_covariates = futuristic_covariates,
-                                                              column_identifier = column_identifier , mode = 'add')
-    else:
-        _, _, futuristic_temporal_units = current_future(data = data.copy(),
-                                                              future_data_table = None,
-                                                              futuristic_covariates = futuristic_covariates,
-                                                              column_identifier = column_identifier , mode = 'split')
-    
-    
-    number_of_futuristic_temporal_units = len(futuristic_temporal_units)
-    data = data.drop_duplicates(subset = ['temporal id','spatial id level 1']).copy()
-    data = data.sort_values(by = ['temporal id','spatial id level 1']).copy()
-    
-    ####################################### main part #######################################
-
-    if verbose > 0:
-        if type(history_length) == int :
-            print("\nMaking historical data with the forecast horizon of {0} and history length of {1} is running.\n".format(forecast_horizon, history_length))
-        else:
-            print("\nMaking historical data with the forecast horizon of {0} is running.\n".format(forecast_horizon))
-        
-    result = pd.DataFrame()  # we store historical data in this dataframe
-    total_number_of_spatial_units = len(data['spatial id level 1'].unique())
-    total_number_of_temporal_units = len(data['temporal id'].unique())
-    
-    if total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)) <= 0:
-        if verbose > 0 :
-            print("\nWarning: The specified history length and forecast horizon is too large for the number of recorded temporal units in the input data.\n")
-        return None
-    
-    if futuristic_covariates is None:
-        futuristic_covariates = {}
-    
-    # in this loop we make historical data
-    for covar in all_covariates:
-        # if covariate is time dependant
-        if covar in temporal_covariates:
-            
-            
-            temporal_data_frame = data[[covar]] # selecting column of the covariate that is being processed
-            # shift data to the size of futuristic temporal interval end point
-            if covar in futuristic_covariates.keys():
-                covar_history_length = history_length_dict['future '+covar]
-                threshold = futuristic_covariates[covar][0]
-    
-                while threshold != futuristic_covariates[covar][1]+1:
-                    temp = temporal_data_frame.tail((total_number_of_temporal_units + (step*(- max_history_length - threshold + 1)))*total_number_of_spatial_units).reset_index(drop=True)
-                    temp.rename(columns={covar: (covar.replace(' ','_') + ' t+' + str(threshold))}, inplace=True) # renaming column
-                    result = pd.concat([result, temp], axis=1)
-                    threshold += 1
-                
-            if covar in history_length_dict.keys():    
-                covar_history_length = history_length_dict[covar]
-                # the first temporal unit of historical data is determined based on the maximum history length of covariates
-                # therefore data of covariates with smaller history length should be shifted forward
-                if covar_history_length < max_history_length:
-                    temporal_data_frame = temporal_data_frame.iloc[(step*(max_history_length-covar_history_length))*total_number_of_spatial_units:]
-
-                threshold = 0
-                while threshold != covar_history_length:
-
-                    # if future_data is true, the feature values of the last temporal units with the size of 
-                    # forecast_horizon (which their target variable values are unknown) will be considered in historical data
-                    if future_data == False:
-                        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
-                    else:
-                        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
-
-                    temp.rename(columns={covar: (covar.replace(' ','_') + ' t-' + str(covar_history_length-threshold-1))}, inplace=True) # renaming column  
-
-                    result = pd.concat([result, temp], axis=1)
-                    # deleting the values in first day in temporal_data_frame dataframe (similiar to shift)
-                    temporal_data_frame = temporal_data_frame.iloc[step*total_number_of_spatial_units:]
-                    threshold += 1
-     
-        # if covariate is independant of time
-        elif covar in spatial_covariates:
-            
-            temporal_data_frame = data[[covar]]
-            if future_data == False:
-                temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
-            else:
-                temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
-            
-            temp.rename(columns={covar: (covar.replace(' ','_'))}, inplace=True)
-            if covar == 'Target':
-                temp.rename(columns={covar: ('Target_0')}, inplace=True)
-            result = pd.concat([result, temp], axis=1)
-    
-    # next 6 lines is for spatial id code to final dataframe
-    temporal_data_frame = data[['spatial id level 1']]
-    if future_data == False:
-        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
-    else:
-        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
-    result.insert(0, 'spatial id', temp)
-
-    # next 7 lines is for adding id of temporal unit (t) to final dataframe
-    temporal_data_frame = data[['temporal id']]
-    temporal_data_frame = temporal_data_frame[total_number_of_spatial_units*(step*(max_history_length - 1)):]
-    if future_data == False:
-        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
-    else:
-        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
-    result.insert(1, 'temporal id', temp)
-
-    # next 3 lines is for adding target to final dataframe
-    temporal_data_frame = data[['target']]
-    temporal_data_frame = temporal_data_frame.tail((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).reset_index(drop=True)
-    result.insert(2, 'Target', temporal_data_frame)
-
-    # next 4 lines is for adding normal target to final dataframe if target mode is not normal
-    if 'Normal target' in data.columns:
-        temporal_data_frame = data[['Normal target']]
-        temporal_data_frame = temporal_data_frame.tail((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).reset_index(drop=True)
-        result.insert(3, 'Normal target', temporal_data_frame)
-    
-    for i in result.columns:
-        if (i.endswith('t-0')) and (i not in spatial_covariates):
-            result.rename(columns={i: i[:-2]}, inplace=True)
-            
-    # last samples are related to the futuristic data and has no values for temporal covariates
-    # so must be removed from historical data
-    if number_of_futuristic_temporal_units > 0:
-        number_of_spatial_units = len(result['spatial id'].unique())
-        result = result.sort_values(by = ['temporal id', 'spatial id'])
-        result = result.iloc[:-(number_of_futuristic_temporal_units*number_of_spatial_units)]
-    
-    return result
-
-################################################################################################
-############################  base function data preprocess ####################################
-################################################################################################ 
-
-def preprocess_data(data, forecast_horizon, history_length = 1, column_identifier = None, spatial_scale_table = None,
-                    spatial_scale_level = 1, temporal_scale_level = 1,
-                    target_mode = 'normal', imputation = True, aggregation_mode = 'mean', augmentation = False,
-                    futuristic_covariates = None, future_data_table = None, save_address = None, verbose = 0):
-    
-    
-    
-    ####################
-    
-    spatial_covariates = []
-    temporal_covariates = []
-    granularity = None
-    target_granularity = None
-    
-    # prepare data (renaming columns, remove extra columns and get spatial and temporal data separately)
-    temporal_data, spatial_data = prepare_data(data.copy(), column_identifier)
-    
-    
-    #################### get list of covariates
-    
-    # if type of each column is specified in column_identifier
-    if column_identifier is not None:
-        temporal_covariates =  list(set(column_identifier['temporal covariates']) & set(temporal_data.columns))
-        if ('spatial covariates' in column_identifier.keys()) and (spatial_data is not None):
-            spatial_covariates =  list(set(column_identifier['spatial covariates']) & set(spatial_data.columns))
-
-    # if type of columns are clear based on column name
-    else:
-        temporal_covariates = list(filter(lambda x: x.startswith('temporal covariate'), temporal_data.columns))
-        if spatial_data is not None:
-            spatial_covariates = list(filter(lambda x: x.startswith('spatial covariate'), spatial_data.columns))
-
-    
-    # if input data has no covariate (spatial or temporal)
-    if len(temporal_covariates) == 0:
-        if (spatial_data is None) or (len(spatial_covariates) == 0):
-            raise ValueError("There is no spatial or temporal covariate included in input data")
-            
-    # if input data has no target
-    if 'target' not in temporal_data.columns:
-        raise ValueError("The target variable is not recorded in input data and doesn't specified in column_identifier.\nmissing column: 'target'")
-
-    ############## check the futuristic_covariate input validity
-    
-    if futuristic_covariates is not None:
-        if type(futuristic_covariates) == dict:
-            for item in futuristic_covariates.keys():
-                if (len(futuristic_covariates[item])!=2) or (futuristic_covariates[item][1]-futuristic_covariates[item][0]<0):
-                    raise ValueError("The temporal interval of each futuristic covariate must be specified in futuristic_covariates dict using a list including start and end of the interval as first and second item.\n")
-                elif (type(futuristic_covariates[item][0])!=int)or(type(futuristic_covariates[item][1])!=int):
-                    raise ValueError("The start and end point of futuristic covariates temporal interval must be of type int.\n")
-                elif futuristic_covariates[item][1] > forecast_horizon:
-                    raise ValueError("The end point of futuristic covariates temporal interval must be smaller than forecast_horizon.\n")
-        else:
-            raise TypeError("The futuristic_covariates must be of type dict.\n")
-            
-        key_list = list(futuristic_covariates.keys())    
-        for item in futuristic_covariates.keys():
-            if type(item) == tuple:
-                for key in item:
-                    futuristic_covariates[key] = futuristic_covariates[item]
-                del futuristic_covariates[item]
-
-            
-        # Removing invalid covariates from data and produce warning if is needed
-        invalid_futuristic_covariates = list(set(futuristic_covariates.keys()) - set(temporal_covariates))    
-        if (len(invalid_futuristic_covariates) > 0) and (verbose > 0):
-            print("\nWarning: The following keys in the futuristic_covariates do not exist in the input data covariates, and thus will be ignored:\n{0}\n".format(invalid_futuristic_covariates))
-
-        futuristic_covariates = {key:value for key, value in futuristic_covariates.items() if key not in invalid_futuristic_covariates}
-
-            
-    ############# check the history_length input validity
-    
-    if type(history_length) == dict :
-        for covar in history_length.keys():
-            if (type(history_length[covar]) != int) and (covar in temporal_covariates) :
-                  raise TypeError("\nThe maximum history length of covariates specified in history_length must be of type int.")
-                    
-        key_list = list(history_length.keys())
-        for item in key_list:
-            if type(item) == tuple:
-                for key in item:
-                    history_length[key] = history_length[item]
-                del history_length[item]
-            
-        extra_hist_covariates = list(set(history_length.keys()) - set(temporal_covariates))
-        
-        if (len(extra_hist_covariates) > 0) and (verbose > 0):
-            print("\nWarning: The following keys in the history_length do not exist in the input data temporal covariates, and thus will be ignored:\n{0}\n".format(extra_hist_covariates))
-        
-        history_length = {key:value for key, value in history_length.items() if key not in extra_hist_covariates}
-        
-    ######################## check type and validity of forecast horizon
-    
-    if type(forecast_horizon) != int:
-        raise TypeError("The forecast_horizon must be of type int.")
-    elif forecast_horizon == 0:
-        forecast_horizon = 1
-        
-    ######################## check type and temporal_scale_level and augmentation
-    
-    if (temporal_scale_level < 2) and (augmentation == True):
-        raise Exception("The augmentation can only be performed for temporal_scale_level greater than one.")
-        
-    ######################## check type of future_data_table
-    
-    if type(future_data_table) == str:
-        try:
-            future_data_table = pd.read_csv(future_data_table)
-        except FileNotFoundError:
-            raise FileNotFoundError("File '{0}' does not exist.\n".format(future_data_table))
-            
-    elif (type(future_data_table) != pd.DataFrame) and (future_data_table is not None):
-        raise TypeError("The future_data_table must be a data frame or address of the data frame containing the values of futuristic covariates in the future.")
-    
-    ############################## Imputation ##############################
-    
-    if imputation == True :
-        
-        # removing the rows related to the future data before imputation
-        if future_data_table is None:
-            temporal_data, future_data_table, _ = current_future(data = temporal_data.copy(), future_data_table = None,
-                                                              futuristic_covariates = futuristic_covariates,
-                                                              column_identifier = column_identifier , mode = 'split')
-        
-        if verbose > 0:
-            print("-"*45+"\nThe imputation of missing values is running.\n"+"-"*45+"\n")
-            
-        temporal_data = impute(temporal_data.copy(), None, verbose = 0)
-        if spatial_data is not None:
-            number_of_raw_spatial_units = spatial_data.shape[0]
-            spatial_data.dropna(inplace = True)
-            number_of_removed_spatial_units = number_of_raw_spatial_units - spatial_data.shape[0]
-
-            if number_of_removed_spatial_units == number_of_raw_spatial_units:
-                raise ValueError("All the spatial units include missing values for spatial covariates. Therefore, no spatial unit remains to make a prediction.\n")
-            elif number_of_removed_spatial_units > 0:
-                print('\nWarning: The number of {0} spatial units has missing values for spatial covariates and will be removed from the data.\n'.format(number_of_removed_spatial_units))
-
-        # Holding only the spatial units that are common in both data frames
-        if spatial_data is not None:
-            temporal_data = temporal_data[temporal_data['spatial id level 1'].isin(spatial_data['spatial id level 1'].unique())]
-            spatial_data = spatial_data[spatial_data['spatial id level 1'].isin(temporal_data['spatial id level 1'].unique())]
-    
-
-    
-    # adding future values of futuristic covariates to the data and get the futuristic temporal units
-    if future_data_table is not None:
-        temporal_data, future_data_table, futuristic_temporal_units = current_future(data = temporal_data.copy(), future_data_table = future_data_table,
-                                                              futuristic_covariates = futuristic_covariates,
-                                                              column_identifier = column_identifier , mode = 'add')
-    else:
-        _, _, futuristic_temporal_units = current_future(data = temporal_data.copy(),
-                                                              future_data_table = None,
-                                                              futuristic_covariates = futuristic_covariates,
-                                                              column_identifier = column_identifier , mode = 'split')
-    
-    ############################## spatial scale transform ##############################
-    
-    if spatial_scale_level > 1:
-        
-        if verbose > 0:
-            print("-"*65+"\nTransformation of data to the desired spatial scale is running.\n"+"-"*65+"\n")
-            
-        if type(aggregation_mode) == dict:
-            extra_covariates_listed = list(set(aggregation_mode.keys())-set(spatial_covariates + temporal_covariates + ['target']))
-            unspecified_covariates = list(set(spatial_covariates + temporal_covariates + ['target'])-set(aggregation_mode.keys()))
-
-            if len(extra_covariates_listed) > 0:
-                print("\nWarning : Some of the covariates specified in aggregation_mode are not exist in the data:\n{0}".format(extra_covariates_listed))
-                aggregation_mode = {covariate : mode for covariate,mode in aggregation_mode.items() if covariate not in extra_covariates_listed}
-
-            if len(unspecified_covariates)>0:
-                if verbose < 2:
-                    print("\nWarning : The aggregation_mode is not specified for some of the covariates.\nThe mean operator will be used to aggregate these covariates' values.\n")
-                if verbose == 2:
-                    print("\nWarning : The aggregation_mode is not specified for some of the covariates:\n{0}\nThe mean operator will be used to aggregate these covariates' values.\n".format(unspecified_covariates))
-                for covar in unspecified_covariates:
-                      aggregation_mode[covar] = 'mean'
-
-            if spatial_data is not None:
-                    spatial_aggregation_mode = {covariate : mode for covariate,mode in aggregation_mode.items() if covariate in spatial_covariates}
-
-            temporal_aggregation_mode = {covariate : mode for covariate,mode in aggregation_mode.items() if covariate in temporal_covariates + ['target']}
-
-        # if aggregation_mode is not dict and is same for all covariates           
-        else:
-            spatial_aggregation_mode = temporal_aggregation_mode = aggregation_mode
-            
-        if spatial_scale_table is not None:
-            spatial_scale_table = rename_columns(spatial_scale_table.copy(), column_identifier)
-        
-        # transformation
-        temporal_data = spatial_scale_transform(temporal_data.copy(), 'temporal', column_identifier = None, spatial_scale_table = spatial_scale_table, spatial_scale_level = spatial_scale_level, aggregation_mode = temporal_aggregation_mode, verbose = 0)
-        if spatial_data is not None:
-            spatial_data = spatial_scale_transform(spatial_data.copy(), 'spatial', column_identifier = None, spatial_scale_table = spatial_scale_table, spatial_scale_level = spatial_scale_level, aggregation_mode = spatial_aggregation_mode, verbose = 0)
-            # if the desired spatial scale has only one spatial unit, the spatial covariates couldn't be used for prediction
-            if len(spatial_data)==1:
-                spatial_data = None
-                print("\nWarning: The desired spatial scale has only one spatial unit in the data, so spatial covariates' values is same for all the data samples and couldn't be used for prediction.\n")
-        
-        # to pass the data to the other functions, it must be same as raw data 
-        spatial_identifier = list(filter(lambda x: x.startswith(('spatial id')),temporal_data.columns))[0]
-        temporal_data.rename(columns = {spatial_identifier:'spatial id level 1'}, inplace = True)
-        
-        if spatial_data is not None:
-            spatial_identifier = list(filter(lambda x: x.startswith(('spatial id')),spatial_data.columns))[0]
-            spatial_data.rename(columns = {spatial_identifier:'spatial id level 1'}, inplace = True)
-            
-    ############################## temporal scale transform ##############################
-    
-    if temporal_scale_level > 1:
-        
-        if verbose > 0:
-            print("-"*65+"\nTransformation of data to the desired temporal scale is running.\n"+"-"*65+"\n")
-            
-        # if user prefer to augment data granularity (number of smaller scale temporal units in the bigger scale temporal unit)
-        # will be needed for making historical data
-        if augmentation == True:
-            granularity = find_granularity(temporal_data.copy(), temporal_scale_level)
-            
-        # filling up the future temporal units null values with inf to recognize the future temporal units
-        # after temporal transform and return its values to null for non futuristic covariates
-        temporal_data = fill_future_nulls(data = temporal_data.copy(), futuristic_temporal_units = futuristic_temporal_units)
-        
-        # transformation
-        temporal_data = temporal_scale_transform(temporal_data.copy(), temporal_scale_level = temporal_scale_level, augmentation = augmentation, verbose = 0)
-        
-        # return null values of non futuristic covariates in future temporal units
-        temporal_data = temporal_data.replace([np.inf, -np.inf], np.nan)
-        
-        # to pass the data to the other functions, it must be same as raw data 
-        # the next lines reset the names of temporal id level columns to start from level one (only needed for non_integrated temporal id format)
-        if augmentation == False:
-
-            current_smallest_temporal_level = 'temporal id level '+str(temporal_scale_level)
-
-            # if non_integrated temporal id format       
-            if current_smallest_temporal_level in temporal_data.columns:
-                temporal_data.rename(columns = {current_smallest_temporal_level:'temporal id level 1'}, inplace = True)
-                for level in range(temporal_scale_level+1, 200):
-                    if 'temporal id level '+str(level) in temporal_data.columns:
-                        # shift the level by temporal_scale_level units
-                        shifted_level = level - temporal_scale_level + 1
-                        temporal_data.rename(columns = {'temporal id level '+str(level):'temporal id level '+str(shifted_level)}, inplace = True)
-                    else:
-                        break
-    ############################## target modification ##############################
-    
-    if (target_mode != 'normal') and (verbose > 0):
-            print("-"*35+"\nTarget modification is running.\n"+"-"*35+"\n")
-        
-    # removing the rows related to the future data before target modification cause it may fill the value of target in future
-    if future_data_table is None:
-        temporal_data, future_data_table, _ = current_future(data = temporal_data.copy(), future_data_table = None,
-                                                          futuristic_covariates = futuristic_covariates,
-                                                          column_identifier = column_identifier , mode = 'split')
-
-    if (target_mode == 'moving average'):
-        target_granularity = find_granularity(data = temporal_data.copy(), temporal_scale_level = None)
-
-    temporal_data = target_modification(temporal_data, target_mode = target_mode, verbose = 1)
-    
-    if future_data_table is not None:
-        temporal_data, future_data_table, _ = current_future(data = temporal_data.copy(), future_data_table = future_data_table,
-                                                              futuristic_covariates = futuristic_covariates,
-                                                              column_identifier = column_identifier , mode = 'add')
-              
-     
-    ############################## make historical data ##############################    
-    
-    if verbose > 0:
-        print("-"*35+"\nMaking historical data is running.\n"+"-"*35+"\n")
-        
-    # next lines is for detecting total number of temporal units in the data
-    # to produce warning if it is less than needed number
-    if 'temporal id' in temporal_data.columns:
-        total_number_of_temporal_units =  len(temporal_data['temporal id'].unique())
-    else: 
-        # add integrated temporal id
-        temporal_data = add_dummy_integrated_temporal_id(temporal_data.copy(), start_level = 1)
-        total_number_of_temporal_units =  len(temporal_data['dummy temporal id'].unique())
-        temporal_data = temporal_data.drop(['dummy temporal id'],axis = 1)    
-    
-    # if augmentation == True, for each sample in temporal unit i, if this sample is in index u,
-    # the next sample in temporal unit i+1 is placed in index u+granularity. so in making historical data,
-    # the step size to go back and get historical values of covariates or move forward to consider future 
-    # values of the target variable must be equal to the granularity
-                  
-    if augmentation == True:
-        step = granularity
-    else:
-        step = 1
-    
-    if type(history_length) == int:
-        
-        if total_number_of_temporal_units + (step*(- history_length - forecast_horizon + 1)) <= 0:
-            print("\nWarning: The specified history length and forecast horizon is too large for the number of recorded temporal units in the input data.\n")
-        
-        
-        # input data
-        if spatial_data is not None:
-            make_hist_data = {'temporal_data':temporal_data.copy(),'spatial_data':spatial_data.copy()}
-        else:
-            make_hist_data = {'temporal_data':temporal_data.copy(),'spatial_data':spatial_data}
-                
-        historical_data = make_historical_data(data = make_hist_data,
-                                               forecast_horizon = forecast_horizon, column_identifier = column_identifier,
-                                               history_length = history_length, futuristic_covariates = futuristic_covariates,
-                                               future_data_table = None, step = step, verbose = 0)
-        if historical_data is not None:
-            historical_data = recorrect_hist_data(historical_data, augmentation, granularity, target_mode, target_granularity)
-
-            if save_address is not None:
-                try:
-                    historical_data.to_csv(save_address+'historical_data h={0}.csv'.format(history_length))
-                except FileNotFoundError:
-                        print("The address '{0}' is not valid.".format(save_address))
-
-    elif type(history_length) == dict:
-        historical_data = {}
-        unspecified_covariate = []
-                  
-        for covar in temporal_covariates:
-            if covar not in history_length.keys():
-                if futuristic_covariates is None:
-                    history_length[covar] = 1
-                    unspecified_covariate.append(covar)
-                elif covar not in futuristic_covariates.keys():
-                    history_length[covar] = 1
-                    unspecified_covariate.append(covar)
-
-        if len(unspecified_covariate)>0:
-            if verbose < 2:
-                print("\nWarning: The maximum history length of some covariates is not specified in history_length. The history length of 1 will be considered for these covariates.\n")
-            elif verbose == 2:
-                print("\nWarning: The maximum history length of some covariates is not specified in history_length. The history length of 1 will be considered for these covariates:\n{0}\n".format(unspecified_covariate))
-        
-        # The max history length of 0 is interpreted to no historical values which is same as history length = 1
-        for key, value in history_length.items():
-            if value == 0: history_length[key] = 1
-                
-        current_history_length = {covar : 0 for covar in history_length.keys()} 
-        
-        max_history_length = max(history_length.values())
-        
-        impossible_histories = []
-        for hist in range(1,max_history_length+1):
-            if total_number_of_temporal_units + (step*(- hist - forecast_horizon + 1)) <= 0:
-                impossible_histories.append(hist)
-        if len(impossible_histories) > 0:
-            print("Warning: The number of temporal units in the data is not enough to construct a historical data with the specified forecast horizon and the history length(s):\n{0}".format(impossible_histories))
-        
-        for stage in range(1,max_history_length+1):
-            for covar in history_length.keys():
-                  if current_history_length[covar]+1 <= history_length[covar]:
-                        current_history_length[covar] = current_history_length[covar] + 1
-                        
-            # input data
-            if spatial_data is not None:
-                make_hist_data = {'temporal_data':temporal_data.copy(),'spatial_data':spatial_data.copy()}
-            else:
-                make_hist_data = {'temporal_data':temporal_data.copy(),'spatial_data':None}
-                
-            historical_data[stage] = make_historical_data(data = make_hist_data,
-                                                    forecast_horizon = forecast_horizon, column_identifier = column_identifier,
-                                                    history_length = current_history_length,
-                                                    futuristic_covariates = futuristic_covariates,
-                                                    future_data_table = None,
-                                                    step = step, verbose = 0)
-            
-            if historical_data[stage] is not None:
-                
-                historical_data[stage] = recorrect_hist_data(historical_data[stage], augmentation, granularity, target_mode, target_granularity)
-
-                if save_address is not None:
-                    try:
-                        historical_data[stage].to_csv(save_address+'historical_data h=' + str(stage) +'.csv', index = False)
-                    except FileNotFoundError:
-                            print("The address '{0}' is not valid.".format(save_address))
-                            
-        historical_data_list =  [value for key,value in historical_data.items()]
-        historical_data = historical_data_list
-        
-    return historical_data
-
-######################
-
-def plot_data(data, spatial_scale_table, temporal_covariate = 'default' ,spatial_scale = 1, spatial_id = None,
-              temporal_scale = 1, temporal_range = None, column_identifier = None, month_format_print=False,
-              saving_plot_path = None):
-    
-    ######################### check validity of input arguments    
-    if type(data) == str:
-        try:
-            data = pd.read_csv(data)
-        except FileNotFoundError:
-            raise FileNotFoundError("File '{0}' does not exist.\n".format(data))
-            
-    elif type(data) != pd.DataFrame:
-        raise TypeError("The input data must be of type DataFrame or string.")
-    
-    df = rename_columns(data, column_identifier)
-    check_validity(df.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier)
-    
-    if type(spatial_id) == list:
-        if len(spatial_id)>3 :
-            print("The number of spatial_ids must be a maximum of 3.")
-        spatial_id = spatial_id[:3]
-    elif spatial_id is not None:
-        raise TypeError("The spatial_id must be of type list.")
-    
-    ################## spatial scale transform #################
-    
-    if spatial_scale > 1:
-        
-        if spatial_scale_table is not None:
-            if type(spatial_scale_table) == str:
-                try:
-                    spatial_scale_table = pd.read_csv(spatial_scale_table)
-                except FileNotFoundError:
-                    raise FileNotFoundError("File '{0}' does not exist.\n".format(spatial_scale_table))
-            spatial_scale_table = rename_columns(spatial_scale_table.copy(), column_identifier)
-
-        df = spatial_scale_transform(df, 'temporal', spatial_scale_table = spatial_scale_table, spatial_scale_level = spatial_scale, aggregation_mode = 'mean')
-    
-    df.rename(columns = {'spatial id level '+str(spatial_scale):'spatial id level 1'},inplace = True)
-
-    ################ temporal scale transform #####################
-
-    if temporal_scale > 1:
-        df = temporal_scale_transform(df, column_identifier=None, temporal_scale_level = temporal_scale
-                                     , augmentation=False, verbose=1)
-
-
-    ################## select desired temporal interval for plot from data ###############
-    
-    if (type(temporal_range) != dict) and (temporal_range is not None):
-        raise TypeError("The temporal_range most be of type dict.")
-    
-    # if temporal id format is integrated
-    if 'temporal id' in df.columns:
-        temporal_identifier_column_name = 'temporal id'
-        
-        scale_format = {'sec':'%Y/%m/%d %H:%M:%S', 'min':'%Y/%m/%d %H:%M', 'hour':'%Y/%m/%d %H', 'day':'%Y/%m/%d', 'week':'%Y/%m/%d', 'month':'%Y/%m', 'year':'%Y'}
-
-        # determining input data temporal scale and transforming temporal id's to timestamp
-        df , scale = check_integrated_temporal_id(df)
-        
-        if temporal_range is not None:
-            
-            first_day = temporal_range['temporal id'][0]
-            last_day = temporal_range['temporal id'][1]
-            # get first_day and last_day timestamp
-            first_day = datetime.datetime.strptime(first_day,scale_format[scale])
-            last_day = datetime.datetime.strptime(last_day,scale_format[scale])
-            df = df[(df['temporal id']>=first_day)&(df['temporal id']<=last_day)]
-
-        if month_format_print == True:
-            df['temporal id'] = df['temporal id'].apply(lambda x:datetime.datetime.strftime(x,'%Y/%B/%d'))
-        else:
-            df['temporal id'] = df['temporal id'].apply(lambda x:datetime.datetime.strftime(x,scale_format[scale]))
-
-    # if temporal id format is non_integrated  
-    else:
-        
-        if temporal_range is not None:
-            for temporal_id_level , interval in temporal_range.items():
-                df = df[(df[temporal_id_level]>=interval[0])&(df[temporal_id_level]<=interval[1])]
-
-        ##### month name for non-integrated ###############
-        
-        if month_format_print==True:
-          if column_identifier is not None:
-            for values in column_identifier.values():
-                if values == 'month':
-                    month_index = [*column_identifier.values()].index(values)
-                    temporal_id_x = [*column_identifier.keys()][month_index]
-            try:
-                df[temporal_id_x] = df[temporal_id_x].apply(lambda x : calendar.month_name[x])
-            except(IndexError,TypeError):
-                pass
-            
-        ##### next 5 lines add dummy temporal id for non_integrated temporal id format
-        
-        if temporal_range is not None:
-            list_to_find_smallest_scale = temporal_range.keys()
-        else:
-            list_to_find_smallest_scale = df.columns
-        
-        # determine smallest temporal id level
-        for level in range(1,200):
-            if 'temporal id level '+str(level) in list_to_find_smallest_scale:
-                smallest_temporal_level = level
-                break
-
-        add_dummy_integrated_temporal_id(df, start_level = level)        
-        temporal_identifier_column_name = 'dummy temporal id'       
-
-        
-    ############ select desired spatial id #########
-    
-    # select random spatial ids if spatial id input is not specified
-    if spatial_id is None:
-        df_spatial_id_values = list(df['spatial id level 1'].unique())
-        spatial_id = list([df_spatial_id_values[0]])
-    
-    df_dict = {}
-    
-    for j in range(int(len(spatial_id))):
-        df0=df['spatial id level 1'] == spatial_id[j]
-        df1 = df[df0]
-        dict_key = spatial_id[j]
-        df_dict[dict_key] = df1
-    
-    ############ making plot ################
-
-    if temporal_covariate == 'default':
-        T_C = df1.keys().tolist()
-        T_C = list(filter(lambda x: not x.startswith(('temporal id','spatial id','dummy temporal id')), T_C))
-
-    else:
-        T_C=[temporal_covariate]
-
-    for par in T_C:
-
-        fig, ax = plt.subplots()
-        for SpatialId, DF in df_dict.items():
-            y = DF[par].tolist()
-            time = DF[temporal_identifier_column_name].tolist()
-            total_temporal_id_number = len(time) + 2
-            plt.plot(time, y, label=SpatialId, linewidth=1.0, marker='o', markersize=5)
-
-        # plt.xlabel('time')
-        plt.legend()
-        plt.ylabel(temporal_covariate)
-        plt.gcf().autofmt_xdate()
-        plt.ylabel(par)
-
-        # plt.grid()
-
-        default_xtick_size = plt.gcf().get_size_inches()[0]
-        plt.gca().margins(x=0.002)
-        plt.gcf().canvas.draw()
-        tl = plt.gca().get_xticklabels()
-        maxsize = max([t.get_window_extent().width for t in tl])
-        inch_margin = 0.5  # inch margin
-        xtick_size = maxsize / plt.gcf().dpi * total_temporal_id_number + inch_margin
-        margin = inch_margin / plt.gcf().get_size_inches()[0]
-
-        plt.gcf().subplots_adjust(left=margin, right=1. - margin)
-        if default_xtick_size < xtick_size:
-            plt.gcf().set_size_inches(xtick_size, plt.gcf().get_size_inches()[1])
-        ax.spines['top'].set_visible(False)
-        ax.spines['right'].set_visible(False)
-        plt.margins(0.1)
-        plt.subplots_adjust(bottom=0.15)
-        figure_to_save = plt.gcf()
-        plt.show()
-        
-        if saving_plot_path is not None:
-            try:
-                figure_to_save.savefig(saving_plot_path + par +' evolution.png', bbox_inches='tight')
-            except FileNotFoundError:
-                print("The address '{0}' is not valid.".format(saving_plot_path))
-        plt.close()
+import warnings
+
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    import pandas as pd
+    import numpy as np
+    import sys
+    import datetime
+    from sklearn.impute import KNNImputer
+    
+    import matplotlib.pyplot as plt
+    import calendar
+    from statsmodels.tsa.ar_model import AutoReg
+    from statsmodels.tsa.stattools import adfuller
+    import statsmodels.api as sm
+
+
+###################### renaming the columns to formal format
+
+def rename_columns(data,column_identifier, mode = 'formalize', error = 1):
+
+    if type(column_identifier) == dict:
+        if (any([key not in list(column_identifier.keys()) for key in ['target','temporal covariates']])) and (error == 1):
+            raise ValueError("The target and temporal covariates are not specified in column_identifier.")
+
+        if 'temporal covariates' in list(column_identifier.keys()):
+            temporal_covariates = column_identifier['temporal covariates']
+        else:
+            temporal_covariates = []
+
+        if mode == 'formalize':
+            for key, value in column_identifier.items():
+                if key not in ['temporal covariates','spatial covariates']:
+                    if (key == 'target') and (value in temporal_covariates) and (value in data.columns):
+                        if 'target' not in data.columns:
+                            data.loc[:,('target')] = list(data[value])
+                    else:
+                        data.rename(columns = {value:key}, inplace = True)
+        elif mode == 'deformalize':
+            for key, value in column_identifier.items():
+                if key not in ['temporal covariates','spatial covariates']:
+                    if (key == 'target') and (value in temporal_covariates) and (value in data.columns):
+                        data = data.drop(['target'],axis = 1)
+                    else:
+                        data.rename(columns = {key:value}, inplace = True)
+
+    elif column_identifier is not None:
+        raise TypeError("The column_identifier must be of type dict")
+
+    return data
+
+###################### check validity of input data
+
+def check_validity(data, input_name = 'temporal_data', data_type = 'temporal', column_identifier = None, error = 1):
+# data argument could accept temporal_data, full_data, spatial_data, spatial_scale_table or future_data_table
+# the type will be determined based on data_type argument and the input_name argument will
+# be used to produce more clear warning errors
+
+    if 'spatial id level 1' not in data.columns:
+        if data_type != 'spatial_scales':
+            raise Exception("The input {0} has no spatial id column, and the name of this column is not specified in the column_identifier.\nmissing column: 'spatial id level 1'".format(input_name))
+        else:
+            raise Exception("The input {0} has no spatial id column.\nmissing column: 'spatial id level 1'".format(input_name))
+
+    else:
+        # check for null values
+        for i in range(1,200):
+            column_name = 'spatial id level ' + str(i)
+            if column_name in data.columns:
+                if data[column_name].isnull().values.any():
+                    raise ValueError('spatial id must have value for all instances but spatial id level '+str(i)+' in {0} includes NULL values'.format(input_name))
+            else: break
+
+    if data_type in ['temporal','full']:
+
+        if 'temporal id' in data.columns: # integrated temporal id format
+            temporal_identifier_column_name = 'temporal id'
+            if data[temporal_identifier_column_name].isnull().values.any():
+                    raise ValueError('temporal id must have value for all instances but temporal id column in {0} includes NULL values'.format(input_name))
+
+        elif 'temporal id level 1' in data.columns: # non-integrated temporal id format
+            data = add_dummy_integrated_temporal_id(data.copy())
+            temporal_identifier_column_name = 'dummy temporal id'
+        else:
+            raise Exception("The input {0} has no temporal id column, and the name of this column is not specified in the column_identifier.\nmissing column: 'temporal id' or 'temporal id level 1'".format(input_name))
+
+        data = data.drop_duplicates(subset = ['spatial id level 1',temporal_identifier_column_name]).copy()
+
+        if len(data) != len(data['spatial id level 1'].unique())* len(data[temporal_identifier_column_name].unique()):
+            raise ValueError("The input {0} has different number of temporal units recorded for each spatial unit".format(input_name))
+        if 'dummy temporal id' in data.columns:
+            data.drop(['dummy temporal id'], axis = 1, inplace = True)
+
+    numerical_columns = []
+    if column_identifier is None:
+        numerical_columns = list(filter(lambda x: x.startswith(('temporal covariate','spatial covariate','target')),data.columns))
+    elif all([key in list(column_identifier.keys()) for key in ['target','spatial covariates','temporal covariates']]):
+        numerical_columns = list(filter(lambda x: x in(['target']+column_identifier['spatial covariates']+column_identifier['temporal covariates']),data.columns))
+    elif all([key in list(column_identifier.keys()) for key in ['target','temporal covariates']]):
+        numerical_columns = list(filter(lambda x: x in(['target']+column_identifier['temporal covariates']),data.columns))
+    elif error == 1:
+        raise ValueError("The target and temporal covariates are not specified in column_identifier.")
+
+    for covar in numerical_columns:
+        try:
+            data[covar].astype(float)
+        except (ValueError, TypeError):
+            raise ValueError("The covariates and target variable must include only numerical values. But non-numerical values are recorded for the {0}".format(covar))
+    return
+
+############################ rename the columns of final historical data
+
+def recorrect_hist_data(data, augmentation, granularity, target_mode, target_granularity):
+
+    # name of target mode
+    target_column_name = 'Target'
+    if augmentation == True:
+        target_column_name = 'Target (augmented with {0} units)'.format(granularity)
+        data = data.rename(columns={'Target':target_column_name})
+
+    if target_mode in ['differential', 'cumulative', 'normal']:
+        data = data.rename(columns={target_column_name:'{0} ({1})'.format(target_column_name, target_mode)})
+        target_column_name = '{0} ({1})'.format(target_column_name, target_mode)
+
+    if target_mode == 'moving average':
+        data = data.rename(columns={target_column_name:'{0} (moving average on {1} units)'.format(target_column_name, target_granularity)})
+        target_column_name = '{0} (moving average on {1} units)'.format(target_column_name, target_granularity)
+
+    data = data.rename(columns={target_column_name:target_column_name.replace(') (',' - ')})
+
+    return data
+
+############################ adding or separating the values of futuristic covariates (future_data_table) to the data
+
+def current_future(data, future_data_table, futuristic_covariates, column_identifier , mode):
+    '''
+    mode = 'split' or 'add'
+    '''
+    if futuristic_covariates == None:
+        return data, None, []
+
+    futuristic_covariate_list = list(futuristic_covariates.keys())
+
+    data = rename_columns(data.copy(), column_identifier)
+    check_validity(data.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier)
+
+    if column_identifier is None:
+        spatial_covariates = list(filter(lambda x:x.startswith('spatial covariate'), data.columns))
+        temporal_covariates = list(filter(lambda x:x.startswith('temporal covariate'), data.columns))
+    else:
+        if 'spatial covariates' in column_identifier.keys():
+            spatial_covariates = [item for item in list(column_identifier['spatial covariates']) if item in data.columns]
+        else: spatial_covariates = []
+        temporal_covariates = [item for item in list(column_identifier['temporal covariates']) if item in data.columns]
+
+    id_columns = list(filter(lambda x: x.startswith(('spatial id','temporal id')),data.columns))
+    spatial_id_columns = list(filter(lambda x: x.startswith(('spatial id')),data.columns))
+    temporal_id_columns = list(filter(lambda x: x.startswith(('temporal id')),data.columns))
+    target_columns = ['target']
+    if 'Normal target' in data.columns:
+        target_columns = target_columns + ['Normal target']
+
+    spatial_data = None
+    temporal_data = data[id_columns + temporal_covariates + target_columns]
+    if len(spatial_covariates) > 0:
+        # if input 'data' is full data, data on spatial covariates is saved to add to the data at the end of the process
+        if len(list(set(spatial_covariates) - set(data.columns))) == 0 :
+            spatial_data = data[spatial_id_columns + spatial_covariates].drop_duplicates(subset = spatial_id_columns)
+
+
+    if future_data_table is not None:
+        future_data_table = rename_columns(future_data_table.copy(), column_identifier)
+        check_validity(future_data_table.copy(), input_name = 'future_data_table',
+                       data_type = 'temporal', column_identifier = column_identifier)
+
+        for col in id_columns:
+            if col not in future_data_table.columns :
+                raise ValueError("The temporal and spatial id columns must be identical in the future_data_table and the input data.")
+
+        extra_columns = (set(future_data_table.columns)-set(id_columns)-set(futuristic_covariate_list))
+        if len(extra_columns) > 0: print("\nWarning: some of the columns in the future_data_table are not in the futuristic_covariates and will be ignored.")
+        unspecified_columns = (set(futuristic_covariate_list)-(set(future_data_table.columns)-set(id_columns)))
+        if len(unspecified_columns) > 0:raise Exception("Some of the futuristic covariates in the futuristic_covariates dict are not included in the future_data_table.")
+
+    if 'temporal id' in temporal_data.columns:
+        temporal_identifier_column_name = 'temporal id'
+        non_futuristic_covariates = list(set(temporal_data.columns) - set(futuristic_covariate_list + spatial_id_columns + ['temporal id']))
+
+
+    else: # non-integrated temporal id format
+        for level in range(1,200):
+            if 'temporal id level ' + str(level) in temporal_data.columns:
+                smallest_temporal_level = level
+                break
+        temporal_data = add_dummy_integrated_temporal_id(temporal_data.copy(), start_level = smallest_temporal_level)
+        if future_data_table is not None:
+            future_data_table = add_dummy_integrated_temporal_id(future_data_table.copy(), start_level = smallest_temporal_level)
+        temporal_identifier_column_name = 'dummy temporal id'
+        non_futuristic_covariates = list(set(temporal_data.columns) - set(futuristic_covariate_list + spatial_id_columns + ['dummy temporal id'] + temporal_id_columns))
+
+
+    if mode == 'split':
+
+        temporal_data = temporal_data.drop_duplicates(subset = ['spatial id level 1', temporal_identifier_column_name]).copy()
+        temporal_data = temporal_data.sort_values(by = [temporal_identifier_column_name,'spatial id level 1'])
+
+        temporal_data['...'] = list(range(len(temporal_data))) # add an unique id to the data frame
+
+        current_data = temporal_data.dropna(subset = non_futuristic_covariates, how='all')
+        current_data_index = list(current_data['...'])
+        future_data = temporal_data[~(temporal_data['...'].isin(current_data_index))]
+        temp = future_data.groupby([temporal_identifier_column_name]).count()
+
+        # remove dates which is not compeletly missed the non_futuristic_covariates (are not related to the future data)
+        total_number_of_spatial_ids = temp['spatial id level 1'].max()
+        incomplete_dates = temp[temp['spatial id level 1'] < total_number_of_spatial_ids].index
+
+        future_data = future_data[~(future_data[temporal_identifier_column_name].isin(incomplete_dates))]
+        current_data = temporal_data[~(temporal_data['...'].isin(future_data['...']))]
+
+        futuristic_temporal_units = list(future_data[temporal_identifier_column_name].unique())
+        future_data_table_columns = id_columns + futuristic_covariate_list
+        future_data_table = future_data[future_data_table_columns]
+
+        if 'dummy temporal id' in current_data.columns:
+            current_data = current_data.drop(['dummy temporal id','...'], axis = 1)
+        else:
+            current_data = current_data.drop(['...'], axis = 1)
+
+        if len(future_data_table) == 0 :
+            future_data_table = None
+
+        if spatial_data is not None:
+            current_data = pd.merge(current_data, spatial_data, on = 'spatial id level 1', how = 'left')
+
+        return current_data, future_data_table, futuristic_temporal_units
+
+    if mode == 'add':
+        for col in non_futuristic_covariates:
+            future_data_table.loc[:,(col)] = np.NaN
+        future_data_table = future_data_table[list(temporal_data.columns)]
+
+        future_data_table = future_data_table[future_data_table['spatial id level 1'].isin(temporal_data['spatial id level 1'].unique())]
+
+        future_data_table = future_data_table[future_data_table[temporal_identifier_column_name]>max(temporal_data[temporal_identifier_column_name])]
+
+        temporal_data = pd.concat([temporal_data,future_data_table], axis=0, join='outer')
+
+        temporal_data.sort_values(by = [temporal_identifier_column_name, 'spatial id level 1'])
+        if 'dummy temporal id' in temporal_data.columns:
+            temporal_data = temporal_data.drop(['dummy temporal id'], axis = 1)
+
+        futuristic_temporal_units = list(future_data_table[temporal_identifier_column_name].unique())
+
+        if spatial_data is not None:
+            data = pd.merge(temporal_data, spatial_data, on = 'spatial id level 1', how = 'left')
+        else: data = temporal_data
+
+        return data, None, futuristic_temporal_units
+
+
+############################ filling up the future temporal units null values with inf to recognize them later
+
+def fill_future_nulls(data, futuristic_temporal_units):
+        if 'temporal id' in data.columns:
+            temporal_identifier_column_name = 'temporal id'
+        else:
+            for level in range(1,200):
+                if 'temporal id level ' + str(level) in data.columns:
+                    smallest_temporal_level = level
+                    break
+            data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
+            temporal_identifier_column_name = 'dummy temporal id'
+        current_data = data[~(data[temporal_identifier_column_name].isin(futuristic_temporal_units))]
+        future_data = data[data[temporal_identifier_column_name].isin(futuristic_temporal_units)]
+        future_data = future_data.fillna(np.inf)
+        data = pd.concat([current_data,future_data],axis=0, join='outer')
+        return data
+
+############################ adding an integrated teporal id to the data for non integrated temporal id format
+
+
+# Integrating the temporal id columns with the scale levels greater than 'start_level',
+# to obtain a single temporal id which is unique for each unit of the temporal scale level 'start_level'
+def add_dummy_integrated_temporal_id(temporal_data, start_level = 1):
+
+    temporal_data_columns = temporal_data.columns
+
+    valid_temporal_id_levels = ['temporal id level ' + str(start_level)] # sequense of temporal levels without gap
+    greatest_temporal_level = start_level
+
+    # determine the greatest temporal scale level and valid temporal id levels
+    for i in range(start_level+1,200):
+
+        if 'temporal id level '+str(i) in temporal_data_columns:
+            greatest_temporal_level += 1
+            valid_temporal_id_levels.append('temporal id level '+str(i))
+
+            # check for null values
+            if temporal_data['temporal id level '+str(i)].isnull().values.any():
+                raise ValueError('temporal id must have value for all instances but temporal id level '+str(i)+' includes NULL values')
+        else:
+            break
+
+    # remove invalid temporal id levels from data
+    all_temporal_id_levels = list(filter(lambda x: x.startswith('temporal id level '), temporal_data.columns))
+    invalid_temporal_id_levels = list(set(all_temporal_id_levels)-set(valid_temporal_id_levels))
+    if len(invalid_temporal_id_levels) > 0:
+        temporal_data.drop(invalid_temporal_id_levels, axis = 1, inplace = True)
+        if start_level>1:
+            smaller_temporal_id_levels = ['temporal id level '+str(i) for i in range(1,start_level)]
+            invalid_temporal_id_levels = list (set(invalid_temporal_id_levels)-set(smaller_temporal_id_levels))
+            if len(invalid_temporal_id_levels) > 0:
+                print('\nWarning: There is a gap in the sequence of temporal scale levels recorded in the data.\nIds for temporal scale levels greater than {0} are ignored.\n'.format(greatest_temporal_level))
+
+    # construct the integrated (sortable) temporal id
+    temporal_data.loc[:,('dummy temporal id')] = temporal_data['temporal id level ' + str(greatest_temporal_level)]
+
+    if greatest_temporal_level > 1:
+        for level in range(start_level,greatest_temporal_level)[::-1]:
+            temporal_data.loc[:,('dummy temporal id')] = temporal_data['dummy temporal id'].astype(str) + '/' + temporal_data['temporal id level ' + str(level)].astype(str)
+
+    return temporal_data
+
+
+############################ adding secondary spatial scale id's to data
+
+def add_spatial_ids(data,spatial_scale_table):
+
+
+    # to use the spatial scale mapping in the spatial_scale_table
+    # first the existing secondary spatial scale levels are removed from the data
+    extra_spatial_ids = list(filter(lambda x: x.startswith('spatial id level '), data.columns))
+    extra_spatial_ids.remove('spatial id level 1')
+    data.drop(extra_spatial_ids, axis = 1, inplace = True)
+
+    # check spatial_scale_table to have information of all the units in the spatial scale level 1
+    intersection = list(set(data['spatial id level 1'].unique()) & set(spatial_scale_table['spatial id level 1'].unique()))
+    if len(intersection) < len(data['spatial id level 1'].unique()):
+        raise ValueError('The ids of some units in the spatial scale level 1 are missed in the spatial_scales_table.')
+
+    spatial_scale_levels = ['spatial id level 1']
+    for i in range(2,200):
+        column_name = 'spatial id level ' + str(i)
+        if column_name in spatial_scale_table.columns:
+            spatial_scale_levels.append(column_name)
+        else: break
+
+    data = pd.merge(data,spatial_scale_table[spatial_scale_levels], how = 'left', on= 'spatial id level 1')
+
+    return data
+
+
+############################ transform temporal ids in the data frame to the time stamp format
+
+def create_time_stamp(data, time_format, required_suffix):
+    try:
+        data.loc[:,('temporal id')] = data['temporal id'].astype(str) + required_suffix
+        data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x:datetime.datetime.strptime(x,time_format))
+    except ValueError:
+        raise ValueError("temporal id values doesn't match any supported integrated format for temporal id.\n")
+    return data
+
+############################ find the scale of temporal ids and transform to the time stamp format
+
+def check_integrated_temporal_id(temporal_data):
+
+    list_of_supported_formats_string_length = [4,7,10,13,16,19]
+    temporal_data = temporal_data.sort_values(by = ['spatial id level 1','temporal id']).copy()
+    temporal_id_instance = str(temporal_data['temporal id'].iloc[0])
+
+    if len(temporal_id_instance) not in list_of_supported_formats_string_length:
+        raise ValueError("temporal id values doesn't match any supported integrated format for temporal id.\n")
+
+    # find the scale
+    if len(temporal_id_instance) == 4:
+        scale = 'year'
+        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d', '/01/01')
+
+    elif len(temporal_id_instance) == 7:
+        scale = 'month'
+        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d', '/01')
+
+    elif len(temporal_id_instance) == 10:
+
+        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d', '')
+
+        first_temporal_id_instance = temporal_data['temporal id'].iloc[0]
+        second_temporal_id_instance = temporal_data['temporal id'].iloc[1]
+
+        delta = second_temporal_id_instance - first_temporal_id_instance
+        if delta.days == 1:
+            scale = 'day'
+        elif delta.days == 7:
+            scale = 'week'
+        else:
+            raise ValueError("temporal ids with format YYYY/MM/DD must be daily or weekly, but two consecutive id's of input data have a difference of {0} days.\n".format(delta.days))
+
+    elif len(temporal_id_instance) == 13:
+        scale = 'hour'
+        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d %H:%M:%S', ':00:00')
+
+    elif len(temporal_id_instance) == 16:
+        scale = 'min'
+        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d %H:%M:%S', ':00')
+
+    elif len(temporal_id_instance) == 19:
+        scale = 'sec'
+        temporal_data = create_time_stamp(temporal_data.copy(), '%Y/%m/%d %H:%M:%S', '')
+
+    return temporal_data, scale
+
+############################ find the number of smaller scale units in each bigger scale unit
+
+def find_granularity(data, temporal_scale_level):
+
+    if (type(temporal_scale_level) != int) and (temporal_scale_level is not None):
+        raise TypeError("The temporal_scale_level must be of type int.\n")
+
+
+    ###################################### integrated temporal id format ################################
+
+    if 'temporal id' in data.columns:
+
+        scale_level_dict = {'sec':1, 'min':2, 'hour':3, 'day':4, 'week':5, 'month':6, 'year':7}
+        scale_format = {'sec':'%Y/%m/%d %H:%M:%S', 'min':'%Y/%m/%d %H:%M', 'hour':'%Y/%m/%d %H', 'day':'%Y/%m/%d', 'week':'%Y/%m/%d', 'month':'%Y/%m', 'year':'%Y'}
+        scale_second_units_number = {'sec':1, 'min':60, 'hour':3600, 'day':24*3600, 'week':7*24*3600, 'month':30*24*3600, 'year':365*24*3600}
+
+        data = data.drop_duplicates(subset = ['spatial id level 1','temporal id']).copy()
+
+        # determining input data temporal scale and transforming temporal id's to timestamp
+        data , scale = check_integrated_temporal_id(data.copy())
+
+        # in moving average target mode the temporal_scale_level is the next level of current level and must be detected
+        # based on current level
+        if temporal_scale_level is None:
+            temporal_scale_level = 2
+            desired_temporal_scale_level = scale_level_dict[scale] + temporal_scale_level - 1
+            if desired_temporal_scale_level > 7:
+                raise exception("The temporal scale level of the data is {0}. Thus the 'moving average' target_mode couldn't be applied cause the temporal scale bigger than {0} is ambiguous.\n".format(scale))
+
+
+        # determine the numerical desired temporal scale level based on the input data
+        # temporal scale and user specified temporal_scale_level
+        desired_temporal_scale_level = scale_level_dict[scale] + temporal_scale_level - 1
+        if desired_temporal_scale_level > 7:
+            raise Exception('The first temporal scale level recorded in the data is {0}. So the temporal scale level {1} is out of the supported range of temporal scale levels: second, minute, hour, day, week, month, year'.format(scale,temporal_scale_level))
+
+        # get the nominal form of desired temporal scale level
+        desired_temporal_scale = list(scale_level_dict.keys())[list(scale_level_dict.values()).index(desired_temporal_scale_level)]
+
+        # get number of smaller temporal units in each bigger temporal unit
+        granularity = scale_second_units_number[desired_temporal_scale]//scale_second_units_number[scale]
+
+    ###################################### non_integrated temporal id format ################################
+
+    if 'temporal id level 1' in data.columns:
+
+        # if function is called for getting granularity of moving average target mode, the temporal_scale_level
+        # is the next level of current level and must be detected based on current level
+        if temporal_scale_level is None:
+            for level in range(1,200):
+                if 'temporal id level ' + str(level) in data.columns:
+                    smallest_temporal_level = level
+                    break
+            temporal_scale_level = smallest_temporal_level + 1
+            desired_scale_column_name = 'temporal id level ' + str(temporal_scale_level)
+            if desired_scale_column_name not in data.columns:
+                raise ValueError("The next bigger temporal scale after data current temporal scale (temporal scale level {0}) isn't included in the data or is located after a gap in the temporal scale levels sequence and is therefore ignored.\n".format(smallest_temporal_level))
+
+        else:
+            smallest_temporal_level = 1
+            desired_scale_column_name = 'temporal id level ' + str(temporal_scale_level)
+            if desired_scale_column_name not in data.columns:
+                raise ValueError("temporal_scale_level {0} is not in the time scale levels recorded in the data or is located after a gap in the temporal scale levels sequence and is therefore ignored. ".format(temporal_scale_level))
+
+
+        # next 2 line removes the duplicate data samples having same spatial and temporal id's.
+        data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
+        data = data.drop_duplicates(subset = ['spatial id level 1','dummy temporal id']).copy()
+
+
+        # get number of smaller temporal units in each bigger temporal unit
+        granularity = data.groupby(['spatial id level 1',desired_scale_column_name]).count()['dummy temporal id'].max()
+
+
+    return granularity
+
+############################ preprocessing the input data and split it to temporal and spatial data
+
+def prepare_data(data, column_identifier):
+
+    # initialize
+    spatial_data = None
+    temporal_data = None
+
+    if type(data) != dict :
+
+        if type(data) == str :
+            try:
+                data = pd.read_csv(data)
+            except FileNotFoundError:
+                raise FileNotFoundError("File '{0}' does not exist.\n".format(data))
+        elif type(data) != pd.DataFrame :
+            raise TypeError("The input data must be of type DataFrame, string, or a dict containing temporal and spatial DataFrames or addresses.\n")
+        data = rename_columns(data.copy(), column_identifier)
+
+        check_validity(data.copy(), input_name = 'data', data_type = 'full',
+                       column_identifier = column_identifier)
+
+        ##### split data to temporal and spatial data
+
+        spatial_columns = []
+        temporal_columns = []
+
+        # if type of each column is specified in column_identifier
+        if column_identifier is not None:
+            temporal_columns = list(filter(lambda x: x.startswith(('temporal id', 'spatial id','target')), data.columns)) + [item for item in column_identifier['temporal covariates'] if item in data.columns]
+            temporal_data = data[temporal_columns]
+            # if data includes spatial covariates
+            if 'spatial covariates' in column_identifier.keys():
+                spatial_columns = list(filter(lambda x: x.startswith('spatial id'), data.columns)) + [item for item in column_identifier['spatial covariates'] if item in data.columns]
+                spatial_data = data[spatial_columns].drop_duplicates(subset = ['spatial id level 1']).copy()
+
+        # if type of columns are clear based on column name
+        else:
+            temporal_columns = list(filter(lambda x: x.startswith(('temporal id', 'spatial id','temporal covariate','target')), data.columns))
+            temporal_data = data[temporal_columns]
+            # if data includes spatial covariates
+            if len(list(filter(lambda x: x.startswith('spatial covariate'), data.columns))) > 0 :
+                spatial_columns = list(filter(lambda x: x.startswith('spatial id','spatial covariate'), data.columns))
+                spatial_data = data[spatial_columns].drop_duplicates(subset = ['spatial id level 1']).copy()
+
+
+        data_extra_columns = list(set(data.columns)-set(spatial_columns+temporal_columns))
+
+        if len(data_extra_columns) > 0:
+            print("\nWarning: Input data column names must match one of the formats:\n{'temporal id', 'temporal id level x', 'spatial id', 'spatial id level x', 'temporal covariate x', 'spatial covariate x', 'target'},")
+            print("or be specified in the column_identifier, but the names of some of the columns do not match any of the supported formats and are not mentioned in the column_identifier:\n{0}\nThese columns will be ignored.\n".format(data_extra_columns))
+
+
+    elif type(data) == dict:
+        if 'temporal_data' in data.keys():
+
+            if type(data['temporal_data']) == str:
+                try:
+                    temporal_data = pd.read_csv(data['temporal_data'])
+                except FileNotFoundError:
+                    raise FileNotFoundError("File '{0}' does not exist.\n".format(data['temporal_data']))
+
+            elif type(data['temporal_data']) == pd.DataFrame:
+                temporal_data = data['temporal_data']
+            else:
+                raise valueError("The value of the 'temporal_data' key in the data dictionary must be a DataFrame or the address of temporal data.\n")
+            temporal_data = rename_columns(temporal_data.copy(), column_identifier)
+            check_validity(temporal_data.copy(), input_name = 'temporal_data',
+                           data_type = 'temporal', column_identifier = column_identifier)
+
+            if column_identifier is not None:
+                if 'temporal covariates' in column_identifier.keys():
+                    temporal_data_extra_columns = list(set(filter(lambda x: not x.startswith(('temporal id','spatial id','target')), temporal_data.columns)) - set(column_identifier['temporal covariates']))
+            else:
+                temporal_data_extra_columns = list(filter(lambda x: not x.startswith('temporal id','spatial id','temporal covariate','target'), temporal_data.columns))
+
+            if len(temporal_data_extra_columns) > 0:
+                print("\nWarning: Input temporal_data column names must match one of the formats:\n{'temporal id', 'temporal id level x', 'spatial id', 'spatial id level x', 'temporal covariate x', 'target'}")
+                print("or be specified in the column_identifier,but the names of some of the columns do not match any of the supported formats and are not mentioned in the column_identifier:\n{0}\nThese columns will be ignored.\n".format(temporal_data_extra_columns))
+            temporal_data.drop(temporal_data_extra_columns, axis = 1, inplace = True)
+
+        else:
+            raise Exception("The data on temporal covariates and target variable must be passed to the function using data argument and as a DataFrame, Data address or value of 'temporal_data' key in the dictionary of data. But none is passed.\n")
+
+
+        if ('spatial_data' in data.keys()) and (data['spatial_data'] is not None):
+
+            if type(data['spatial_data']) == str:
+                try:
+                    spatial_data = pd.read_csv(data['spatial_data'])
+                except FileNotFoundError:
+                    raise FileNotFoundError("File '{0}' does not exist.\n".format(data['spatial_data']))
+
+            elif type(data['spatial_data']) == pd.DataFrame:
+                spatial_data = data['spatial_data']
+            else:
+                raise ValueError("The value of the 'spatial_data' key in the data dictionary must be a DataFrame or the address of spatial data.\n")
+
+            spatial_data = rename_columns(spatial_data.copy(), column_identifier)
+            check_validity(spatial_data.copy(), input_name = 'spatial_data',
+                           data_type = 'spatial', column_identifier = column_identifier)
+            spatial_data = spatial_data.drop_duplicates(subset = ['spatial id level 1']).copy()
+
+            if column_identifier is not None:
+                if 'spatial covariates' in column_identifier.keys():
+                    spatial_data_extra_columns = list(set(filter(lambda x: not x.startswith('spatial id'), spatial_data.columns)) - set(column_identifier['spatial covariates']))
+            else:
+                spatial_data_extra_columns = list(filter(lambda x: not x.startswith(('spatial id','spatial covariate')), spatial_data.columns))
+
+            if len(spatial_data_extra_columns) > 0:
+                print("\nWarning: Input spatial_data column names must match one of the formats:\n{'spatial id', 'spatial id level x', 'spatial covariate x'}")
+                print("or be specified in the column_identifier,but the names of some of the columns do not match any of the supported formats and are not mentioned in the column_identifier:\n{0}\nThis columns will be ignored.\n".format(spatial_data_extra_columns))
+            spatial_data.drop(spatial_data_extra_columns, axis = 1, inplace = True)
+
+    return temporal_data, spatial_data
+
+
+#############################################################################################
+############################  imputing the tepmoral data ####################################
+#############################################################################################
+
+def impute(data, column_identifier = None, verbose = 0):
+
+    if type(data) == str:
+        data = pd.read_csv(data)
+
+    data = rename_columns(data = data.copy(), column_identifier = column_identifier, error = 0)
+
+    check_validity(data.copy(), input_name = 'data', data_type = 'temporal',
+                   column_identifier = column_identifier, error = 0)
+
+    if 'temporal id' in data.columns:
+        temporal_identifier_column_name = 'temporal id'
+
+    elif 'temporal id level 1' in data.columns: # non-integrated temporal id format
+        # first integrated format for temporal id must constructed
+        data = add_dummy_integrated_temporal_id(data.copy())
+        temporal_identifier_column_name = 'dummy temporal id'
+
+    data = data.drop_duplicates(subset = ['spatial id level 1', temporal_identifier_column_name]).copy()
+
+    covariate_names = list(filter(lambda x: not x.startswith(('temporal id', 'spatial id', 'dummy temporal id')), data.columns))
+
+    if 'target' in data.columns:
+        if data['target'].isnull().values.any():
+            if verbose > 0: print("\nWarning: The target variable includes missing values. This values will be imputed.\n")
+
+    spatial_units_observed_value_count = data.groupby('spatial id level 1').count()
+    temporal_units_observed_value_count = data.groupby(temporal_identifier_column_name).count()
+
+
+
+    for covar in covariate_names:
+        spatial_units_with_all_nulls=spatial_units_observed_value_count[spatial_units_observed_value_count[covar]==0].index
+        temporal_units_with_all_nulls=temporal_units_observed_value_count[temporal_units_observed_value_count[covar]==0].index
+
+        # check if covariate has no value for an temporal unit
+        if len(temporal_units_with_all_nulls) > 0:
+            raise ValueError("The input data has no value for {0}, in some temporal units.\nThe covariates must have value for at least one spatial unit in each temporal units recorded in the data".format(covar))
+
+        data = data.drop_duplicates(subset = ['spatial id level 1',temporal_identifier_column_name]).copy()
+
+        # create data frame with each row representing a spatial unit and each column representing a temporal unit
+        temp = data.pivot(index='spatial id level 1', columns=temporal_identifier_column_name, values=covar)
+
+        # impute missing values using KNN imputation
+        X = np.array(temp)
+        imputer = KNNImputer(n_neighbors=5)
+        imp=imputer.fit_transform(X)
+        imp=pd.DataFrame(imp, index = temp.index, columns = temp.columns)
+
+        # reshape imputed values of covariate into one column
+        imp = pd.melt(imp.reset_index(), id_vars='spatial id level 1', value_vars=list(imp.columns),
+                     var_name=temporal_identifier_column_name, value_name=covar)
+
+        # add the imputed values back to the data set
+        data.drop([covar], axis = 1, inplace = True)
+        data = pd.merge(data, imp, how = 'left')
+
+        # remove the imputed values for the spatial units with no observed values
+        data.loc[data['spatial id level 1'].isin(spatial_units_with_all_nulls),covar]=np.NaN
+        if len(spatial_units_with_all_nulls)>0:
+            if verbose == 2:
+                print('\nWarning: Following spatial units has no recorded values for {0} and therefore will be removed from the data:\n{1}\n'.format(covar,list(spatial_units_with_all_nulls)))
+            elif verbose == 1:
+                print('\nWarning: The number of {0} spatial units has no recorded values for {1} and therefore will be removed from the data\n.'.format(len(list(spatial_units_with_all_nulls)),covar))
+
+    # remove temporarily added column
+    if 'dummy temporal id' in data.columns: data.drop(['dummy temporal id'], axis = 1, inplace = True)
+
+    # produce warning for removed spatial units
+    number_of_spatial_units = len(data['spatial id level 1'].unique())
+    imputed_data = data.dropna()
+    number_of_removed_spatial_units = number_of_spatial_units - len(imputed_data['spatial id level 1'].unique())
+
+    if number_of_removed_spatial_units == number_of_spatial_units:
+        raise Exception("All the spatial units have no value for at least one temporal covariate and are removed from the data. Therefore, no spatial unit remains to make a prediction.\n")
+    elif number_of_removed_spatial_units > 0:
+        if verbose == 0:
+            print('\nWarning: The number of {0} spatial units has no value for at least one temporal covariate and are removed from the data.\n'.format(number_of_removed_spatial_units))
+
+    imputed_data = rename_columns(imputed_data.copy(), column_identifier, 'deformalize', 0)
+
+    return imputed_data
+
+#################################################################################################
+############################  transforming the spatial scale ####################################
+#################################################################################################
+
+def spatial_scale_transform(data, data_type, spatial_scale_table = None, spatial_scale_level = 2, aggregation_mode = 'mean', column_identifier = None, verbose = 0):
+
+    # initializing list of covariates with sum or mean aggregation modes
+    mean_covariates = []
+    sum_covariates = []
+
+    desired_scale_column_name = 'spatial id level ' + str(spatial_scale_level)
+    base_columns = [desired_scale_column_name]
+
+    if type(data) == str:
+        data = pd.read_csv(data)
+    data = rename_columns(data = data.copy(), column_identifier = column_identifier, error = 0)
+
+    check_validity(data.copy(), input_name = 'data', data_type = data_type, column_identifier = column_identifier, error = 0)
+    if spatial_scale_table is not None:
+        if type(spatial_scale_table) == str:
+            spatial_scale_table = pd.read_csv(spatial_scale_table)
+        spatial_scale_table = rename_columns(data = spatial_scale_table.copy(), column_identifier = column_identifier, error = 0)
+        check_validity(spatial_scale_table.copy(), input_name = 'spatial_scale_table',
+                       data_type = 'spatial_scales', column_identifier = column_identifier, error = 0)
+        # drop duplicate is needed ????
+        data = add_spatial_ids(data.copy(),spatial_scale_table)
+
+    if desired_scale_column_name not in data.columns:
+        raise ValueError("spatial_scale_level {0} isn't in the spatial scale levels included in the data.\n".format(spatial_scale_level))
+
+
+    if data_type == 'temporal':
+
+        if 'temporal id' in data.columns: # integrated temporal id format
+            temporal_identifier_column_name = 'temporal id'
+
+        elif 'temporal id level 1' in data.columns: # non-integrated temporal id format
+            # first integrated format for temporal id must constructed
+            data = add_dummy_integrated_temporal_id(data.copy())
+            temporal_identifier_column_name = 'dummy temporal id'
+
+            non_integrated_temporal_levels = list(filter(lambda x: x.startswith('temporal id level '), data.columns))
+            temporal_levels_data_frame = data[non_integrated_temporal_levels + ['dummy temporal id']]
+            data.drop(non_integrated_temporal_levels, axis = 1, inplace = True)
+
+        base_columns.append(temporal_identifier_column_name)
+        data = data.drop_duplicates(subset = ['spatial id level 1',temporal_identifier_column_name]).copy()
+
+    else:
+        data = data.drop_duplicates(subset = ['spatial id level 1']).copy()
+
+
+    # removing spatial id columns except for desired spatial scale ids
+    extra_spatial_ids = list(filter(lambda x: x.startswith('spatial id '), data.columns))
+    extra_spatial_ids.remove(desired_scale_column_name)
+    data.drop(extra_spatial_ids, axis = 1, inplace = True)
+
+    covariate_names = list(filter(lambda x: not x.startswith(('temporal id','spatial id','dummy temporal id')), data.columns))
+
+
+    if aggregation_mode == 'mean':
+        mean_covariates = covariate_names.copy()
+    elif aggregation_mode == 'sum':
+        sum_covariates = covariate_names.copy()
+    elif type(aggregation_mode) == dict:
+        extra_covariates_listed = list(set(aggregation_mode.keys())-set(covariate_names))
+        if len(extra_covariates_listed) > 0:
+            aggregation_mode = {covar:operator for covar,operator in aggregation_mode.items() if covar in covariate_names}
+            if verbose == 1:
+                print("\nWarning : Some of the covariates specified in aggregation_mode are not exist in the data.\n")
+            if verbose == 2:
+                print("\nWarning : Some of the covariates specified in aggregation_mode are not exist in the data:\n{0}\n".format(extra_covariates_listed))
+        mean_covariates = [covar for covar,operator in aggregation_mode.items() if operator == 'mean']
+        sum_covariates = [covar for covar,operator in aggregation_mode.items() if operator == 'sum']
+    else:
+        raise ValueError("aggregation_mode must be 'sum' or 'mean' or a dictionary with covariates name as the keys and 'sum' or 'mean' as the values")
+
+    unspecified_covariates = list(set(covariate_names)-set(mean_covariates + sum_covariates))
+    if len(unspecified_covariates)>0:
+        if verbose < 2:
+            print("\nWarning : The aggregation_mode is not specified for some of the covariates.\nThe mean operator will be used to aggregate these covariates' values.\n")
+        if verbose == 2:
+            print("\nWarning : The aggregation_mode is not specified for some of the covariates:\n{0}\nThe mean operator will be used to aggregate these covariates' values.\n".format(unspecified_covariates))
+        mean_covariates = mean_covariates + unspecified_covariates
+
+    if len(mean_covariates)>0:
+        mean_covariates+=base_columns
+        mean_data = data.copy()[mean_covariates]
+        mean_data = mean_data.groupby(base_columns).mean()
+        mean_data = mean_data.reset_index()
+
+    if len(sum_covariates)>0:
+        sum_covariates+=base_columns
+        sum_data = data.copy()[sum_covariates]
+        sum_data = sum_data.groupby(base_columns).sum(min_count=1)
+        sum_data = sum_data.reset_index()
+
+    if len(mean_covariates)>0 and len(sum_covariates)>0:
+        data = pd.merge(mean_data,sum_data,on=base_columns)
+    elif len(mean_covariates)>0:
+        data = mean_data
+    elif len(sum_covariates)>0:
+        data = sum_data
+
+    if 'dummy temporal id' in data.columns:
+        data = pd.merge(temporal_levels_data_frame.drop_duplicates(), data, on = ['dummy temporal id']).drop_duplicates().copy()
+        data.drop(['dummy temporal id'], axis=1, inplace = True)
+        ordered_columns = [desired_scale_column_name]+list(temporal_levels_data_frame.columns.drop(['dummy temporal id']))+covariate_names
+    elif 'temporal id' in data.columns:
+        ordered_columns = [desired_scale_column_name,'temporal id']+covariate_names
+    else:
+        ordered_columns = [desired_scale_column_name]+covariate_names
+
+    data = data.copy()[ordered_columns]
+
+    data = rename_columns(data.copy(), column_identifier, 'deformalize', 0)
+
+    return data
+
+##############################################################################################
+############################  transforming temporal scale ####################################
+##############################################################################################
+
+def temporal_scale_transform(data, column_identifier = None, temporal_scale_level = 2, augmentation = False, verbose = 0):
+
+    if type(data) == str:
+        data = pd.read_csv(data)
+    data = rename_columns(data = data.copy(), column_identifier = column_identifier, error =0)
+    check_validity(data.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier, error =0)
+
+    if type(temporal_scale_level) != int:
+        raise TypeError("The temporal_scale_level must be of type int.\n")
+
+    if temporal_scale_level == 1:
+        if verbose > 0: print ('The temporal_scale_level = 1 is interpreted to no temporal transformation')
+        return data
+
+    # Next 4 lines save the secondary spatial scale levels information in a data frame to be added to the transformed data
+    secondary_spatial_levels = list(filter(lambda x: x.startswith('spatial id level '), data.columns))
+    spatial_levels_data_frame = data[secondary_spatial_levels].drop_duplicates().copy()
+    secondary_spatial_levels.remove('spatial id level 1')
+    data.drop(secondary_spatial_levels, axis = 1, inplace = True)
+
+    ###################################### integrated temporal id format ################################
+
+    if 'temporal id' in data.columns:
+
+        scale_level_dict = {'sec':1, 'min':2, 'hour':3, 'day':4, 'week':5, 'month':6, 'year':7}
+        scale_format = {'sec':'%Y/%m/%d %H:%M:%S', 'min':'%Y/%m/%d %H:%M', 'hour':'%Y/%m/%d %H', 'day':'%Y/%m/%d', 'week':'%Y/%m/%d', 'month':'%Y/%m', 'year':'%Y'}
+        scale_second_units_number = {'sec':1, 'min':60, 'hour':3600, 'day':24*3600, 'week':7*24*3600, 'month':30*24*3600, 'year':365*24*3600}
+
+        data = data.drop_duplicates(subset = ['spatial id level 1','temporal id']).copy()
+
+        # determining input data temporal scale and transforming temporal id's to timestamp
+        data , scale = check_integrated_temporal_id(data.copy())
+
+        # determine the numerical desired temporal scale level based on the input data
+        # temporal scale and user specified temporal_scale_level
+        desired_temporal_scale_level = scale_level_dict[scale] + temporal_scale_level - 1
+        if desired_temporal_scale_level > 7:
+            raise Exception('The first temporal scale level recorded in the data is {0}. So the temporal scale level {1} is out of the supported range of temporal scale levels: second, minute, hour, day, week, month, year'.format(scale,temporal_scale_level))
+
+        # get the nominal form of desired temporal scale level
+        desired_temporal_scale = list(scale_level_dict.keys())[list(scale_level_dict.values()).index(desired_temporal_scale_level)]
+        if verbose > 0 : print("\nTransformation of data to the temporal scale of the {0} is running.\n".format(desired_temporal_scale))
+
+        # get number of smaller temporal units in each bigger temporal unit
+        granularity = scale_second_units_number[desired_temporal_scale]//scale_second_units_number[scale]
+
+        number_of_temporal_units=len(data['temporal id'].unique())
+        number_of_spatial_units=len(data['spatial id level 1'].unique())
+
+        if augmentation == False:
+
+            # For the temporal scale of the week, each date must be replaced with the date of the first day
+            # of the corresponding week
+            if desired_temporal_scale == 'week' :
+                data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x : x - datetime.timedelta(days=x.weekday()))
+
+            data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x : datetime.datetime.strftime(x,scale_format[desired_temporal_scale]))
+
+            # remove the data of the smaller scale temporal units in beggining and
+            # ending of data which does'nt make up a complete bigger tempral scale unit
+            max_temporal_id = max(data['temporal id'])
+            min_temporal_id = min(data['temporal id'])
+            if len(data[data['temporal id'] == max_temporal_id])<number_of_spatial_units*granularity:
+                data = data[data['temporal id'] != max_temporal_id]
+            if len(data[data['temporal id'] == min_temporal_id])<number_of_spatial_units*granularity:
+                data = data[data['temporal id'] != min_temporal_id]
+
+            base_columns = ['temporal id', 'spatial id level 1']
+            data = data.groupby(base_columns).mean()
+            data = data.reset_index()
+
+        if augmentation == True:
+
+            data = data.sort_values(by = ['temporal id' , 'spatial id level 1']).copy()
+            data.reset_index(drop = True, inplace = True)
+
+            transformed_data = pd.DataFrame(columns = data.columns)
+
+            while number_of_temporal_units >= granularity:
+                bigger_scale_unit_data = data.copy().tail(number_of_spatial_units*granularity)
+                current_temporal_id = data.copy().tail(1)['temporal id'].values[0]
+
+                # average of covariates and target values on last bigger temporal scale unit for all spatial scale units
+                bigger_scale_unit_data_average = bigger_scale_unit_data.groupby(['spatial id level 1']).mean(numeric_only=True).reset_index()
+                bigger_scale_unit_data_average.loc[:,('temporal id')] = current_temporal_id
+
+                transformed_data = pd.concat([transformed_data,bigger_scale_unit_data_average], axis=0, join='outer')
+                # remove last smaller temporal scale unit for all spatial units from base data
+                data = data.iloc[:-(number_of_spatial_units),:]
+                number_of_temporal_units = number_of_temporal_units - 1
+
+            data = transformed_data.copy()
+            data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x : datetime.datetime.strftime(x,scale_format[scale]))
+
+        data = data.sort_values(by=['spatial id level 1','temporal id']).copy()
+
+    ###################################### non_integrated temporal id format ################################
+
+    if 'temporal id level 1' in data.columns:
+
+        # next 2 line removes the duplicate data samples having same spatial and temporal id's.
+        data = add_dummy_integrated_temporal_id(data.copy(), start_level = 1)
+        data = data.drop_duplicates(subset = ['spatial id level 1','dummy temporal id']).copy()
+
+        desired_scale_column_name = 'temporal id level ' + str(temporal_scale_level)
+        if desired_scale_column_name not in data.columns:
+            raise ValueError("temporal_scale_level {0} is not in the temporal scale levels recorded in the data or is located after a gap in the temporal scale levels sequence and is therefore ignored. ".format(temporal_scale_level))
+        elif verbose > 0 :
+            if column_identifier is not None:
+                print("\nTransformation of data to the temporal scale of the {0} is running.\n".format(column_identifier[desired_scale_column_name]))
+            else:
+                print("\nTransformation of data to the temporal scale of the {0} is running.\n".format(desired_scale_column_name))
+
+        if augmentation == False :
+
+            # remove dummy temporal id which is based on level 1 to add dummy temporal id based on 'temporal_scale_level'
+            data.drop(['dummy temporal id'], axis = 1, inplace = True)
+            data = add_dummy_integrated_temporal_id(data.copy(), start_level = temporal_scale_level)
+
+            secondary_temporal_levels = list(filter(lambda x: x.startswith('temporal id level '), data.columns))
+            temporal_levels_data_frame = data[secondary_temporal_levels + ['dummy temporal id']]
+            data.drop(secondary_temporal_levels, axis = 1, inplace = True)
+
+            base_columns = ['dummy temporal id', 'spatial id level 1']
+
+            data = data.groupby(base_columns).mean()
+            data = data.reset_index()
+            data = pd.merge(temporal_levels_data_frame.drop_duplicates(), data, on = 'dummy temporal id', how = 'right').drop_duplicates().copy()
+            # sorting columns
+            data_columns = list(data.columns).copy()
+            data_columns.remove('dummy temporal id')
+            data = data[['dummy temporal id']+data_columns]
+
+
+        elif augmentation == True :
+
+            # get number of smaller temporal units in each bigger temporal unit
+            granularity = data.groupby(['spatial id level 1',desired_scale_column_name]).count()['dummy temporal id'].max()
+
+            secondary_temporal_levels = list(filter(lambda x: x.startswith('temporal id level '), data.columns))
+            temporal_levels_data_frame = data[secondary_temporal_levels + ['dummy temporal id']]
+            data.drop(secondary_temporal_levels, axis = 1, inplace = True)
+
+            data = data.sort_values(by = ['dummy temporal id' , 'spatial id level 1']).copy()
+            data.reset_index(drop = True, inplace = True)
+            number_of_temporal_units=len(data['dummy temporal id'].unique())
+            number_of_spatial_units=len(data['spatial id level 1'].unique())
+
+            transformed_data = pd.DataFrame(columns = data.columns)
+
+            while number_of_temporal_units >= granularity:
+                bigger_scale_unit_data = data.copy().tail(number_of_spatial_units*granularity)
+                current_temporal_id = data.copy().tail(1)['dummy temporal id'].values[0]
+
+                # average of covariates and target values on last bigger temporal scale unit for all spatial scale units
+                bigger_scale_unit_data_average = bigger_scale_unit_data.groupby(['spatial id level 1']).mean(numeric_only=True).reset_index()
+                bigger_scale_unit_data_average.loc[:,('dummy temporal id')] = current_temporal_id
+
+
+                transformed_data = pd.concat([transformed_data,bigger_scale_unit_data_average], axis=0, join='outer')
+                data = data.iloc[:-(number_of_spatial_units),:]# remove last smaller temporal scale unit for all spatial units from base data
+                number_of_temporal_units = number_of_temporal_units - 1
+
+            data = transformed_data.copy()
+
+            data = pd.merge(temporal_levels_data_frame.drop_duplicates(), data, on = 'dummy temporal id', how = 'right').drop_duplicates().copy()
+
+        data = data.sort_values(by=['spatial id level 1','dummy temporal id']).copy()
+        data.drop(['dummy temporal id'] ,axis = 1 , inplace = True)
+
+
+    # add secondary spatial scale levels back to data
+    data = pd.merge(spatial_levels_data_frame.drop_duplicates(), data, on = 'spatial id level 1', how = 'right').drop_duplicates().copy()
+
+    # sorting columns
+    data_columns = list(data.columns).copy()
+    data_columns.remove('spatial id level 1')
+    data = data[['spatial id level 1']+data_columns]
+
+    if column_identifier is not None:
+        if 'temporal id' in data.columns: # integrated temporal_id format
+            data = rename_columns(data, {key:value for key,value in column_identifier.items() if key != 'temporal id'}, 'deformalize', 0)
+        else: # non_integrated temporal_id format
+            data = rename_columns(data, column_identifier, 'deformalize', 0)
+
+    if len(data)<1:
+        raise Exception("The number of recorded units in the data with the specified temporal scale level is less than one.")
+
+    return data
+
+######################################################################################
+############################  target modification ####################################
+######################################################################################
+
+# modifying target to the cumulative or differential or moving average mode
+
+def target_modification(data, target_mode, column_identifier = None, verbose = 0):
+
+    if type(data) == str:
+        data = pd.read_csv(data)
+    data = rename_columns(data = data.copy(), column_identifier = column_identifier, error =0)
+
+    check_validity(data.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier, error =0)
+
+    if 'target' not in data.columns:
+        raise ValueError("There is no column named 'target' in the input data, and the corresponding column is not specified in the column_identifier.\n")
+    try:
+        data.loc[:,('target')] = data['target'].astype(float)
+    except ValueError:
+        raise ValueError("The target column includes non-numerical values.\n")
+
+    if (data['target'].isnull().values.any()) and (target_mode in ['cumulative', 'differential', 'moving average']):
+        print("\nWarning: The target variable column includes Null values and therefore the resulting values of applying {0} target_mode is not valid.\n".format(target_mode))
+
+    if 'temporal id' in data.columns: # integrated temporal id format
+        temporal_identifier_column_name = 'temporal id'
+    else: # Non_integrated temporal id format
+        for level in range(1,200):
+            if 'temporal id level ' + str(level) in data.columns:
+                smallest_temporal_level = level
+                break
+        data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
+        temporal_identifier_column_name = 'dummy temporal id'
+
+
+    data = data.drop_duplicates(subset = [temporal_identifier_column_name,'spatial id level 1']).copy()
+    data = data.sort_values(by=[temporal_identifier_column_name,'spatial id level 1']).copy()
+
+    normal_target_df = data[['spatial id level 1', temporal_identifier_column_name, 'target']].rename(columns = {'target':'Normal target'})
+
+    ######################################################################### cumulative
+
+    if target_mode == 'cumulative':
+        temporal_ids = data[temporal_identifier_column_name].unique()
+        for i in range(len(temporal_ids)-1):
+            data.loc[data[temporal_identifier_column_name]==temporal_ids[i+1],'target']=\
+            list(np.array(data.loc[data[temporal_identifier_column_name]==temporal_ids[i+1],'target'])+\
+                  np.array(data.loc[data[temporal_identifier_column_name]==temporal_ids[i],'target']))
+
+
+    ######################################################################### differential
+
+    elif target_mode == 'differential': # make target differential
+        reverse_temporal_ids = data[temporal_identifier_column_name].unique()[::-1]
+        for i in range(len(reverse_temporal_ids)):
+            temprl_unit = reverse_temporal_ids[i]
+            past_temprl_unit = reverse_temporal_ids[i+1]
+            data.loc[data[temporal_identifier_column_name] == temprl_unit,'target']=\
+            list(np.array(data.loc[data[temporal_identifier_column_name]==temprl_unit,'target'])-\
+                 np.array(data.loc[data[temporal_identifier_column_name]==past_temprl_unit,'target']))
+            if i == len(reverse_temporal_ids)-2:
+                break
+
+    ######################################################################### moving average
+
+    elif target_mode == 'moving average':
+
+        ############### integrated temporal id format
+        if temporal_identifier_column_name == 'temporal id':
+
+            scale_level_dict = {'sec':1, 'min':2, 'hour':3, 'day':4, 'week':5, 'month':6, 'year':7}
+            scale_format = {'sec':'%Y/%m/%d %H:%M:%S', 'min':'%Y/%m/%d %H:%M', 'hour':'%Y/%m/%d %H', 'day':'%Y/%m/%d', 'week':'%Y/%m/%d', 'month':'%Y/%m', 'year':'%Y'}
+            scale_second_units_number = {'sec':1, 'min':60, 'hour':3600, 'day':24*3600, 'week':7*24*3600, 'month':30*24*3600, 'year':365*24*3600}
+
+            # determining input data temporal scale and transforming temporal id's to timestamp
+            data , scale = check_integrated_temporal_id(data.copy())
+
+            # determine the numerical level of the next temporal scale after input data
+            # temporal scale for applying moving average on target values
+
+            desired_temporal_scale_level = scale_level_dict[scale] + 1
+            if desired_temporal_scale_level > 7:
+                raise Exception("The temporal scale level of the data is {0}. Thus the 'moving average' target_mode couldn't be applied cause the temporal scale bigger than {0} is ambiguous.\n".format(scale))
+
+             # get the nominal form of desired temporal scale level
+            desired_temporal_scale = list(scale_level_dict.keys())[list(scale_level_dict.values()).index(desired_temporal_scale_level)]
+
+            if verbose > 0:
+                print("\nThe temporal scale level of the data is {0}, and using 'moving average' target_mode, the target value for each {0} is the average of values in the previous {1} of that {0}.\n".format(scale,desired_temporal_scale))
+
+            # get number of smaller temporal units in each bigger temporal unit
+            granularity = scale_second_units_number[desired_temporal_scale]//scale_second_units_number[scale]
+
+
+            data = data.sort_values(by = ['temporal id' , 'spatial id level 1']).copy()
+            data.reset_index(drop = True, inplace = True)
+            number_of_temporal_units=len(data['temporal id'].unique())
+            number_of_spatial_units=len(data['spatial id level 1'].unique())
+
+            transformed_data = pd.DataFrame(columns = data.columns)
+
+            while number_of_temporal_units >= granularity:
+
+                bigger_scale_unit_data = data.copy().tail(number_of_spatial_units*granularity)
+                smaller_scale_unit_data = data.copy().tail(number_of_spatial_units)
+
+                # average of target values on last bigger temporal scale unit for all spatial scale units
+                bigger_scale_unit_data_average = bigger_scale_unit_data.groupby(['spatial id level 1']).mean(numeric_only=True).reset_index()
+                # add averaged target values of last bigger temporal scale unit to the smaller temporal scale unit
+                smaller_scale_unit_data.loc[:,('target')] = bigger_scale_unit_data_average.loc[:,('target')].tolist()
+
+                transformed_data = pd.concat([transformed_data,smaller_scale_unit_data], axis=0, join='outer')
+                # remove last smaller temporal scale unit for all spatial units from base data
+                data = data.iloc[:-(number_of_spatial_units),:]
+                number_of_temporal_units = number_of_temporal_units - 1
+
+            data = transformed_data.copy()
+            data.loc[:,('temporal id')] = data['temporal id'].apply(lambda x : datetime.datetime.strftime(x,scale_format[scale]))
+            data = data.sort_values(by=['spatial id level 1','temporal id']).copy()
+
+        ####################### non_integrated temporal id format
+
+        elif temporal_identifier_column_name == 'dummy temporal id':
+
+            desired_scale_column_name = 'temporal id level ' + str(smallest_temporal_level+1)
+            if desired_scale_column_name not in data.columns:
+                raise Exception("The next bigger temporal scale after data current temporal scale (temporal scale level {0}) isn't included in the data or is located after a gap in the temporal scale levels sequence and is therefore ignored.\n".format(smallest_temporal_level))
+
+            # get number of smaller temporal units in each bigger temporal unit
+            granularity = data.groupby(['spatial id level 1',desired_scale_column_name]).count()['dummy temporal id'].max()
+
+            data = data.sort_values(by = ['dummy temporal id' , 'spatial id level 1']).copy()
+            data.reset_index(drop = True, inplace = True)
+            number_of_temporal_units=len(data['dummy temporal id'].unique())
+            number_of_spatial_units=len(data['spatial id level 1'].unique())
+
+            transformed_data = pd.DataFrame(columns = data.columns)
+
+            while number_of_temporal_units >= granularity:
+
+                bigger_scale_unit_data = data.copy().tail(number_of_spatial_units*granularity)
+                smaller_scale_unit_data = data.copy().tail(number_of_spatial_units)
+
+                # average of target values on last bigger temporal scale unit for all spatial scale units
+                bigger_scale_unit_data_average = bigger_scale_unit_data.groupby(['spatial id level 1']).mean(numeric_only=True).reset_index()
+                # add averaged target values of last bigger temporal scale unit to the smaller temporal scale unit
+                smaller_scale_unit_data.loc[:,('target')] = bigger_scale_unit_data_average.loc[:,('target')].tolist()
+
+                transformed_data = pd.concat([transformed_data,smaller_scale_unit_data], axis=0, join='outer')
+                # remove last smaller temporal scale unit for all spatial units from base data
+                data = data.iloc[:-(number_of_spatial_units),:]
+                number_of_temporal_units = number_of_temporal_units - 1
+
+            data = transformed_data.sort_values(by=['spatial id level 1','dummy temporal id']).copy()
+
+    elif target_mode == 'normal':
+        data = data
+    else:
+        raise ValueError("The specified target_mode is not recognized. The supported target_modes are:\n{'normal', 'cumulative', 'differential', 'moving average'}")
+
+    data = pd.merge(data,
+            normal_target_df[normal_target_df[temporal_identifier_column_name].isin(data[temporal_identifier_column_name].unique())],
+            on = ['spatial id level 1', temporal_identifier_column_name], how = 'inner')
+
+    if 'dummy temporal id' in data.columns:
+        data.drop(['dummy temporal id'], axis = 1, inplace = True)
+    
+    column_identifier_copy = None
+    if column_identifier is not None:
+        column_identifier_copy = column_identifier.copy()
+        if 'target' in list(column_identifier.keys()):
+            del column_identifier_copy['target']
+
+    data = rename_columns(data.copy(), column_identifier_copy, 'deformalize', 0)
+    
+    return data
+
+#########################################################################################
+############################ making neighbouring data ###################################
+#########################################################################################
+
+def make_neighbouring_data(data, column_identifier = None, number_of_layers = 1, neighbouring_matrix = None,
+                            time_dependency_flag = 1, verbose = 0):
+
+    
+    if type(data) == str :
+        try:
+            data = pd.read_csv(data)
+        except FileNotFoundError:
+            raise FileNotFoundError("File '{0}' does not exist.\n".format(data))
+    elif type(data) != pd.DataFrame :
+        raise TypeError("The input data must be of type DataFrame or string (data address).\n")
+    data = rename_columns(data = data.copy(), column_identifier = column_identifier, error = 0)
+
+    if time_dependency_flag == 1:
+        check_validity(data.copy(), input_name = 'data', data_type = 'full', column_identifier = column_identifier, error = 0)
+    else:
+        check_validity(data.copy(), input_name = 'data', data_type = 'spatial', column_identifier = column_identifier, error = 0)
+
+
+    number_of_spatial_units = len(data['spatial id level 1'].unique())
+    temporal_identifier_column_name = 'temporal id'
+
+    # Non_integrated temporal id format
+    if 'temporal id' not in data.columns and time_dependency_flag == 1:
+            # find smallest temporal level
+            for level in range(1,200):
+                if 'temporal id level ' + str(level) in data.columns:
+                    smallest_temporal_level = level
+                    break
+            # add integrated temporal id
+            data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
+            temporal_identifier_column_name = 'dummy temporal id'
+
+    elif time_dependency_flag == 0:
+        data['temporal id'] = 1 # adding temporary dummy temporal id to avoid the exceptions
+
+    data = data.drop_duplicates(subset = [temporal_identifier_column_name,'spatial id level 1']).copy()
+
+
+    # check neighbouring_matrix
+
+    if not isinstance(neighbouring_matrix,np.ndarray):
+        raise TypeError("The neighbouring_matrix must be of type numpy array.\n")
+    elif len(neighbouring_matrix.shape)<2 or neighbouring_matrix.shape[0] != number_of_spatial_units or neighbouring_matrix.shape[1] != number_of_spatial_units:
+        raise ValueError("The adjacency matrix must be a two-dimensional numpy array with dimensions equal to the number of spatial units. Each element of this matrix specifies the adjacency (1) or lack of adjacency (0) between two spatial units.\n")
+
+    covariate_names = list(filter(lambda x: not x.startswith(('temporal id', 'spatial id', 'dummy temporal id', 'target')), data.columns))
+
+    if len(covariate_names) == 0:
+        raise  Exception("\n There is no covariate in the data.")
+
+    data = data.sort_values(by = [temporal_identifier_column_name,'spatial id level 1']).copy()
+
+    layer_matrix_dict = {}
+    layer_matrix_dict[1] = neighbouring_matrix
+
+    zero_neighbour_flag = 0
+    for layer in range(1,number_of_layers+1):
+        if layer > 1:
+            layer_matrix = np.matmul(layer_matrix_dict[layer-1],neighbouring_matrix) # take the number of paths with length l (layer) between the spatial units (neighbouring_matrix^layer)
+            layer_matrix = (layer_matrix > 0).astype(int) # set the elements greater than 1 to 1
+            for l in range(1,layer):
+                layer_matrix = layer_matrix - layer_matrix_dict[l] # Remove the neighbours that are already in the previous layers
+            layer_matrix = layer_matrix - np.identity(layer_matrix.shape[0]).astype(int) # Remove the self neighbourhoods
+
+            layer_matrix = (layer_matrix == 1).astype(int)
+            layer_matrix_dict[layer] = layer_matrix
+        else:
+            layer_matrix = neighbouring_matrix
+
+        for covar in covariate_names:
+            covar_df = data.pivot(index=temporal_identifier_column_name, columns='spatial id level 1', values=covar)
+            covar_array = covar_df.to_numpy()
+            covar_array = np.matmul(covar_array,layer_matrix) # Get the sum of the covar values for the neighbours
+            n_neighbours = layer_matrix.sum(axis=0) # Number of neighbours for each spatial unit
+
+            # Print a warning if it is the first layer with no neighbour for some of the spatial units
+            if len(n_neighbours[n_neighbours==0])>0 and zero_neighbour_flag ==0 and verbose != -1:
+                zero_neighbour_flag = 1
+                print("\nWarning: Some spatial units in layer {0} have no neighbors. The value 0 is considered for these spatial units.\n".format(layer))
+
+            n_neighbours[n_neighbours==0] = 1 # Avoiding division by zero error
+            covar_array = covar_array/n_neighbours # Get the mean of the covar values for the neighbours
+            covar_df = pd.DataFrame(data = covar_array, index = list(covar_df.index), columns = list(covar_df.columns))
+            spatial_ids = list(covar_df.columns)
+            covar_df[temporal_identifier_column_name] = list(covar_df.index)
+            covar_df = pd.melt(covar_df, id_vars = [temporal_identifier_column_name], value_vars = spatial_ids, var_name = 'spatial id level 1', value_name = covar+'_l'+str(layer))
+            data = pd.merge(data, covar_df, on = [temporal_identifier_column_name,'spatial id level 1'], sort = True, how = 'left')
+
+    if time_dependency_flag == 0:
+        data.drop('temporal id', axis = 1, inplace = True)
+
+    if 'dummy temporal id' in data.columns:
+        data.drop(['dummy temporal id'], axis = 1, inplace = True)
+
+    data = rename_columns(data.copy(), column_identifier, 'deformalize', 0)
+
+    return data
+
+
+#########################################################################################
+############################  making historical data ####################################
+#########################################################################################
+
+
+def make_historical_data(data, forecast_horizon, history_length = 1, column_identifier = None,
+                         futuristic_covariates = None, future_data_table = None, step = 1, verbose = 0):
+
+    future_data = True
+    if type(data) != dict :
+        if type(data) == str :
+            try:
+                data = pd.read_csv(data)
+            except FileNotFoundError:
+                raise FileNotFoundError("File '{0}' does not exist.\n".format(data))
+        elif type(data) != pd.DataFrame :
+            raise TypeError("The input data must be of type DataFrame, string, or a dict containing temporal and spatial DataFrames or addresses.\n")
+        data = rename_columns(data.copy(), column_identifier)
+
+        check_validity(data.copy(), input_name = 'data', data_type = 'full', column_identifier = column_identifier)
+
+    elif type(data) == dict:
+        if 'temporal_data' in data.keys():
+
+            if type(data['temporal_data']) == str:
+                try:
+                    temporal_data = pd.read_csv(data['temporal_data'])
+                except FileNotFoundError:
+                    raise FileNotFoundError("File '{0}' does not exist.\n".format(data['temporal_data']))
+
+            elif type(data['temporal_data']) == pd.DataFrame:
+                temporal_data = data['temporal_data']
+            else:
+                raise ValueError("The value of the 'temporal_data' key in the data dictionary must be a DataFrame or the address of temporal data.\n")
+            temporal_data = rename_columns(temporal_data.copy(), column_identifier)
+            check_validity(temporal_data.copy(), input_name = 'temporal_data',
+                           data_type = 'temporal', column_identifier = column_identifier)
+
+        else:
+            raise Exception("The data on temporal covariates and target variable must be passed to the function using data argument and as a DataFrame, Data address or value of 'temporal_data' key in the dictionary of data. But none is passed.\n")
+
+
+        if ('spatial_data' in data.keys()) and (data['spatial_data'] is not None):
+
+            if type(data['spatial_data']) == str:
+                try:
+                    spatial_data = pd.read_csv(data['spatial_data'])
+                except FileNotFoundError:
+                    raise ("File '{0}' does not exist.\n".format(data['spatial_data']))
+
+            elif type(data['spatial_data']) == pd.DataFrame:
+                spatial_data = data['spatial_data']
+            else:
+                raise ValueError("The value of the 'spatial_data' key in the data dictionary must be a DataFrame or the address of spatial data.\n")
+
+            spatial_data = rename_columns(spatial_data.copy(), column_identifier)
+            check_validity(spatial_data.copy(), input_name = 'spatial_data',
+                           data_type = 'spatial', column_identifier = column_identifier)
+
+            if len(list(set(temporal_data['spatial id level 1'].unique())-set(spatial_data['spatial id level 1'].unique())))>0:
+                print("\nWarning: Some of the spatial units in the temporal_data, are not recorded in the spatial_data. These spatial units will be ignored.\n")
+                temporal_data = temporal_data[temporal_data['spatial id level 1'].isin(spatial_data['spatial id level 1'].unique())]
+
+            data = pd.merge(temporal_data, spatial_data, on = 'spatial id level 1', how = 'left')
+
+        else:
+            data = temporal_data.copy()
+
+    # Non_integrated temporal id format
+    if 'temporal id' not in data.columns:
+            # find smallest temporal level
+            for level in range(1,200):
+                if 'temporal id level ' + str(level) in data.columns:
+                    smallest_temporal_level = level
+                    break
+            # add integrated temporal id
+            data = add_dummy_integrated_temporal_id(data.copy(), start_level = smallest_temporal_level)
+            # remove discrete temporal id columns
+            extra_temporal_ids = list(filter(lambda x:x.startswith('temporal id level '), data.columns))
+            data.drop(extra_temporal_ids, axis = 1, inplace = True)
+            data.rename(columns = {'dummy temporal id':'temporal id'}, inplace = True)
+
+
+    if 'target' not in data.columns:
+        raise ValueError("There is no column named 'target' in input data")
+
+    if column_identifier is None:
+        spatial_covariates = list(filter(lambda x:x.startswith('spatial covariate'), data.columns))
+        temporal_covariates = list(filter(lambda x:x.startswith('temporal covariate'), data.columns))
+    else:
+        if 'spatial covariates' in column_identifier.keys():
+            spatial_covariates = [item for item in list(column_identifier['spatial covariates']) if item in data.columns]
+        else: spatial_covariates = []
+        temporal_covariates = [item for item in list(column_identifier['temporal covariates']) if item in data.columns]
+
+    all_covariates = list(filter(lambda x: not x.startswith(('temporal id', 'spatial id', 'target', 'Normal target')), data.columns))
+    extra_columns = list(set(all_covariates)-set(spatial_covariates + temporal_covariates))
+
+    if len(extra_columns) > 0 :
+        print("\nWarning: Input data column names must match one of the specified formats:\n{'temporal id', 'temporal id level x', 'spatial id', 'spatial id level x', 'temporal covariate x', 'spatial covariate x', 'target'}, or be specified in column_identifier.\n")
+        print("But the names of some of the columns do not match any of the supported formats and is not mentioned in column_identifier:\n{0}\nThis columns will be ignored.\n".format(extra_columns))
+
+    ######################## check type of future_data_table
+
+    if type(future_data_table) == str:
+        try:
+            future_data_table = pd.read_csv(future_data_table)
+        except FileNotFoundError:
+            raise ("File '{0}' does not exist.\n".format(future_data_table))
+
+    elif (type(future_data_table) != pd.DataFrame) and (future_data_table is not None):
+        raise TypeError("The future_data_table must be a data frame or address of the data frame containing the values of futuristic covariates in the future.")
+
+
+    ######################## check type and validity of input history_length and futuristic_covariates #####################
+    if type(history_length) == int:
+        if history_length == 0 : history_length = 1
+        history_length_dict = {covar:history_length for covar in temporal_covariates}
+        max_history_length = history_length # maximum history length of all temporal covariates
+
+    elif type(history_length) == dict:
+
+        key_list = list(history_length.keys())
+        for item in key_list:
+            if type(item) == tuple:
+                for key in item:
+                    history_length[key] = history_length[item]
+                del history_length[item]
+
+        extra_hist_covariates = list(set(history_length.keys()) - set(temporal_covariates))
+
+        if (len(extra_hist_covariates) > 0) and (verbose > 0):
+            print("\nWarning: The following keys in the history_length do not exist in the input data temporal covariates, and thus will be ignored:\n{0}\n".format(extra_hist_covariates))
+
+        history_length = {key:value for key, value in history_length.items() if key not in extra_hist_covariates}
+        # The history length of 0 is interpreted to no historical values which is same as history length = 1
+        for key, value in history_length.items():
+            if value == 0: history_length[key] = 1
+
+        history_length_dict = history_length.copy()
+
+        # if covariate doesnt mentioned in history_length or futuristic_covariates
+        unspecified_history_covariates = list(set(temporal_covariates)-set(history_length_dict.keys()))
+        if (futuristic_covariates is not None) and (type(futuristic_covariates) == dict):
+            unspecified_history_covariates = list(set(unspecified_history_covariates) - set(futuristic_covariates.keys()))
+
+        if len(unspecified_history_covariates)> 0:
+            print("\nWarning: The history length of some temporal covariates is not specified in history_length:\n{0}\nFor these covariates the history length of 1 will be considered.\n".format(unspecified_history_covariates))
+        for covar in unspecified_history_covariates:
+            history_length_dict[covar] = 1
+        for covar in history_length_dict.keys():
+            if type(history_length_dict[covar]) != int:
+                raise ValueError("The specified history length for each covariate in the history_length dict must be of type int.\n")
+        max_history_length = max(history_length_dict.values())
+
+    else:
+        raise TypeError("The history_length must be of type int or dict.\n")
+
+    if futuristic_covariates is not None:
+        if type(futuristic_covariates) == dict:
+            for covar in futuristic_covariates.keys():
+                if (len(futuristic_covariates[covar])!=2) or (futuristic_covariates[covar][1]-futuristic_covariates[covar][0]<0):
+                    raise ValueError("The temporal interval of each futuristic covariate must be specified in futuristic_covariates dict using a list including start and end of the interval as first and second item.\n")
+                elif (type(futuristic_covariates[covar][0])!=int)or(type(futuristic_covariates[covar][1])!=int):
+                    raise ValueError("The start and end point of futuristic covariates temporal interval must be of type int.\n")
+                elif futuristic_covariates[covar][1] > forecast_horizon:
+                    raise ValueError("The end point of futuristic covariates temporal interval must be smaller than forecast_horizon.\n")
+                else:
+                    history_length_dict['future '+covar] = futuristic_covariates[covar][1] - futuristic_covariates[covar][0] + 1
+
+        else:
+            raise TypeError("The futuristic_covariates must be of type dict.\n")
+
+        key_list = list(futuristic_covariates.keys())
+        for item in key_list:
+            if type(item) == tuple:
+                for key in item:
+                    futuristic_covariates[key] = futuristic_covariates[item]
+                del futuristic_covariates[item]
+
+        invalid_futuristic_covariates = list(set(futuristic_covariates.keys()) - set(temporal_covariates))
+
+        if (len(invalid_futuristic_covariates) > 0) and (verbose > 0):
+            print("\nWarning: The following keys in the futuristic_covariates do not exist in the input data temporal covariates, and thus will be ignored:\n{0}\n".format(invalid_futuristic_covariates))
+
+        futuristic_covariates = {key:value for key, value in futuristic_covariates.items() if key not in invalid_futuristic_covariates}
+
+    ######################## check type and validity of forecast horizon
+
+    if type(forecast_horizon) != int:
+        raise TypeError("The forecast_horizon must be of type int.")
+    elif forecast_horizon == 0:
+        forecast_horizon = 1
+
+    ############## preparing data
+
+    # adding future values of futuristic covariates to the data
+    if future_data_table is not None:
+        data, future_data_table, futuristic_temporal_units = current_future(data = data.copy(), future_data_table = future_data_table,
+                                                              futuristic_covariates = futuristic_covariates,
+                                                              column_identifier = column_identifier , mode = 'add')
+    else:
+        _, _, futuristic_temporal_units = current_future(data = data.copy(),
+                                                              future_data_table = None,
+                                                              futuristic_covariates = futuristic_covariates,
+                                                              column_identifier = column_identifier , mode = 'split')
+
+
+    number_of_futuristic_temporal_units = len(futuristic_temporal_units)
+    data = data.drop_duplicates(subset = ['temporal id','spatial id level 1']).copy()
+    data = data.sort_values(by = ['temporal id','spatial id level 1']).copy()
+
+    ####################################### main part #######################################
+
+    if verbose > 0:
+        if type(history_length) == int :
+            print("\nMaking historical data with the forecast horizon of {0} and history length of {1} is running.\n".format(forecast_horizon, history_length))
+        else:
+            print("\nMaking historical data with the forecast horizon of {0} is running.\n".format(forecast_horizon))
+
+    result = pd.DataFrame()  # we store historical data in this dataframe
+    total_number_of_spatial_units = len(data['spatial id level 1'].unique())
+    total_number_of_temporal_units = len(data['temporal id'].unique())
+
+    if total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)) <= 0:
+        if verbose > 0 :
+            print("\nWarning: The specified history length and forecast horizon is too large for the number of recorded temporal units in the input data.\n")
+        return None
+
+    if futuristic_covariates is None:
+        futuristic_covariates = {}
+
+    # in this loop we make historical data
+    for covar in all_covariates:
+        # if covariate is time dependant
+        if covar in temporal_covariates:
+
+
+            temporal_data_frame = data[[covar]] # selecting column of the covariate that is being processed
+            # shift data to the size of futuristic temporal interval end point
+            if covar in futuristic_covariates.keys():
+                covar_history_length = history_length_dict['future '+covar]
+                threshold = futuristic_covariates[covar][0]
+
+                while threshold != futuristic_covariates[covar][1]+1:
+                    temp = temporal_data_frame.tail((total_number_of_temporal_units + (step*(- max_history_length - threshold + 1)))*total_number_of_spatial_units).reset_index(drop=True)
+                    temp.rename(columns={covar: (covar.replace(' ','_') + ' t+' + str(threshold))}, inplace=True) # renaming column
+                    result = pd.concat([result, temp], axis=1)
+                    threshold += 1
+
+            if covar in history_length_dict.keys():
+                covar_history_length = history_length_dict[covar]
+                # the first temporal unit of historical data is determined based on the maximum history length of covariates
+                # therefore data of covariates with smaller history length should be shifted forward
+                if covar_history_length < max_history_length:
+                    temporal_data_frame = temporal_data_frame.iloc[(step*(max_history_length-covar_history_length))*total_number_of_spatial_units:]
+
+                threshold = 0
+                while threshold != covar_history_length:
+
+                    # if future_data is true, the feature values of the last temporal units with the size of
+                    # forecast_horizon (which their target variable values are unknown) will be considered in historical data
+                    if future_data == False:
+                        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
+                    else:
+                        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
+
+                    temp.rename(columns={covar: (covar.replace(' ','_') + ' t-' + str(covar_history_length-threshold-1))}, inplace=True) # renaming column
+
+                    result = pd.concat([result, temp], axis=1)
+                    # deleting the values in first day in temporal_data_frame dataframe (similiar to shift)
+                    temporal_data_frame = temporal_data_frame.iloc[step*total_number_of_spatial_units:]
+                    threshold += 1
+
+        # if covariate is independant of time
+        elif covar in spatial_covariates:
+
+            temporal_data_frame = data[[covar]]
+            if future_data == False:
+                temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
+            else:
+                temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
+
+            temp.rename(columns={covar: (covar.replace(' ','_'))}, inplace=True)
+            if covar == 'Target':
+                temp.rename(columns={covar: ('Target_0')}, inplace=True)
+            result = pd.concat([result, temp], axis=1)
+
+    # next 6 lines is for spatial id code to final dataframe
+    temporal_data_frame = data[['spatial id level 1']]
+    if future_data == False:
+        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
+    else:
+        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
+    result.insert(0, 'spatial id', temp)
+
+    # next 7 lines is for adding id of temporal unit (t) to final dataframe
+    temporal_data_frame = data[['temporal id']]
+    temporal_data_frame = temporal_data_frame[total_number_of_spatial_units*(step*(max_history_length - 1)):]
+    if future_data == False:
+        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
+    else:
+        temp = temporal_data_frame.head((total_number_of_temporal_units + (step*(- max_history_length + 1)))*total_number_of_spatial_units).copy().reset_index(drop=True)
+    result.insert(1, 'temporal id', temp)
+
+    # next 3 lines is for adding target to final dataframe
+    temporal_data_frame = data[['target']]
+    temporal_data_frame = temporal_data_frame.tail((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).reset_index(drop=True)
+    result.insert(2, 'Target', temporal_data_frame)
+
+    # next 4 lines is for adding normal target to final dataframe if target mode is not normal
+    if 'Normal target' in data.columns:
+        temporal_data_frame = data[['Normal target']]
+        temporal_data_frame = temporal_data_frame.tail((total_number_of_temporal_units + (step*(- max_history_length - forecast_horizon + 1)))*total_number_of_spatial_units).reset_index(drop=True)
+        result.insert(3, 'Normal target', temporal_data_frame)
+
+    for i in result.columns:
+        if (i.endswith('t-0')) and (i not in spatial_covariates):
+            result.rename(columns={i: i[:-2]}, inplace=True)
+
+    # last samples are related to the futuristic data and has no values for temporal covariates
+    # so must be removed from historical data
+    if number_of_futuristic_temporal_units > 0:
+        number_of_spatial_units = len(result['spatial id'].unique())
+        result = result.sort_values(by = ['temporal id', 'spatial id'])
+        result = result.iloc[:-(number_of_futuristic_temporal_units*number_of_spatial_units)]
+
+    return result
+
+################################################################################################
+############################  base function data preprocess ####################################
+################################################################################################
+
+def preprocess_data(data, forecast_horizon, history_length = 1, column_identifier = None, spatial_scale_table = None,
+                    spatial_scale_level = 1, temporal_scale_level = 1,
+                    target_mode = 'normal', imputation = True, aggregation_mode = 'mean', augmentation = False,
+                    futuristic_covariates = None, future_data_table = None, neighbouring_matrix = None, neighbouring_layers = 0,
+                    save_address = None, verbose = 0):
+
+
+    ####################
+
+    spatial_covariates = []
+    temporal_covariates = []
+    granularity = None
+    target_granularity = None
+
+    # prepare data (renaming columns, remove extra columns and get spatial and temporal data separately)
+    temporal_data, spatial_data = prepare_data(data.copy(), column_identifier)
+
+
+    #################### get list of covariates
+
+    # if type of each column is specified in column_identifier
+    if column_identifier is not None:
+        temporal_covariates =  list(set(column_identifier['temporal covariates']) & set(temporal_data.columns))
+        if ('spatial covariates' in column_identifier.keys()) and (spatial_data is not None):
+            spatial_covariates =  list(set(column_identifier['spatial covariates']) & set(spatial_data.columns))
+
+    # if type of columns are clear based on column name
+    else:
+        temporal_covariates = list(filter(lambda x: x.startswith('temporal covariate'), temporal_data.columns))
+        if spatial_data is not None:
+            spatial_covariates = list(filter(lambda x: x.startswith('spatial covariate'), spatial_data.columns))
+
+
+    # if input data has no covariate (spatial or temporal)
+    if len(temporal_covariates) == 0:
+        if (spatial_data is None) or (len(spatial_covariates) == 0):
+            raise ValueError("There is no spatial or temporal covariate included in input data")
+
+    # if input data has no target
+    if 'target' not in temporal_data.columns:
+        raise ValueError("The target variable is not recorded in input data and doesn't specified in column_identifier.\nmissing column: 'target'")
+
+    ############## check the futuristic_covariate input validity
+
+    if futuristic_covariates is not None:
+        if type(futuristic_covariates) == dict:
+            for item in futuristic_covariates.keys():
+                if (len(futuristic_covariates[item])!=2) or (futuristic_covariates[item][1]-futuristic_covariates[item][0]<0):
+                    raise ValueError("The temporal interval of each futuristic covariate must be specified in futuristic_covariates dict using a list including start and end of the interval as first and second item.\n")
+                elif (type(futuristic_covariates[item][0])!=int)or(type(futuristic_covariates[item][1])!=int):
+                    raise ValueError("The start and end point of futuristic covariates temporal interval must be of type int.\n")
+                elif futuristic_covariates[item][1] > forecast_horizon:
+                    raise ValueError("The end point of futuristic covariates temporal interval must be smaller than forecast_horizon.\n")
+        else:
+            raise TypeError("The futuristic_covariates must be of type dict.\n")
+
+        key_list = list(futuristic_covariates.keys())
+        for item in futuristic_covariates.keys():
+            if type(item) == tuple:
+                for key in item:
+                    futuristic_covariates[key] = futuristic_covariates[item]
+                del futuristic_covariates[item]
+
+
+        # Removing invalid covariates from data and produce warning if is needed
+        invalid_futuristic_covariates = list(set(futuristic_covariates.keys()) - set(temporal_covariates))
+        if (len(invalid_futuristic_covariates) > 0) and (verbose > 0):
+            print("\nWarning: The following keys in the futuristic_covariates do not exist in the input data covariates, and thus will be ignored:\n{0}\n".format(invalid_futuristic_covariates))
+
+        futuristic_covariates = {key:value for key, value in futuristic_covariates.items() if key not in invalid_futuristic_covariates}
+
+
+    ############# check the history_length input validity
+
+    if type(history_length) == dict :
+        for covar in history_length.keys():
+            if (type(history_length[covar]) != int) and (covar in temporal_covariates) :
+                  raise TypeError("\nThe maximum history length of covariates specified in history_length must be of type int.")
+
+        key_list = list(history_length.keys())
+        for item in key_list:
+            if type(item) == tuple:
+                for key in item:
+                    history_length[key] = history_length[item]
+                del history_length[item]
+
+        extra_hist_covariates = list(set(history_length.keys()) - set(temporal_covariates))
+
+        if (len(extra_hist_covariates) > 0) and (verbose > 0):
+            print("\nWarning: The following keys in the history_length do not exist in the input data temporal covariates, and thus will be ignored:\n{0}\n".format(extra_hist_covariates))
+
+        history_length = {key:value for key, value in history_length.items() if key not in extra_hist_covariates}
+
+    ######################## check type and validity of forecast horizon
+
+    if type(forecast_horizon) != int:
+        raise TypeError("The forecast_horizon must be of type int.")
+    elif forecast_horizon == 0:
+        forecast_horizon = 1
+
+    ######################## check type and temporal_scale_level and augmentation
+
+    if (temporal_scale_level < 2) and (augmentation == True):
+        raise Exception("The augmentation can only be performed for temporal_scale_level greater than one.")
+
+    ######################## check type of future_data_table
+
+    if type(future_data_table) == str:
+        try:
+            future_data_table = pd.read_csv(future_data_table)
+        except FileNotFoundError:
+            raise FileNotFoundError("File '{0}' does not exist.\n".format(future_data_table))
+
+    elif (type(future_data_table) != pd.DataFrame) and (future_data_table is not None):
+        raise TypeError("The future_data_table must be a data frame or address of the data frame containing the values of futuristic covariates in the future.")
+
+    ######################## check neighbouring_matrix
+    if neighbouring_matrix is not None:
+        if not isinstance(neighbouring_matrix,np.ndarray):
+            raise TypeError("The neighbouring_matrix must be of type numpy array.\n")
+        elif len(neighbouring_matrix.shape)<2:
+            raise ValueError("The adjacency matrix must be a two-dimensional numpy array with dimensions equal to the number of spatial units. Each element of this matrix specifies the adjacency (1) or lack of adjacency (0) between two spatial units.\n")
+
+
+    ############################## Imputation ##############################
+
+    if imputation == True :
+
+        # removing the rows related to the future data before imputation
+        if future_data_table is None:
+            temporal_data, future_data_table, _ = current_future(data = temporal_data.copy(), future_data_table = None,
+                                                              futuristic_covariates = futuristic_covariates,
+                                                              column_identifier = column_identifier , mode = 'split')
+
+        if verbose > 0:
+            print("-"*45+"\nThe imputation of missing values is running.\n"+"-"*45+"\n")
+
+        temporal_data = impute(temporal_data.copy(), None, verbose = 0)
+
+        if spatial_data is not None:
+            number_of_raw_spatial_units = spatial_data.shape[0]
+            spatial_data.dropna(inplace = True)
+            number_of_removed_spatial_units = number_of_raw_spatial_units - spatial_data.shape[0]
+
+            if number_of_removed_spatial_units == number_of_raw_spatial_units:
+                raise ValueError("All the spatial units include missing values for spatial covariates. Therefore, no spatial unit remains to make a prediction.\n")
+            elif number_of_removed_spatial_units > 0:
+                print('\nWarning: The number of {0} spatial units has missing values for spatial covariates and will be removed from the data.\n'.format(number_of_removed_spatial_units))
+
+        # Holding only the spatial units that are common in both data frames
+        if spatial_data is not None:
+
+            non_common_spatial_units = set(temporal_data['spatial id level 1'].unique()).union(set(spatial_data['spatial id level 1'].unique())) - set(temporal_data['spatial id level 1'].unique()).intersection(set(spatial_data['spatial id level 1'].unique()))
+
+            if len(list(non_common_spatial_units)) > 0:
+                print("\nWarning: The following spatial units exists only in one of the spatial or temporal data:\n",list(non_common_spatial_units))
+                print("\n These spatial units will be removed from the data.\n")
+
+            temporal_data = temporal_data[temporal_data['spatial id level 1'].isin(spatial_data['spatial id level 1'].unique())]
+            spatial_data = spatial_data[spatial_data['spatial id level 1'].isin(temporal_data['spatial id level 1'].unique())]
+
+    # adding future values of futuristic covariates to the data and get the futuristic temporal units
+    if future_data_table is not None:
+        temporal_data, future_data_table, futuristic_temporal_units = current_future(data = temporal_data.copy(), future_data_table = future_data_table,
+                                                              futuristic_covariates = futuristic_covariates,
+                                                              column_identifier = column_identifier , mode = 'add')
+    else:
+        _, _, futuristic_temporal_units = current_future(data = temporal_data.copy(),
+                                                              future_data_table = None,
+                                                              futuristic_covariates = futuristic_covariates,
+                                                              column_identifier = column_identifier , mode = 'split')
+
+    ############################## spatial scale transform ##############################
+
+    if spatial_scale_level > 1:
+
+        if verbose > 0:
+            print("-"*65+"\nTransformation of data to the desired spatial scale is running.\n"+"-"*65+"\n")
+
+        if type(aggregation_mode) == dict:
+            extra_covariates_listed = list(set(aggregation_mode.keys())-set(spatial_covariates + temporal_covariates + ['target']))
+            unspecified_covariates = list(set(spatial_covariates + temporal_covariates + ['target'])-set(aggregation_mode.keys()))
+
+            if len(extra_covariates_listed) > 0:
+                print("\nWarning : Some of the covariates specified in aggregation_mode are not exist in the data:\n{0}".format(extra_covariates_listed))
+                aggregation_mode = {covariate : mode for covariate,mode in aggregation_mode.items() if covariate not in extra_covariates_listed}
+
+            if len(unspecified_covariates)>0:
+                if verbose < 2:
+                    print("\nWarning : The aggregation_mode is not specified for some of the covariates.\nThe mean operator will be used to aggregate these covariates' values.\n")
+                if verbose == 2:
+                    print("\nWarning : The aggregation_mode is not specified for some of the covariates:\n{0}\nThe mean operator will be used to aggregate these covariates' values.\n".format(unspecified_covariates))
+                for covar in unspecified_covariates:
+                      aggregation_mode[covar] = 'mean'
+
+            if spatial_data is not None:
+                    spatial_aggregation_mode = {covariate : mode for covariate,mode in aggregation_mode.items() if covariate in spatial_covariates}
+
+            temporal_aggregation_mode = {covariate : mode for covariate,mode in aggregation_mode.items() if covariate in temporal_covariates + ['target']}
+
+        # if aggregation_mode is not dict and is same for all covariates
+        else:
+            spatial_aggregation_mode = temporal_aggregation_mode = aggregation_mode
+
+        if spatial_scale_table is not None:
+            spatial_scale_table = rename_columns(data = spatial_scale_table.copy(), column_identifier = column_identifier)
+
+        # transformation
+        temporal_data = spatial_scale_transform(temporal_data.copy(), 'temporal', column_identifier = None, spatial_scale_table = spatial_scale_table, spatial_scale_level = spatial_scale_level, aggregation_mode = temporal_aggregation_mode, verbose = 0)
+        if spatial_data is not None:
+            spatial_data = spatial_scale_transform(spatial_data.copy(), 'spatial', column_identifier = None, spatial_scale_table = spatial_scale_table, spatial_scale_level = spatial_scale_level, aggregation_mode = spatial_aggregation_mode, verbose = 0)
+            # if the desired spatial scale has only one spatial unit, the spatial covariates couldn't be used for prediction
+            if len(spatial_data)==1:
+                spatial_data = None
+                print("\nWarning: The desired spatial scale has only one spatial unit in the data, so spatial covariates' values is same for all the data samples and couldn't be used for prediction.\n")
+
+        # to pass the data to the other functions, it must be same as raw data
+        spatial_identifier = list(filter(lambda x: x.startswith(('spatial id')),temporal_data.columns))[0]
+        temporal_data.rename(columns = {spatial_identifier:'spatial id level 1'}, inplace = True)
+
+        if spatial_data is not None:
+            spatial_identifier = list(filter(lambda x: x.startswith(('spatial id')),spatial_data.columns))[0]
+            spatial_data.rename(columns = {spatial_identifier:'spatial id level 1'}, inplace = True)
+
+    ############################## temporal scale transform ##############################
+
+    if temporal_scale_level > 1:
+
+        if verbose > 0:
+            print("-"*65+"\nTransformation of data to the desired temporal scale is running.\n"+"-"*65+"\n")
+
+        # if user prefer to augment data granularity (number of smaller scale temporal units in the bigger scale temporal unit)
+        # will be needed for making historical data
+        if augmentation == True:
+            granularity = find_granularity(temporal_data.copy(), temporal_scale_level)
+
+        # filling up the future temporal units null values with inf to recognize the future temporal units
+        # after temporal transform and return its values to null for non futuristic covariates
+        temporal_data = fill_future_nulls(data = temporal_data.copy(), futuristic_temporal_units = futuristic_temporal_units)
+
+        # transformation
+        temporal_data = temporal_scale_transform(temporal_data.copy(), temporal_scale_level = temporal_scale_level, augmentation = augmentation, verbose = 0)
+
+        # return null values of non futuristic covariates in future temporal units
+        temporal_data = temporal_data.replace([np.inf, -np.inf], np.nan)
+
+        # to pass the data to the other functions, it must be same as raw data
+        # the next lines reset the names of temporal id level columns to start from level one (only needed for non_integrated temporal id format)
+        if augmentation == False:
+
+            current_smallest_temporal_level = 'temporal id level '+str(temporal_scale_level)
+
+            # if non_integrated temporal id format
+            if current_smallest_temporal_level in temporal_data.columns:
+                temporal_data.rename(columns = {current_smallest_temporal_level:'temporal id level 1'}, inplace = True)
+                for level in range(temporal_scale_level+1, 200):
+                    if 'temporal id level '+str(level) in temporal_data.columns:
+                        # shift the level by temporal_scale_level units
+                        shifted_level = level - temporal_scale_level + 1
+                        temporal_data.rename(columns = {'temporal id level '+str(level):'temporal id level '+str(shifted_level)}, inplace = True)
+                    else:
+                        break
+    ############################## target modification ##############################
+
+    if (target_mode != 'normal') and (verbose > 0):
+            print("-"*35+"\nTarget modification is running.\n"+"-"*35+"\n")
+
+    # removing the rows related to the future data before target modification cause it may fill the value of target in future
+    if future_data_table is None:
+        temporal_data, future_data_table, _ = current_future(data = temporal_data.copy(), future_data_table = None,
+                                                          futuristic_covariates = futuristic_covariates,
+                                                          column_identifier = column_identifier , mode = 'split')
+
+    if (target_mode == 'moving average'):
+        target_granularity = find_granularity(data = temporal_data.copy(), temporal_scale_level = None)
+
+    temporal_data = target_modification(temporal_data, target_mode = target_mode, verbose = 1)
+
+    if future_data_table is not None:
+        temporal_data, future_data_table, _ = current_future(data = temporal_data.copy(), future_data_table = future_data_table,
+                                                              futuristic_covariates = futuristic_covariates,
+                                                              column_identifier = column_identifier , mode = 'add')
+
+    ############################# make neighbouring data #############################
+
+    if neighbouring_layers > 0:
+
+        if verbose > 0:
+            print("-"*35+"\nMaking neighbouring data is running.\n"+"-"*35+"\n")
+
+        if neighbouring_matrix.shape[0] != len(temporal_data['spatial id level 1'].unique()) or neighbouring_matrix.shape[1] != len(temporal_data['spatial id level 1'].unique()):
+            raise ValueError("The dimensions of neighboring_matrix do not match to the number of spatial units in the temporal data.")
+        temporal_data = make_neighbouring_data(data = temporal_data.copy(), column_identifier = column_identifier,
+                                               number_of_layers = neighbouring_layers, neighbouring_matrix = neighbouring_matrix,
+                                               time_dependency_flag = 1, verbose = verbose)
+        if neighbouring_matrix.shape[0] != len(spatial_data['spatial id level 1'].unique()) or neighbouring_matrix.shape[1] != len(spatial_data['spatial id level 1'].unique()):
+            raise ValueError("The dimensions of neighboring_matrix do not match to the number of spatial units in the spatial data.")
+        if spatial_data is not None:
+            spatial_data = make_neighbouring_data(data = spatial_data.copy(), column_identifier = column_identifier,
+                                                   number_of_layers = neighbouring_layers, neighbouring_matrix = neighbouring_matrix,
+                                                   time_dependency_flag = 0, verbose = -1)
+        # recorrecting column_identifier
+        for layer in range(1,neighbouring_layers+1):
+            if column_identifier is not None:
+                for covar in temporal_covariates:
+                    if covar+'_l'+str(layer) in list(temporal_data.columns):
+                        column_identifier['temporal covariates'] = column_identifier['temporal covariates'] + [covar+'_l'+str(layer)]
+
+                for covar in spatial_covariates:
+                    if covar+'_l'+str(layer) in list(spatial_data.columns):
+                        column_identifier['spatial covariates'] = column_identifier['spatial covariates'] + [covar+'_l'+str(layer)]
+
+            if type(history_length) == dict:
+                copy_of_history_length = history_length.copy()
+                for covar,hist_len in copy_of_history_length.items():
+                    if type(covar) == str:
+                        if covar + '_l' + str(layer) in list(temporal_data.columns):
+                            history_length[covar + '_l' + str(layer)] = history_length[covar]
+                    elif type(covar) == tuple:
+                        for cov in covar:
+                            if cov + '_l' + str(layer) in list(temporal_data.columns):
+                                history_length[cov + '_l' + str(layer)] = history_length[covar]
+            copy_of_futuristic_covariates = futuristic_covariates.copy()
+            for covar, interval in copy_of_futuristic_covariates.items():
+                if type(covar) == str:
+                    if covar + '_l' + str(layer) in list(temporal_data.columns):
+                        futuristic_covariates[covar + '_l' + str(layer)] = futuristic_covariates[covar]
+                elif type(covar) == tuple:
+                    for cov in covar:
+                        if cov + '_l' + str(layer) in list(temporal_data.columns):
+                            futuristic_covariates[cov + '_l' + str(layer)] = futuristic_covariates[covar]
+
+
+    temporal_data = rename_columns(temporal_data.copy(), column_identifier)
+    if spatial_data is not None:
+        spatial_data = rename_columns(spatial_data.copy(), column_identifier)
+
+    ############################## make historical data ##############################
+
+    if verbose > 0:
+        print("-"*35+"\nMaking historical data is running.\n"+"-"*35+"\n")
+
+    # next lines is for detecting total number of temporal units in the data
+    # to produce warning if it is less than needed number
+    if 'temporal id' in temporal_data.columns:
+        total_number_of_temporal_units =  len(temporal_data['temporal id'].unique())
+    else:
+        # add integrated temporal id
+        temporal_data = add_dummy_integrated_temporal_id(temporal_data.copy(), start_level = 1)
+        total_number_of_temporal_units =  len(temporal_data['dummy temporal id'].unique())
+        temporal_data = temporal_data.drop(['dummy temporal id'],axis = 1)
+
+    # if augmentation == True, for each sample in temporal unit i, if this sample is in index u,
+    # the next sample in temporal unit i+1 is placed in index u+granularity. so in making historical data,
+    # the step size to go back and get historical values of covariates or move forward to consider future
+    # values of the target variable must be equal to the granularity
+
+    if augmentation == True:
+        step = granularity
+    else:
+        step = 1
+
+    if type(history_length) == int:
+
+        if total_number_of_temporal_units + (step*(- history_length - forecast_horizon + 1)) <= 0:
+            print("\nWarning: The specified history length and forecast horizon is too large for the number of recorded temporal units in the input data.\n")
+
+
+        # input data
+        if spatial_data is not None:
+            make_hist_data = {'temporal_data':temporal_data.copy(),'spatial_data':spatial_data.copy()}
+        else:
+            make_hist_data = {'temporal_data':temporal_data.copy(),'spatial_data':spatial_data}
+
+        historical_data = make_historical_data(data = make_hist_data,
+                                               forecast_horizon = forecast_horizon, column_identifier = column_identifier,
+                                               history_length = history_length, futuristic_covariates = futuristic_covariates,
+                                               future_data_table = None, step = step, verbose = 0)
+        if historical_data is not None:
+            historical_data = recorrect_hist_data(historical_data, augmentation, granularity, target_mode, target_granularity)
+
+            if save_address is not None:
+                try:
+                    historical_data.to_csv(save_address+'historical_data h={0}.csv'.format(history_length))
+                except FileNotFoundError:
+                        print("The address '{0}' is not valid.".format(save_address))
+
+    elif type(history_length) == dict:
+        historical_data = {}
+        unspecified_covariate = []
+
+        for covar in temporal_covariates:
+            if covar not in history_length.keys():
+                if futuristic_covariates is None:
+                    history_length[covar] = 1
+                    unspecified_covariate.append(covar)
+                elif covar not in futuristic_covariates.keys():
+                    history_length[covar] = 1
+                    unspecified_covariate.append(covar)
+
+        if len(unspecified_covariate)>0:
+            if verbose < 2:
+                print("\nWarning: The maximum history length of some covariates is not specified in history_length. The history length of 1 will be considered for these covariates.\n")
+            elif verbose == 2:
+                print("\nWarning: The maximum history length of some covariates is not specified in history_length. The history length of 1 will be considered for these covariates:\n{0}\n".format(unspecified_covariate))
+
+        # The max history length of 0 is interpreted to no historical values which is same as history length = 1
+        for key, value in history_length.items():
+            if value == 0: history_length[key] = 1
+
+        current_history_length = {covar : 0 for covar in history_length.keys()}
+
+        max_history_length = max(history_length.values())
+
+        impossible_histories = []
+        for hist in range(1,max_history_length+1):
+            if total_number_of_temporal_units + (step*(- hist - forecast_horizon + 1)) <= 0:
+                impossible_histories.append(hist)
+        if len(impossible_histories) > 0:
+            print("Warning: The number of temporal units in the data is not enough to construct a historical data with the specified forecast horizon and the history length(s):\n{0}".format(impossible_histories))
+
+        for stage in range(1,max_history_length+1):
+            for covar in history_length.keys():
+                  if current_history_length[covar]+1 <= history_length[covar]:
+                        current_history_length[covar] = current_history_length[covar] + 1
+
+            # input data
+            if spatial_data is not None:
+                make_hist_data = {'temporal_data':temporal_data.copy(),'spatial_data':spatial_data.copy()}
+            else:
+                make_hist_data = {'temporal_data':temporal_data.copy(),'spatial_data':None}
+
+            historical_data[stage] = make_historical_data(data = make_hist_data,
+                                                    forecast_horizon = forecast_horizon, column_identifier = column_identifier,
+                                                    history_length = current_history_length,
+                                                    futuristic_covariates = futuristic_covariates,
+                                                    future_data_table = None,
+                                                    step = step, verbose = 0)
+
+            if historical_data[stage] is not None:
+
+                historical_data[stage] = recorrect_hist_data(historical_data[stage], augmentation, granularity, target_mode, target_granularity)
+
+                if save_address is not None:
+                    try:
+                        historical_data[stage].to_csv(save_address+'historical_data h=' + str(stage) +'.csv', index = False)
+                    except FileNotFoundError:
+                            print("The address '{0}' is not valid.".format(save_address))
+
+        historical_data_list =  [value for key,value in historical_data.items()]
+        historical_data = historical_data_list
+
+    return historical_data
+
+################################################################################################
+#################################  plotting the data ###########################################
+################################################################################################
+
+def plot_data(data, spatial_scale_table, temporal_covariate = 'default' ,spatial_scale = 1, spatial_id = None,
+              temporal_scale = 1, temporal_range = None, column_identifier = None, month_format_print=False,
+              saving_plot_path = None):
+
+    ######################### check validity of input arguments
+    if type(data) == str:
+        try:
+            data = pd.read_csv(data)
+        except FileNotFoundError:
+            raise FileNotFoundError("File '{0}' does not exist.\n".format(data))
+
+    elif type(data) != pd.DataFrame:
+        raise TypeError("The input data must be of type DataFrame or string.")
+
+    df = rename_columns(data = data, column_identifier = column_identifier, error = 0)
+    check_validity(df.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier, error = 0)
+
+    if type(spatial_id) == list:
+        if len(spatial_id)>3 :
+            print("The number of spatial_ids must be a maximum of 3.")
+        spatial_id = spatial_id[:3]
+    elif spatial_id is not None:
+        raise TypeError("The spatial_id must be of type list.")
+
+    ################## spatial scale transform #################
+
+    if spatial_scale > 1:
+
+        if spatial_scale_table is not None:
+            if type(spatial_scale_table) == str:
+                try:
+                    spatial_scale_table = pd.read_csv(spatial_scale_table)
+                except FileNotFoundError:
+                    raise FileNotFoundError("File '{0}' does not exist.\n".format(spatial_scale_table))
+            spatial_scale_table = rename_columns(data = spatial_scale_table.copy(), column_identifier = column_identifier, error = 0)
+
+        df = spatial_scale_transform(df, 'temporal', spatial_scale_table = spatial_scale_table, spatial_scale_level = spatial_scale, aggregation_mode = 'mean')
+
+    df.rename(columns = {'spatial id level '+str(spatial_scale):'spatial id level 1'},inplace = True)
+
+    ################ temporal scale transform #####################
+
+    if temporal_scale > 1:
+        df = temporal_scale_transform(df, column_identifier=None, temporal_scale_level = temporal_scale
+                                     , augmentation=False, verbose=1)
+
+
+    ################## select desired temporal interval for plot from data ###############
+
+    if (type(temporal_range) != dict) and (temporal_range is not None):
+        raise TypeError("The temporal_range most be of type dict.")
+
+    # if temporal id format is integrated
+    if 'temporal id' in df.columns:
+        temporal_identifier_column_name = 'temporal id'
+
+        scale_format = {'sec':'%Y/%m/%d %H:%M:%S', 'min':'%Y/%m/%d %H:%M', 'hour':'%Y/%m/%d %H', 'day':'%Y/%m/%d', 'week':'%Y/%m/%d', 'month':'%Y/%m', 'year':'%Y'}
+
+        # determining input data temporal scale and transforming temporal id's to timestamp
+        df , scale = check_integrated_temporal_id(df)
+
+        if temporal_range is not None:
+
+            first_day = temporal_range['temporal id'][0]
+            last_day = temporal_range['temporal id'][1]
+            # get first_day and last_day timestamp
+            first_day = datetime.datetime.strptime(first_day,scale_format[scale])
+            last_day = datetime.datetime.strptime(last_day,scale_format[scale])
+            df = df[(df['temporal id']>=first_day)&(df['temporal id']<=last_day)]
+
+        if month_format_print == True:
+            df['temporal id'] = df['temporal id'].apply(lambda x:datetime.datetime.strftime(x,'%Y/%B/%d'))
+        else:
+            df['temporal id'] = df['temporal id'].apply(lambda x:datetime.datetime.strftime(x,scale_format[scale]))
+
+    # if temporal id format is non_integrated
+    else:
+
+        if temporal_range is not None:
+            for temporal_id_level , interval in temporal_range.items():
+                df = df[(df[temporal_id_level]>=interval[0])&(df[temporal_id_level]<=interval[1])]
+
+        ##### month name for non-integrated ###############
+
+        if month_format_print==True:
+          if column_identifier is not None:
+            for values in column_identifier.values():
+                if values == 'month':
+                    month_index = [*column_identifier.values()].index(values)
+                    temporal_id_x = [*column_identifier.keys()][month_index]
+            try:
+                df[temporal_id_x] = df[temporal_id_x].apply(lambda x : calendar.month_name[x])
+            except(IndexError,TypeError):
+                pass
+
+        ##### next 5 lines add dummy temporal id for non_integrated temporal id format
+
+        if temporal_range is not None:
+            list_to_find_smallest_scale = temporal_range.keys()
+        else:
+            list_to_find_smallest_scale = df.columns
+
+        # determine smallest temporal id level
+        for level in range(1,200):
+            if 'temporal id level '+str(level) in list_to_find_smallest_scale:
+                smallest_temporal_level = level
+                break
+
+        add_dummy_integrated_temporal_id(df, start_level = level)
+        temporal_identifier_column_name = 'dummy temporal id'
+
+
+    ############ select desired spatial id #########
+
+    # select random spatial ids if spatial id input is not specified
+    if spatial_id is None:
+        df_spatial_id_values = list(df['spatial id level 1'].unique())
+        spatial_id = list([df_spatial_id_values[0]])
+
+    df_dict = {}
+
+    for j in range(int(len(spatial_id))):
+        df0=df['spatial id level 1'] == spatial_id[j]
+        df1 = df[df0]
+        dict_key = spatial_id[j]
+        df_dict[dict_key] = df1
+
+    ############ making plot ################
+
+    if temporal_covariate == 'default':
+        T_C = df1.keys().tolist()
+        T_C = list(filter(lambda x: not x.startswith(('temporal id','spatial id','dummy temporal id')), T_C))
+
+    else:
+        T_C=[temporal_covariate]
+
+    for par in T_C:
+
+        fig, ax = plt.subplots()
+        for SpatialId, DF in df_dict.items():
+            y = DF[par].tolist()
+            time = DF[temporal_identifier_column_name].tolist()
+            total_temporal_id_number = len(time) + 2
+            plt.plot(time, y, label=SpatialId, linewidth=1.0, marker='o', markersize=5)
+
+        # plt.xlabel('time')
+        plt.legend()
+        plt.ylabel(temporal_covariate)
+        plt.gcf().autofmt_xdate()
+        plt.ylabel(par)
+
+        # plt.grid()
+
+        default_xtick_size = plt.gcf().get_size_inches()[0]
+        plt.gca().margins(x=0.002)
+        plt.gcf().canvas.draw()
+        tl = plt.gca().get_xticklabels()
+        maxsize = max([t.get_window_extent().width for t in tl])
+        inch_margin = 0.5  # inch margin
+        xtick_size = maxsize / plt.gcf().dpi * total_temporal_id_number + inch_margin
+        margin = inch_margin / plt.gcf().get_size_inches()[0]
+
+        plt.gcf().subplots_adjust(left=margin, right=1. - margin)
+        if default_xtick_size < xtick_size:
+            plt.gcf().set_size_inches(xtick_size, plt.gcf().get_size_inches()[1])
+        ax.spines['top'].set_visible(False)
+        ax.spines['right'].set_visible(False)
+        plt.margins(0.1)
+        plt.subplots_adjust(bottom=0.15)
+        figure_to_save = plt.gcf()
+        plt.show()
+
+        if saving_plot_path is not None:
+            try:
+                figure_to_save.savefig(saving_plot_path + par +' evolution.png', bbox_inches='tight')
+            except FileNotFoundError:
+                print("The address '{0}' is not valid.".format(saving_plot_path))
+        plt.close()
+        
+
+################################################################################################
+###############################  perform temporal tests ########################################
+################################################################################################
+
+def temporal_test(data, spatial_id = None, test_type='ADF',# autoreg,ACF
+              lags = 1, column_identifier = None, saving_plot_path = './'):
+
+    ######################### check validity of input arguments
+    if isinstance(data,str):
+        try:
+            data = pd.read_csv(data)
+        except FileNotFoundError:
+            raise FileNotFoundError("File '{0}' does not exist.\n".format(data))
+
+    elif type(data) != pd.DataFrame:
+        raise TypeError("The input data must be of type DataFrame or string.")
+
+    df = rename_columns(data = data, column_identifier = column_identifier, error = 0)
+    check_validity(df.copy(), input_name = 'data', data_type = 'temporal', column_identifier = column_identifier, error = 0)
+
+    if type(spatial_id) == list:
+      if test_type == 'ACF' and len(spatial_id)>1:
+            raise ValueError("ACF can be plotted for only one spatial_id.")
+    elif spatial_id is not None:
+      raise TypeError("The spatial_id must be of type list.")
+
+    if  (spatial_id is None) and (test_type == 'ACF'):
+      raise ValueError("ACF can be plotted for only one spatial_id. Please specify it.")
+
+
+    ################## select desired temporal interval for plot from data ###############
+
+    # if temporal id format is integrated
+    if 'temporal id' in df.columns:
+        temporal_identifier_column_name = 'temporal id'
+
+        # determining input data temporal scale and transforming temporal id's to timestamp
+        df , scale = check_integrated_temporal_id(df)
+
+    # if temporal id format is non_integrated
+    else:
+
+        ##### next 8 lines add dummy temporal id for non_integrated temporal id format
+        list_to_find_smallest_scale = df.columns
+        # determine smallest temporal id level
+        for level in range(1,200):
+            if 'temporal id level '+str(level) in list_to_find_smallest_scale:
+                smallest_temporal_level = level
+                break
+        add_dummy_integrated_temporal_id(df, start_level = level)
+        temporal_identifier_column_name = 'dummy temporal id'
+
+
+    ############ select desired spatial id #########
+
+    # select random spatial ids if spatial id input is not specified
+    if spatial_id is None:
+        spatial_id = list(df['spatial id level 1'].unique())
+
+    df_dict = {}
+
+    for j in range(int(len(spatial_id))):
+        df0=df['spatial id level 1'] == spatial_id[j]
+        df1 = df[df0]
+        df1 = df1.sort_values(by=[temporal_identifier_column_name])
+        dict_key = spatial_id[j]
+        df_dict[dict_key] = df1
+
+    ############ Test the temporal correlation ################
+
+    result = {}
+
+    if test_type == 'autoreg':
+      for SpatialId, DF in df_dict.items():
+        y = DF['target'].tolist()
+        # fit the autoregression
+        model = AutoReg(y, lags=lags)
+        model_fit = model.fit()
+        result[SpatialId] = {"Coef "+str(key):value for key,value in enumerate(model_fit.params)}
+        result[SpatialId]['Intercept'] = result[SpatialId]['Coef 0']
+        del result[SpatialId]['Coef 0']
+        result[SpatialId]['AIC'] = model_fit.aic
+        result[SpatialId]['BIC'] = model_fit.bic
+        result[SpatialId]['HQIC'] = model_fit.hqic
+      return(result)
+
+    if test_type == 'ADF':
+      for SpatialId, DF in df_dict.items():
+        y = DF['target'].tolist()
+        test = adfuller(y)
+        result[SpatialId] = {}
+        result[SpatialId]['ADF Statistic'] = test[0]
+        result[SpatialId]['p-value'] = test[1]
+        for key, value in test[4].items():
+          result[SpatialId]["Critical Value "+str(key)]=value
+
+      return(result)
+
+    if test_type == 'ACF':
+      for SpatialId, DF in df_dict.items(): # only one item
+        y = DF['target'].tolist()
+        fig, ax = plt.subplots()
+        ax = sm.graphics.tsa.plot_acf(y, lags=lags, ax=ax)
+
+        if saving_plot_path is not None:
+            try:
+                plt.savefig(saving_plot_path + 'Auto correlation.png', bbox_inches='tight')
+            except FileNotFoundError:
+                print("The address '{0}' is not valid.".format(saving_plot_path))
+        plt.show()
+        plt.close()
```

### Comparing `stpredict-0.0.8/src/stpredict/rank_covariates.py` & `stpredict-0.0.9/src/stpredict/rank_covariates.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/rank_features.py` & `stpredict-0.0.9/src/stpredict/rank_features.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/scaling.py` & `stpredict-0.0.9/src/stpredict/scaling.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/select_features.py` & `stpredict-0.0.9/src/stpredict/select_features.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/split_data.py` & `stpredict-0.0.9/src/stpredict/split_data.py`

 * *Files identical despite different names*

### Comparing `stpredict-0.0.8/src/stpredict/train_evaluate.py` & `stpredict-0.0.9/src/stpredict/train_evaluate.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,47 +4,47 @@
     warnings.simplefilter("ignore")
     import pandas as pd
     import numpy as np
     import sys
     import datetime
     import traceback
     from .models import KNN_REGRESSOR, KNN_CLASSIFIER, NN_REGRESSOR, NN_CLASSIFIER, GLM_REGRESSOR, GLM_CLASSIFIER, \
-        GBM_REGRESSOR, GBM_CLASSIFIER
+        GBM_REGRESSOR, GBM_CLASSIFIER, SGCRF_REGRESSOR, SGCRF_CLASSIFIER
 
 
 def complete_predicted_probabilities(predictions, all_labels, present_labels):
-    
+
     present_probabilities = predictions
     all_probabilities = np.zeros([len(present_probabilities),len(all_labels)])
     ind = 0
     for label_number, label in enumerate(all_labels):
         if label in present_labels:
             all_probabilities[:,label_number] = present_probabilities[:,ind]
             ind += 1
 
         else:
             all_probabilities[:,label_number] = 0
-            
+
     return all_probabilities
 
 def run_model(X_training, X_validation, Y_training, model, model_type, supported_models_name, model_parameters=None,\
-              labels=None, verbose=0):
-    
+              labels=None, data_ids=None, verbose=0):
+
     # Labels presented in input training data
     present_labels = list(np.unique(Y_training))
     present_labels.sort()
-    
+
     # reading user defined models from dump file 'user_defined_models.py', where they have already been saved in train_validate function
     if (type(model) == str)  and (model not in supported_models_name and model not in ['mixed_' + name for name in supported_models_name]):
         try:
             from . import user_defined_models
             model = getattr(user_defined_models, model)
         except Exception:
             raise ValueError(
-            "The model must be name of one of the supported models: {'gbm', 'glm', 'knn', 'nn'} Or user defined function.")
+            "The model must be name of one of the supported models: {'gbm', 'glm', 'knn', 'nn', 'sgcrf'} or user defined function.")
 
     if type(model) == str:
         try:
             if model == 'gbm' or model == 'mixed_gbm':
 
                 if model_type == 'classification':
                     validation_predictions, train_predictions, trained_model = GBM_CLASSIFIER(X_training, X_validation,
@@ -80,84 +80,97 @@
                     validation_predictions, train_predictions, trained_model = NN_CLASSIFIER(X_training, X_validation,
                                                                                               Y_training, model_parameters,
                                                                                               verbose)
                 if model_type == 'regression':
                     validation_predictions, train_predictions, trained_model = NN_REGRESSOR(X_training, X_validation,
                                                                                             Y_training, model_parameters,
                                                                                             verbose)
+
+            elif model == 'sgcrf' or model == 'mixed_sgcrf':
+
+                if model_type == 'classification':
+                    validation_predictions, train_predictions, trained_model = SGCRF_CLASSIFIER(X_training, X_validation,
+                                                                                              Y_training, model_parameters,
+                                                                                              data_ids, verbose)
+                if model_type == 'regression':
+                    validation_predictions, train_predictions, trained_model = SGCRF_REGRESSOR(X_training, X_validation,
+                                                                                             Y_training, model_parameters,
+                                                                                             data_ids, verbose)
         except Exception as ex:
             raise Exception("{0} model\n\t   {1}\n\n{2}".format(model.upper(),str(ex),traceback.format_exc()))
-            
+
         if model_type == 'classification':
             if (model == 'nn') and (not np.allclose(1, train_predictions.sum(axis=1))) or (not np.allclose(1, validation_predictions.sum(axis=1))):
                  raise Exception(
                      "The output predictions of the neural network model need to be probabilities "
                      "i.e. they should sum up to 1.0 over classes. But the output does not match the condition. "
                      "Revise the model parameters to solve the problem.")
-        
+
     elif callable(model):
         try:
             train_predictions, validation_predictions, trained_model = model(X_training, X_validation, Y_training)
         except Exception as ex:
             raise Exception("The user-defined model '{0}' encountered an error:\n\t   {1}\n\n{2}".format(model.__name__,str(ex),traceback.format_exc()))
-        
+
         if (type(train_predictions) not in (np.ndarray,list)) or (type(validation_predictions) not in (np.ndarray,list)):
             raise Exception("The output predictions of the user-defined model must be of type array.")
-        
+
         train_predictions = np.array(train_predictions)
         validation_predictions = np.array(validation_predictions)
-        
+
         if (len(train_predictions) != len(X_training)) or (len(validation_predictions) != len(X_validation)):
             raise Exception("The output of the user-defined model has a different length from the input data.")
-        
+
         if model_type == 'classification':
             try:
                 train_predictions.shape[1]
                 validation_predictions.shape[1]
             except IndexError:
                 raise Exception("The output of the user_defined classification model must be an array of shape (n_samples,n_classes).")
-                                    
+
             if ((train_predictions.shape[1] != len(present_labels)) or (validation_predictions.shape[1] != len(present_labels))):
                 raise Exception("The probability predictions of the user-defined model are not compatible with the number of classes in the input data.")
-            
+
             if (not np.allclose(1, train_predictions.sum(axis=1))) or (not np.allclose(1, validation_predictions.sum(axis=1))):
                  raise Exception(
                      "The output predictions of the user-defined model need to be probabilities "
                      "i.e. they should sum up to 1.0 over classes")
 
     else:
         raise ValueError(
-            "The model must be name of one of the supported models: {'gbm', 'glm', 'knn', 'nn'} Or user defined function.")
-    
-    # adding the zero probability for the labels which are not included in the train data and thus are 
+            "The model must be name of one of the supported models: {'gbm', 'glm', 'knn', 'nn', 'sgcrf'} or user defined function.")
+
+    # adding the zero probability for the labels which are not included in the train data and thus are
     # not considered in the predictions
     if (model_type == 'classification') and (labels is not None):
-        
+
         train_predictions = complete_predicted_probabilities(predictions = train_predictions,
                                                              all_labels = labels, present_labels = present_labels)
         validation_predictions = complete_predicted_probabilities(predictions = validation_predictions,
                                                                   all_labels = labels, present_labels = present_labels)
-        
+
     return train_predictions, validation_predictions, trained_model
 
 
 def train_evaluate(training_data, validation_data, model, model_type, model_parameters = None,
                    labels = None, base_models = None, verbose = 0):
-    
-    
+
+
     # initializing
     train_predictions = None
     validation_predictions = None
     trained_model = None
+    data_ids = None
     base_model_list = []
     base_model_name_list = []
     base_model_parameter_list = []
-    supported_models_name = ['gbm', 'glm', 'knn', 'nn']
-    
-    
+    supported_models_name = ['gbm', 'glm', 'knn', 'nn', 'sgcrf']
+
+
+
     if type(training_data) == str:
         try:
             training_data = pd.read_csv(training_data)
         except FileNotFoundError:
             raise FileNotFoundError("File '{0}' does not exist.".format(training_data))
     elif type(training_data) != pd.DataFrame:
       raise TypeError("The training_data input must be a data frame or data address.")
@@ -166,14 +179,22 @@
         try:
             validation_data = pd.read_csv(validation_data)
         except FileNotFoundError:
             raise FileNotFoundError("File '{0}' does not exist.".format(validation_data))
     elif type(validation_data) != pd.DataFrame:
       raise TypeError("The validation_data input must be a data frame or data address.")
 
+
+    # Save the spatial and temporal ids
+    if 'spatial id' in training_data.columns.values and 'temporal id' in training_data.columns.values and \
+       'spatial id' in validation_data.columns.values and 'temporal id' in validation_data.columns.values:
+        data_ids = {}
+        data_ids['training'] = training_data[['spatial id', 'temporal id']]
+        data_ids['validation'] = validation_data[['spatial id', 'temporal id']]
+
     # split features and target
     if 'spatial id' in training_data.columns.values or 'temporal id' in training_data.columns.values:
         X_training = training_data.drop(['Target', 'spatial id', 'temporal id'], axis=1)
     else:
         X_training = training_data.drop(['Target'], axis=1)
     Y_training = np.array(training_data['Target']).reshape(-1)
     if 'spatial id' in validation_data.columns.values or 'temporal id' in validation_data.columns.values:
@@ -182,30 +203,34 @@
         X_validation = validation_data.drop(['Target'], axis=1)
     Y_validation = np.array(validation_data['Target']).reshape(-1)
 
     if 'Normal target' in X_training.columns:
         X_training = X_training.drop(['Normal target'], axis=1)
         X_validation = X_validation.drop(['Normal target'], axis=1)
         
+    # check labels
+    if labels is not None:
+    	labels = sorted(labels)
+
     # check base model input
     if base_models is not None:
         if type(base_models) not in (np.ndarray, list):
             raise TypeError('The base_models must be of type list.')
-            
+
         for item_number, item in enumerate(base_models):
 
             # if the item is the dictionary of model name and its parameters
-            if type(item) == dict:       
+            if type(item) == dict:
                 base_model = list(item.keys())[0]
 
                 # if the dictionary contain only one of the supported models
                 if (len(item) == 1) and (base_model in supported_models_name):
 
                     base_model_list.append(base_model)
-                    # if model is not duplicate 
+                    # if model is not duplicate
                     if base_model not in base_model_name_list:
                         base_model_name_list.append(base_model)
                     else:
                         base_model_name_list.append(base_model + str(item_number))
 
                     # if the value of the model name is dictionary of models parameter list
                     if type(item[base_model]) == dict:
@@ -227,90 +252,105 @@
                         base_model_name_list.append(item + str(item_number))
                 else:
                     print("\nWarning: The string items in the base_models list must be one of the supported model names. The incompatible cases will be ignored.\n")
 
             # if the item is user defined function
             elif callable(item):
                 if item.__name__ in supported_models_name:
-                    raise Exception("User-defined model names must be different from predefined models:['knn', 'glm', 'gbm', 'nn']")
+                    raise Exception("User-defined model name must be different from predefined models:['knn', 'glm', 'gbm', 'nn', 'sgcrf']")
                 base_model_list.append(item)
                 base_model_name_list.append(item.__name__)
                 base_model_parameter_list.append(None)
 
             else:
                 print("\nWarning: The items in the base_models list must be of type string, dict or callable. The incompatible cases will be ignored.\n")
 
         if len(base_model_list) < 1:
             raise ValueError("There is no item in the base_models list or the items are invalid.")
-        
+
+
+    # Check the spatial and temporal ids for SGCRF model
+    if (model in ['sgcrf','mixed_sgcrf'] or 'sgcrf' in base_model_list):
+        if ('spatial id' not in training_data.columns.values or 'temporal id' not in training_data.columns.values):
+            raise ValueError("To use the SGCRF model, the 'spatial id' and 'temporal id' columns must be included in training_data and \
+                          validation_data.\n")
+        if model_type == 'classification' and len(np.unique(Y_training)) > 2:
+            raise ValueError("The SGCRF classifier can only be used for binary classification.\n")
+
+
     # if model is non-mixed
     if base_models is None:
         train_predictions, validation_predictions, trained_model = run_model(X_training, X_validation, Y_training, model, model_type,\
-                                                                                supported_models_name,model_parameters, labels, verbose)
+                                                                                supported_models_name,model_parameters, labels, data_ids,\
+                                                                                verbose)
     # if model is mixed
     else:
         mixed_X_training = pd.DataFrame()
         mixed_X_validation = pd.DataFrame()
 
         for base_model_number, base_model_name in enumerate(base_model_name_list):
             train_predictions, validation_predictions, trained_model = run_model(X_training.copy(), X_validation.copy(), Y_training.copy(),\
                                                                                  base_model_list[base_model_number], model_type,\
                                                                                   supported_models_name, base_model_parameter_list[base_model_number],\
-                                                                                 labels, verbose)
+                                                                                 labels, data_ids, verbose)
             if model_type == 'classification':
 #                 train_predictions = [labels[index] for index in np.argmax(train_predictions, axis=1)]
 #                 validation_predictions = [labels[index] for index in np.argmax(validation_predictions, axis=1)]
 
                 total_class_number = 1 if train_predictions.shape[1] == 2 else train_predictions.shape[1]
                 for class_num in range(total_class_number):
                     mixed_X_training[base_model_name+str(class_num)] = list(train_predictions[:,class_num])
                     mixed_X_validation[base_model_name+str(class_num)] = list(validation_predictions[:,class_num])
             else:
                 mixed_X_training[base_model_name] = list(train_predictions)
                 mixed_X_validation[base_model_name] = list(validation_predictions)
 
         train_predictions, validation_predictions, trained_model = run_model(mixed_X_training, mixed_X_validation, Y_training, model, model_type,\
-                                                                             supported_models_name, model_parameters, labels, verbose)
-    
+                                                                             supported_models_name, model_parameters, labels, data_ids, verbose)
+
     return train_predictions, validation_predictions, trained_model
 
 
 #####################################################################################################
 
 def inner_train_evaluate(training_data, validation_data, model, model_type, model_parameters = None, labels = None, base_models=None, verbose = 0):
-    
+
     train_predictions, validation_predictions, trained_model = train_evaluate(training_data = training_data,
                                                                               validation_data = validation_data,
-                                                                              model = model, 
+                                                                              model = model,
                                                                               model_type = model_type,
-                                                                              model_parameters = model_parameters, 
+                                                                              model_parameters = model_parameters,
                                                                               labels = labels,
                                                                               base_models = base_models,
                                                                               verbose = verbose)
-    
+
     if model == 'gbm' or model == 'mixed_gbm':
         # get the number of trees
         number_of_parameters = None # trained_model.n_estimators_
-        
+
     elif model == 'glm' or model == 'mixed_glm':
         # get the number of coefficients and intercept
         if model_type == 'classification':
             number_of_parameters = trained_model.coef_.shape[0]*trained_model.coef_.shape[1]
             if not all(trained_model.intercept_ == 0):
                 number_of_parameters += trained_model.intercept_.shape[0]
         if model_type == 'regression':
             number_of_parameters = None # trained_model.coef_.shape[0]
             # if trained_model.get_params()['fit_intercept']:
                 # number_of_parameters += 1
-                
+
     elif model == 'knn' or model == 'mixed_knn':
         # get the number of nearest neighbours
         number_of_parameters = None # trained_model.get_params()['n_neighbors']
-        
+
     elif model == 'nn' or model == 'mixed_nn':
         # get the number of parameters
         number_of_parameters = None # trained_model.count_params()
         
+    elif model == 'sgcrf' or model == 'mixed_sgcrf':
+        # get the number of parameters
+        number_of_parameters = None # trained_model.count_params()
+
     else:
         number_of_parameters = None
-        
+
     return train_predictions, validation_predictions, trained_model, number_of_parameters
```

### Comparing `stpredict-0.0.8/src/stpredict/train_test.py` & `stpredict-0.0.9/src/stpredict/train_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         history_length:    int
             history length of the input "data", history length is just used for the reports in "train_test"
 
         model:    string or callable or dict
             string: one of the pre-defined model names 
             function: a user-defined function
             dict: pre-defined model names and corresponding hyper parameters
-            pre-defined model names: 'knn', 'nn' , 'gbm', 'glm'
+            pre-defined model names: 'knn', 'nn' , 'gbm', 'glm', 'sgcrf'
 
         model_type:    string
 
         model_parameters:    list<int> or None
 
         feature_scaler:    string
 
@@ -190,26 +190,26 @@
     if all(temp_data.tail(granularity*forecast_horizon*number_of_spatial_units)['Target'].isna()):
         data = temp_data.iloc[:-(granularity*forecast_horizon*number_of_spatial_units)]
     
     # check if model is a string or function
     model_name = ''
     if isinstance(model, str) == False:
         model_name = model.__name__
-        if model_name in ['nn', 'knn', 'glm', 'gbm']:
+        if model_name in ['nn', 'knn', 'glm', 'gbm', 'sgcrf']:
             raise TypeError("Name of the user defined model matches the name of one of our predefined models.")
     else:
         model_name = model
 
     # find labels for classification problem
     if labels == None:
         if model_type == 'regression':    # just an empty list
             labels = []
         elif model_type == 'classification':    # unique values in 'Target' column of data
             labels = data.Target.unique()
-            labels.sort()
+    labels.sort()
 
     # select features
     processed_data = select_features(
         data=data.copy(), 
         ordered_covariates_or_features=feature_or_covariate_set
     )
 
@@ -280,15 +280,15 @@
     
     
     # getting back previous points (useful for one-by-one method, also works for one-as-whole method)
     previous_test_points = pd.read_csv(test_process_backup_file_name)
     
     # append current point to previous points
     test_target.insert(2, 'model name', model_name, True)
-    test_target = test_target.append(previous_test_points[['spatial id', 'temporal id', 'model name', 'Target', 'Normal target']], ignore_index=True)
+    test_target = pd.concat([test_target, previous_test_points[['spatial id', 'temporal id', 'model name', 'Target', 'Normal target']]], ignore_index=True)
     if model_type == 'regression':
         previous_testing_predictions = previous_test_points['prediction'].tolist()
         testing_predictions = list(testing_predictions) + previous_testing_predictions
     elif model_type == 'classification':
         previous_testing_predictions = previous_test_points.filter(regex='^prediction class ',axis=1)
         testing_predictions = np.concatenate((np.array(testing_predictions),np.array(previous_testing_predictions)))
         testing_predictions_df = pd.DataFrame(testing_predictions)
@@ -302,15 +302,15 @@
         df_for_backup = pd.concat([df_for_backup,testing_predictions_df],axis = 1)
     df_for_backup.to_csv(test_process_backup_file_name, index=False)
     
     test_target = test_target.drop(['model name'], axis = 1)
 
     # get normal data
     training_target, test_target, training_prediction, test_prediction = get_normal_target(
-        training_target=training_target.append(gap_data[['spatial id', 'temporal id', 'Target', 'Normal target']], ignore_index=True), 
+        training_target=pd.concat([training_target,gap_data[['spatial id', 'temporal id', 'Target', 'Normal target']]], ignore_index=True), 
         test_target=test_target.copy(), 
         training_prediction=list(training_predictions) + gap_data['Target'].tolist(), 
         test_prediction=testing_predictions, 
         target_mode=target_mode, 
         target_granularity=target_granularity
     )
```

### Comparing `stpredict-0.0.8/src/stpredict/train_validate.py` & `stpredict-0.0.9/src/stpredict/train_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import pandas as pd
     import numpy as np
     import sys
     import shutil
     import datetime
-    from .models import KNN_REGRESSOR,KNN_CLASSIFIER,NN_REGRESSOR,NN_CLASSIFIER,GLM_REGRESSOR,GLM_CLASSIFIER,GBM_REGRESSOR,GBM_CLASSIFIER
+    from .models import KNN_REGRESSOR,KNN_CLASSIFIER,NN_REGRESSOR,NN_CLASSIFIER,GLM_REGRESSOR,GLM_CLASSIFIER,GBM_REGRESSOR,GBM_CLASSIFIER,SGCRF_REGRESSOR
     from sklearn.model_selection import ParameterGrid
     from sklearn.model_selection import KFold
     from multiprocessing import Pool
     from functools import partial
     from tqdm import tqdm
     import random
     import os
@@ -181,14 +181,29 @@
 
         
         for key in user_params.keys():
             if type(user_params[key]) not in [np.ndarray,list]:
                 user_params[key] = list([user_params[key]])
 
         parameter_list = list(ParameterGrid(user_params))
+    
+    if model_name == 'sgcrf':
+
+        for parameter in ['learning_rate', 'n_iter', 'lamL', 'lamT']:
+            if parameter in user_params.keys():
+                if type(user_params[parameter]) in (np.ndarray,list):
+                    grid_flag = True
+        
+        for key in user_params.keys():
+            if type(user_params[key]) not in [np.ndarray,list]:
+                user_params[key] = list([user_params[key]])
+                
+        user_params['neighbouring_matrix'] = list([user_params['neighbouring_matrix']])
+        
+        parameter_list = list(ParameterGrid(user_params))
         
         
     return parameter_list
 
 # reporting the performance of models in csv file
 def report_performance(errors_dict, max_history, ordered_covariates_or_features,
                        feature_sets_indices, performance_measures, feature_selection_type,
@@ -221,15 +236,15 @@
             for measure in performance_measures:
                 errors_list = []
                 for feature_set_number in range(len(feature_sets_indices[history-1])):
                     model_best_parameters_number = models_best_parameters_number[model_name][(history, feature_set_number)]
                     errors_list.append(errors_dict[measure][model_name][(history, feature_set_number, model_best_parameters_number)])
                 temp.loc[:,(measure)] = list(errors_list)
             
-            output_data_frame = output_data_frame.append(temp)
+            output_data_frame = pd.concat([output_data_frame,temp], ignore_index=True)
     
     address = './performance/validation process/'
     if os.path.exists(address):
         files = [f for f in os.listdir(address) if ((os.path.isfile(os.path.join(address, f))) and (report_type in f))]
         
         if len(files) == 0:
             output_data_frame.to_csv('{0}{1} performance report forecast horizon = {2}.csv'.format(address, report_type, forecast_horizon), index = False)
@@ -308,15 +323,15 @@
         temp = temp.drop(['Target'], axis = 1)
         temp.rename(columns = {'Normal target':'real'}, inplace = True)
         if model_type == 'regression':
             temp = temp[['model name', 'spatial id', 'temporal id', 'real', 'prediction']]
         elif model_type == 'classification':
             temp = temp[['model name', 'spatial id', 'temporal id', 'real'] + ['class '+str(item) for item in labels]]
 
-        prediction_data_frame = prediction_data_frame.append(temp)
+        prediction_data_frame = pd.concat([prediction_data_frame,temp],ignore_index=True)
     
     # prediction_data_frame = prediction_data_frame.rename(columns = {'temporal id':'predictive time point'})
     address = './prediction/validation process/'
     
     if os.path.exists(address):
         files = [f for f in os.listdir(address) if ((os.path.isfile(os.path.join(address, f))) and (prediction_type in f))]
         if len(files) == 0:
@@ -376,15 +391,15 @@
                    fold_total_number = 5, instance_random_partitioning = False,
                    forecast_horizon = 1, models = ['knn'], mixed_models = None,  model_type = 'regression',
                    splitting_type = 'training-validation',
                    performance_measures = None, performance_benchmark = None, performance_mode = 'normal', 
                    feature_scaler = None, target_scaler = None, labels = None, performance_report = True,
                    save_predictions = True, save_ranked_features = True, verbose = 0):
     
-    supported_models_name = ['nn', 'knn', 'glm', 'gbm']
+    supported_models_name = ['nn', 'knn', 'glm', 'gbm', 'sgcrf']
     supported_performance_measures = ['MAE', 'MAPE', 'MASE', 'MSE', 'R2_score', 'AIC', 'BIC', 'likelihood', 'AUC', 'AUPR']
     models_list = [] # list of models (str or callable)
     models_parameter_list = [] # list of models' parameters (dict or None)
     models_name_list = [] # list of models' names (str)
     base_models_name_list = [] # list of base models' names (str)
     mixed_models_name_list = [] # list of base models' names (str)
     same_train_validation_sets = False # Flag to specify whether or not both training and validation must be performed based on same set
@@ -487,15 +502,15 @@
             else:
                 models.remove(item)
                 print("\nWarning: The string items in the models list must be one of the supported model names. The incompatible cases will be ignored.\n")
         
         # if the item is user defined function
         elif callable(item):
             if item.__name__ in supported_models_name:
-                raise Exception("User-defined model names must be different from predefined models:['knn', 'glm', 'gbm', 'nn']")
+                raise Exception("User-defined model names must be different from predefined models:['knn', 'glm', 'gbm', 'nn', 'sgcrf']")
             if item.__name__ in models_name_list:
                 raise Exception("User-defined models can not have the same names.")
             models_list.append(item)
             models_name_list.append(item.__name__)
             base_models_name_list.append(item.__name__)
             models_parameter_list.append([None])
             number_of_user_defined_models += 1
@@ -564,15 +579,15 @@
             else:
                 mixed_models.remove(item)
                 print("\nWarning: The string items in the mixed_models list must be one of the supported model names. The incompatible cases will be ignored.\n")
         
         # if the item is user defined function
         elif callable(item):
             if item.__name__ in supported_models_name:
-                raise Exception("User-defined model names must be different from predefined models:['knn', 'glm', 'gbm', 'nn']")
+                raise Exception("User-defined model names must be different from predefined models:['knn', 'glm', 'gbm', 'nn', 'sgcrf']")
             if item.__name__ in models_name_list:
                 raise Exception("User-defined models can not have the same names.")
             models_list.append(item)
             models_name_list.append(item.__name__)
             mixed_models_name_list.append(item.__name__)
             models_parameter_list.append([None])
             number_of_user_defined_models += 1
@@ -634,21 +649,22 @@
         raise ValueError("No valid measure is specified.")
         
     ############## performance_benchmark input
     
     if (performance_benchmark not in supported_performance_measures) or (performance_benchmark is None):
         if model_type == 'regression':
             if zero_encounter_flag == 0:
-                performance_benchmark = 'MAPE'
+                alternative_performance_benchmark = 'MAPE'
             else:
-                performance_benchmark = 'MAE'
+                alternative_performance_benchmark = 'MAE'
         else:
-            performance_benchmark = 'AUC'
+            alternative_performance_benchmark = 'AUC'
         if performance_benchmark is not None:
-            print("\nWarning: The specified performance_benchmark must be one of the supported performance measures: ['MAE', 'MAPE', 'MASE', 'MSE', 'R2_score', 'AIC', 'BIC', 'likelihood', 'AUC', 'AUPR']\nThe incompatible cases will be ignored and replaced with '{0}'.\n".format(performance_benchmark))
+            print("\nWarning: The specified performance_benchmark must be one of the supported performance measures: ['MAE', 'MAPE', 'MASE', 'MSE', 'R2_score', 'AIC', 'BIC', 'likelihood', 'AUC', 'AUPR']\nThe incompatible cases will be ignored and replaced with '{0}'.\n".format(alternative_performance_benchmark))
+        performance_benchmark = alternative_performance_benchmark
             
     if (performance_benchmark in ['likelihood', 'AUC', 'AUPR', 'AIC', 'BIC']) and (model_type == 'regression'): 
         if zero_encounter_flag == 0:
             performance_benchmark = 'MAPE'
         else:
             performance_benchmark = 'MAE'
         print("\nWarning: The specified performance_benchmark can not be measured for regression models. Thus the performance_benchmark will be set to '{0}'.\n".format(performance_benchmark))
@@ -691,19 +707,19 @@
 
     
     ############## model_type input and labels
     
     if model_type == 'classification':
         if labels is None:
             labels = list(data_list[0]['Normal target'].unique())
-            labels.sort()
         elif type(labels) != list:
             raise TypeError("The labels input must be of type list.")
         elif any([len(set(data['Normal target'].dropna().unique())-set(labels))>0 for data in data_list]):
             raise ValueError("Some of the class labels in the input data are not in labels input.")
+        labels.sort()
         
         if performance_mode != 'normal':
             if performance_mode is not None:
                 print("\nWarning: The 'cumulative' or 'moving average' performance_mode can not be used for the classification.")
             performance_mode = 'normal'
         if target_scaler is not None:
             target_scaler = None
@@ -713,14 +729,15 @@
             
     elif model_type == 'regression':
         labels = []
     else:
         raise ValueError("The specified model_type is not valid. The supported values are 'regression' and 'classification'.")
     
     
+    
     ############## feature_sets, forced_covariates
     
     if (type(feature_sets) != dict) or (len(feature_sets) > 1):
         raise TypeError("The feature_sets input must be of type dictionary with only one item.")
         
     feature_selection_type = list(feature_sets.keys())[0]
     ranking_method = list(feature_sets.values())[0]
```

### Comparing `stpredict-0.0.8/src/stpredict/whole_as_one.py` & `stpredict-0.0.9/src/stpredict/whole_as_one.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,14 +249,15 @@
             print("Warning: The input 'performance_mode' is set to 'normal' according to model_type=classification'.")
         if target_scaler is not None:
             target_scaler = None
             print("Warning: The input 'target_scaler' is set to None according to model_type=classification'.")
         target_column_name = list(filter(lambda x: x.startswith('Target'), data[0].columns.values))[0]
         labels = data[0].loc[:, target_column_name].unique().tolist()
         labels = [label for label in labels if not (label is None or str(label) == 'nan')]
+        labels = sorted(labels)
         if len(labels) < 2:
             raise Exception("Error: The labels length must be at least two.")
     else:
         if not set(performance_measures) <= set(REGRESSION_PERFORMANCE_MEASURES):
             raise Exception("Error: The input 'performance_measures' is not valid according to 'model_type=regression'.")
     if performance_benchmark not in performance_measures:
         performance_measures.append(performance_benchmark)
```

### Comparing `stpredict-0.0.8/src/stpredict.egg-info/PKG-INFO` & `stpredict-0.0.9/src/stpredict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: stpredict
-Version: 0.0.8
+Version: 0.0.9
 Summary: Spatio-temporal prediction package
 Home-page: https://github.com/network-and-Data-Science-IUT/stpredict
 Author: Arash Mari Oriyad, Maryam Meghdadi, Mahdi Naderi, Arezoo Haratian
 Author-email: arashmarioriyad@gmail.com, arezo.h1371@yahoo.com
 Maintainer: cndalab
 Maintainer-email: cndalab.iut@gmail.com, pramazi@brocku.ca, arashmarioriyad@gmail.com, arezo.h1371@yahoo.com
 Project-URL: Documentation, https://stpredict.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas<=1.1.5
+Requires-Dist: scikit-learn>=0.24
+Requires-Dist: scikeras>=0.13.0
 
 
 STPredict package
 =================
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stpredict?logo=python)
 ![Read the Docs](https://img.shields.io/readthedocs/stpredict?logo=readthedocs)
```

### Comparing `stpredict-0.0.8/src/stpredict.egg-info/SOURCES.txt` & `stpredict-0.0.9/src/stpredict.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 src/stpredict/__init__.py
 src/stpredict/apply_performance_mode.py
 src/stpredict/configurations.py
 src/stpredict/get_future_data.py
+src/stpredict/get_map.py
 src/stpredict/get_normal_target.py
 src/stpredict/get_target_quantities.py
 src/stpredict/get_target_temporal_ids.py
 src/stpredict/get_trivial_values.py
 src/stpredict/models.py
 src/stpredict/one_by_one.py
 src/stpredict/performance.py
@@ -20,19 +21,22 @@
 src/stpredict/predict_func.py
 src/stpredict/predict_future.py
 src/stpredict/preprocess.py
 src/stpredict/rank_covariates.py
 src/stpredict/rank_features.py
 src/stpredict/scaling.py
 src/stpredict/select_features.py
+src/stpredict/sgcrf.py
 src/stpredict/split_data.py
 src/stpredict/train_evaluate.py
 src/stpredict/train_test.py
 src/stpredict/train_validate.py
 src/stpredict/whole_as_one.py
 src/stpredict.egg-info/PKG-INFO
 src/stpredict.egg-info/SOURCES.txt
 src/stpredict.egg-info/dependency_links.txt
 src/stpredict.egg-info/requires.txt
 src/stpredict.egg-info/top_level.txt
 src/stpredict/data/USA_COVID_19_data.csv
-src/stpredict/data/earthquake_data.csv
+src/stpredict/data/earthquake_data.csv
+tests/test_predict.py
+tests/test_preprocess.py
```

