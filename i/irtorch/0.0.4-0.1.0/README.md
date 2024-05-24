# Comparing `tmp/irtorch-0.0.4.tar.gz` & `tmp/irtorch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irtorch-0.0.4.tar", last modified: Thu Apr 18 13:28:33 2024, max compression
+gzip compressed data, was "irtorch-0.1.0.tar", last modified: Fri May 24 18:19:23 2024, max compression
```

## Comparing `irtorch-0.0.4.tar` & `irtorch-0.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:33.010614 irtorch-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-02-08 14:34:51.000000 irtorch-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2158 2024-04-18 13:28:33.009615 irtorch-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1812 2024-04-18 13:25:52.000000 irtorch-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.970152 irtorch-0.0.4/irtorch/
--rw-rw-rw-   0        0        0      255 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/__init__.py
--rw-rw-rw-   0        0        0    14040 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/_internal_utils.py
--rw-rw-rw-   0        0        0     3279 2024-02-25 18:33:40.000000 irtorch-0.0.4/irtorch/activation_functions.py
--rw-rw-rw-   0        0        0     1000 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/config.py
--rw-rw-rw-   0        0        0     5326 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/cross_validation.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.958153 irtorch-0.0.4/irtorch/datasets/
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.983152 irtorch-0.0.4/irtorch/datasets/big_five/
--rw-rw-rw-   0        0        0  3944929 2024-02-27 14:06:14.000000 irtorch-0.0.4/irtorch/datasets/big_five/big_five.pt
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.987156 irtorch-0.0.4/irtorch/datasets/national_mathematics/
--rw-rw-rw-   0        0        0   114121 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/datasets/national_mathematics/mathematics_1.pt
--rw-rw-rw-   0        0        0   158089 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/datasets/national_mathematics/mathematics_2.pt
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.991155 irtorch-0.0.4/irtorch/datasets/swedish_sat/
--rw-rw-rw-   0        0        0  1601324 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt
--rw-rw-rw-   0        0        0  1601319 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt
--rw-rw-rw-   0        0        0       80 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_quant_correct.txt
--rw-rw-rw-   0        0        0       82 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_verb_correct.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.993156 irtorch-0.0.4/irtorch/estimation_algorithms/
--rw-rw-rw-   0        0        0      104 2024-02-08 14:34:51.000000 irtorch-0.0.4/irtorch/estimation_algorithms/__init__.py
--rw-rw-rw-   0        0        0    14839 2024-04-04 11:55:33.000000 irtorch-0.0.4/irtorch/estimation_algorithms/aeirt.py
--rw-rw-rw-   0        0        0     2893 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/estimation_algorithms/base_irt_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.996157 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/
--rw-rw-rw-   0        0        0      184 2024-02-08 14:34:51.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/__init__.py
--rw-rw-rw-   0        0        0      751 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/base_encoder.py
--rw-rw-rw-   0        0        0     1427 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/bounded_encoder.py
--rw-rw-rw-   0        0        0     1361 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/standard_encoder.py
--rw-rw-rw-   0        0        0     1478 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/estimation_algorithms/encoders/variational_encoder.py
--rw-rw-rw-   0        0        0    14716 2024-04-04 11:55:33.000000 irtorch-0.0.4/irtorch/estimation_algorithms/vaeirt.py
--rw-rw-rw-   0        0        0     4002 2024-04-04 11:55:33.000000 irtorch-0.0.4/irtorch/gaussian_mixture_model.py
--rw-rw-rw-   0        0        0    67843 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/irt.py
--rw-rw-rw-   0        0        0    34296 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/irt_evaluator.py
--rw-rw-rw-   0        0        0    55406 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/irt_plotter.py
--rw-rw-rw-   0        0        0    62880 2024-04-04 11:55:33.000000 irtorch-0.0.4/irtorch/irt_scorer.py
--rw-rw-rw-   0        0        0     2644 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/latent_variable_functions.py
--rw-rw-rw-   0        0        0     8310 2024-02-20 20:30:27.000000 irtorch-0.0.4/irtorch/layers.py
--rw-rw-rw-   0        0        0     5137 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/load_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:33.000615 irtorch-0.0.4/irtorch/models/
--rw-rw-rw-   0        0        0      308 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/__init__.py
--rw-rw-rw-   0        0        0     8219 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/base_irt_model.py
--rw-rw-rw-   0        0        0     6441 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/generalized_partial_credit.py
--rw-rw-rw-   0        0        0    13816 2024-04-03 14:22:41.000000 irtorch-0.0.4/irtorch/models/monotone_nn.py
--rw-rw-rw-   0        0        0     7627 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/nominal_response.py
--rw-rw-rw-   0        0        0     4895 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/one_parameter_logistic.py
--rw-rw-rw-   0        0        0     5240 2024-04-18 13:25:53.000000 irtorch-0.0.4/irtorch/models/two_parameter_logistic.py
--rw-rw-rw-   0        0        0     6868 2024-02-25 18:33:40.000000 irtorch-0.0.4/irtorch/outlier_detector.py
--rw-rw-rw-   0        0        0     3163 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/quantile_mv_normal.py
--rw-rw-rw-   0        0        0      767 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/timer.py
--rw-rw-rw-   0        0        0     6670 2024-03-08 13:28:02.000000 irtorch-0.0.4/irtorch/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:32.982153 irtorch-0.0.4/irtorch.egg-info/
--rw-rw-rw-   0        0        0     2158 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2151 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-08 14:36:17.000000 irtorch-0.0.4/irtorch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      107 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 13:28:32.000000 irtorch-0.0.4/irtorch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 13:28:33.010614 irtorch-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1099 2024-04-18 13:25:53.000000 irtorch-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 13:28:33.009615 irtorch-0.0.4/tests/
--rw-rw-rw-   0        0        0     1132 2024-02-20 20:30:27.000000 irtorch-0.0.4/tests/test_activation_functions.py
--rw-rw-rw-   0        0        0     4099 2024-03-08 13:28:02.000000 irtorch-0.0.4/tests/test_aeirt.py
--rw-rw-rw-   0        0        0      984 2024-02-21 12:30:49.000000 irtorch-0.0.4/tests/test_config.py
--rw-rw-rw-   0        0        0     2196 2024-04-04 11:55:33.000000 irtorch-0.0.4/tests/test_gaussian_mixture_torch.py
--rw-rw-rw-   0        0        0     9680 2024-04-18 13:25:53.000000 irtorch-0.0.4/tests/test_integration.py
--rw-rw-rw-   0        0        0     7678 2024-04-03 14:22:41.000000 irtorch-0.0.4/tests/test_internal_utils.py
--rw-rw-rw-   0        0        0    17038 2024-04-03 14:22:41.000000 irtorch-0.0.4/tests/test_irt_evaluator.py
--rw-rw-rw-   0        0        0     3632 2024-02-25 18:33:40.000000 irtorch-0.0.4/tests/test_irt_plotter.py
--rw-rw-rw-   0        0        0    14999 2024-04-04 11:55:33.000000 irtorch-0.0.4/tests/test_irt_scorer.py
--rw-rw-rw-   0        0        0     3310 2024-03-08 13:28:02.000000 irtorch-0.0.4/tests/test_latent_variable_functions.py
--rw-rw-rw-   0        0        0     5111 2024-02-08 14:34:51.000000 irtorch-0.0.4/tests/test_layers.py
--rw-rw-rw-   0        0        0     1799 2024-04-18 13:25:53.000000 irtorch-0.0.4/tests/test_load_dataset.py
--rw-rw-rw-   0        0        0     2850 2024-02-08 14:34:51.000000 irtorch-0.0.4/tests/test_outlier_detector.py
--rw-rw-rw-   0        0        0     3252 2024-02-08 14:34:51.000000 irtorch-0.0.4/tests/test_quantile_mv_normal.py
--rw-rw-rw-   0        0        0     4670 2024-03-08 13:28:02.000000 irtorch-0.0.4/tests/test_utils.py
--rw-rw-rw-   0        0        0     6369 2024-03-08 13:28:02.000000 irtorch-0.0.4/tests/test_vaeirt.py
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.796207 irtorch-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-02-08 14:34:51.000000 irtorch-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2158 2024-05-24 18:19:23.796207 irtorch-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1812 2024-04-18 13:25:52.000000 irtorch-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.750203 irtorch-0.1.0/irtorch/
+-rw-rw-rw-   0        0        0      233 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/__init__.py
+-rw-rw-rw-   0        0        0    12946 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/_internal_utils.py
+-rw-rw-rw-   0        0        0     3279 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/activation_functions.py
+-rw-rw-rw-   0        0        0    43017 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/bit_scales.py
+-rw-rw-rw-   0        0        0     1000 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/config.py
+-rw-rw-rw-   0        0        0     5431 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/cross_validation.py
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.736203 irtorch-0.1.0/irtorch/datasets/
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.767204 irtorch-0.1.0/irtorch/datasets/big_five/
+-rw-rw-rw-   0        0        0  3944929 2024-02-27 14:06:14.000000 irtorch-0.1.0/irtorch/datasets/big_five/big_five.pt
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.772203 irtorch-0.1.0/irtorch/datasets/national_mathematics/
+-rw-rw-rw-   0        0        0   114121 2024-03-08 13:28:02.000000 irtorch-0.1.0/irtorch/datasets/national_mathematics/mathematics_1.pt
+-rw-rw-rw-   0        0        0   158089 2024-03-08 13:28:02.000000 irtorch-0.1.0/irtorch/datasets/national_mathematics/mathematics_2.pt
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.776203 irtorch-0.1.0/irtorch/datasets/swedish_sat/
+-rw-rw-rw-   0        0        0  1601324 2024-04-18 13:25:53.000000 irtorch-0.1.0/irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt
+-rw-rw-rw-   0        0        0  1601319 2024-04-18 13:25:53.000000 irtorch-0.1.0/irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt
+-rw-rw-rw-   0        0        0       80 2024-04-03 14:22:41.000000 irtorch-0.1.0/irtorch/datasets/swedish_sat/swesat22b_quant_correct.txt
+-rw-rw-rw-   0        0        0       82 2024-04-03 14:22:41.000000 irtorch-0.1.0/irtorch/datasets/swedish_sat/swesat22b_verb_correct.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.779204 irtorch-0.1.0/irtorch/estimation_algorithms/
+-rw-rw-rw-   0        0        0      114 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/estimation_algorithms/__init__.py
+-rw-rw-rw-   0        0        0    14639 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/estimation_algorithms/ae.py
+-rw-rw-rw-   0        0        0     1757 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/estimation_algorithms/base_irt_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.782203 irtorch-0.1.0/irtorch/estimation_algorithms/encoders/
+-rw-rw-rw-   0        0        0      184 2024-02-08 14:34:51.000000 irtorch-0.1.0/irtorch/estimation_algorithms/encoders/__init__.py
+-rw-rw-rw-   0        0        0      751 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/estimation_algorithms/encoders/base_encoder.py
+-rw-rw-rw-   0        0        0     1427 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/estimation_algorithms/encoders/bounded_encoder.py
+-rw-rw-rw-   0        0        0     1361 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/estimation_algorithms/encoders/standard_encoder.py
+-rw-rw-rw-   0        0        0     1486 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/estimation_algorithms/encoders/variational_encoder.py
+-rw-rw-rw-   0        0        0    12600 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/estimation_algorithms/mml.py
+-rw-rw-rw-   0        0        0    16449 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/estimation_algorithms/vae.py
+-rw-rw-rw-   0        0        0    40029 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/evaluation.py
+-rw-rw-rw-   0        0        0     4002 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/gaussian_mixture_model.py
+-rw-rw-rw-   0        0        0     2644 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/latent_variable_functions.py
+-rw-rw-rw-   0        0        0     8346 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/layers.py
+-rw-rw-rw-   0        0        0     5137 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/load_dataset.py
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.786203 irtorch-0.1.0/irtorch/models/
+-rw-rw-rw-   0        0        0      308 2024-04-18 13:25:53.000000 irtorch-0.1.0/irtorch/models/__init__.py
+-rw-rw-rw-   0        0        0    34565 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/models/base_irt_model.py
+-rw-rw-rw-   0        0        0     8137 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/models/generalized_partial_credit.py
+-rw-rw-rw-   0        0        0    14674 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/models/monotone_nn.py
+-rw-rw-rw-   0        0        0     9226 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/models/nominal_response.py
+-rw-rw-rw-   0        0        0     5468 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/models/one_parameter_logistic.py
+-rw-rw-rw-   0        0        0     5818 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/models/two_parameter_logistic.py
+-rw-rw-rw-   0        0        0     6868 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/outlier_detector.py
+-rw-rw-rw-   0        0        0    58074 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/plotting.py
+-rw-rw-rw-   0        0        0     3163 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/quantile_mv_normal.py
+-rw-rw-rw-   0        0        0      767 2024-05-20 12:51:01.000000 irtorch-0.1.0/irtorch/timer.py
+-rw-rw-rw-   0        0        0     8958 2024-05-24 18:17:58.000000 irtorch-0.1.0/irtorch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.767204 irtorch-0.1.0/irtorch.egg-info/
+-rw-rw-rw-   0        0        0     2158 2024-05-24 18:19:23.000000 irtorch-0.1.0/irtorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2144 2024-05-24 18:19:23.000000 irtorch-0.1.0/irtorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 18:19:23.000000 irtorch-0.1.0/irtorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-08 14:36:17.000000 irtorch-0.1.0/irtorch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2024-05-24 18:19:23.000000 irtorch-0.1.0/irtorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 18:19:23.000000 irtorch-0.1.0/irtorch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 18:19:23.796207 irtorch-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1099 2024-05-24 18:17:58.000000 irtorch-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 18:19:23.795207 irtorch-0.1.0/tests/
+-rw-rw-rw-   0        0        0     1132 2024-02-20 20:30:27.000000 irtorch-0.1.0/tests/test_activation_functions.py
+-rw-rw-rw-   0        0        0     4451 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_ae.py
+-rw-rw-rw-   0        0        0     8090 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_bit_scales.py
+-rw-rw-rw-   0        0        0      984 2024-05-20 12:51:01.000000 irtorch-0.1.0/tests/test_config.py
+-rw-rw-rw-   0        0        0    17943 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_evaluation.py
+-rw-rw-rw-   0        0        0     2196 2024-04-04 11:55:33.000000 irtorch-0.1.0/tests/test_gaussian_mixture_torch.py
+-rw-rw-rw-   0        0        0     9764 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_integration.py
+-rw-rw-rw-   0        0        0     6679 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_internal_utils.py
+-rw-rw-rw-   0        0        0     3310 2024-03-08 13:28:02.000000 irtorch-0.1.0/tests/test_latent_variable_functions.py
+-rw-rw-rw-   0        0        0     5119 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_layers.py
+-rw-rw-rw-   0        0        0     1799 2024-04-18 13:25:53.000000 irtorch-0.1.0/tests/test_load_dataset.py
+-rw-rw-rw-   0        0        0     4247 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_mml.py
+-rw-rw-rw-   0        0        0     2850 2024-02-08 14:34:51.000000 irtorch-0.1.0/tests/test_outlier_detector.py
+-rw-rw-rw-   0        0        0     3252 2024-02-08 14:34:51.000000 irtorch-0.1.0/tests/test_quantile_mv_normal.py
+-rw-rw-rw-   0        0        0     5666 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0     5283 2024-05-24 18:17:58.000000 irtorch-0.1.0/tests/test_vae.py
```

### Comparing `irtorch-0.0.4/LICENSE.txt` & `irtorch-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/PKG-INFO` & `irtorch-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irtorch
-Version: 0.0.4
+Version: 0.1.0
 Summary: IRTorch: An item response theory package for python.
 Home-page: https://github.com/joakimwallmark/irtorch
 Author: Joakim Wallmark
 Author-email: wallmark.joakim@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `irtorch-0.0.4/README.md` & `irtorch-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/irtorch/_internal_utils.py` & `irtorch-0.1.0/irtorch/_internal_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,56 +20,44 @@
     bias = torch.cat([torch.ones(x.size(0), 1), x], dim=1)
 
     # Compute the weights using the normal equation
     w = torch.inverse(bias.t().mm(bias)).mm(bias.t()).mm(y)
 
     return w
 
-
-def impute_missing(data: torch.tensor, mc_correct: list[int] = None, item_categories: list[int] = None):
+def fix_missing_values(data: torch.Tensor, model_missing: bool = False, imputation_method: str = "zero"):
     """
-    Impute missing values in the data. For multiple choice data for which missing is not modeled, imputes randomly from incorrect responses.
+    Deal with missing values so that the data can be used for fitting.
 
     Parameters
-    -----------
+    ----------
     data : torch.Tensor
-        A 2D tensor where each row represents one respondent and each column represents an item.
-        The values should be the scores/possible responses on the items, starting from 0.
-        Missing item responses need to be coded as -1 or 'nan'.
-    mc_correct : list[int], optional
-        A list of integers where each integer is the correct response for the corresponding item. If None, the data is assumed to be non multiple choice (or dichotomously scored multiple choice with only 0's and 1's). (default is None)
-    item_categories : list[int], optional
-        A list of integers where each integer is the number of possible responses for the corresponding item. If None, the number of possible responses is calculated from the data. (default is None)
+        The data to fix.
+    model_missing : bool, optional
+        Whether the model can handle missing values. If True, missing values are encoded as -1. If False, missing values are imputed. (default is False)
+    imputation_method : str, optional
+        The method to use for imputing missing values. The default is "zero".
 
     Returns
-    ----------
+    -------
     torch.Tensor
-        A 2D tensor with missing values imputed. Rows are respondents and columns are items.
+        The data with missing values imputed.
     """
     if data.isnan().any():
         data[data.isnan()] = -1
 
-    if mc_correct is None:
-        data[data==-1] = 0
-        return data
-    else: 
-        if item_categories is None:
-            raise ValueError("item_categories are required for multiple choice imputation")
-        for col in range(data.shape[1]):
-            # Get the incorrect non-missing responses from the column
-            incorrect_responses = torch.arange(0, item_categories[col])
-            incorrect_responses = incorrect_responses[incorrect_responses != mc_correct[col]-1]
-
-            # Find the indices of -1 values in the column
-            missing_indices = (data[:, col] == -1).squeeze()
-
-            # randomly sample from the incorrect responses and replace missing
-            data[missing_indices, col] = incorrect_responses[torch.randint(0, incorrect_responses.size(0), (missing_indices.sum(),))].float()
+    if model_missing:
+        data = data + 1 # handled in theta_scores for nn
+    else:
+        if imputation_method == "zero":
+            data[data == -1] = 0
+        else:
+            raise NotImplementedError("Imputation methods not implemented yet")
 
-        return data
+    return data
 
 def random_guessing_data(
     item_categories: list[int],
     size: int,
     guessing_probabilities: list[float] = None,
     mc_correct: list[int] = None
 ):
@@ -143,28 +131,28 @@
     return response_matrix
 
 def conditional_score_distribution(
     probabilities: torch.Tensor,
     item_categories: list[int],
 ):
     """
-    Compute total score distribution conditional on z as by (Thissen et. al. 1995).
+    Compute total score distribution conditional on theta as by (Thissen et. al. 1995).
 
     Parameters
     ----------
     probabilities : torch.Tensor
-        A 3D tensor containing item score probabilities for each z quadrature point.
+        A 3D tensor containing item score probabilities for each theta quadrature point.
         The first dimension represents the quadrature points, the second dimension represents the items and the third dimension represents the item categories.
     item_categories : list[list]
         A list of integers where each integer is the number of possible responses for the corresponding item.
 
     Returns
     -------
     torch.Tensor
-        A 2D torch tensor of total score probabilities, rows being quadrature z points and columns being total scores. (rows sum to 1)
+        A 2D torch tensor of total score probabilities, rows being quadrature theta points and columns being total scores. (rows sum to 1)
     """
     no_items = probabilities.shape[1]
     q_points = probabilities.shape[0]
     max_score = sum(item_categories) - no_items
 
     # Rows are quadrature points, columns are total scores
     nsprobs = torch.zeros(q_points, max_score + 1).to(probabilities.device)
@@ -194,15 +182,15 @@
     """
     Sum incorrect score probabilities for multiple choice items. Useful for approximating sum scores.
 
     Parameters
     ----------
     probabilities : list[torch.Tensor]
         A list of 2D tensors containing item score probabilities for each item.
-        Rows are z quadrature points from the z density and columns correspond to item responses. (rows sum to 1)
+        Rows are theta quadrature points from the theta density and columns correspond to item responses. (rows sum to 1)
     modeled_item_responses : list[int]
         A list of integers where each integer is the number of possible responses for the corresponding item.
     mc_correct : list[int]
         A list of integers where each integer is correct response for the corresponding item.
     missing_modeled : bool
         Whether probabilities come from a model that modeled missing responses.
 
@@ -294,25 +282,26 @@
 class PytorchIRTDataset(torch.utils.data.Dataset):
     def __init__(self, data: torch.Tensor):
         super().__init__()
         self.data = data
         # set missing responses to 0 in the response mask (all non-missing are ones)
         self.mask = torch.zeros_like(data, dtype=torch.int)
         self.mask[data == -1] = 1
+        self.mask[data.isnan()] = 1
 
     def __len__(self) -> int:
         return len(self.data)
 
     def __getitem__(self, index: int):
         return self.data[index], self.mask[index]
 
 def is_jupyter():
     try:
         from IPython import get_ipython
-        if 'IPKernelApp' not in get_ipython().config:
+        if "IPKernelApp" not in get_ipython().config:
             raise ImportError("Not in IPython")
         return True
     except Exception:
         return False
 
 def dynamic_print(string_to_print):
     """
@@ -321,8 +310,8 @@
     Parameters
     ----------
     *args : str
         Strings to print
 
     """
     formatted_string = f"\r{string_to_print} " # small space after to make it look better in terminal
-    print(formatted_string, end='', flush=True)
+    print(formatted_string, end="", flush=True)
```

### Comparing `irtorch-0.0.4/irtorch/activation_functions.py` & `irtorch-0.1.0/irtorch/activation_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import torch
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 class BoundedELU(torch.autograd.Function):
     # Set generate_vmap_rule to True to ask PyTorch to automatically generate a vmap rule.
     generate_vmap_rule = True
 
     @staticmethod
     def forward(input_tensor: torch.Tensor, alpha=1.0):
@@ -38,16 +38,16 @@
         middle_mask = 1 - neg_mask - pos_mask
 
         neg_part = alpha * (torch.exp(input_tensor + 1) - 1) - 1
         pos_part = -alpha * (torch.exp(-input_tensor + 1) - 1) + 1
         middle_part = input_tensor
 
         # we need to remove possible infinities to avoid nan in the output
-        neg_part = torch.where(neg_part == float('inf'), torch.zeros_like(neg_part), neg_part)
-        pos_part = torch.where(pos_part == float('-inf'), torch.zeros_like(pos_part), pos_part)
+        neg_part = torch.where(neg_part == float("inf"), torch.zeros_like(neg_part), neg_part)
+        pos_part = torch.where(pos_part == float("-inf"), torch.zeros_like(pos_part), pos_part)
 
         output = neg_mask * neg_part + pos_mask * pos_part + middle_mask * middle_part
 
         return output
 
     @staticmethod
     def setup_context(ctx, inputs, output):
@@ -80,12 +80,12 @@
         middle_mask = 1 - neg_mask - pos_mask
 
         neg_part_grad = alpha * torch.exp(input_tensor + 1)
         pos_part_grad = alpha * torch.exp(-input_tensor + 1)
         middle_part_grad = 1
 
         # Ensuring gradient is not infinite
-        neg_part_grad = torch.where(neg_part_grad == float('inf'), torch.zeros_like(neg_part_grad), neg_part_grad)
-        pos_part_grad = torch.where(pos_part_grad == float('inf'), torch.zeros_like(pos_part_grad), pos_part_grad)
+        neg_part_grad = torch.where(neg_part_grad == float("inf"), torch.zeros_like(neg_part_grad), neg_part_grad)
+        pos_part_grad = torch.where(pos_part_grad == float("inf"), torch.zeros_like(pos_part_grad), pos_part_grad)
 
         grad_input = neg_mask * neg_part_grad + pos_mask * pos_part_grad + middle_mask * middle_part_grad
         return grad_input * grad_output, None
```

### Comparing `irtorch-0.0.4/irtorch/config.py` & `irtorch-0.1.0/irtorch/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 def set_verbosity(level) -> None:
     """
     Specifies the severity of log messages that the package will display.
 
     Parameters
     ----------
```

### Comparing `irtorch-0.0.4/irtorch/cross_validation.py` & `irtorch-0.1.0/irtorch/cross_validation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import logging
 import torch
 import copy
 import pandas as pd
 from itertools import product
 import torch.multiprocessing as mp
-from irtorch.irt import IRT
+from irtorch.models import BaseIRTModel
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 def cross_validation(
-    irt_model: IRT,
+    model: BaseIRTModel,
     data: torch.Tensor,
     folds: int,
     params_grid: dict,
     device: str = "cuda" if torch.cuda.is_available() else "cpu",
-    z_estimation_method: str = "ML",
+    theta_estimation: str = "ML",
     **kwargs
 ) -> pd.DataFrame:
     """
-    Perform cross-validation on the given model and data. Uses log-likelihood for model evaluation. Note that for running on the CPU on windows, `if __name__ == "__main__":` needs to be added to the main script before calling this function, see examples.
+    Perform cross-validation on the given model and data. Uses log-likelihood for model evaluation. Note that for running on the CPU on windows, `if __name__ == '__main__':` needs to be added to the main script before calling this function, see examples.
 
     Parameters
     ----------
     irt_model : IRT
         The irt model to train. Note that this should be an untrained model.
     data : torch.Tensor
         The data to use for cross-validation. The data is randomly shuffled before splitting into folds.
     folds : int
         The number of folds to use for cross-validation.
     params_grid : dict
         The hyperparameters to use for cross-validation. All need to be arguments for the model fit method.
-    z_estimation_method : str, optional
-        Method used to obtain the z scores. Also used for bit scores as they require the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
+    theta_estimation : str, optional
+        Method used to obtain the theta scores. Also used for bit scores as they require the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
     device : str, optional
         The device to use for training. Can be 'cpu' for CPU or 'cuda' for GPU (if available). The default is 'cuda' if a GPU is available, otherwise 'cpu'.
     **kwargs
         Additional keyword arguments to pass to the model fit method.
 
     Returns
     -------
@@ -44,36 +44,37 @@
 
     Examples
     --------
     This example demonstrates how to use cross_validation() function with the Swedish National Mathematics dataset.
 
     First, we import necessary modules, load the data and split it into a training and testing set:
 
-    >>> from irtorch import IRT
+    >>> from irtorch.models import MonotoneNN
+    >>> from irtorch.estimation_algorithms import AE
     >>> from irtorch.load_dataset import swedish_national_mathematics_2
     >>> from irtorch.utils import split_data
     >>> from irtorch.cross_validation import cross_validation
     >>> data_math = swedish_national_mathematics_2()
     >>> train_data, test_data = split_data(data_math, 0.8)
 
     Next, we initialize the IRT model:
 
-    >>> irt_model = IRT(data=data_math)
+    >>> model = MonotoneNN(data=data_math)
 
     We then set up a grid of parameters for cross-validation:
 
     >>> params_grid = {
     ...     'learning_rate': [0.05, 0.1],
     ...     'batch_size': [64, 128],
     ... }
 
     Finally, we perform cross-validation to find a good set of parameters:
 
-    >>> if __name__ == "__main__":
-    ...     result = cross_validation(irt_model, data=train_data, folds=5, params_grid=params_grid, z_estimation_method="NN", device="cpu")
+    >>> if __name__ == '__main__':
+    ...     result = cross_validation(model, data=train_data, folds=5, params_grid=params_grid, theta_estimation='NN', device='cpu', algorithm = AE())
     """
     if device == "cuda" and not torch.cuda.is_available():
         raise ValueError("CUDA is not available on this machine, use device = 'cpu'.")
 
     # randomly scrable the data
     data = data[torch.randperm(data.shape[0])]
     data_folds = torch.chunk(data, folds, dim=0)
@@ -92,15 +93,15 @@
 
     # Prepare arguments for multiprocessing
     jobs = []
     for params in param_dicts:
         for fold in range(folds):
             train_data = torch.cat([data_folds[i] for i in range(folds) if i != fold])
             validation_data = data_folds[fold]
-            jobs.append((copy.deepcopy(irt_model), train_data, validation_data, params, z_estimation_method, device))
+            jobs.append((copy.deepcopy(model), train_data, validation_data, params, theta_estimation, device))
 
     if device == "cpu":
         cores_to_use = mp.cpu_count()
         print(f"Using {cores_to_use} cores")
         original_threads = torch.get_num_threads()
         try:
             with mp.Pool(cores_to_use) as pool:
@@ -115,15 +116,15 @@
 
     # average over folds
     results = pd.DataFrame(results)
     results.drop(list(kwargs.keys()), axis=1, inplace=True)
     results = results.groupby(param_comb_names).mean().reset_index()
     return results
 
-def _cv_fold(irt_model : IRT, train_data, validation_data, params, z_estimation_method, device):
+def _cv_fold(irt_model : BaseIRTModel, train_data, validation_data, params, theta_estimation, device):
     if device == "cpu":
         torch.set_num_threads(1) # One thread per core, to avoid overloading the CPU
 
     irt_model.fit(train_data, device=device, **params)
-    log_likelihood = irt_model.log_likelihood(validation_data, z_estimation_method = z_estimation_method, reduction="sum").item()
+    log_likelihood = irt_model.evaluation.log_likelihood(validation_data, theta_estimation = theta_estimation, reduction="sum").item()
 
     return {**params, "log_likelihood": log_likelihood}
```

### Comparing `irtorch-0.0.4/irtorch/datasets/big_five/big_five.pt` & `irtorch-0.1.0/irtorch/datasets/big_five/big_five.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/irtorch/datasets/national_mathematics/mathematics_1.pt` & `irtorch-0.1.0/irtorch/datasets/national_mathematics/mathematics_1.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/irtorch/datasets/national_mathematics/mathematics_2.pt` & `irtorch-0.1.0/irtorch/datasets/national_mathematics/mathematics_2.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt` & `irtorch-0.1.0/irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt` & `irtorch-0.1.0/irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/irtorch/estimation_algorithms/aeirt.py` & `irtorch-0.1.0/irtorch/estimation_algorithms/ae.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,137 +1,119 @@
 import logging
 import copy
 import torch
-from torch import nn
 from irtorch.models import BaseIRTModel
 from irtorch.estimation_algorithms import BaseIRTAlgorithm
-from irtorch.estimation_algorithms.encoders import BaseEncoder, StandardEncoder
+from irtorch.estimation_algorithms.encoders import StandardEncoder
 from irtorch._internal_utils import dynamic_print, PytorchIRTDataset
 from irtorch.utils import one_hot_encode_test_data, decode_one_hot_test_data
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
-class AEIRT(BaseIRTAlgorithm, nn.Module):
+class AE(BaseIRTAlgorithm):
     """
     Autoencoder neural network for fitting IRT models.
-
-    Parameters
-    ----------
-    model : BaseIRTModel
-        The model to fit. Needs to inherit irtorch.models.BaseIRTModel.
-    encoder : BaseEncoder, optional
-        The encoder instance to use. Needs to inherit irtorch.models.BaseEncoder. Overrides hidden_layers_encoder, nonlinear_encoder and batch_normalization_encoder if provided. (default is None)
-    one_hot_encoded : bool, optional
-        Whether the model uses one-hot encoded data. (default is False)
-    hidden_layers_encoder : list[int], optional
-        List of hidden layers for the encoder. Each element is a layer with the number of neurons represented as integers. If not provided, uses one hidden layer with 2 * sum(item_categories) neurons.
-    nonlinear_encoder : torch.nn.Module, optional
-        The non-linear function to use after each hidden layer in the encoder. (default is torch.nn.ELU())
-    batch_normalization_encoder : bool, optional
-        Whether to use batch normalization for the encoder. (default is True)
     """
-    def __init__(
-        self,
-        model: BaseIRTModel,
-        encoder: BaseEncoder = None,
-        one_hot_encoded: bool = False,
-        hidden_layers_encoder: list[int] = None,
-        nonlinear_encoder = torch.nn.ELU(),
-        batch_normalization_encoder: bool = True,
-    ):
-        super().__init__(model = model, one_hot_encoded=one_hot_encoded)
+    def __init__(self):
+        super().__init__()
         self.imputation_method = "zero"
-        self.batch_normalization = batch_normalization_encoder
-
-        if encoder is not None and self.model is not None:
-            if encoder.latent_variables != self.model.latent_variables:
-                raise ValueError(
-                    "Encoder and decoder must have the same number of latent variables"
-                )
-        
-        if encoder is not None:
-            self.model.latent_variables = encoder.latent_variables
-            self.encoder = encoder
-        else:
-            if self.one_hot_encoded:
-                input_dim = sum(self.model.modeled_item_responses)
-            else:
-                input_dim = len(self.model.modeled_item_responses)
-            if hidden_layers_encoder is None:  # 1 layer with 2x number of categories as neurons is default
-                hidden_layers_encoder = [2 * sum(self.model.modeled_item_responses)]
-            self.encoder = StandardEncoder(
-                input_dim=input_dim,
-                latent_variables=self.model.latent_variables,
-                hidden_dim=hidden_layers_encoder,
-                batch_normalization=batch_normalization_encoder,
-                nonlinear=nonlinear_encoder,
-            )
-
-        self.training_z_scores = None
+        self.one_hot_encoded = True
+        self.batch_normalization = False
+        self.encoder = None
+        self.training_theta_scores = None
+        self.data_loader = None
+        self.validation_data_loader = None
+        self.optimizer = None
         self.training_history = {
             "train_loss": [],
             "validation_loss": [],
         }
 
-        # always set to eval mode by default
-        self.model.eval()
-        self.encoder.eval()
-
-    def forward(self, data):
-        return self.model(self.encoder(data))
-
     def fit(
         self,
+        model: BaseIRTModel,
         train_data: torch.Tensor,
         validation_data: torch.Tensor = None,
+        one_hot_encoded: bool = True,
+        hidden_layers_encoder: list[int] = None,
+        nonlinear_encoder = torch.nn.ELU(),
+        batch_normalization_encoder: bool = True,
         batch_size: int = 64,
         max_epochs: int = 1000,
         learning_rate: float = 0.04,
         learning_rate_update_patience: int = 4,
         learning_rate_updates_before_stopping: int = 5,
         device: str = "cuda" if torch.cuda.is_available() else "cpu",
         imputation_method: str = "zero",
     ):
         """
         Train the autoencoder model.
 
         Parameters
         ----------
+        model : BaseIRTModel
+            The model to fit. Needs to inherit :class:`irtorch.models.BaseIRTModel`.
         train_data : torch.Tensor
             The training data. Item responses should be coded 0, 1, ... and missing responses coded as nan or -1.
         validation_data : torch.Tensor, optional
             The validation data. (default is None)
+        one_hot_encoded : bool, optional
+            Whether or not to one-hot encode the train data as encoder input inside this fit method. (default is True)
+        hidden_layers_encoder : list[int], optional
+            List of hidden layers for the encoder. Each element is a layer with the number of neurons represented as integers. If not provided, uses one hidden layer with 2 * sum(item_categories) neurons.
+        nonlinear_encoder : torch.nn.Module, optional
+            The non-linear function to use after each hidden layer in the encoder. (default is torch.nn.ELU())
+        batch_normalization_encoder : bool, optional
+            Whether to use batch normalization for the encoder. (default is True)
         batch_size : int, optional
             The batch size for training. (default is 64)
         max_epochs : int, optional
             The maximum number of epochs to train for. (default is 1000)
         learning_rate : float, optional
-            The initial learning rate for the optimizer. (default is 0.08)
+            The initial learning rate for the optimizer. (default is 0.04)
         learning_rate_update_patience : int, optional
             The number of epochs to wait before reducing the learning rate. (default is 4)
         learning_rate_updates_before_stopping : int, optional
             The number of times the learning rate can be reduced before stopping training. (default is 5)
         device : str, optional
             The device to run the model on. (default is "cuda" if available else "cpu".)
         imputation_method : str, optional
             The method to use for imputing missing data. (default is "zero")
         """
-        super().fit(train_data)
+        super().fit(model = model, train_data = train_data)
+        self.one_hot_encoded = one_hot_encoded
+        self.batch_normalization = batch_normalization_encoder
         self.imputation_method = imputation_method
 
-        # Initialize the training history
+        if self.one_hot_encoded:
+            input_dim = sum(model.modeled_item_responses)
+        else:
+            input_dim = len(model.modeled_item_responses)
+
+        if hidden_layers_encoder is None:  # 1 layer with 2x number of categories as neurons is default
+            hidden_layers_encoder = [2 * sum(model.modeled_item_responses)]
+
+        self.encoder = StandardEncoder(
+            input_dim=input_dim,
+            latent_variables=model.latent_variables,
+            hidden_dim=hidden_layers_encoder,
+            batch_normalization=batch_normalization_encoder,
+            nonlinear=nonlinear_encoder,
+        )
+
+        # Re-initialize the training history
         self.training_history = {
             "train_loss": [],
             "validation_loss": [],
         }
 
         if self.one_hot_encoded:
-            train_data = one_hot_encode_test_data(train_data, self.model.item_categories, encode_missing=self.model.model_missing)
+            train_data = one_hot_encode_test_data(train_data, model.item_categories, encode_missing=model.model_missing)
             if validation_data is not None:
-                validation_data = one_hot_encode_test_data(validation_data, self.model.item_categories, encode_missing=self.model.model_missing)
+                validation_data = one_hot_encode_test_data(validation_data, model.item_categories, encode_missing=model.model_missing)
 
         self.data_loader = torch.utils.data.DataLoader(
             PytorchIRTDataset(data=train_data.to(device)),
             batch_size=batch_size,
             shuffle=True,
             pin_memory=False,
         )
@@ -140,220 +122,232 @@
             self.validation_data_loader = torch.utils.data.DataLoader(
                 PytorchIRTDataset(data=validation_data),
                 batch_size=batch_size,
                 shuffle=False,
             )
 
         self.optimizer = torch.optim.Adam(
-            [{"params": self.parameters()}], lr=learning_rate, amsgrad=True
+            list(self.encoder.parameters()) + list(model.parameters()), lr=learning_rate, amsgrad=True
         )
 
         # Reduce learning rate when loss stops decreasing ("min")
         # we multiply the learning rate by the factor
-        # patience: We need to improvement after 5 epochs for it to trigger
+        # patience: We need no improvement after x epochs for it to trigger
         scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(
             self.optimizer, mode="min", factor=0.6, patience=learning_rate_update_patience
         )
 
-        self.to(device)
-        self._training_loop(max_epochs, scheduler, validation_data, learning_rate_updates_before_stopping)
-        self.to("cpu")
-        self.eval()
+        self.encoder.to(device)
+        model.to(device)
+        self._training_loop(model, max_epochs, scheduler, validation_data, learning_rate_updates_before_stopping)
+        self.encoder.to("cpu")
+        model.to("cpu")
+        self.encoder.eval()
+        model.eval()
 
-        # store the latent z scores of the training data
+        # store the latent theta scores of the training data
         # used for more efficient computation when using other methods
         if not self.one_hot_encoded:
-            train_data = self.fix_missing_values(train_data)
-        self.training_z_scores = self.z_scores(train_data).clone().detach()
+            if train_data.isnan().any():
+                train_data[train_data.isnan()] = -1
+            if model.model_missing:
+                train_data = train_data + 1 # handled in theta_scores for nn
+            else:
+                train_data[train_data == -1] = 0
+
+        self.training_theta_scores = self.theta_scores(train_data).clone().detach()
 
     def _training_loop(
         self,
+        model: BaseIRTModel,
         max_epochs: int,
         scheduler: torch.optim.lr_scheduler.ReduceLROnPlateau,
         validation_data: torch.Tensor = None,
         learning_rate_updates_before_stopping: int = 5,
     ):
         """
         The training loop for the model.
 
         Parameters
         ----------
+        model : BaseIRTModel
+            The model to train.
         max_epochs : int
             The maximum number of epochs to train for.
+        scheduler : torch.optim.lr_scheduler.ReduceLROnPlateau
+            The learning rate scheduler.
         validation_data : torch.Tensor, optional
             The validation data.
+        learning_rate_updates_before_stopping : int, optional
+            The number of times the learning rate can be reduced before stopping training. (default is 5)
         """
         lr_update_count = 0
-        best_loss = float('inf')
-        prev_lr = [group['lr'] for group in self.optimizer.param_groups]
+        best_loss = float("inf")
+        prev_lr = [group["lr"] for group in self.optimizer.param_groups]
         for epoch in range(max_epochs):
-            # logger.info("-----------\nEpoch: %s\n-----------", epoch)
-            
             if hasattr(self, "anneal"):
                 if self.anneal:
                     self.annealing_factor = min(1.0, epoch / self.annealing_epochs)
                 else:
                     self.annealing_factor = 1.0
 
-            train_loss = self._train_step(epoch)
+            train_loss = self._train_step(model)
 
             if validation_data is not None:
-                validation_loss = self._validation_step()
+                validation_loss = self._validation_step(model)
                 current_loss = validation_loss
                 scheduler.step(validation_loss)
                 dynamic_print(f"Epoch: {epoch}. Average training batch loss: {train_loss:.4f}. Average validation batch loss: {validation_loss:.4f}")
             else:
                 current_loss = train_loss
                 scheduler.step(train_loss)
                 dynamic_print(f"Epoch: {epoch}. Average training batch loss function: {train_loss:.4f}")
 
             if current_loss < best_loss:
                 best_loss = current_loss
                 best_epoch = epoch
-                best_model_state = { 'state_dict': copy.deepcopy(self.state_dict()),
-                                    'optimizer': copy.deepcopy(self.optimizer.state_dict()) }
+                best_model_state = { 
+                    "state_dict_model": copy.deepcopy(model.state_dict()),
+                    "state_dict_encoder": copy.deepcopy(self.encoder.state_dict()),
+                    "optimizer": copy.deepcopy(self.optimizer.state_dict()) 
+                }
             
-            # Break if the learning rate has been updated 3 times
             if lr_update_count >= learning_rate_updates_before_stopping:
                 logger.info("Stopping training after %s learning rate updates.", learning_rate_updates_before_stopping)
                 break
 
-            current_lr = [group['lr'] for group in self.optimizer.param_groups]
+            current_lr = [group["lr"] for group in self.optimizer.param_groups]
             # Check if the learning rate has been updated
             if current_lr != prev_lr:
                 lr_update_count += 1
                 prev_lr = current_lr
 
-            logger.debug("Current learning rate: %s", self.optimizer.param_groups[0]['lr'])
+            logger.debug("Current learning rate: %s", self.optimizer.param_groups[0]["lr"])
 
         # Load the best model state
         if best_model_state is not None:
-            self.load_state_dict(best_model_state['state_dict'])
-            self.optimizer.load_state_dict(best_model_state['optimizer'])
+            model.load_state_dict(best_model_state["state_dict_model"])
+            self.encoder.load_state_dict(best_model_state["state_dict_encoder"])
+            self.optimizer.load_state_dict(best_model_state["optimizer"])
             logger.info("Best model found at epoch %s with loss %.4f.", best_epoch, best_loss)
 
-    def _train_step(self, epoch):
+    def _train_step(self, model: BaseIRTModel):
         """
         Perform a training step for the model.
 
         Returns
         -------
         float
             The loss after the training step.
         """
-        self.train()
+        self.encoder.train()
+        model.train()
         loss = 0
 
         for _, (batch, mask) in enumerate(self.data_loader):
             # small batches leads to inaccurate batch variance, so we drop the last few observations
             if batch.shape[0] < 4 and self.batch_normalization:
                 continue
             batch = self._impute_missing(batch, mask)
             self.optimizer.zero_grad()
-            batch_loss = self._train_batch(batch)
+            batch_loss = self._train_batch(model, batch)
             batch_loss.backward()
 
             self.optimizer.step()
             loss += batch_loss.item()
 
-        # Calculate averge per batch loss and accuracy per epoch and print out what's happening
+        # Calculate averge per batch loss and accuracy per epoch and print
         loss /= len(self.data_loader)
         self.training_history["train_loss"].append(loss)
         return loss
 
     def _impute_missing(self, batch, missing_mask):
         if torch.sum(missing_mask) > 0:
             if self.imputation_method == "zero":
                 imputed_batch = batch
                 imputed_batch = imputed_batch.masked_fill(missing_mask.bool(), 0)
-            elif self.imputation_method == "prior":
-                imputed_batch = self._impute_missing_with_prior(batch, missing_mask)
             elif self.imputation_method == "mean":
                 raise NotImplementedError("Mean imputation not implemented")
             else:
                 raise ValueError(
                     f"Imputation method {self.imputation_method} not implmented"
                 )
             return imputed_batch
 
         return batch
 
-    def _impute_missing_with_prior(self, batch, missing_mask):
-        raise NotImplementedError(
-            "There is no prior for non-variational autoencoder models"
-        )
-
-    def _train_batch(self, batch: torch.Tensor):
+    def _train_batch(self, model: BaseIRTModel, batch: torch.Tensor):
         """
         Train the model on a batch of data.
 
         Parameters
         ----------
         batch : torch.Tensor
             The batch of data.
 
         Returns
         -------
         tuple
             The logits and loss after training on the batch.
         """
-        batch_logits = self(batch)
+        batch_logits = model(self.encoder(batch))
         if self.one_hot_encoded:
             # for running with loss_function
-            batch = decode_one_hot_test_data(batch, self.model.modeled_item_responses)
-        batch_loss = -self.model.log_likelihood(batch, batch_logits) / batch.shape[0]
+            batch = decode_one_hot_test_data(batch, model.modeled_item_responses)
+        batch_loss = -model.log_likelihood(batch, batch_logits) / batch.shape[0]
         return batch_loss
 
-    @torch.inference_mode()  # decorator applies with torch.inference_mode(): to entire function
-    def _validation_step(self):
+    @torch.inference_mode()
+    def _validation_step(self, model: BaseIRTModel):
         """
         Perform a validation step.
 
         Returns
         -------
         torch.Tensor
             The loss after the validation step.
         """
-        self.eval()
+        self.encoder.eval()
+        model.eval()
         loss = 0
         for _, (batch, mask) in enumerate(self.validation_data_loader):
             batch = self._impute_missing(batch, mask)
-            batch_loss, _ = self._batch_fit_measures(batch)
+            batch_loss, _ = self._batch_fit_measures(model, batch)
 
             loss += batch_loss.item()
         loss /= len(self.validation_data_loader)
         self.training_history["validation_loss"].append(loss)
         return loss
 
     @torch.inference_mode()
-    def _batch_fit_measures(self, batch: torch.Tensor):
+    def _batch_fit_measures(self, model: BaseIRTModel, batch: torch.Tensor):
         """
         Calculate the fit measures for a batch.
 
         Parameters
         ----------
         batch : torch.Tensor
             The batch of data.
 
         Returns
         -------
         tuple
             The loss, log likelihood, and accuracy for the batch.
         """
-        output = self(batch)
+        output = model(self.encoder(batch))
         if self.one_hot_encoded:
             # for running with loss_function
-            batch = decode_one_hot_test_data(batch, self.model.modeled_item_responses)
+            batch = decode_one_hot_test_data(batch, model.modeled_item_responses)
         # negative ce is log likelihood
-        log_likelihood = self.model.log_likelihood(batch, output)
+        log_likelihood = model.log_likelihood(batch, output)
         loss = -log_likelihood / batch.shape[0]
         return loss, log_likelihood
 
     @torch.inference_mode()
-    def z_scores(self, data: torch.Tensor):
+    def theta_scores(self, data: torch.Tensor):
         """
         Get the latent scores from an input
 
         Parameters
         ----------
         data: torch.Tensor
             A 2D tensor with test data. Columns are items and rows are respondents.
```

### Comparing `irtorch-0.0.4/irtorch/estimation_algorithms/base_irt_algorithm.py` & `irtorch-0.1.0/irtorch/estimation_algorithms/base_irt_algorithm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,44 @@
-import logging
+from __future__ import annotations
+from typing import TYPE_CHECKING
 from abc import ABC, abstractmethod
 import torch
-from irtorch.models import BaseIRTModel
 
-logger = logging.getLogger('irtorch')
+if TYPE_CHECKING:
+    from irtorch.models import BaseIRTModel
 
 class BaseIRTAlgorithm(ABC):
     """
     Abstract base class for IRT algorithms. All IRT algorithms should inherit from this class.
 
     Parameters
     ----------
     model : BaseIRTModel, optional
-        The model to train. Needs to inherit irtorch.models.BaseIRTModel.
+        The model to train. Needs to inherit :class:`irtorch.models.BaseIRTModel`.
     one_hot_encoded : bool, optional
-        Whether the algorithm uses one-hot encoded data. (default is False)
+        Whether the algorithm uses one-hot encoded data. (default is True)
     """
-    def __init__(
-        self,
-        model: BaseIRTModel,
-        one_hot_encoded: bool = False,
-    ):
+    def __init__(self):
         super().__init__()
-        self.model = model
-        self.imputation_method = "zero"
         self.train_data = None
 
-        if model.mc_correct is not None:
-            self.one_hot_encoded = True
-        else:
-            self.one_hot_encoded = one_hot_encoded
-
     @abstractmethod
-    def fit(self, train_data: torch.Tensor, **kwargs):
+    def fit(self, model: BaseIRTModel, train_data: torch.Tensor, **kwargs):
         """
         Fit the model to the data.
 
         Parameters
         ----------
+        model : BaseIRTModel, optional
+            The model to train. Needs to inherit :class:`irtorch.models.BaseIRTModel`.
         train_data : torch.Tensor
             The training data.
+        **kwargs
+            Additional keyword arguments for the algorithm fit method.
         """
-        # Store all training data within the model instance
+        if (train_data.isnan().any() or (train_data == -1).any()) and model.mc_correct and not model.model_missing:
+            raise ValueError("Missing responses are not supported with multiple choice models when missing responses are not modeled. Please impute missing responses or remove the observations.")
+        # Store all training data within the algorithm instance
         if self.train_data is not None:
             self.train_data = torch.cat((self.train_data, train_data), dim=0).contiguous()
         else:
             self.train_data = train_data.contiguous()
-
-    @abstractmethod
-    def _impute_missing_with_prior(self, batch, missing_mask):
-        """
-        Impute missing values with the prior.
-
-        Parameters
-        ----------
-        batch : torch.Tensor
-            The batch of data.
-        missing_mask : torch.Tensor
-            The mask of missing values.
-
-        Returns
-        -------
-        torch.Tensor
-            The imputed data.
-        """
-        raise NotImplementedError(
-            "Prior imputation not implemented for this algorithm."
-        )
-
-    def fix_missing_values(self, data: torch.Tensor):
-        """
-        Deal with missing values so that the data can be used for fitting.
-
-        Parameters
-        ----------
-        data : torch.Tensor
-            The data to fix.
-
-        Returns
-        -------
-        torch.Tensor
-            The data with missing values imputed.
-        """
-        if data.isnan().any():
-            data[data.isnan()] = -1
-
-        if self.model.model_missing:
-            data = data + 1 # handled in z_scores for nn
-        else:
-            if self.imputation_method == "zero":
-                data[data == -1] = 0
-            else:
-                # self._impute_missing(data, data.isnan())
-                # see also helper_function impute_missing
-                raise NotImplementedError("Imputation methods not implemented yet")
-
-        return data
```

### Comparing `irtorch-0.0.4/irtorch/estimation_algorithms/encoders/base_encoder.py` & `irtorch-0.1.0/irtorch/estimation_algorithms/encoders/base_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from abc import ABC, abstractmethod
 from torch import nn
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 class BaseEncoder(ABC, nn.Module):
     """
     Abstract base class for Item Response Theory models.
     """
 
     def __init__(
```

### Comparing `irtorch-0.0.4/irtorch/estimation_algorithms/encoders/bounded_encoder.py` & `irtorch-0.1.0/irtorch/estimation_algorithms/encoders/standard_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import torch.nn as nn
 from irtorch.estimation_algorithms.encoders import BaseEncoder
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
-class BoundedEncoder(BaseEncoder):
+class StandardEncoder(BaseEncoder):
     def __init__(
         self,
         input_dim: int,
         latent_variables: int,
         hidden_dim: list[int],
         batch_normalization: bool = True,
         nonlinear=nn.ReLU(),
@@ -23,18 +23,17 @@
 
         # Hidden layers
         for i in range(1, len(hidden_dim)):
             self.layers.add_module(
                 f"linear{i}", nn.Linear(hidden_dim[i - 1], hidden_dim[i])
             )
             if batch_normalization:
-                self.layers.add_module("batchnorm0", nn.BatchNorm1d(hidden_dim[i]))
+                self.layers.add_module(f"batchnorm0{i}", nn.BatchNorm1d(hidden_dim[i]))
             self.layers.add_module(f"nonlinear{i}", nonlinear)
 
         # output layer
         self.layers.add_module(
             f"linear{len(hidden_dim)+1}", nn.Linear(hidden_dim[-1], latent_variables)
         )
-        self.layers.add_module(f"tanh{len(hidden_dim)+1}", nn.Tanh())
 
     def forward(self, x):
         return self.layers(x)
```

### Comparing `irtorch-0.0.4/irtorch/estimation_algorithms/encoders/standard_encoder.py` & `irtorch-0.1.0/irtorch/estimation_algorithms/encoders/bounded_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import torch.nn as nn
 from irtorch.estimation_algorithms.encoders import BaseEncoder
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
-class StandardEncoder(BaseEncoder):
+class BoundedEncoder(BaseEncoder):
     def __init__(
         self,
         input_dim: int,
         latent_variables: int,
         hidden_dim: list[int],
         batch_normalization: bool = True,
         nonlinear=nn.ReLU(),
@@ -23,17 +23,18 @@
 
         # Hidden layers
         for i in range(1, len(hidden_dim)):
             self.layers.add_module(
                 f"linear{i}", nn.Linear(hidden_dim[i - 1], hidden_dim[i])
             )
             if batch_normalization:
-                self.layers.add_module(f"batchnorm0{i}", nn.BatchNorm1d(hidden_dim[i]))
+                self.layers.add_module("batchnorm0", nn.BatchNorm1d(hidden_dim[i]))
             self.layers.add_module(f"nonlinear{i}", nonlinear)
 
         # output layer
         self.layers.add_module(
             f"linear{len(hidden_dim)+1}", nn.Linear(hidden_dim[-1], latent_variables)
         )
+        self.layers.add_module(f"tanh{len(hidden_dim)+1}", nn.Tanh())
 
     def forward(self, x):
         return self.layers(x)
```

### Comparing `irtorch-0.0.4/irtorch/estimation_algorithms/encoders/variational_encoder.py` & `irtorch-0.1.0/irtorch/estimation_algorithms/encoders/variational_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 import torch.nn as nn
 from irtorch.estimation_algorithms.encoders import BaseEncoder
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 class VariationalEncoder(BaseEncoder):
     def __init__(
         self,
         input_dim: int,
         latent_variables: int,
         hidden_dim: list[int],
-        batch_normalization: bool,
+        batch_normalization: bool = False,
         nonlinear=nn.ReLU(),
     ):
         super().__init__(input_dim, latent_variables)
         self.layers = nn.Sequential()
         # Input layer
         self.layers.add_module("linear0", nn.Linear(input_dim, hidden_dim[0]))
         if batch_normalization:
```

### Comparing `irtorch-0.0.4/irtorch/estimation_algorithms/vaeirt.py` & `irtorch-0.1.0/irtorch/estimation_algorithms/vae.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,39 @@
 import logging
 import torch
 from torch.distributions import Normal
 from irtorch.models import BaseIRTModel
-from irtorch.estimation_algorithms.aeirt import AEIRT
-from irtorch.estimation_algorithms.encoders import BaseEncoder
+from irtorch.estimation_algorithms.ae import AE
 from irtorch.estimation_algorithms.encoders import VariationalEncoder
-from irtorch.utils import decode_one_hot_test_data
+from irtorch._internal_utils import PytorchIRTDataset
+from irtorch.utils import one_hot_encode_test_data, decode_one_hot_test_data
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
-class VAEIRT(AEIRT):
+class VAE(AE):
     """
     Variational autoencoder neural network for fitting IRT models.
 
-    Parameters
-    ----------
-    model : BaseIRTModel
-        The model to fit. Needs to inherit irtorch.models.BaseIRTModel.
-    encoder : BaseEncoder, optional
-        The encoder instance to use. Needs to inherit irtorch.models.BaseEncoder. Overrides hidden_layers_encoder, nonlinear_encoder and batch_normalization_encoder if provided. (default is None)
-    one_hot_encoded : bool, optional
-        Whether the model uses one-hot encoded data. (default is False)
-    hidden_layers_encoder : list[int], optional
-        List of hidden layers for the encoder. Each element is a layer with the number of neurons represented as integers. If not provided, uses one hidden layer with 2 * sum(item_categories) neurons.
-    nonlinear_encoder : torch.nn.Module, optional
-        The non-linear function to use after each hidden layer in the encoder. (default is torch.nn.ELU())
-    batch_normalization_encoder : bool, optional
-        Whether to use batch normalization for the encoder. (default is True)
-    iw_samples : int, optional
-        The number of importance weighted samples to use. (default is 1)
-    anneal : bool, optional
-        Whether to anneal the KL divergence. (default is True)
-    annealing_epochs : int, optional
-        The number of epochs to anneal the KL divergence. (default is 5)
     """
-    def __init__(
-        self,
-        model: BaseIRTModel,
-        encoder: BaseEncoder = None,
-        one_hot_encoded: bool = False,
-        hidden_layers_encoder: list[int] = None,
-        nonlinear_encoder = torch.nn.ELU(),
-        batch_normalization_encoder: bool = True,
-        iw_samples: int = 1,
-        anneal: bool = True,
-        annealing_epochs: int = 5,
-    ):
-        self.iw_samples = iw_samples
-        self.annealing_epochs = annealing_epochs
-        self.anneal = anneal
+    def __init__(self):
+        super().__init__()
+        self.iw_samples = 1
+        self.annealing_epochs = 5
+        self.anneal = True
         self.annealing_factor = 1.0
 
-        if encoder is not None:
-            self.encoder = encoder
-        else:
-            if one_hot_encoded:
-                input_dim = sum(model.modeled_item_responses)
-            else:
-                input_dim = len(model.modeled_item_responses)
-            if hidden_layers_encoder is None:  # 1 layer with 2x number of categories as neurons is default
-                hidden_layers_encoder = [2 * sum(model.modeled_item_responses)]
-            encoder = (
-                VariationalEncoder(
-                    input_dim,
-                    model.latent_variables,
-                    hidden_layers_encoder,
-                    batch_normalization=batch_normalization_encoder,
-                    nonlinear=nonlinear_encoder,
-                )
-                if encoder is None
-                else encoder
-            )
-        super().__init__(
-            model=model,
-            encoder=encoder,
-            one_hot_encoded=one_hot_encoded,
-        )
-
     def fit(
         self,
+        model: BaseIRTModel,
         train_data: torch.Tensor,
         validation_data: torch.Tensor = None,
+        one_hot_encoded: bool = True,
+        hidden_layers_encoder: list[int] = None,
+        nonlinear_encoder = torch.nn.ELU(),
+        batch_normalization_encoder: bool = True,
         batch_size: int = 32,
         max_epochs: int = 1000,
         learning_rate: float = 0.004,
         learning_rate_update_patience: int = 4,
         learning_rate_updates_before_stopping: int = 5,
         device: str = "cuda" if torch.cuda.is_available() else "cpu",
         imputation_method: str = "zero",
@@ -93,239 +42,325 @@
         iw_samples: int = 1,
     ):
         """
         Train the variational autoencoder model.
 
         Parameters
         ----------
+        model : BaseIRTModel
+            The model to fit. Needs to inherit :class:`irtorch.models.BaseIRTModel`.
         train_data : torch.Tensor
             The training data. Item responses should be coded 0, 1, ... and missing responses coded as nan or -1.
         validation_data : torch.Tensor, optional
             The validation data. (default is None)
+        one_hot_encoded : bool, optional
+            Whether the model uses one-hot encoded data. (default is False)
+        hidden_layers_encoder : list[int], optional
+            List of hidden layers for the encoder. Each element is a layer with the number of neurons represented as integers. If not provided, uses one hidden layer with 2 * sum(item_categories) neurons.
+        nonlinear_encoder : torch.nn.Module, optional
+            The non-linear function to use after each hidden layer in the encoder. (default is torch.nn.ELU())
+        batch_normalization_encoder : bool, optional
+            Whether to use batch normalization for the encoder. (default is True)
         batch_size : int, optional
             The batch size for training. (default is 64)
         max_epochs : int, optional
             The maximum number of epochs to train for. (default is 1000)
         learning_rate : float, optional
             The initial learning rate for the optimizer. (default is 0.004)
         learning_rate_update_patience : int, optional
             The number of epochs to wait before reducing the learning rate. (default is 4)
         learning_rate_updates_before_stopping : int, optional
             The number of times the learning rate can be reduced before stopping training. (default is 5)
         device : str, optional
             The device to run the model on. (default is "cuda" if available else "cpu".)
         imputation_method : str, optional
             The method to use for imputing missing data. (default is "zero")
+        anneal : bool, optional
+            Whether to anneal the KL divergence. (default is True)
+        annealing_epochs : int, optional
+            The number of epochs to anneal the KL divergence. (default is 5)
+        iw_samples : int, optional
+            The number of importance weighted samples to use. (default is 1)
         """
+        if self.train_data is not None:
+            self.train_data = torch.cat((self.train_data, train_data), dim=0).contiguous()
+        else:
+            self.train_data = train_data.contiguous()
+
         self.iw_samples = iw_samples
         self.annealing_epochs = annealing_epochs
         self.anneal = anneal
-        super().fit(
-            train_data=train_data,
-            validation_data=validation_data,
-            batch_size=batch_size,
-            max_epochs=max_epochs,
-            learning_rate=learning_rate,
-            learning_rate_update_patience=learning_rate_update_patience,
-            learning_rate_updates_before_stopping=learning_rate_updates_before_stopping,
-            device=device,
-            imputation_method=imputation_method,
+        self.imputation_method = imputation_method
+        self.one_hot_encoded = one_hot_encoded
+
+        if one_hot_encoded:
+            input_dim = sum(model.modeled_item_responses)
+        else:
+            input_dim = len(model.modeled_item_responses)
+        if hidden_layers_encoder is None:  # 1 layer with 2x number of categories as neurons is default
+            hidden_layers_encoder = [2 * sum(model.modeled_item_responses)]
+
+        self.encoder = VariationalEncoder(
+            input_dim,
+            model.latent_variables,
+            hidden_layers_encoder,
+            batch_normalization=batch_normalization_encoder,
+            nonlinear=nonlinear_encoder,
         )
+        
+        # Re-initialize the training history
+        self.training_history = {
+            "train_loss": [],
+            "validation_loss": [],
+        }
 
-    def forward(self, data) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
-        """
-        Samples self.iw_samples logit outputs for each respondent in the input.
+        if self.one_hot_encoded:
+            train_data = one_hot_encode_test_data(train_data, model.item_categories, encode_missing=model.model_missing)
+            if validation_data is not None:
+                validation_data = one_hot_encode_test_data(validation_data, model.item_categories, encode_missing=model.model_missing)
 
-        Parameters
-        ----------
-        data : torch.Tensor
-            The input test data
+        self.data_loader = torch.utils.data.DataLoader(
+            PytorchIRTDataset(data=train_data.to(device)),
+            batch_size=batch_size,
+            shuffle=True,
+            pin_memory=False,
+        )
+        if validation_data is not None:
+            validation_data = validation_data.to(device)
+            self.validation_data_loader = torch.utils.data.DataLoader(
+                PytorchIRTDataset(data=validation_data),
+                batch_size=batch_size,
+                shuffle=False,
+            )
 
-        Returns
-        -------
-        tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]
-            Four 2D tensors with rows corresponding respondent samples.
-            -   Output logits tensor
-            -   z samples tensor
-            -   Encoder means for each sample
-            -   Encoder log variances for each sample
-            A sample for each respondent reoccurs every data.shape[0]'th row.
-        """
-        mean, logvar = self.encoder(data)
+        self.optimizer = torch.optim.Adam(
+            list(self.encoder.parameters()) + list(model.parameters()), lr=learning_rate, amsgrad=True
+        )
 
-        # takes iw_samples from the latent space for each data point (for importance weighting)
-        mean = mean.repeat(self.iw_samples, 1)
-        logvar = logvar.repeat(self.iw_samples, 1)
-        z_samples = self.reparameterize(mean, logvar)
+        # Reduce learning rate when loss stops decreasing ("min")
+        # we multiply the learning rate by the factor
+        # patience: We need no improvement after x epochs for it to trigger
+        scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(
+            self.optimizer, mode="min", factor=0.6, patience=learning_rate_update_patience
+        )
 
-        logits = self.model(z_samples)
-        return logits, z_samples, mean, logvar
+        self.encoder.to(device)
+        model.to(device)
+        self._training_loop(model, max_epochs, scheduler, validation_data, learning_rate_updates_before_stopping)
+        self.encoder.to("cpu")
+        model.to("cpu")
+        self.encoder.eval()
+        model.eval()
+
+        # store the latent theta scores of the training data
+        # used for more efficient computation when using other methods
+        if not self.one_hot_encoded:
+            if train_data.isnan().any():
+                train_data[train_data.isnan()] = -1
+            if model.model_missing:
+                train_data = train_data + 1 # handled in theta_scores for nn
+            else:
+                train_data[train_data == -1] = 0
+                
+        self.training_theta_scores = self.theta_scores(train_data).clone().detach()
 
-    def _train_batch(self, batch):
+    def _train_batch(self, model: BaseIRTModel, batch):
         """
         Train the model on a batch of data.
 
         Parameters
         ----------
+        model : BaseIRTModel
+            The model to fit.
         batch : torch.Tensor
             The batch of data.
 
         Returns
         -------
         tuple
             The logits and loss after training on the batch.
         """
-        batch_logits, z_samples, mean, logvar = self(batch)
+        mean, logvar = self.encoder(batch)
+
+        # takes iw_samples from the latent space for each data point (for importance weighting)
+        mean = mean.repeat(self.iw_samples, 1)
+        logvar = logvar.repeat(self.iw_samples, 1)
+        theta_samples = self.reparameterize(mean, logvar)
+
+        batch_logits = model(theta_samples)
+
         if self.one_hot_encoded:
             # for running with loss_function
-            batch = decode_one_hot_test_data(batch, self.model.modeled_item_responses)
-        batch_loss = self._loss_function(batch, batch_logits, z_samples, mean, logvar)
+            batch = decode_one_hot_test_data(batch, model.modeled_item_responses)
+        batch_loss = self._loss_function(model, batch, batch_logits, theta_samples, mean, logvar)
         return batch_loss
 
     def reparameterize(self, mean, logvar):
         std = torch.exp(0.5 * logvar)
         eps = torch.randn_like(std)
         return mean + eps * std
 
     # IWAE Loss = E log (1/K Σ_{k=1}^{K} w_k) (ELBO for 1 iw sample)
     def _loss_function(
         self,
+        model: BaseIRTModel,
         data: torch.Tensor,
         logits: torch.Tensor,
-        z_samples: torch.Tensor,
+        theta_samples: torch.Tensor,
         mean: torch.Tensor,
         logvar: torch.Tensor,
     ):
         """
         The IWAE loss function for the model as introduced by Burda et. al. (2015).
         When self.iw_samples == 1 this generalizes to the standard VAE ELBO loss.
 
         Parameters
         ----------
+        model : BaseIRTModel
+            The model to fit.
         data : torch.Tensor
             The input data.
         logits : torch.Tensor
             The logits output by the model.
-        z_samples : torch.Tensor
+        theta_samples : torch.Tensor
             Samples from the encoder distribution
         mean : torch.Tensor
             Means from the encoder
         logvar : torch.Tensor
             Log of the variance from the encoder
 
         Returns
         -------
         torch.Tensor
             The calculated loss.
         """
-        log_p_x_z = self.model.log_likelihood(
+        log_p_x_theta = model.log_likelihood(
             data.repeat(self.iw_samples, 1),
             logits,
             loss_reduction="none",
         )
 
         # Reshape tensor by each iw-sample
         # we need to keep a dimension for each respondent, but we can sum over items
-        log_p_x_z = log_p_x_z.view(
+        log_p_x_theta = log_p_x_theta.view(
             self.iw_samples,
-            log_p_x_z.shape[0] // (self.iw_samples * data.shape[1]),
+            log_p_x_theta.shape[0] // (self.iw_samples * data.shape[1]),
             data.shape[1],
         ).sum(2)
 
         if self.iw_samples == 1:
             # ELBO (1 sample) can be computed using the true means and variances
             # sum up kl div for each person (row)
             kl_div = 0.5 * torch.sum(mean.pow(2) + logvar.exp() - 1 - logvar, dim=1)
-            iwae_bound = log_p_x_z - self.annealing_factor * kl_div
+            iwae_bound = log_p_x_theta - self.annealing_factor * kl_div
         else:
-            log_p_z = Normal(0, 1).log_prob(z_samples)
-            log_q_z_x = Normal(mean, torch.exp(0.5 * logvar)).log_prob(z_samples)
-            kl_div = log_q_z_x - log_p_z
+            log_p_theta = Normal(0, 1).log_prob(theta_samples)
+            log_q_theta_x = Normal(mean, torch.exp(0.5 * logvar)).log_prob(theta_samples)
+            kl_div = log_q_theta_x - log_p_theta
             kl_div = kl_div.view(
                 self.iw_samples, kl_div.shape[0] // self.iw_samples, kl_div.shape[1]
             ).sum(2)
 
-            iwae_bound = log_p_x_z - self.annealing_factor * kl_div
+            iwae_bound = log_p_x_theta - self.annealing_factor * kl_div
             if self.iw_samples > 1:
                 iwae_bound = torch.logsumexp(iwae_bound, dim=0) - torch.log(
                     torch.tensor(self.iw_samples).float()
                 )  # Importance weighting log (1/K Σ_{k=1}^{K} w_k)
 
         # Estimate expectation
         return -iwae_bound.mean()
 
-    def _batch_fit_measures(self, batch):
+    def _batch_fit_measures(self, model: BaseIRTModel, batch):
         """
         Calculate the fit measures for a batch.
 
         Parameters
         ----------
+        model : BaseIRTModel
+            The model to fit.
         batch : torch.Tensor
             The batch of data.
 
         Returns
         -------
         tuple
             The loss, log likelihood, and accuracy for the batch.
         """
         encoder_mean, encoder_logvar = self.encoder(batch)
-        output = self.model(encoder_mean)
-        z_sample = self.reparameterize(encoder_mean, encoder_logvar)
-        output_stochastic = self.model(z_sample)
+        output = model(encoder_mean)
+        theta_sample = self.reparameterize(encoder_mean, encoder_logvar)
+        output_stochastic = model(theta_sample)
 
         if self.one_hot_encoded:
             # for running with loss_function
-            batch = decode_one_hot_test_data(batch, self.model.item_categories)
+            batch = decode_one_hot_test_data(batch, model.item_categories)
 
         # negative ce is log lik
-        log_likelihood = self.model.log_likelihood(
+        log_likelihood = model.log_likelihood(
             batch, output,
         )
-        log_lik_stochastic = self.model.log_likelihood(
+        log_lik_stochastic = model.log_likelihood(
             batch, output_stochastic,
         )
         kl_loss = 0.5 * torch.sum(
             encoder_mean.pow(2) + encoder_logvar.exp() - 1 - encoder_logvar
         )
         loss = (log_lik_stochastic + self.annealing_factor * kl_loss) / batch.shape[0]
         return loss, log_likelihood
 
+    def _impute_missing(self, model: BaseIRTModel, batch, missing_mask):
+        if torch.sum(missing_mask) > 0:
+            if self.imputation_method == "zero":
+                imputed_batch = batch
+                imputed_batch = imputed_batch.masked_fill(missing_mask.bool(), 0)
+            elif self.imputation_method == "prior":
+                imputed_batch = self._impute_missing_with_prior(model, batch, missing_mask)
+            elif self.imputation_method == "mean":
+                raise NotImplementedError("Mean imputation not implemented")
+            else:
+                raise ValueError(
+                    f"Imputation method {self.imputation_method} not implmented"
+                )
+            return imputed_batch
+
+        return batch
+
     @torch.inference_mode()
-    def _impute_missing_with_prior(self, batch, missing_mask):
+    def _impute_missing_with_prior(self, model: BaseIRTModel, batch, missing_mask):
         # get the decoder logits for the prior mean person
-        prior_logits = self.model(
-            torch.zeros(1, self.model.latent_variables).to(next(self.parameters()).device)
+        prior_logits = model(
+            torch.zeros(1, model.latent_variables).to(next(model.parameters()).device)
         )
-        prior_mean_scores = self._mean_scores(prior_logits)
+        prior_mean_scores = self._mean_scores(model, prior_logits)
         batch[missing_mask.bool()] = prior_mean_scores.repeat(batch.shape[0], 1).to(
-            next(self.parameters()).device
+            next(model.parameters()).device
         )[missing_mask.bool()]
 
         return batch
 
     @torch.inference_mode()
-    def _mean_scores(self, output_logits):
-        mean_scores = torch.zeros(len(self.model.modeled_item_responses))
+    def _mean_scores(self, model: BaseIRTModel, output_logits):
+        mean_scores = torch.zeros(len(model.modeled_item_responses))
         start = 0
-        for item, item_cat in enumerate(self.model.modeled_item_responses):
+        for item, item_cat in enumerate(model.modeled_item_responses):
             end = start + item_cat
             probabilities = torch.softmax(output_logits[:, start:end], dim=1)
-            item_scores = torch.arange(item_cat).to(next(self.parameters()).device)
+            item_scores = torch.arange(item_cat).to(next(model.parameters()).device)
             mean_scores[item] = torch.sum(probabilities * item_scores)
             start = end
 
         return mean_scores
 
     @torch.inference_mode()
-    def z_scores(
+    def theta_scores(
         self,
         data: torch.Tensor,
     ):
         """
-        Get the z scores from an input
+        Get the theta scores from an input
 
         Parameters
         ----------
         data: torch.Tensor
             A 2D tensor with test data. Columns are items and rows are respondents.
         
         Returns
@@ -334,45 +369,45 @@
             A 2D tensor of latent scores. Rows are respondents and columns are latent variables.
         """
         data = data.contiguous()
         return self.encoder(data)[0]
 
     @torch.inference_mode()
     def sample_latent_variables(
-        self, sample_size: int, input_data: torch.Tensor = None
+        self, model: BaseIRTModel, sample_size: int, input_data: torch.Tensor = None
     ):
         if input_data is None:
             input_data = self.train_data
         else:
-            input_data = input_data.contiguous().to(next(self.parameters()).device)
+            input_data = input_data.contiguous().to(next(model.parameters()).device)
 
         # Sample test scores until we have sample_size
         indices = torch.randint(low=0, high=input_data.size(0), size=(sample_size,)).to(
-            next(self.parameters()).device
+            next(model.parameters()).device
         )
         samples = torch.index_select(input_data, 0, indices)
         # run the sample through the encoder
         mean, logvar = self.encoder(samples)
         return self.reparameterize(mean, logvar)
 
     @torch.inference_mode()
     def latent_credible_interval(
         self, input_data: torch.Tensor, alpha=0.05
     ) -> torch.tensor:
-        input_data = input_data.contiguous().to(self.device)
+        input_data = input_data.contiguous()
         mean, logvar = self.encoder(input_data)
         # Create a Gaussian distribution with the calculated mean and std
         dist = Normal(mean, torch.exp(0.5 * logvar))
 
         # Prepare alpha tensors of the same shape as mean and std
         lower_alpha = torch.full_like(mean, alpha / 2)
         upper_alpha = torch.full_like(mean, 1 - alpha / 2)
 
         # Calculate the lower and upper bounds of the credible interval
         lower = dist.icdf(
-            lower_alpha.clone().detach().to(next(self.parameters()).device)
+            lower_alpha.clone().detach()
         )
         upper = dist.icdf(
-            upper_alpha.clone().detach().to(next(self.parameters()).device)
+            upper_alpha.clone().detach()
         )
 
         return lower, mean, upper
```

### Comparing `irtorch-0.0.4/irtorch/gaussian_mixture_model.py` & `irtorch-0.1.0/irtorch/gaussian_mixture_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import torch
 import torch.distributions as dist
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 class GaussianMixtureModel(torch.nn.Module):
     """
     Gaussian mixture model for approximating a multivariate joint density function.
 
     Parameters
     ----------
```

### Comparing `irtorch-0.0.4/irtorch/irt_evaluator.py` & `irtorch-0.1.0/irtorch/evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,188 +1,261 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING
 import logging
 import torch
-from irtorch.models import BaseIRTModel
-from irtorch.estimation_algorithms import BaseIRTAlgorithm, VAEIRT
+from torch.distributions import MultivariateNormal
+from irtorch.estimation_algorithms import VAE, AE, MML
 from irtorch.quantile_mv_normal import QuantileMVNormal
 from irtorch.gaussian_mixture_model import GaussianMixtureModel
-from irtorch.irt_scorer import IRTScorer
 from irtorch._internal_utils import (
-    impute_missing,
     conditional_score_distribution,
     sum_incorrect_probabilities,
+    fix_missing_values
 )
+from irtorch.utils import impute_missing
 
-logger = logging.getLogger('irtorch')
+if TYPE_CHECKING:
+    from irtorch.models.base_irt_model import BaseIRTModel
 
-class IRTEvaluator:
-    def __init__(self, model: BaseIRTModel, algorithm: BaseIRTAlgorithm, scorer: IRTScorer):
-        """
-        Initializes the IRTEvaluator class.
+logger = logging.getLogger("irtorch")
 
-        Parameters
-        ----------
-        model : BaseIRTModel
-            BaseIRTModel object.
-        algorithm : BaseIRTAlgorithm
-            BaseIRTAlgorithm object.
-        scorer : IRTScorer
-            IRTScorer object used to obtain latent variable scores.
-        """
+class Evaluation:
+    """
+    Class for evaluating IRT model performance using various metrics.
+
+    Parameters
+    ----------
+    model : BaseIRTModel
+        The IRT model to evaluate.
+    """
+    def __init__(self, model: BaseIRTModel):
         self.model = model
-        self.algorithm = algorithm
-        self.scorer = scorer
+        self.latent_density = None
 
-    def _evaluate_data_z_input(
+    def _evaluate_data_theta_input(
             self,
             data: torch.Tensor = None,
-            z: torch.Tensor = None,
-            z_estimation_method: str = "ML",
+            theta: torch.Tensor = None,
+            theta_estimation: str = "ML",
             ml_map_device: str = "cuda" if torch.cuda.is_available() else "cpu",
             lbfgs_learning_rate: float = 0.3,
         ):
         """"
-        Helper function for evaluating the data and z inputs for various performance measure methods.
+        Helper function for evaluating the data and theta inputs for various performance measure methods.
 
         Parameters
         ----------
         data : torch.Tensor
             The input data.
-        z: torch.Tensor, optional
-            The latent variable z scores for the provided data. If not provided, they will be computed using z_estimation_method.
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively.
+        theta: torch.Tensor, optional
+            The latent variable theta scores for the provided data. If not provided, they will be computed using theta_estimation.
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively.
         ml_map_device: str, optional
             For ML and MAP. The device to use for computation. Can be 'cpu' or 'cuda'. (default is "cuda" if available else "cpu")
         lbfgs_learning_rate: float, optional
             For ML and MAP. The learning rate to use for the LBFGS optimizer. (default is 0.3)
         """
         if data is None:
-            data = self.algorithm.train_data
+            data = self.model.algorithm.train_data
         else:
             data = data.contiguous()
 
         if not self.model.model_missing:
             data = impute_missing(data, self.model.mc_correct, self.model.item_categories)
 
-        if z is None:
-            z = self.scorer.latent_scores(data=data, scale="z", z_estimation_method=z_estimation_method, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
+        if theta is None:
+            theta = self.model.latent_scores(data=data, theta_estimation=theta_estimation, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
 
-        data = self.algorithm.fix_missing_values(data)
+        if self.model.model_missing:
+            data[data.isnan()] = -1
+            data = data + 1
+
+        data = fix_missing_values(data)
         
-        return data, z
+        return data, theta
+
+
+    @torch.inference_mode()
+    def approximate_latent_density(
+        self,
+        theta_scores: torch.Tensor,
+        approximation: str = "qmvn",
+        cv_n_components: list[int] = None,
+    ) -> None:
+        """
+        Approximate the latent space density.
+
+        Parameters
+        ----------
+        theta_scores : torch.Tensor
+            A 2D tensor with theta scores. Each row represents one respondent, and each column an item.
+        approximation : str, optional
+            The approximation method to use. (default is 'qmvn')
+            - 'qmvn' for quantile multivariate normal approximation of a multivariate joint density function (QuantileMVNormal class).
+            - 'gmm' for a gaussian mixture model.
+
+        cv_n_components: list[int], optional
+            The number of components to use for cross-validation with Gaussian Mixture Models. (default is [2, 3, 4, 5, 10])
+
+        Returns
+        -------
+        torch.Tensor
+            A 2D tensor of latent scores, with latent variables as columns.
+        """
+        if approximation == "gmm":
+            cv_n_components = [2, 3, 4, 5, 10] if cv_n_components is None else cv_n_components
+            self.latent_density = self._cv_gaussian_mixture_model(theta_scores, cv_n_components)
+        elif approximation == "qmvn":
+            self.latent_density = QuantileMVNormal()
+            self.latent_density.fit(theta_scores)
+        else:
+            raise ValueError("Invalid approximation method. Choose either 'qmvn' or 'gmm'.")
+
+    def _cv_gaussian_mixture_model(self, data: torch.Tensor, cv_n_components: list[int]) -> GaussianMixtureModel:
+        if len(cv_n_components) > 1:
+            logger.info("Performing cross-validation for Gaussian Mixture Model components...")
+            n_folds = 5
+            average_log_likelihood = torch.zeros(len(cv_n_components))
+            for comp_ind, components in enumerate(cv_n_components):
+                log_likelihoods = torch.zeros(n_folds)
+                data_chunks = data.chunk(n_folds)
+                for i, data_val in enumerate(data_chunks):
+                    train_chunks = [x for j, x in enumerate(data_chunks) if j != i]
+                    data_train = torch.cat(train_chunks, dim=0)
+
+                    gmm = GaussianMixtureModel(n_components=components, n_features=data.shape[1])
+                    gmm.fit(data_train)
+
+                    # Compute the log likelihood on the validation data
+                    log_likelihoods[i] = gmm(data_val)
+
+                # Compute the average log likelihood over the folds
+                average_log_likelihood[comp_ind] = log_likelihoods.mean()
+
+            # Select the number of components that maximizes the average log likelihood
+            optimal_n_components = cv_n_components[average_log_likelihood.argmax()]
+            logger.info("Fitting Gaussian Mixture Model for latent trait density.")
+            gmm = GaussianMixtureModel(n_components=optimal_n_components, n_features=data.shape[1])
+        else:
+            logger.info("Fitting Gaussian Mixture Model for latent trait density.")
+            gmm = GaussianMixtureModel(n_components=cv_n_components[0], n_features=data.shape[1])
+
+        gmm.fit(data)
+        return gmm
 
     @torch.inference_mode()
     def residuals(
         self,
         data: torch.Tensor = None,
-        z: torch.Tensor = None,
-        z_estimation_method: str = "ML",
+        theta: torch.Tensor = None,
+        theta_estimation: str = "ML",
         average_over: str = "none",
     ) -> torch.Tensor:
         """
         Compute model residuals using the supplied data. 
         
         For multiple choice models, the residuals are computed as 1 - the probability of the selected response option.
         For other models, the residuals are computed as the difference between the observed and model expected item scores.
 
         Parameters
         ----------
         data : torch.Tensor
             The input data.
-        z: torch.Tensor, optional
-            The latent variable z scores for the provided data. If not provided, they will be computed using z_estimation_method.
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively.
+        theta: torch.Tensor, optional
+            The latent variable theta scores for the provided data. If not provided, they will be computed using theta_estimation.
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively.
         average_over: str = "none", optional
             Whether to average the residuals and over which level. Can be 'everything', 'items', 'respondents' or 'none'. Use 'none' for no average. For example, with 'respondent' the residuals are averaged over all respondents and is thus an average per item. (default is 'none')
             
         Returns
         -------
         torch.Tensor
             The residuals.
         """
-        data, z = self._evaluate_data_z_input(data, z, z_estimation_method)
+        data, theta = self._evaluate_data_theta_input(data, theta, theta_estimation)
 
         # 3D tensor with dimensions (respondents, items, item categories)
         if self.model.mc_correct is not None:
-            probabilities = self.model.item_probabilities(z)
+            probabilities = self.model.item_probabilities(theta)
             # Creating a range tensor for slice indices
             respndents = torch.arange(probabilities.size(0)).view(-1, 1)
             # Expand slices to match the shape of indices
             expanded_respondents = respndents.expand_as(data)
             model_probs = probabilities[expanded_respondents, torch.arange(probabilities.size(1)), data.int()]
             residuals = 1 - model_probs
         else:
-            residuals = data - self.model.expected_scores(z, return_item_scores=True)
+            residuals = data - self.model.expected_scores(theta, return_item_scores=True)
 
         if average_over == "items":
             return residuals.mean(dim=1)
         if average_over == "respondents":
             return residuals.mean(dim=0)
         if average_over == "everything":
             return residuals.mean(dim=None)
 
         return residuals
 
     @torch.inference_mode()
     def group_fit_residuals(
         self,
         data: torch.Tensor = None,
-        z: torch.Tensor = None,
-        scale: str = "z",
+        theta: torch.Tensor = None,
+        scale: str = "theta",
         latent_variable: int = 1,
         standardize: bool = True,
         groups: int = 10,
-        z_estimation_method: str = "ML",
-        population_z: torch.Tensor = None,
+        theta_estimation: str = "ML",
+        population_theta: torch.Tensor = None,
         **kwargs
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """
         Group the respondents based on their ordered latent variable scores.
         Calculate the residuals between the model estimated and observed data within each group.
         See ch. 20 in Handbook of Item Response Theory, Volume Two: Statistical Tools for more details.
 
         If 'data' is not supplied, the function defaults to using the model's training data.
 
         Parameters
         ----------
         data : torch.Tensor, optional
             A 2D tensor containing test data. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
-        z : torch.Tensor, optional
-            A 2D tensor containing the pre-estimated z scores for each respondent in the data. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
+        theta : torch.Tensor, optional
+            A 2D tensor containing the pre-estimated theta scores for each respondent in the data. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
         scale : str, optional
-            The grouping method scale, which can either be 'bit' or 'z'. Note: for uni-dimensional
-            models, 'z' and 'bit' are equivalent. (default is 'z')
+            The grouping method scale, which can either be 'bit' or 'theta'. Note: for uni-dimensional
+            models, 'theta' and 'bit' are equivalent. (default is 'theta')
         latent_variable: int, optional
             Specifies the latent variable along which ordering and grouping should be performed. (default is 1)
         standardize : bool, optional
             Specifies whether the residuals should be standardized. (default is True)
         groups: int
             The number of groups. (default is 10)
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'NN')
-        population_z : torch.Tensor, optional
-            Only for bit scores. The latent variable z scores for the population. If not provided, they will be computed using z_estimation_method with the model training data. (default is None)
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'NN')
+        population_theta : torch.Tensor, optional
+            Only for bit scores. The latent variable theta scores for the population. If not provided, they will be computed using theta_estimation with the model training data. (default is None)
         **kwargs : dict, optional
-            Additional keyword arguments to be passed to the bit_scores_from_z method if scale is 'bit'. See :meth:`bit_scores_from_z` for details.
+            Additional keyword arguments to be passed to the bit_scores_from_theta method if scale is 'bit'. See :meth:`bit_scores_from_theta` for details.
             
         Returns
         -------
         tuple[torch.Tensor, torch.Tensor]
             A tuple with torch tensors. The first one holds the residuals for each group and has dimensions (groups, items, item categories). The second one is a 1D tensor and holds the mid points of the groups.
         """
         grouped_data_probabilties, grouped_model_probabilties, group_mid_points = \
             self.latent_group_probabilities(
                 data=data,
-                z=z,
+                theta=theta,
                 scale=scale,
                 latent_variable=latent_variable,
                 groups=groups,
-                z_estimation_method=z_estimation_method,
-                population_z=population_z,
+                theta_estimation=theta_estimation,
+                population_theta=population_theta,
                 **kwargs
             )
 
         raw_residuals = grouped_data_probabilties - grouped_model_probabilties
         if standardize:
             # get number of people in each group
             data = torch.chunk(data, groups)
@@ -198,40 +271,40 @@
 
         return raw_residuals, group_mid_points
     
     @torch.inference_mode()
     def accuracy(
         self,
         data: torch.Tensor = None,
-        z: torch.Tensor = None,
-        z_estimation_method: str = "ML",
+        theta: torch.Tensor = None,
+        theta_estimation: str = "ML",
         level: str = "all",
     ):
         """
         Calculate the prediction accuracy of the model for the supplied data.
 
         Parameters
         ----------
         data : torch.Tensor
             The input data.
-        z: torch.Tensor, optional
-            The latent variable z scores for the provided data. If not provided, they will be computed using z_estimation_method.
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively.
+        theta: torch.Tensor, optional
+            The latent variable theta scores for the provided data. If not provided, they will be computed using theta_estimation.
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively.
         level: str = "all", optional
             Specifies the level at which the accuracy is calculated. Can be 'all', 'item' or 'respondent'. For example, for 'item' the accuracy is calculated for each item. (default is 'all')
 
         Returns
         -------
         torch.Tensor
             The accuracy.
         """
-        data, z = self._evaluate_data_z_input(data, z, z_estimation_method)
+        data, theta = self._evaluate_data_theta_input(data, theta, theta_estimation)
 
-        probabilities = self.model.item_probabilities(z)
+        probabilities = self.model.item_probabilities(theta)
         accuracy = (torch.argmax(probabilities, dim=2) == data).float()
 
         if level == "item":
             dim = 0
         elif level == "respondent":
             dim = 1
         else:
@@ -239,31 +312,31 @@
         
         return accuracy.mean(dim=dim)
 
     @torch.inference_mode()
     def infit_outfit(
         self,
         data: torch.Tensor = None,
-        z: torch.Tensor = None,
-        z_estimation_method: str = "ML",
+        theta: torch.Tensor = None,
+        theta_estimation: str = "ML",
         level: str = "item",
     ):
         """
         Calculate person or item infit and outfit statistics. These statistics help identifying items that do not behave as expected according to the model
         or respondents with unusual response patterns. Items that do not behave as expectedly can be reviewed for possible revision or removal 
         to improve the overall test quality and reliability. Respondents with unusual response patterns can be reviewed for possible cheating or other issues.
 
         Parameters
         ----------
         data : torch.Tensor
             The input data.
-        z: torch.Tensor, optional
-            The latent variable z scores for the provided data. If not provided, they will be computed using z_estimation_method.
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively.
+        theta: torch.Tensor, optional
+            The latent variable theta scores for the provided data. If not provided, they will be computed using theta_estimation.
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively.
         level: str = "item", optional
             Specifies whether to compute item or respondent statistics. Can be 'item' or 'respondent'. (default is 'item')
 
         Returns
         -------
         torch.Tensor
             The infit statistics.
@@ -288,18 +361,18 @@
         - :math:`E_{ij}` is the expected score on the :math:`j`-th item from the :math:`i`-th respondent, calculated from the IRT model.
         - :math:`W_{ij}` is the weight on the :math:`j`-th item from the :math:`j`-th respondent. This is the variance of the item score :math:`W_{ij}=\\sum^{M_j}_{m=0}(m-E_{ij})^2P_{ijk}` where :math:`M_j` is the maximum item score and :math:`P_{ijk}` is the model probability of a score :math:`k` on the :math:`j`-th item from the :math:`i`-th respondent.
         
         """
         if level not in ["item", "respondent"]:
             raise ValueError("Invalid level. Choose either 'item' or 'respondent'.")
 
-        data, z = self._evaluate_data_z_input(data, z, z_estimation_method)
+        data, theta = self._evaluate_data_theta_input(data, theta, theta_estimation)
 
-        expected_scores = self.model.expected_scores(z, return_item_scores=True)
-        probabilities = self.model.item_probabilities(z)
+        expected_scores = self.model.expected_scores(theta, return_item_scores=True)
+        probabilities = self.model.item_probabilities(theta)
         observed_scores = data
         if self.model.mc_correct is not None:
             score_indices = torch.zeros(probabilities.shape[1], probabilities.shape[2])
             score_indices.scatter_(1, (torch.tensor(self.model.mc_correct) - 1 + self.model.model_missing).unsqueeze(1), 1)
             score_indices = score_indices.unsqueeze(0).expand(probabilities.shape[0], -1, -1)
             correct_probabilities = (probabilities*score_indices.int()).sum(dim=2)
             variance = correct_probabilities * (1-correct_probabilities)
@@ -323,261 +396,216 @@
         
         return infit, outfit
 
     @torch.inference_mode()
     def log_likelihood(
         self,
         data: torch.Tensor = None,
-        z: torch.Tensor = None,
-        z_estimation_method: str = "ML",
+        theta: torch.Tensor = None,
+        theta_estimation: str = "ML",
         reduction: str = "sum",
         level: str = "all",
     ):
         """
         Calculate the log-likelihood for the provided data.
 
         If 'data' is not supplied, the function defaults to using the model's training data.
 
         Parameters
         ----------
         data : torch.Tensor, optional
             A 2D tensor containing test data. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
-        z : torch.Tensor, optional
-            A 2D tensor containing latent variable z scores. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'NN')
+        theta : torch.Tensor, optional
+            A 2D tensor containing latent variable theta scores. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'NN')
         reduction : str, optional
             Specifies the reduction method for the log-likelihood. Can be 'sum', 'none' or 'mean'. (default is 'sum')
         level : str, optional
             For reductions other than 'none', specifies the level at which the log-likelihood is summed/averaged. Can be 'all', 'item' or 'respondent'. For example, for 'item' the log-likelihood is summed/averaged for each item. (default is 'all')
             
         Returns
         -------
         torch.Tensor
             The log-likelihood for the provided data.
         """
-        data, z = self._evaluate_data_z_input(data, z, z_estimation_method)
+        data, theta = self._evaluate_data_theta_input(data, theta, theta_estimation)
 
         if reduction != "none":
             if level == "item":
                 dim = 0
             elif level == "respondent":
                 dim = 1
             else:
                 dim = None
 
         likelihoods = self.model.log_likelihood(
             data,
-            self.model(z),
+            self.model(theta),
             loss_reduction="none"
         )
         
         if reduction in "mean":
-            return likelihoods.view(z.shape[0], -1).mean(dim=dim)
+            return likelihoods.view(theta.shape[0], -1).mean(dim=dim)
         if reduction == "sum":
-            return likelihoods.view(z.shape[0], -1).sum(dim=dim)
+            return likelihoods.view(theta.shape[0], -1).sum(dim=dim)
         
         return likelihoods
 
     @torch.inference_mode()
     def group_fit_log_likelihood(
         self,
         data: torch.Tensor = None,
-        z: torch.Tensor = None,
-        z_estimation_method: str = "ML",
+        theta: torch.Tensor = None,
+        theta_estimation: str = "ML",
         groups: int = 10,
         latent_variable: int = 1,
     ):
         """
         Group the respondents based on their ordered latent variable scores.
         Calculate the average log-likelihood of the data within each group.
 
         If 'data' is not supplied, the function defaults to using the model's training data.
 
         Parameters
         ----------
         data : torch.Tensor, optional
             A 2D tensor containing test data. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
-        z : torch.Tensor, optional
-            A 2D tensor containing the pre-estimated z scores for each respondent in the data. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'NN')
+        theta : torch.Tensor, optional
+            A 2D tensor containing the pre-estimated theta scores for each respondent in the data. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'NN')
         groups: int
             The number of groups. (default is 10)
         latent_variable: int, optional
             Specifies the latent variable along which ordering and grouping should be performed. (default is 1)
 
         Returns
         -------
         torch.Tensor
             The average log-likelihood for each group.
         """
-        data, z = self._evaluate_data_z_input(data, z, z_estimation_method)
+        data, theta = self._evaluate_data_theta_input(data, theta, theta_estimation)
 
-        indicies = torch.sort(z[:, latent_variable - 1], dim=0)[1]
-        z = z[indicies]
+        indicies = torch.sort(theta[:, latent_variable - 1], dim=0)[1]
+        theta = theta[indicies]
         data = data[indicies]
         likelihoods = self.model.log_likelihood(
             data,
-            self.model(z),
+            self.model(theta),
             loss_reduction="none"
         )
-        respondent_likelihoods = likelihoods.view(z.shape[0], -1).sum(dim=1)
+        respondent_likelihoods = likelihoods.view(theta.shape[0], -1).sum(dim=1)
         group_mean_likelihoods = torch.zeros(groups)
         start_index = 0
         for group in range(groups):
             group_size = respondent_likelihoods.shape[0] // groups
             remainder = len(respondent_likelihoods) % groups
             if group < remainder:
                 group_size += 1
             group_mean_likelihoods[group] = respondent_likelihoods[start_index: start_index + group_size].mean()
             start_index += group_size
             
         return group_mean_likelihoods
-
+    
     def latent_group_probabilities(
         self,
         data: torch.Tensor = None,
-        z: torch.Tensor = None,
-        scale: str = "z",
+        theta: torch.Tensor = None,
+        scale: str = "theta",
         latent_variable: int = 1,
         groups: int = 10,
-        z_estimation_method: str = "ML",
-        population_z: torch.Tensor = None,
+        theta_estimation: str = "ML",
+        population_theta: torch.Tensor = None,
         **kwargs
     ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         Group the respondents based on their ordered latent variable scores.
         Calculate both the observed and IRT model probabilities for each possible item response, within each group.
 
         If 'data' is not supplied, the function defaults to using the model's training data.
 
         Parameters
         ----------
         data : torch.Tensor, optional
-        z : torch.Tensor, optional
-            The latent variable z scores for the provided data. If not provided, they will be computed using z_estimation_method. (default is None)
+        theta : torch.Tensor, optional
+            The latent variable theta scores for the provided data. If not provided, they will be computed using theta_estimation. (default is None)
         scale : str, optional
-            The grouping method scale, which can either be 'bit' or 'z'. Note: for uni-dimensional
-            models, 'z' and 'bit' are equivalent. (default is 'z')
+            The grouping method scale, which can either be 'bit' or 'theta'. Note: for uni-dimensional
+            models, 'theta' and 'bit' are equivalent. (default is 'theta')
         latent_variable: int, optional
             Specifies the latent variable along which ordering and grouping should be performed. (default is 1)
         groups: int
             The number of groups. (default is 10)
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'NN')
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'NN')
             A 2D tensor containing test data. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
-        population_z : torch.Tensor, optional
-            Only for bit scores. The latent variable z scores for the population. If not provided, they will be computed using z_estimation_method with the model training data. (default is None)
+        population_theta : torch.Tensor, optional
+            Only for bit scores. The latent variable theta scores for the population. If not provided, they will be computed using theta_estimation with the model training data. (default is None)
         **kwargs : dict, optional
-            Additional keyword arguments to be passed to the latent_scores method if scores_to_plot is not provided. See :meth:`latent_scores` for details.
+            Additional keyword arguments to be passed to the bit_scores_from_theta method.
 
         Returns
         -------
         tuple[torch.Tensor, torch.Tensor, torch.Tensor]
             A 3D torch tensor with data group averages. The first dimension represents the groups, the second dimension represents the items and the third dimension represents the item categories.
 
             A 3D torch tensor with model group averages. The first dimension represents the groups, the second dimension represents the items and the third dimension represents the item categories.
 
             The third tensor contains the average latent variable values within each group along the specified latent_variable.
         """
 
-        if scale not in ["bit", "z"]:
-            raise ValueError("Invalid scale. Choose either 'z' or 'bit'.")
+        if scale not in ["bit", "theta"]:
+            raise ValueError("Invalid scale. Choose either 'theta' or 'bit'.")
 
-        data, z = self._evaluate_data_z_input(data, z, z_estimation_method)
+        data, theta = self._evaluate_data_theta_input(data, theta, theta_estimation)
 
         if scale == "bit":
-            if population_z is None and data is self.algorithm.train_data:
-                population_z = z
+            if population_theta is None and data is self.model.algorithm.train_data:
+                population_theta = theta
             
-            bit_scores, _ = self.scorer.bit_scores_from_z(
-                z=z,
+            bit_scores, _ = self.model.bit_scales.bit_scores_from_theta(
+                theta=theta,
                 one_dimensional=False,
-                z_estimation_method=z_estimation_method,
+                theta_estimation=theta_estimation,
                 **kwargs
             )
 
             # Sort based on correct column and get the sorted indices
             _, indices = torch.sort(
                 bit_scores[:, latent_variable - 1], dim=0
             )
             # Use the indices to sort
             bit_scores = bit_scores[indices]
-            z = z[indices]
+            theta = theta[indices]
 
             grouped_bit = torch.chunk(bit_scores, groups)
-            grouped_z = torch.chunk(z, groups)
+            grouped_theta = torch.chunk(theta, groups)
 
             group_mid_points = torch.tensor(
                 [
                     group[:, latent_variable - 1].mean()
                     for group in grouped_bit
                 ]
             )
-        elif scale == "z":
-            _, indices = torch.sort(z[:, latent_variable - 1], dim=0)
-            z = z[indices]
-            grouped_z = torch.chunk(z, groups)
+        elif scale == "theta":
+            _, indices = torch.sort(theta[:, latent_variable - 1], dim=0)
+            theta = theta[indices]
+            grouped_theta = torch.chunk(theta, groups)
             group_mid_points = torch.tensor(
-                [group[:, latent_variable - 1].median() for group in grouped_z]
+                [group[:, latent_variable - 1].median() for group in grouped_theta]
             )
 
         data = data[indices]
         grouped_data = torch.chunk(data, groups)
         grouped_data_probabilties = self._grouped_data_probabilities(grouped_data)
-        grouped_model_probabilties = self._grouped_z_probabilities(grouped_z)
+        grouped_model_probabilties = self._grouped_theta_probabilities(grouped_theta)
         return grouped_data_probabilties, grouped_model_probabilties, group_mid_points
 
     @torch.inference_mode()
-    def _grouped_z_probabilities(self, grouped_z: tuple[torch.Tensor, ...]):
-        """
-        Computes the average probabilities for each potential item response for each group.
-
-        Parameters
-        ----------
-        grouped_z : tuple[torch.Tensor, ...]
-            A tuple containing 2D tensors. Each tensor represents a group of respondents, with the first dimension corresponding to the respondents and the second dimension representing their latent variables in the form of z-scores.
-
-        Returns
-        -------
-        torch.Tensor
-            A 3D torch tensor with group averages. The first dimension represents the groups, the second dimension represents the items and the third dimension represents the item categories.
-        """
-        group_probabilities = torch.zeros(len(grouped_z), len(self.model.modeled_item_responses), max(self.model.modeled_item_responses))
-        for group_i, group in enumerate(grouped_z):
-            item_probabilities = self.model.item_probabilities(group)
-            group_probabilities[group_i, :, :] = item_probabilities.mean(dim=0)
-        return group_probabilities
-
-    @torch.inference_mode()
-    def _grouped_data_probabilities(self, grouped_data: tuple[torch.Tensor, ...]):
-        """
-        Computes the average probabilities for each potential item response for each group.
-
-        Parameters
-        ----------
-        grouped_data : tuple[torch.Tensor, ...]
-            A tuple containing 2D tensors. Each tensor represents a group of respondents, with the first dimension representing the respondents and the second dimension representing items.
-
-        Returns
-        -------
-        torch.Tensor
-            A 3D torch tensor with group averages. The first dimension represents the groups, the second dimension represents the items and the third dimension represents the item categories.
-        """
-        modeled_item_responses = self.model.modeled_item_responses
-        group_probabilities = torch.zeros(len(grouped_data), len(modeled_item_responses), max(modeled_item_responses))
-        for group_i, group in enumerate(grouped_data):
-            for item_i, _ in enumerate(modeled_item_responses):
-                counts = torch.bincount(group[:, item_i].int(), minlength=max(modeled_item_responses))
-                group_probabilities[group_i, item_i, :] = counts.float() / counts.sum()
-
-        return group_probabilities
-
-    @torch.inference_mode()
     def sum_score_probabilities(
         self,
         latent_density_method: str = "data",
         population_data: torch.Tensor = None,
         trapezoidal_segments: int = 1000,
         sample_size: int = 100000,
     ):
@@ -585,34 +613,34 @@
         Computes the marginal probabilities for each sum score, averged over the latent space density. For 'qmvn' and 'gmm' densities, the trapezoidal rule is used for integral approximation.
 
         Parameters
         ----------
         latent_density_method : str, optional
             Specifies the method used to approximate the latent space density.
             Possible options are
-            - 'data' averages over the z scores from the population data.
-            - 'encoder sampling' samples z scores from the encoder. Only available for VariationalAutoencoderIRT models
+            - 'data' averages over the theta scores from the population data.
+            - 'encoder sampling' samples theta scores from the encoder. Only available for VariationalAutoencoderIRT models
             - 'qmvn' for quantile multivariate normal approximation of a multivariate joint density function (QuantileMVNormal class).
             - 'gmm' for a gaussian mixture model.
         population_data : torch.Tensor, optional
             The population data used for approximating sum score probabilities. Default is None and uses the training data.
         trapezoidal_segments : int, optional
-            The number of integration approximation intervals for each z dimension. (Default is 1000)
+            The number of integration approximation intervals for each theta dimension. (Default is 1000)
         sample_size : int, optional
             Sample size for the 'encoder sampling' method. (Default is 100000)
         Returns
         -------
         torch.Tensor
             A 1D tensor with the probability for each total score.
         """
         self._validate_latent_density_method(latent_density_method)
-        z_scores, weights = self._get_z_scores_and_weights(
+        theta_scores, weights = self._get_theta_scores_and_weights(
             latent_density_method, population_data, trapezoidal_segments, sample_size
         )
-        probabilities = self.model.item_probabilities(z_scores)
+        probabilities = self.model.item_probabilities(theta_scores)
         # sum incorrect response option probabilities if MC
         if self.model.mc_correct is not None:
             probabilities = sum_incorrect_probabilities(
                 probabilities=probabilities,
                 modeled_item_responses=self.model.modeled_item_responses,
                 mc_correct=self.model.mc_correct,
                 missing_modeled=self.model.model_missing
@@ -627,97 +655,182 @@
         
         conditional_total_score_probs = conditional_score_distribution(
             probabilities, item_categories
         )
         sum_score_probabilities = conditional_total_score_probs * weights.view(-1, 1)
         return sum_score_probabilities.sum(dim=0)
 
+    @torch.inference_mode()
+    def _min_max_theta_for_integration(
+        self,
+        theta: torch.Tensor = None,
+    ) -> tuple[torch.Tensor, torch.Tensor]:
+        """
+        Retrieve the minimum and maximum theta score for approximating integrals over the latent space. Uses one standard deviation below/above the min/max of each theta score vector.
+
+        Parameters
+        ----------
+        theta : torch.Tensor, optional
+            A 2D tensor. Columns are each latent variable, rows are respondents. Default is None and uses training data theta scores.
+
+        Returns
+        -------
+        tuple[torch.Tensor, torch.Tensor]
+            A tuple with 1D tensors, containing the min and max integration theta scores of each latent variable.
+        """
+        if theta is None:
+            if isinstance(self.model.algorithm, (AE, VAE)):
+                theta = self.model.algorithm.training_theta_scores
+                theta_min = theta.min(dim=0)[0]
+                theta_max = theta.max(dim=0)[0]
+                theta_stds = theta.std(dim=0)
+            elif isinstance(self.model.algorithm, MML):
+                theta_min = torch.full((self.model.latent_variables,), -3)
+                theta_max = torch.full((self.model.latent_variables,), 3)
+                theta_stds = torch.ones(self.model.latent_variables)
+        else:
+            theta_min = theta.min(dim=0)[0]
+            theta_max = theta.max(dim=0)[0]
+            theta_stds = theta.std(dim=0)
+
+        return theta_min - theta_stds, theta_max + theta_stds
+
+    @torch.inference_mode()
+    def _grouped_theta_probabilities(self, grouped_theta: tuple[torch.Tensor, ...]):
+        """
+        Computes the average probabilities for each potential item response for each group.
+
+        Parameters
+        ----------
+        grouped_theta : tuple[torch.Tensor, ...]
+            A tuple containing 2D tensors. Each tensor represents a group of respondents, with the first dimension corresponding to the respondents and the second dimension representing their latent variables in the form of theta-scores.
+
+        Returns
+        -------
+        torch.Tensor
+            A 3D torch tensor with group averages. The first dimension represents the groups, the second dimension represents the items and the third dimension represents the item categories.
+        """
+        group_probabilities = torch.zeros(len(grouped_theta), len(self.model.modeled_item_responses), max(self.model.modeled_item_responses))
+        for group_i, group in enumerate(grouped_theta):
+            item_probabilities = self.model.item_probabilities(group)
+            group_probabilities[group_i, :, :] = item_probabilities.mean(dim=0)
+        return group_probabilities
+
+    @torch.inference_mode()
+    def _grouped_data_probabilities(self, grouped_data: tuple[torch.Tensor, ...]):
+        """
+        Computes the average probabilities for each potential item response for each group.
+
+        Parameters
+        ----------
+        grouped_data : tuple[torch.Tensor, ...]
+            A tuple containing 2D tensors. Each tensor represents a group of respondents, with the first dimension representing the respondents and the second dimension representing items.
+
+        Returns
+        -------
+        torch.Tensor
+            A 3D torch tensor with group averages. The first dimension represents the groups, the second dimension represents the items and the third dimension represents the item categories.
+        """
+        modeled_item_responses = self.model.modeled_item_responses
+        group_probabilities = torch.zeros(len(grouped_data), len(modeled_item_responses), max(modeled_item_responses))
+        for group_i, group in enumerate(grouped_data):
+            for item_i, _ in enumerate(modeled_item_responses):
+                counts = torch.bincount(group[:, item_i].int(), minlength=max(modeled_item_responses))
+                group_probabilities[group_i, item_i, :] = counts.float() / counts.sum()
+
+        return group_probabilities
+
     def _validate_latent_density_method(self, latent_density_method: str) -> None:
         valid_methods = ["data", "encoder sampling", "qmvn", "gmm"]
         if latent_density_method not in valid_methods:
             raise ValueError(
                 f"Invalid latent density method. Must be one of {valid_methods}."
             )
         if latent_density_method == "encoder sampling" and not isinstance(
-            self.algorithm, VAEIRT
+            self.model.algorithm, VAE
         ):
             raise ValueError(
                 "Encoder sampling is only available for variational autoencoder models."
             )
 
-    def _get_z_scores_and_weights(
+    def _get_theta_scores_and_weights(
         self,
         latent_density_method: str,
         population_data: torch.Tensor,
         trapezoidal_segments: int,
         sample_size: int,
         ml_map_device: str = "cuda" if torch.cuda.is_available() else "cpu",
         lbfgs_learning_rate: float = 0.3,
     ):
         if population_data is None:
-            z_scores = self.algorithm.training_z_scores
+            if isinstance(self.model.algorithm, (AE, VAE)):
+                theta_scores = self.model.algorithm.training_theta_scores
+            elif isinstance(self.model.algorithm, MML):
+                logger.info("Sampling from multivariate normal as population theta scores.")
+                mvn = MultivariateNormal(torch.zeros(self.model.latent_variables), self.model.algorithm.covariance_matrix)
+                theta_scores = mvn.sample((4000,)).to(dtype=torch.float32)
         else:
-            z_scores = self.scorer.latent_scores(population_data, scale="z", z_estimation_method="NN", ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
+            theta_scores = self.model.latent_scores(population_data, theta_estimation="NN", ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
 
         if latent_density_method in ["data", "encoder sampling"]:
             weights = (
-                torch.ones(z_scores.shape[0])
-                / z_scores.shape[0]
+                torch.ones(theta_scores.shape[0])
+                / theta_scores.shape[0]
             )
             if latent_density_method == "encoder sampling":
-                z_scores = self.algorithm.sample_latent_variables(
+                theta_scores = self.model.algorithm.sample_latent_variables(
                     sample_size=sample_size, input_data=population_data
                 )
         else:
             (
-                z_scores,
+                theta_scores,
                 weights,
-            ) = self._get_z_scores_and_weights_for_latent_density_methods(
-                latent_density_method, z_scores, population_data, trapezoidal_segments
+            ) = self._get_theta_scores_and_weights_for_latent_density_methods(
+                latent_density_method, theta_scores, population_data, trapezoidal_segments
             )
 
-        return z_scores, weights
+        return theta_scores, weights
 
-    def _get_z_scores_and_weights_for_latent_density_methods(
+    def _get_theta_scores_and_weights_for_latent_density_methods(
         self,
         latent_density_method: str,
-        z_scores: torch.Tensor,
+        theta_scores: torch.Tensor,
         population_data: torch.Tensor,
         trapezoidal_segments: int,
     ):
         # We approximate the density if
         # population_data is not none and the correct density
-        # is not already in self.scorer.latent_density
+        # is not already in self.model.evaluation.latent_density
         if population_data is not None or (
             (
                 latent_density_method != "qmvn"
-                or not isinstance(self.scorer.latent_density, QuantileMVNormal)
+                or not isinstance(self.latent_density, QuantileMVNormal)
             )
             and (
                 latent_density_method != "gmm"
-                or not isinstance(self.scorer.latent_density, GaussianMixtureModel)
+                or not isinstance(self.latent_density, GaussianMixtureModel)
             )
         ):
-            self.scorer.approximate_latent_density(
-                z_scores=z_scores, approximation=latent_density_method
+            self.approximate_latent_density(
+                theta_scores=theta_scores, approximation=latent_density_method
             )
 
         # get the min/max points for integration
-        min_z, max_z = self.scorer.min_max_z_for_integration(z_scores)
+        min_theta, max_theta = self._min_max_theta_for_integration(theta_scores)
 
         # Create a list of linspace tensors for each dimension
         lin_spaces = [
-            torch.linspace(min_z[i], max_z[i], trapezoidal_segments)
-            for i in range(len(min_z))
+            torch.linspace(min_theta[i], max_theta[i], trapezoidal_segments)
+            for i in range(len(min_theta))
         ]
 
         # Use torch.cartesian_prod to generate all combinations
-        z_scores = torch.cartesian_prod(*lin_spaces)
+        theta_scores = torch.cartesian_prod(*lin_spaces)
 
-        if z_scores.dim() == 1:
+        if theta_scores.dim() == 1:
             # Add an extra dimension for 1D models to make it a 2D tensor with 1 column
-            z_scores = z_scores.unsqueeze(1)
+            theta_scores = theta_scores.unsqueeze(1)
 
-        weights = self.scorer.latent_density.pdf(z_scores)
+        weights = self.latent_density.pdf(theta_scores)
         weights = weights / weights.sum()
 
-        return z_scores, weights
+        return theta_scores, weights
```

### Comparing `irtorch-0.0.4/irtorch/irt_plotter.py` & `irtorch-0.1.0/irtorch/plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,83 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING
 import logging
 import torch
 import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 import plotly.express as px
 import plotly.io as pio
-from irtorch.models import BaseIRTModel
-from irtorch.estimation_algorithms import BaseIRTAlgorithm
-from irtorch.irt_scorer import IRTScorer
-from irtorch.irt_evaluator import IRTEvaluator
+from irtorch.estimation_algorithms import AE, VAE, MML
 from irtorch._internal_utils import output_to_item_entropy
 
+if TYPE_CHECKING:
+    from irtorch.models.base_irt_model import BaseIRTModel
+
 pio.templates.default = "plotly_white"
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
-class IRTPlotter:
+class Plotting:
     """
-    Initializes the IRTPlotter class with a given model, fitting algorithm, scorer and evaluator.
+    Plotting class for IRT models.
 
     Parameters
     ----------
     model : BaseIRTModel
-        BaseIRTModel object.
-    algorithm : BaseIRTAlgorithm
-        BaseIRTAlgorithm object.
-    scorer : IRTScorer
-        IRTScorer object used to obtain latent variable scores.
-    evaluator : IRTEvaluator
-        IRTEvaluator object used to obtain evaluation measures.
+        The IRT model to use for plotting.
     """
     def __init__(
-        self, model: BaseIRTModel, algorithm: BaseIRTAlgorithm, scorer: IRTScorer, evaluator: IRTEvaluator
+        self, model: BaseIRTModel
     ):
         self.model = model
-        self.algorithm = algorithm
-        self.scorer = scorer
-        self.evaluator = evaluator
         self.linewidth = 2.5
         self.markersize = 9
         self.color_map = "tab10"
 
 
     def plot_training_history(self) -> go.Figure:
         """
         Plots the training history of the model.
 
         Returns
         -------
         go.Figure
             The Plotly Figure object for the plot.
         """
-        if all(len(val) == 0 for val in self.algorithm.training_history.values()):
+        if all(len(val) == 0 for val in self.model.algorithm.training_history.values()):
             logging.error("Model has not been trained yet")
             raise AttributeError("Model has not been trained yet")
 
         data_frames = []
 
-        if 'train_loss' in self.algorithm.training_history and len(self.algorithm.training_history['train_loss']) > 0:
+        if "train_loss" in self.model.algorithm.training_history and len(self.model.algorithm.training_history["train_loss"]) > 0:
             train_df = pd.DataFrame({
-                'Epoch': range(1, len(self.algorithm.training_history['train_loss']) + 1),
-                'Loss': self.algorithm.training_history['train_loss'],
-                'Type': 'Training'
+                "Epoch": range(1, len(self.model.algorithm.training_history["train_loss"]) + 1),
+                "Loss": self.model.algorithm.training_history["train_loss"],
+                "Type": "Training"
             })
             data_frames.append(train_df)
 
-        if 'validation_loss' in self.algorithm.training_history and len(self.algorithm.training_history['validation_loss']) > 0:
+        if "validation_loss" in self.model.algorithm.training_history and len(self.model.algorithm.training_history["validation_loss"]) > 0:
             validation_df = pd.DataFrame({
-                'Epoch': range(1, len(self.algorithm.training_history['validation_loss']) + 1),
-                'Loss': self.algorithm.training_history['validation_loss'],
-                'Type': 'Validation'
+                "Epoch": range(1, len(self.model.algorithm.training_history["validation_loss"]) + 1),
+                "Loss": self.model.algorithm.training_history["validation_loss"],
+                "Type": "Validation"
             })
             data_frames.append(validation_df)
 
         if not data_frames:
             raise ValueError("No training or validation loss data available for plotting.")
 
         plot_df = pd.concat(data_frames)
 
         fig = px.line(
-            plot_df, x='Epoch', y='Loss', color='Type',
-            labels={'Loss': 'Loss', 'Epoch': 'Epoch'},
-            title='Training History')
+            plot_df, x="Epoch", y="Loss", color="Type",
+            labels={"Loss": "Loss", "Epoch": "Epoch"},
+            title="Training History")
 
         return fig
 
     @torch.inference_mode()
     def plot_latent_score_distribution(
         self,
         scores_to_plot: torch.Tensor = None,
@@ -106,18 +99,18 @@
         ----------
         scores_to_plot : torch.Tensor, optional
             If provided, the requested latent variable distributions are plotted directly.
             If None, scores are computed from the population data or the model training data. (default is None)
         population_data : torch.Tensor, optional
             The data used to compute the latent scores. If None, uses the training data. (default is None)
         scale : str, optional
-            The scale to plot against. Can be 'bit' or 'z'. (default is 'bit')
+            The scale to plot against. Can be 'bit' or 'theta'. (default is 'bit')
         latent_variables_to_plot : tuple[int], optional
             The latent dimensions to include in the plot. (default is (1,))
-                title : str, optional
+        title : str, optional
             The title for the plot. (default is None)
         x_label : str, optional
             The label for the X-axis. (default is None and uses "Latent variable" for one latent variable and "Latent variable 1" for two latent variables)
         y_label : str, optional
             The label for the Y-axis. (default is None and uses "Density" for one latent variable and "Latent variable 2" for two latent variables)
         color : str, optional
             The color to use for plots with one latent variable. (default is None and uses the default color sequence for the plotly_white template)
@@ -144,23 +137,27 @@
             raise ValueError(
                 f"Cannot plot latent variable {latent_variables_to_plot}. "
                 f"Fitted model is a {self.model.latent_variables} dimensional model."
             )
 
         if scores_to_plot is None:
             if population_data is None:
-                population_data = self.algorithm.train_data
+                population_data = self.model.algorithm.train_data
             else:
                 population_data = population_data.contiguous()
 
-            scores = self.scorer.latent_scores(
+            scores = self.model.latent_scores(
                 data=population_data,
-                scale=scale,
                 **kwargs
             )
+            if scale == "bit":
+                scores = self.model.bit_scales.bit_scores_from_theta(
+                    theta=scores,
+                    **kwargs
+                )[0]
         else:
             scores = scores_to_plot
 
         return self._distribution_plot(
             latent_scores=scores[:, [i - 1 for i in latent_variables_to_plot]],
             title=title,
             x_label=x_label,
@@ -176,94 +173,94 @@
         scale: str = "bit",
         latent_variables: tuple[int] = (1,),
         title: str = None,
         x_label: str = None,
         y_label: str = None,
         color: str = None,
         colorscale: str = "Plasma",
-        z_range: tuple[float, float] = None,
-        second_z_range: tuple[float, float] = None,
+        theta_range: tuple[float, float] = None,
+        second_theta_range: tuple[float, float] = None,
         steps: int = None,
-        fixed_zs: torch.Tensor = None,
+        fixed_thetas: torch.Tensor = None,
         **kwargs
     ) -> go.Figure:
         """
         Plot the entropy of an item against the latent variable(s).
 
         Parameters
         ----------
         item : int
             The item for which to plot the entropy.
         scale : str, optional
-            The scale to plot against. Can be 'bit' or 'z'. (default is 'bit')
+            The scale to plot against. Can be 'bit' or 'theta'. (default is 'bit')
         latent_variables : tuple[int], optional
             The latent variables to plot. (default is (1,))
         title : str, optional
             The title for the plot. (default is None and prints "Item {item} entropy")
         x_label : str, optional
             The label for the X-axis. (default is None and uses "Latent variable" for one latent variable and "Latent variable 1" for two latent variables)
         y_label : str, optional
             The label for the Y-axis. (default is None and uses 'Entropy' for one latent variable, and "Latent variable 2" for two latent variables)
         color : str, optional
             The color to use for plots with one latent variable. (default is None and uses the default color sequence for the plotly_white template)
         colorscale : str, optional
             Sets the colorscale for the multiple latent variable surface plots. See https://plotly.com/python/builtin-colorscales/ (default is "Plasma")
-        z_range : tuple[float, float], optional
-            Only for scale = 'z'. The z range for plotting. (default is None and uses limits based on training data)
-        second_z_range : tuple[float, float], optional
-            Only for scale = 'z'. The range for plotting for the second latent variable. (default is None and uses limits based on training data)
+        theta_range : tuple[float, float], optional
+            Only for scale = 'theta'. The theta range for plotting. (default is None and uses limits based on training data)
+        second_theta_range : tuple[float, float], optional
+            Only for scale = 'theta'. The range for plotting for the second latent variable. (default is None and uses limits based on training data)
         steps : int, optional
-            The number of steps along each z axis to construct the latent variable grid for which the sum score is evaluated at. (default is None and uses 100 for one latent variable and 18 for two latent variables)
-        fixed_zs: torch.Tensor, optional
+            The number of steps along each theta axis to construct the latent variable grid for which the sum score is evaluated at. (default is None and uses 100 for one latent variable and 18 for two latent variables)
+        fixed_thetas: torch.Tensor, optional
             Only for multdimensional models. Fixed values for latent space variable not plotted. (default is None and uses the medians in the training data)
         **kwargs : dict, optional
-            Additional keyword arguments used for bit score computation. See :meth:`irtorch.irt.IRT.bit_scores_from_z` for details. 
+            Additional keyword arguments used for bit score computation. See :meth:`irtorch.irt.IRT.bit_scores_from_theta` for details. 
 
         Returns
         -------
         go.Figure
             The Plotly Figure object for the plot.
         """
         model_dim = self.model.latent_variables
         if len(latent_variables) > 2:
             raise TypeError("Cannot plot more than two latent variables in one plot.")
         if len(latent_variables) > model_dim:
             raise TypeError(f"Cannot plot {len(latent_variables)} latent variables with a {model_dim}-dimensional model.")
         if not all(num <= model_dim for num in latent_variables):
             raise TypeError(f"The latent variables to plot need to be smaller than or equal to {model_dim} (the number of variabels in the model).")
-        if z_range is not None and len(z_range) != 2:
-            raise TypeError("z_range needs to have a length of 2.")
-        if len(latent_variables) == 1 and second_z_range is not None and len(second_z_range) != 2:
-            raise TypeError("second_z_range needs to have a length of 2 if specified.")
+        if theta_range is not None and len(theta_range) != 2:
+            raise TypeError("theta_range needs to have a length of 2.")
+        if len(latent_variables) == 1 and second_theta_range is not None and len(second_theta_range) != 2:
+            raise TypeError("second_theta_range needs to have a length of 2 if specified.")
         if steps is None:
             steps = 100 if len(latent_variables) == 1 else 18
 
-        latent_indices = [z - 1 for z in latent_variables]
+        latent_indices = [theta - 1 for theta in latent_variables]
 
-        z_grid = self._get_z_grid_for_plotting(latent_variables, z_range, second_z_range, steps, fixed_zs, latent_indices)
+        theta_grid = self._get_theta_grid_for_plotting(latent_variables, theta_range, second_theta_range, steps, fixed_thetas, latent_indices)
         
-        mean_output = self.model(z_grid)
+        mean_output = self.model(theta_grid)
         item_entropies = output_to_item_entropy(
             mean_output, self.model.modeled_item_responses
         )[:, item - 1]
 
         if scale == "bit":
-            scores_to_plot = self.scorer.bit_scores_from_z(
-                z=z_grid,
+            scores_to_plot = self.model.bit_scales.bit_scores_from_theta(
+                theta=theta_grid,
                 **kwargs
             )[0][:, latent_indices]
         else:
-            scores_to_plot = z_grid[:, [var - 1 for var in latent_variables]]
+            scores_to_plot = theta_grid[:, [var - 1 for var in latent_variables]]
             if scores_to_plot.dim() == 1:
                 scores_to_plot = scores_to_plot.unsqueeze(1)
 
         if len(latent_variables) == 1:
             scores_to_plot.squeeze_()
             min_indices = (scores_to_plot == scores_to_plot.min()).nonzero().flatten()
-            if min_indices[-1] == len(scores_to_plot) - 1:  # if we have reversed z scale
+            if min_indices[-1] == len(scores_to_plot) - 1:  # if we have reversed theta scale
                 start_idx = min_indices[0].item()  # get the first index
                 scores_to_plot = scores_to_plot[:start_idx]
                 item_entropies = item_entropies[:start_idx]
             else:
                 start_idx = min_indices[-1].item()  # get the last index
                 scores_to_plot = scores_to_plot[start_idx:]
                 item_entropies = item_entropies[start_idx:]
@@ -280,19 +277,19 @@
             return fig
         
         if len(latent_variables) == 2:
             grid_size = int(np.sqrt(item_entropies.size()))
             return self._3d_surface_plot(
                 x = scores_to_plot[:, 0].reshape((grid_size, grid_size)),
                 y = scores_to_plot[:, 1].reshape((grid_size, grid_size)),
-                z = item_entropies.reshape((grid_size, grid_size)),
+                theta = item_entropies.reshape((grid_size, grid_size)),
                 title = title or f"Item {item} entropy",
                 x_label = x_label or "Latent variable 1",
                 y_label = y_label or "Latent variable 2",
-                z_label = "Entropy",
+                theta_label = "Entropy",
                 colorscale = colorscale
             )
         
     @torch.inference_mode()
     def plot_item_latent_variable_relationships(
         self,
         relationships: torch.Tensor,
@@ -350,142 +347,146 @@
         self,
         item: int,
         scale: str = "bit",
         latent_variables: tuple = (1, ),
         title: str = None,
         x_label: str = None,
         y_label: str = None,
-        z_range: tuple[float, float] = None,
-        second_z_range: tuple[float, float] = None,
+        theta_range: tuple[float, float] = None,
+        second_theta_range: tuple[float, float] = None,
         steps: int = 300,
-        fixed_zs: torch.Tensor = None,
+        fixed_thetas: torch.Tensor = None,
         plot_group_fit: bool = False,
         group_fit_groups: int = 10,
         group_fit_data: int = None,
-        group_fit_population_z: torch.Tensor = None,
+        group_fit_population_theta: torch.Tensor = None,
         grayscale: bool = False,
         plot_derivative: bool = False,
         **kwargs
     ) -> go.Figure:
         """
         Plots the item probability curves for a given item. Supports 2D and 3D plots.
 
         Parameters
         ----------
         item : int
             The item to plot.
         scale : str, optional
-            The scale to plot against. Can be 'bit' or 'z'. (default is 'bit')
+            The scale to plot against. Can be 'bit' or 'theta'. (default is 'bit')
         latent_variables : tuple, optional
             The latent variables to plot. (default is (1,))
         title : str, optional
             The title for the plot. (default is None and uses "IRF - Item {item}")
         x_label : str, optional
             The label for the X-axis. (default is None and uses "Latent variable" for one latent variable and "Latent variable 1" for two latent variables)
         y_label : str, optional
             The label for the Y-axis. (default is None and uses "Probability")
-        z_range : tuple, optional
-            Only for scale = 'z'. The z range for plotting. (default is None and uses limits based on training data)
-        second_z_range : tuple, optional
-            Only for scale = 'z'. The range for plotting for the second latent variable. (default is None and uses limits based on training data)
+        theta_range : tuple, optional
+            Only for scale = 'theta'. The theta range for plotting. (default is None and uses limits based on training data)
+        second_theta_range : tuple, optional
+            Only for scale = 'theta'. The range for plotting for the second latent variable. (default is None and uses limits based on training data)
         steps : int, optional
-            The number of steps along each z axis used for probability evaluation. (default is 300)
-        fixed_zs: torch.Tensor, optional
+            The number of steps along each theta axis used for probability evaluation. (default is 300)
+        fixed_thetas: torch.Tensor, optional
             Only for multdimensional models. Fixed values for latent space variable not plotted. (default is None and uses the medians in the training data)
         plot_group_fit : bool, optional
             Plot group average probabilities to assess fit. (default is False)
         group_fit_groups : int, optional
             Only for plot_group_fit = True. The number of groups. (default is 10)
         group_fit_data: torch.tensor, optional
             Only for plot_group_fit = True. The data used for group fit plots. Uses training data if not provided. (default is None)
-        group_fit_population_z : torch.tensor, optional
-            Only for plot_group_fit = True. The z scores corresponding to group_fit_data. Will be estimated using group_z_estimation_method if not provided. (default is None)
+        group_fit_population_theta : torch.tensor, optional
+            Only for plot_group_fit = True. The theta scores corresponding to group_fit_data. Will be estimated using group_theta_estimation if not provided. (default is None)
         grayscale : bool, optional
             Plot the item probability curves in grey scale. (default is False)
         plot_derivative : bool, optional
             Plot the first derivative of the item probability curves. Only for plots with one latent variable. (default is False)
         **kwargs : dict, optional
-            Additional keyword arguments used for bit score computation. See :meth:`irtorch.irt.IRT.bit_scores_from_z` for details. 
+            Additional keyword arguments used for bit score computation. See :meth:`irtorch.irt.IRT.bit_scores_from_theta` for details. 
 
         Returns
         -------
         go.Figure
             The Plotly Figure object for the plot.
         """
         model_dim = self.model.latent_variables
         if len(latent_variables) > 2:
             raise TypeError("Cannot plot more than two latent variables in one plot.")
         if len(latent_variables) > model_dim:
             raise TypeError(f"Cannot plot {len(latent_variables)} latent variables with a {model_dim}-dimensional model.")
         if not all(num <= model_dim for num in latent_variables):
             raise TypeError(f"The latent variables to plot need to be smaller than or equal to {model_dim} (the number of variabels in the model).")
-        if z_range is not None and len(z_range) != 2:
-            raise TypeError("z_range needs to have a length of 2.")
-        if len(latent_variables) == 1 and second_z_range is not None and len(second_z_range) != 2:
-            raise TypeError("second_z_range needs to have a length of 2 if specified.")
+        if theta_range is not None and len(theta_range) != 2:
+            raise TypeError("theta_range needs to have a length of 2.")
+        if len(latent_variables) == 1 and second_theta_range is not None and len(second_theta_range) != 2:
+            raise TypeError("second_theta_range needs to have a length of 2 if specified.")
 
-        latent_indices = [z - 1 for z in latent_variables]
+        latent_indices = [theta - 1 for theta in latent_variables]
 
         mask = torch.ones(model_dim, dtype=bool)
         mask[latent_indices] = 0
-        if fixed_zs is None:
-            fixed_zs = self.algorithm.training_z_scores[:, mask].median(dim=0).values
+        if fixed_thetas is None:
+            if isinstance(self.model.algorithm, (AE, VAE)):
+                fixed_thetas = self.model.algorithm.training_theta_scores[:, mask].median(dim=0).values
+            elif isinstance(self.model.algorithm, MML):
+                fixed_thetas = torch.zeros(model_dim)
 
-        elif len(fixed_zs) is not model_dim - len(latent_variables):
+        elif len(fixed_thetas) is not model_dim - len(latent_variables):
             raise TypeError("If specified, the number of fixed latent variables needs to be the same as the number of variables in the model not used for plotting.")
 
-        min_z, max_z = self.scorer.min_max_z_for_integration()
-        if z_range is None:
-            z_range = min_z[latent_indices[0]].item(), max_z[latent_indices[0]].item()
-        if second_z_range is None and len(latent_indices) > 1:
-            second_z_range = min_z[latent_indices[1]].item(), max_z[latent_indices[1]].item()
+        min_theta, max_theta = self.model.evaluation._min_max_theta_for_integration()
+        if theta_range is None:
+            theta_range = min_theta[latent_indices[0]].item(), max_theta[latent_indices[0]].item()
+        if second_theta_range is None and len(latent_indices) > 1:
+            second_theta_range = min_theta[latent_indices[1]].item(), max_theta[latent_indices[1]].item()
 
-        latent_z_1 = torch.linspace(z_range[0], z_range[1], steps=steps)
+        latent_theta_1 = torch.linspace(theta_range[0], theta_range[1], steps=steps)
         if len(latent_indices) == 1:
-            z_grid = latent_z_1.unsqueeze(1).repeat(1, model_dim)
-            z_grid[:, mask] = fixed_zs
+            theta_grid = latent_theta_1.unsqueeze(1).repeat(1, model_dim)
+            theta_grid[:, mask] = fixed_thetas
         else:
-            latent_z_2 = torch.linspace(second_z_range[0], second_z_range[1], steps=steps)
-            latent_z_1, latent_z_2 = torch.meshgrid(latent_z_1, latent_z_2, indexing="ij")
-            z_grid = torch.zeros(latent_z_1.numel(), model_dim)
-            z_grid[:, latent_indices[0]] = latent_z_1.flatten()
-            z_grid[:, latent_indices[1]] = latent_z_2.flatten()
-            z_grid[:, mask] = fixed_zs
+            latent_theta_2 = torch.linspace(second_theta_range[0], second_theta_range[1], steps=steps)
+            latent_theta_1, latent_theta_2 = torch.meshgrid(latent_theta_1, latent_theta_2, indexing="ij")
+            theta_grid = torch.zeros(latent_theta_1.numel(), model_dim)
+            theta_grid[:, latent_indices[0]] = latent_theta_1.flatten()
+            theta_grid[:, latent_indices[1]] = latent_theta_2.flatten()
+            theta_grid[:, mask] = fixed_thetas
             
         if scale == "bit":
-            scores_to_plot, start_z = self.scorer.bit_scores_from_z(
-                z=z_grid,
+            scores_to_plot, start_theta = self.model.bit_scales.bit_scores_from_theta(
+                theta=theta_grid,
                 one_dimensional=False,
                 **kwargs
             )
         else:
-            scores_to_plot = z_grid
+            scores_to_plot = theta_grid
 
         if plot_derivative and len(latent_variables) == 1:
-            prob_matrix = self.model.probability_gradients(z_grid)[:, item - 1, :self.model.modeled_item_responses[item - 1], latent_variables[0] - 1]
+            prob_matrix = self.model.probability_gradients(theta_grid)[:, item - 1, :self.model.modeled_item_responses[item - 1], latent_variables[0] - 1]
             if scale == "bit":
-                bit_z_gradients = self.scorer.bit_score_gradients(z_grid, independent_z=latent_variables[0], start_z=start_z, **kwargs)
-                prob_matrix = prob_matrix / bit_z_gradients[:, latent_variables[0] - 1].view(-1, 1)
+                bit_theta_gradients = self.model.bit_scales.bit_score_gradients(theta_grid, independent_theta=latent_variables[0], start_theta=start_theta, **kwargs)
+                prob_matrix = prob_matrix / bit_theta_gradients[:, latent_variables[0] - 1].view(-1, 1)
         else:
-            prob_matrix = self.model.item_probabilities(z_grid)[:, item - 1, :self.model.modeled_item_responses[item - 1]]
+            prob_matrix = self.model.item_probabilities(theta_grid)[:, item - 1, :self.model.modeled_item_responses[item - 1]]
 
         if len(latent_variables) == 1:
             if plot_group_fit:
                 (
                     group_probs_data,
                     group_probs_model,
                     latent_group_means,
-                ) = self.evaluator.latent_group_probabilities(
+                ) = self.model.evaluation.latent_group_probabilities(
                     data=group_fit_data,
-                    z=group_fit_population_z,
+                    theta=group_fit_population_theta,
                     scale=scale,
                     latent_variable=latent_variables[0],
                     groups=group_fit_groups,
                     **kwargs
                 )
+
                 group_probs_data = group_probs_data[:, item - 1, 0:self.model.modeled_item_responses[item - 1]]
                 group_probs_model = group_probs_model[:, item - 1, 0:self.model.modeled_item_responses[item - 1]]
                 
             else:
                 group_probs_data = group_probs_model = latent_group_means = None
 
             return self._item_probabilities_plot(
@@ -504,45 +505,45 @@
             return self._item_probabilities_3dplot(
                 scores_to_plot[:, latent_indices[0]],
                 scores_to_plot[:, latent_indices[1]],
                 prob_matrix,
                 title=title or f"IRF - Item {item}",
                 x_label=x_label or f"Latent variable {latent_variables[0]}",
                 y_label=y_label or f"Latent variable {latent_variables[1]}",
-                z_label="Probability",
+                theta_label="Probability",
                 grayscale=grayscale
             )
 
     def plot_information(
         self,
         items: list[int] = None,
-        scale: str = "z",
+        scale: str = "theta",
         latent_variables: tuple[int] = (1,),
         degrees: list[int] = None,
         title: str = None,
         x_label: str = None,
         y_label: str = None,
         color: str = None,
         colorscale: str = "Plasma",
-        z_range: tuple[float, float] = None,
-        second_z_range: tuple[float, float] = None,
+        theta_range: tuple[float, float] = None,
+        second_theta_range: tuple[float, float] = None,
         steps: int = None,
-        fixed_zs: torch.Tensor = None,
+        fixed_thetas: torch.Tensor = None,
         **kwargs
     ) -> go.Figure:
         """
         Plots the Fisher information function against the latent variable(s).
         Supports both item and test information.
 
         Parameters
         ----------
         items : list[int], optional
             The items to plot. If None, the full test information is plotted. (default is None)
         scale : str, optional
-            The scale to plot against. Can be 'bit' or 'z'. (default is 'bit')
+            The scale to plot against. Can be 'bit' or 'theta'. (default is 'bit')
         latent_variables : tuple[int], optional
             The latent variables to plot. (default is (1,))
         degrees : list[int], optional
             A list of angles in degrees between 0 and 90. One degree for each latent variable.
             Only applicable when the model is multidimensional.
             Information will be computed in the direction of the angles. (default is None)
         title : str, optional
@@ -551,71 +552,78 @@
             The label for the X-axis. (default is None and uses "Latent variable" for one latent variable and "Latent variable 1" for two latent variables)
         y_label : str, optional
             The label for the Y-axis. (default is None and uses "Information" for one latent variable and "Latent variable 2" for two latent variables)
         color : str, optional
             The color to use for plots with one latent variable. (default is None and uses the default color sequence for the plotly_white template)
         colorscale : str, optional
             Sets the colorscale for the multiple latent variable surface plots. See https://plotly.com/python/builtin-colorscales/ (default is "Plasma")
-        z_range : tuple[float, float], optional
-            Only for scale = 'z'. The z range for plotting. (default is None and uses limits based on training data)
-        second_z_range : tuple[float, float], optional
-            Only for scale = 'z'. The range for plotting for the second latent variable. (default is None and uses limits based on training data)
+        theta_range : tuple[float, float], optional
+            Only for scale = 'theta'. The theta range for plotting. (default is None and uses limits based on training data)
+        second_theta_range : tuple[float, float], optional
+            Only for scale = 'theta'. The range for plotting for the second latent variable. (default is None and uses limits based on training data)
         steps : int, optional
-            The number of steps along each z axis to construct the latent variable grid for which information is evaluated at. (default is None and uses 100 for one latent variable and 18 for two latent variables)
-        fixed_zs: torch.Tensor, optional
+            The number of steps along each theta axis to construct the latent variable grid for which information is evaluated at. (default is None and uses 100 for one latent variable and 18 for two latent variables)
+        fixed_thetas: torch.Tensor, optional
             Only for multdimensional models. Fixed values for latent space variable not plotted. (default is None and uses the medians in the training data)
         **kwargs : dict, optional
-            Additional keyword arguments used for bit score computation. See :meth:`irtorch.irt.IRT.bit_scores_from_z` for details. 
+            Additional keyword arguments used for bit score computation. See :meth:`irtorch.irt.IRT.bit_scores_from_theta` for details. 
         """
         model_dim = self.model.latent_variables
         if len(latent_variables) > 2:
             raise TypeError("Cannot plot more than two latent variables in one plot.")
         if len(latent_variables) > model_dim:
             raise TypeError(f"Cannot plot {len(latent_variables)} latent variables with a {model_dim}-dimensional model.")
         if not all(num <= model_dim for num in latent_variables):
             raise TypeError(f"The latent variables to plot need to be smaller than or equal to {model_dim} (the number of variabels in the model).")
-        if z_range is not None and len(z_range) != 2:
-            raise TypeError("z_range needs to have a length of 2.")
-        if len(latent_variables) == 1 and second_z_range is not None and len(second_z_range) != 2:
-            raise TypeError("second_z_range needs to have a length of 2 if specified.")
+        if theta_range is not None and len(theta_range) != 2:
+            raise TypeError("theta_range needs to have a length of 2.")
+        if len(latent_variables) == 1 and second_theta_range is not None and len(second_theta_range) != 2:
+            raise TypeError("second_theta_range needs to have a length of 2 if specified.")
         if degrees is None and model_dim > 1:
             raise ValueError("Degrees must be provided for multidimensional models.")
         if steps is None:
             steps = 100 if len(latent_variables) == 1 else 18
 
-        latent_indices = [z - 1 for z in latent_variables]
+        latent_indices = [theta - 1 for theta in latent_variables]
 
-        z_grid = self._get_z_grid_for_plotting(latent_variables, z_range, second_z_range, steps, fixed_zs, latent_indices)
+        theta_grid = self._get_theta_grid_for_plotting(latent_variables, theta_range, second_theta_range, steps, fixed_thetas, latent_indices)
         
-        if z_grid.shape[0] > 2000:
+        if theta_grid.shape[0] > 2000:
             logger.warning("A large grid of latent variable values is used for plotting. This may take a while. Consider lowering the steps argument.")
 
         if scale == "bit":
-            scores_to_plot, start_z = self.scorer.bit_scores_from_z(
-                z=z_grid,
+            scores_to_plot, start_theta = self.model.bit_scales.bit_scores_from_theta(
+                theta=theta_grid,
                 **kwargs
             )
             scores_to_plot = scores_to_plot[:, latent_indices]
         else:
-            start_z = None
-            scores_to_plot = z_grid[:, [var - 1 for var in latent_variables]]
+            start_theta = None
+            scores_to_plot = theta_grid[:, [var - 1 for var in latent_variables]]
             if scores_to_plot.dim() == 1:
                 scores_to_plot = scores_to_plot.unsqueeze(1)
 
         if items is not None:
             item_mask = torch.zeros(self.model.items, dtype=bool)
             item_mask[[item - 1 for item in items]] = 1
-            information = self.scorer.information(z_grid, item=True, scale = scale, degrees=degrees, start_z = start_z, **kwargs)[:, item_mask].sum(dim=1)
+            if scale == "bit":
+                information = self.model.bit_scales.bit_information(theta_grid, item=True, degrees=degrees, start_theta = start_theta, **kwargs)[:, item_mask].sum(dim=1)
+            else:
+                information = self.model.information(theta_grid, item=True, degrees=degrees, **kwargs)[:, item_mask].sum(dim=1)
+
         else:
-            information = self.scorer.information(z_grid, item=False, scale = scale, degrees=degrees, start_z = start_z, **kwargs)
+            if scale == "bit":
+                information = self.model.bit_scales.bit_information(theta_grid, item=False, degrees=degrees, start_theta = start_theta, **kwargs)
+            else:
+                information = self.model.information(theta_grid, item=False, degrees=degrees, **kwargs)
 
         if len(latent_variables) == 1:
             scores_to_plot.squeeze_()
             min_indices = (scores_to_plot == scores_to_plot.min()).nonzero().flatten()
-            if min_indices[-1] == len(scores_to_plot) - 1:  # if we have reversed z scale
+            if min_indices[-1] == len(scores_to_plot) - 1:  # if we have reversed theta scale
                 start_idx = min_indices[0].item()  # get the first index
                 scores_to_plot = scores_to_plot[:start_idx]
                 information = information.detach_().squeeze_()[:start_idx]
             else:
                 start_idx = min_indices[-1].item()  # get the last index
                 scores_to_plot = scores_to_plot[start_idx:]
                 information = information.detach_().squeeze_()[start_idx:]
@@ -629,120 +637,120 @@
                 color = color or None
             )
         if len(latent_variables) == 2:
             grid_size = int(np.sqrt(information.size()))
             return self._3d_surface_plot(
                 x = scores_to_plot[:, 0].reshape((grid_size, grid_size)),
                 y = scores_to_plot[:, 1].reshape((grid_size, grid_size)),
-                z = information.reshape((grid_size, grid_size)),
+                theta = information.reshape((grid_size, grid_size)),
                 title = title or "Information",
                 x_label = x_label or "Latent variable 1",
                 y_label = y_label or "Latent variable 2",
-                z_label = "Information",
+                theta_label = "Information",
                 colorscale = colorscale
             )
 
     def plot_expected_sum_score(
         self,
         items: list[int] = None,
         scale: str = "bit",
         latent_variables: tuple[int] = (1,),
         title: str = None,
         x_label: str = None,
         y_label: str = None,
         color: str = None,
         colorscale: str = "Plasma",
-        z_range: tuple[float, float] = None,
-        second_z_range: tuple[float, float] = None,
+        theta_range: tuple[float, float] = None,
+        second_theta_range: tuple[float, float] = None,
         steps: int = None,
-        fixed_zs: torch.Tensor = None,
+        fixed_thetas: torch.Tensor = None,
         **kwargs
     ) -> go.Figure:
         """
         Plots the expected sum score from the model against the latent variable(s).
         Supports full test scores, a single item or a subset of items.
 
         Parameters
         ----------
         items : list[int], optional
             The items used to compte the sum score. If None, all items are used. (default is None)
         scale : str, optional
-            The scale to plot against. Can be 'bit' or 'z'. (default is 'bit')
+            The scale to plot against. Can be 'bit' or 'theta'. (default is 'bit')
         latent_variables : tuple[int], optional
             The latent variables to plot. (default is (1,))
         title : str, optional
             The title for the plot. (default is None)
         x_label : str, optional
             The label for the X-axis. (default is None and uses "Latent variable" for one latent variable and "Latent variable 1" for two latent variables)
         y_label : str, optional
             The label for the Y-axis. (default is None and uses "Expected sum score" or "Expected item score" for one latent variable, and "Latent variable 2" for two latent variables)
         color : str, optional
             The color to use for plots with one latent variable. (default is None and uses the default color sequence for the plotly_white template)
         colorscale : str, optional
             Sets the colorscale for the multiple latent variable surface plots. See https://plotly.com/python/builtin-colorscales/ (default is "Plasma")
-        z_range : tuple[float, float], optional
-            Only for scale = 'z'. The z range for plotting. (default is None and uses limits based on training data)
-        second_z_range : tuple[float, float], optional
-            Only for scale = 'z'. The range for plotting for the second latent variable. (default is None and uses limits based on training data)
+        theta_range : tuple[float, float], optional
+            Only for scale = 'theta'. The theta range for plotting. (default is None and uses limits based on training data)
+        second_theta_range : tuple[float, float], optional
+            Only for scale = 'theta'. The range for plotting for the second latent variable. (default is None and uses limits based on training data)
         steps : int, optional
-            The number of steps along each z axis to construct the latent variable grid for which the sum score is evaluated at. (default is None and uses 100 for one latent variable and 18 for two latent variables)
-        fixed_zs: torch.Tensor, optional
+            The number of steps along each theta axis to construct the latent variable grid for which the sum score is evaluated at. (default is None and uses 100 for one latent variable and 18 for two latent variables)
+        fixed_thetas: torch.Tensor, optional
             Only for multdimensional models. Fixed values for latent space variable not plotted. (default is None and uses the medians in the training data)
         **kwargs : dict, optional
-            Additional keyword arguments used for bit score computation. See :meth:`irtorch.irt.IRT.bit_scores_from_z` for details. 
+            Additional keyword arguments used for bit score computation. See :meth:`irtorch.irt.IRT.bit_scores_from_theta` for details. 
 
         Returns
         -------
         go.Figure
             The plotly Figure object for the plot.
         """
         model_dim = self.model.latent_variables
         if len(latent_variables) > 2:
             raise TypeError("Cannot plot more than two latent variables in one plot.")
         if len(latent_variables) > model_dim:
             raise TypeError(f"Cannot plot {len(latent_variables)} latent variables with a {model_dim}-dimensional model.")
         if not all(num <= model_dim for num in latent_variables):
             raise TypeError(f"The latent variables to plot need to be smaller than or equal to {model_dim} (the number of variabels in the model).")
-        if z_range is not None and len(z_range) != 2:
-            raise TypeError("z_range needs to have a length of 2.")
-        if len(latent_variables) == 1 and second_z_range is not None and len(second_z_range) != 2:
-            raise TypeError("second_z_range needs to have a length of 2 if specified.")
+        if theta_range is not None and len(theta_range) != 2:
+            raise TypeError("theta_range needs to have a length of 2.")
+        if len(latent_variables) == 1 and second_theta_range is not None and len(second_theta_range) != 2:
+            raise TypeError("second_theta_range needs to have a length of 2 if specified.")
         if steps is None:
             steps = 100 if len(latent_variables) == 1 else 18
 
-        latent_indices = [z - 1 for z in latent_variables]
+        latent_indices = [theta - 1 for theta in latent_variables]
 
-        z_grid = self._get_z_grid_for_plotting(latent_variables, z_range, second_z_range, steps, fixed_zs, latent_indices)
+        theta_grid = self._get_theta_grid_for_plotting(latent_variables, theta_range, second_theta_range, steps, fixed_thetas, latent_indices)
         
         if items is not None:
             item_mask = torch.zeros(self.model.items, dtype=bool)
             item_mask[[item - 1 for item in items]] = 1
-            sum_scores = self.model.expected_scores(z_grid, return_item_scores=True)[:, [item - 1 for item in items]].sum(dim=1)
+            sum_scores = self.model.expected_scores(theta_grid, return_item_scores=True)[:, [item - 1 for item in items]].sum(dim=1)
         else:
-            sum_scores = self.model.expected_scores(z_grid, return_item_scores=False)
+            sum_scores = self.model.expected_scores(theta_grid, return_item_scores=False)
 
         if scale == "bit":
-            scores_to_plot = self.scorer.bit_scores_from_z(
-                z=z_grid,
+            scores_to_plot = self.model.bit_scales.bit_scores_from_theta(
+                theta=theta_grid,
                 **kwargs
             )[0][:, latent_indices]
         else:
-            scores_to_plot = z_grid[:, [var - 1 for var in latent_variables]]
+            scores_to_plot = theta_grid[:, [var - 1 for var in latent_variables]]
             if scores_to_plot.dim() == 1:
                 scores_to_plot = scores_to_plot.unsqueeze(1)
 
         if items is not None and len(items) == 1:
             title = f"Expected score. Item {items[0]}" if title is None else title
 
         if len(latent_variables) == 1:
             if items is not None and len(items) == 1:
                 y_label = "Expected item score" if y_label is None else y_label
             scores_to_plot.squeeze_()
             min_indices = (scores_to_plot == scores_to_plot.min()).nonzero().flatten()
-            if min_indices[-1] == len(scores_to_plot) - 1:  # if we have reversed z scale
+            if min_indices[-1] == len(scores_to_plot) - 1:  # if we have reversed theta scale
                 start_idx = min_indices[0].item()  # get the first index
                 scores_to_plot = scores_to_plot[:start_idx]
                 sum_scores = sum_scores[:start_idx]
             else:
                 start_idx = min_indices[-1].item()  # get the last index
                 scores_to_plot = scores_to_plot[start_idx:]
                 sum_scores = sum_scores[start_idx:]
@@ -759,93 +767,102 @@
             return fig
         
         if len(latent_variables) == 2:
             grid_size = int(np.sqrt(sum_scores.size()))
             return self._3d_surface_plot(
                 x = scores_to_plot[:, 0].reshape((grid_size, grid_size)),
                 y = scores_to_plot[:, 1].reshape((grid_size, grid_size)),
-                z = sum_scores.reshape((grid_size, grid_size)),
+                theta = sum_scores.reshape((grid_size, grid_size)),
                 title = title or "Expected sum score",
                 x_label = x_label or "Latent variable 1",
                 y_label = y_label or "Latent variable 2",
-                z_label = "Expected sum score",
+                theta_label = "Expected sum score",
                 colorscale = colorscale
             )
 
-    def _get_z_grid_for_plotting(self, latent_variables, z_range, second_z_range, steps, fixed_zs, latent_indices):
+    def _get_theta_grid_for_plotting(self, latent_variables, theta_range, second_theta_range, steps, fixed_thetas, latent_indices):
         mask = torch.ones(self.model.latent_variables, dtype=bool)
         mask[latent_indices] = 0
-        if fixed_zs is None:
-            fixed_zs = self.algorithm.training_z_scores[:, mask].median(dim=0).values
+        if fixed_thetas is None:
+            if isinstance(self.model.algorithm, (AE, VAE)):
+                fixed_thetas = self.model.algorithm.training_theta_scores[:, mask].median(dim=0).values
+            elif isinstance(self.model.algorithm, MML):
+                fixed_thetas = torch.zeros(self.model.latent_variables)
         
-        if z_range is None:
-            z_range = (
-                self.algorithm.training_z_scores[:, latent_variables[0] - 1].min().item(),
-                self.algorithm.training_z_scores[:, latent_variables[0] - 1].max().item()
-            )
-        if second_z_range is None and len(latent_indices) > 1:
-            second_z_range = (
-                self.algorithm.training_z_scores[:, latent_variables[1] - 1].min().item(),
-                self.algorithm.training_z_scores[:, latent_variables[1] - 1].max().item()
-            )
+        if theta_range is None:
+            if isinstance(self.model.algorithm, (AE, VAE)):
+                theta_range = (
+                    self.model.algorithm.training_theta_scores[:, latent_variables[0] - 1].min().item(),
+                    self.model.algorithm.training_theta_scores[:, latent_variables[0] - 1].max().item()
+                )
+            elif isinstance(self.model.algorithm, MML):
+                theta_range = (-3, 3)
+        if second_theta_range is None and len(latent_indices) > 1:
+            if isinstance(self.model.algorithm, (AE, VAE)):
+                second_theta_range = (
+                    self.model.algorithm.training_theta_scores[:, latent_variables[1] - 1].min().item(),
+                    self.model.algorithm.training_theta_scores[:, latent_variables[1] - 1].max().item()
+                )
+            elif isinstance(self.model.algorithm, MML):
+                second_theta_range = (-3, 3)
 
-        latent_z_1 = torch.linspace(z_range[0], z_range[1], steps=steps)
+        latent_theta_1 = torch.linspace(theta_range[0], theta_range[1], steps=steps)
         if len(latent_indices) == 1:
-            z_grid = latent_z_1.unsqueeze(1).repeat(1, self.model.latent_variables)
-            z_grid[:, mask] = fixed_zs
+            theta_grid = latent_theta_1.unsqueeze(1).repeat(1, self.model.latent_variables)
+            theta_grid[:, mask] = fixed_thetas
         else:
-            latent_z_2 = torch.linspace(second_z_range[0], second_z_range[1], steps=steps)
-            latent_z_1, latent_z_2 = torch.meshgrid(latent_z_1, latent_z_2, indexing="ij")
-            z_grid = torch.zeros(latent_z_1.numel(), self.model.latent_variables)
-            z_grid[:, latent_indices[0]] = latent_z_1.flatten()
-            z_grid[:, latent_indices[1]] = latent_z_2.flatten()
-            z_grid[:, mask] = fixed_zs
+            latent_theta_2 = torch.linspace(second_theta_range[0], second_theta_range[1], steps=steps)
+            latent_theta_1, latent_theta_2 = torch.meshgrid(latent_theta_1, latent_theta_2, indexing="ij")
+            theta_grid = torch.zeros(latent_theta_1.numel(), self.model.latent_variables)
+            theta_grid[:, latent_indices[0]] = latent_theta_1.flatten()
+            theta_grid[:, latent_indices[1]] = latent_theta_2.flatten()
+            theta_grid[:, mask] = fixed_thetas
         
-        return z_grid
+        return theta_grid
 
     def _2d_line_plot(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         title: str,
         x_label: str,
         y_label: str,
         color: str
     ) -> go.Figure:
         df = pd.DataFrame({
-            'x': x.cpu().detach().numpy() if x.is_cuda else x.detach().numpy(), 
-            'y': y.cpu().detach().numpy() if y.is_cuda else y.detach().numpy()
+            "x": x.cpu().detach().numpy() if x.is_cuda else x.detach().numpy(), 
+            "y": y.cpu().detach().numpy() if y.is_cuda else y.detach().numpy()
         })
-        fig = px.line(df, x='x', y='y', title=title, color_discrete_sequence=[color])
+        fig = px.line(df, x="x", y="y", title=title, color_discrete_sequence=[color])
         fig.update_layout(xaxis_title=x_label, yaxis_title=y_label)
         return fig
 
     def _3d_surface_plot(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
-        z: torch.Tensor,
+        theta: torch.Tensor,
         title: str,
         x_label: str,
         y_label: str,
-        z_label: str,
+        theta_label: str,
         colorscale: str
     ) -> go.Figure:
         x = x.cpu().detach().numpy() if x.is_cuda else x.detach().numpy()
         y = y.cpu().detach().numpy() if y.is_cuda else y.detach().numpy()
-        z = z.cpu().detach().numpy() if z.is_cuda else z.detach().numpy()
+        theta = theta.cpu().detach().numpy() if theta.is_cuda else theta.detach().numpy()
         fig = go.Figure(data=[
-            go.Surface(z=z, x=x, y=y, colorscale=colorscale)
+            go.Surface(theta=theta, x=x, y=y, colorscale=colorscale)
         ])
         fig.update_layout(
             title=title,
             scene = {
                 "xaxis": {"title": x_label},
                 "yaxis": {"title": y_label},
-                "zaxis": {"title": z_label}
+                "zaxis": {"title": theta_label}
             }
         )
 
         return fig
 
     def _item_probabilities_plot(
         self,
@@ -885,15 +902,15 @@
 
         Returns
         -------
         go.Figure
             The Plotly Figure object for the plot.
         """
         min_indices = (latent_scores == latent_scores.min()).nonzero().flatten()
-        if min_indices[-1] == len(latent_scores) - 1:  # if we have reversed z scale
+        if min_indices[-1] == len(latent_scores) - 1:  # if we have reversed theta scale
             start_idx = min_indices[0].item()  # get the first index
             latent_scores = latent_scores[:start_idx]
             prob_matrix = prob_matrix[:start_idx, :]
         else:
             start_idx = min_indices[-1].item()  # get the last index
             latent_scores = latent_scores[start_idx:]
             prob_matrix = prob_matrix[start_idx:, :]
@@ -917,40 +934,57 @@
         
         # Adjust the size of the palette if there are more categories than colors
         if len(colors) < num_categories:
             colors = colors * (num_categories // len(colors) + 1)
 
         # Plot each response category
         for i in range(prob_matrix.shape[1]):
-            response_text = f"Option {i+1}" if self.model.mc_correct is not None else f"{i}"
-            response_to_show = i+1 if self.model.mc_correct is not None else i
+            if self.model.model_missing:
+                if i == 0:
+                    response_text = "Missing"
+                else:
+                    response_text = f"Option {i}" if self.model.mc_correct is not None else f"{i}"
+            else:
+                response_text = f"Option {i+1}" if self.model.mc_correct is not None else f"{i}"
+
             color = colors[i % len(colors)]  # Ensure color wraps around if more categories than colors
             fig.add_trace(go.Scatter(
                 x=latent_scores,
                 y=prob_matrix[:, i],
-                mode='lines',
+                mode="lines",
                 name=response_text,
                 line=dict(color=color)
             ))
 
             if latent_group_means is not None and group_probs_data is not None and group_probs_model is not None:
+                if self.model.model_missing:
+                    if i == 0:
+                        data_text = "Data missing"
+                        model_text = "Model missing"
+                    else:
+                        data_text = f"Data {i}" if self.model.mc_correct is not None else f"{i}"
+                        model_text = f"Model {i}" if self.model.mc_correct is not None else f"{i}"
+                else:
+                    data_text = f"Data {i+1}" if self.model.mc_correct is not None else f"{i}"
+                    model_text = f"Model {i+1}" if self.model.mc_correct is not None else f"{i}"
+
                 # Adding scatter plot for group data
                 fig.add_trace(go.Scatter(
                     x=latent_group_means,
                     y=group_probs_data[:, i],
-                    mode='markers', name=f'Data {response_to_show}',
-                    marker=dict(symbol='circle-open', color=color)
+                    mode="markers", name=data_text,
+                    marker=dict(symbol="circle-open", color=color)
                 ))
                 # Adding scatter plot for group model predictions
                 fig.add_trace(go.Scatter(
                     x=latent_group_means,
                     y=group_probs_model[:, i],
-                    mode='markers',
-                    name=f'Model {response_to_show}',
-                    marker=dict(symbol='circle', color=color)
+                    mode="markers",
+                    name=model_text,
+                    marker=dict(symbol="circle", color=color)
                 ))
 
         legend_title = "Item response" if self.model.mc_correct is not None else "Score"
         fig.update_layout(
             title=title,
             xaxis_title=x_label,
             yaxis_title=y_label,
@@ -963,15 +997,15 @@
         self,
         latent_variable_x: torch.Tensor,
         latent_variable_y: torch.Tensor,
         prob_matrix: torch.Tensor,
         title: str = "IRF",
         x_label: str = "Latent variable",
         y_label: str = "Latent variable",
-        z_label: str = "Probability",
+        theta_label: str = "Probability",
         grayscale: bool = False,
     ) -> go.Figure:
         """
         Creates a 3D plot of item probabilities against two latent variables.
 
         Parameters
         ----------
@@ -981,15 +1015,15 @@
             A tensor of latent scores for the Y-axis.
         prob_matrix : torch.Tensor
             A 2D tensor with the probabilities. These form the Z-axis values for the plot.
         x_label : str, optional
             The label for the X-axis. (default is "Latent variable")
         y_label : str, optional
             The label for the Y-axis. (default is "Latent variable")
-        z_label : str, optional
+        theta_label : str, optional
             The label for the Z-axis. (default is "Probability")
         title : str, optional
             The title for the plot. (default is "IRF")
         grayscale : bool, optional
             Grayscale plot. (default is False)
 
         Returns
@@ -1015,34 +1049,34 @@
 
         # Ensure we have enough colors for the number of responses
         if len(colors) < num_responses:
             colors += colors * (num_responses // len(colors) + 1) 
 
         fig = go.Figure()
         for response_category in range(num_responses):
-            z = prob_matrix[:, response_category].reshape((steps, steps))
+            theta = prob_matrix[:, response_category].reshape((steps, steps))
             fig.add_trace(go.Surface(
-                x=x, y=y, z=z, 
-                name=f'Response {response_category}',
+                x=x, y=y, theta=theta, 
+                name=f"Response {response_category}",
                 showscale=False,  # Optionally hide the color scale
                 colorscale=[(0, colors[response_category % len(colors)]), (1, colors[response_category % len(colors)])],
             ))
             # Dummy trace for legend
             fig.add_trace(go.Scatter3d(
-                x=[None], y=[None], z=[None], mode='markers',
+                x=[None], y=[None], theta=[None], mode="markers",
                 marker=dict(size=10, color=colors[response_category % len(colors)]),
-                showlegend=True, name=f'Response {response_category}'
+                showlegend=True, name=f"Response {response_category}"
             ))
 
         fig.update_layout(
             title=title,
             scene=dict(
                 xaxis_title=x_label,
                 yaxis_title=y_label,
-                zaxis_title=z_label,
+                zaxis_title=theta_label,
             ),
             legend_title="Item responses",
             autosize=True,
         )
 
         return fig
 
@@ -1103,21 +1137,21 @@
         self,
         scores: np.ndarray,
         title: str,
         x_label: str,
         y_label: str,
         color: str
     ) -> go.Figure:
-        df = pd.DataFrame(scores, columns=['values'])
+        df = pd.DataFrame(scores, columns=["values"])
         histogram_kwargs = {
-            'x': "values",
-            'marginal': "box"
+            "x": "values",
+            "marginal": "box"
         }
         if color:
-            histogram_kwargs['color_discrete_sequence'] = [color]
+            histogram_kwargs["color_discrete_sequence"] = [color]
         fig = px.histogram(df, **histogram_kwargs)
         fig.update_layout(title=title, xaxis_title=x_label, yaxis_title=y_label)
         return fig
 
     def _two_latent_variables_distribution_plot(
         self, 
         scores: np.ndarray,
@@ -1130,24 +1164,24 @@
         if contour_plot_bins is None:
             contour_plot_bins = int(np.log2(scores.shape[0])) + 1 # Sturges’ Rule
         histogram2d, x_edges, y_edges = np.histogram2d(scores[:, 0], scores[:, 1], bins=contour_plot_bins, density=True)
         x_centers = (x_edges[:-1] + x_edges[1:]) / 2
         y_centers = (y_edges[:-1] + y_edges[1:]) / 2
         fig = go.Figure(data =
             go.Contour(
-                z=histogram2d,
+                theta=histogram2d,
                 x=x_centers, # Centers of bins (x-axis)
                 y=y_centers, # Centers of bins (y-axis)
                 colorscale=contour_colorscale
             )
         )
         fig.update_layout(title=title, xaxis_title=x_label, yaxis_title=y_label)
         return fig
 
-    def _generate_grayscale_colors(self, n, start_color='#b0b0b0'):
+    def _generate_grayscale_colors(self, n, start_color="#b0b0b0"):
         """
         Generates a list of n colors in grayscale from light gray to black.
 
         Parameters
         ----------
         n : int
             The number of colors to generate.
@@ -1161,9 +1195,9 @@
         """
         start_rgb = np.array([int(start_color[i:i+2], 16) for i in (1, 3, 5)])  # Convert start_color to RGB
         end_rgb = np.array([0, 0, 0])  # RGB for black
         colors = [(
             start_rgb + (end_rgb - start_rgb) * i / (n - 1)
         ).astype(int) for i in range(n)]
         # Convert RGB to hexadecimal
-        hex_colors = ['#' + ''.join(f'{int(c):02x}' for c in color) for color in colors]
+        hex_colors = ["#" + "".join(f"{int(c):02x}" for c in color) for color in colors]
         return hex_colors
```

### Comparing `irtorch-0.0.4/irtorch/irt_scorer.py` & `irtorch-0.1.0/irtorch/bit_scales.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,483 +1,70 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING
 import logging
 import torch
 from torch.distributions import MultivariateNormal
-from irtorch.models.base_irt_model import BaseIRTModel
-from irtorch.estimation_algorithms.base_irt_algorithm import BaseIRTAlgorithm
-from irtorch.estimation_algorithms.aeirt import AEIRT
-from irtorch.quantile_mv_normal import QuantileMVNormal
-from irtorch.gaussian_mixture_model import GaussianMixtureModel
-from irtorch._internal_utils import output_to_item_entropy, random_guessing_data, linear_regression, dynamic_print
+from irtorch._internal_utils import output_to_item_entropy, random_guessing_data, linear_regression
 from irtorch.outlier_detector import OutlierDetector
-from irtorch.utils import one_hot_encode_test_data
+from irtorch.estimation_algorithms import AE, VAE, MML
 
-logger = logging.getLogger('irtorch')
+if TYPE_CHECKING:
+    from irtorch.models.base_irt_model import BaseIRTModel
 
-class IRTScorer:
-    def __init__(self, model: BaseIRTModel, algorithm: BaseIRTAlgorithm):
-        """
-        Initializes the IRTScorer class with a given model and fitting algorithm.
+logger = logging.getLogger("irtorch")
 
-        Parameters
-        ----------
-        model : BaseIRTModel
-            BaseIRTModel object.
-        algorithm : BaseIRTAlgorithm
-            BaseIRTAlgorithm object.
-        """
+class BitScales:
+    """
+    Class for bit scale related features.
+
+    Parameters
+    ----------
+    model : BaseIRTModel
+        The IRT model to use for bit scale computation.
+    """
+    def __init__(self, model: BaseIRTModel):
         self.model = model
-        self.algorithm = algorithm
-        self.latent_density = None
-
-
-    @torch.inference_mode()
-    def approximate_latent_density(
-        self,
-        z_scores: torch.Tensor,
-        approximation: str = "qmvn",
-        cv_n_components: list[int] = [2, 3, 4, 5, 10],
-    ) -> None:
-        """
-        Approximate the latent space density.
-
-        Parameters
-        ----------
-        z_scores : torch.Tensor
-            A 2D tensor with z scores. Each row represents one respondent, and each column an item.
-        approximation : str, optional
-            The approximation method to use. (default is 'qmvn')
-            - 'qmvn' for quantile multivariate normal approximation of a multivariate joint density function (QuantileMVNormal class).
-            - 'gmm' for a gaussian mixture model.
-
-        cv_n_components: int, optional
-            The number of components to use for cross-validation in the Gaussian Mixture Model. (default is [2, 3, 4, 5, 10])
-
-        Returns
-        -------
-        torch.Tensor
-            A 2D tensor of latent scores, with latent variables as columns.
-        """
-        if approximation == "gmm":
-            cv_n_components = [2, 3, 4, 5, 10] if cv_n_components is None else cv_n_components
-            self.latent_density = self._cv_gaussian_mixture_model(z_scores, cv_n_components)
-        elif approximation == "qmvn":
-            self.latent_density = QuantileMVNormal()
-            self.latent_density.fit(z_scores)
-        else:
-            raise ValueError("Invalid approximation method. Choose either 'qmvn' or 'gmm'.")
-
-    def _cv_gaussian_mixture_model(self, data: torch.Tensor, cv_n_components: list[int]) -> GaussianMixtureModel:
-        if len(cv_n_components) > 1:
-            logger.info("Performing cross-validation for Gaussian Mixture Model components...")
-            n_folds = 5
-            average_log_likelihood = torch.zeros(len(cv_n_components))
-            for comp_ind, components in enumerate(cv_n_components):
-                log_likelihoods = torch.zeros(n_folds)
-                data_chunks = data.chunk(n_folds)
-                for i, data_val in enumerate(data_chunks):
-                    train_chunks = [x for j, x in enumerate(data_chunks) if j != i]
-                    data_train = torch.cat(train_chunks, dim=0)
-
-                    gmm = GaussianMixtureModel(n_components=components, n_features=data.shape[1])
-                    gmm.fit(data_train)
-
-                    # Compute the log likelihood on the validation data
-                    log_likelihoods[i] = gmm(data_val)
-
-                # Compute the average log likelihood over the folds
-                average_log_likelihood[comp_ind] = log_likelihoods.mean()
-
-            # Select the number of components that maximizes the average log likelihood
-            optimal_n_components = cv_n_components[average_log_likelihood.argmax()]
-            logger.info("Fitting Gaussian Mixture Model for latent trait density.")
-            gmm = GaussianMixtureModel(n_components=optimal_n_components, n_features=data.shape[1])
-        else:
-            logger.info("Fitting Gaussian Mixture Model for latent trait density.")
-            gmm = GaussianMixtureModel(n_components=cv_n_components[0], n_features=data.shape[1])
-
-        gmm.fit(data)
-        return gmm
-
-    @torch.inference_mode()
-    def min_max_z_for_integration(
-        self,
-        z: torch.Tensor = None,
-    ) -> tuple[torch.Tensor, torch.Tensor]:
-        """
-        Retrieve the minimum and maximum z score for approximating integrals over the latent space. Uses one standard deviation below/above the min/max of each z score vector.
-
-        Parameters
-        ----------
-        z : torch.Tensor, optional
-            A 2D tensor. Columns are each latent variable, rows are respondents. Default is None and uses training data z scores.
-
-        Returns
-        -------
-        tuple[torch.Tensor, torch.Tensor]
-            A tuple with 1D tensors, containing the min and max integration z scores of each latent variable.
-        """
-        if z is None:
-            z = self.algorithm.training_z_scores
-
-        z_min = z.min(dim=0)[0]
-        z_max = z.max(dim=0)[0]
-        z_stds = z.std(dim=0)
-
-        return z_min - z_stds, z_max + z_stds
-
-
-    @torch.inference_mode()
-    def latent_scores(
-        self,
-        data: torch.Tensor,
-        scale: str = "z",
-        standard_errors: bool = False,
-        z: torch.Tensor = None,
-        z_estimation_method: str = "ML",
-        ml_map_device: str = "cuda" if torch.cuda.is_available() else "cpu",
-        lbfgs_learning_rate: float = 0.25,
-        eap_z_integration_points: int = None,
-        bit_score_one_dimensional: bool = False,
-        bit_score_population_z: torch.Tensor = None,
-        bit_score_grid_points: int = 300,
-        bit_score_z_grid_method: str = None,
-        bit_score_start_z: torch.Tensor = None,
-        bit_score_start_z_guessing_probabilities: list[float] = None,
-        bit_score_start_z_guessing_iterations: int = 10000,
-        bit_score_items: list[int] = None
-    ):
-        """
-        Returns the latent scores for given test data using encoder the neural network (NN), maximum likelihood (ML), expected a posteriori (EAP) or maximum a posteriori (MAP). 
-        ML and MAP uses the LBFGS algorithm. EAP and MAP are not recommended for non-variational autoencoder models as there is nothing pulling the latent distribution towards a normal.        
-        EAP for models with more than three factors is not recommended since the integration grid becomes huge.
-
-        Parameters
-        ----------
-        data : torch.Tensor
-            A 2D tensor with test data. Each row represents one respondent, each column an item.
-        scale : str, optional
-            The scoring method to use. Can be 'bit' or 'z'. (default is 'z')
-        standard_errors : bool, optional
-            Whether to return standard errors for the latent scores. (default is False)
-        z : torch.Tensor, optional
-            For bit scores. A 2D tensor containing the pre-estimated z scores for each respondent in the data. If not provided, will be estimated using z_estimation_method. Each row corresponds to one respondent and each column represents a latent variable. (default is None)
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Also used for bit scores as they require the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
-        ml_map_device: str, optional
-            For ML and MAP. The device to use for computation. Can be 'cpu' or 'cuda'. (default is "cuda" if available else "cpu")
-        lbfgs_learning_rate: float, optional
-            For ML and MAP. The learning rate to use for the LBFGS optimizer. Try lowering this if your loss runs rampant. (default is 0.3)
-        eap_z_integration_points: int, optional
-            For EAP. The number of integration points for each latent variable. (default is 'None' and uses a function of the number of latent variables)
-        bit_score_one_dimensional: bool, optional
-            Whether to estimate one combined bit score for a multidimensional model. (default is False)
-        bit_score_population_z: torch.Tensor, optional
-            A 2D tensor with z scores of the population. Used to estimate relationships between each z and sum scores. Columns are latent variables and rows are respondents. (default is None and uses z_estimation_method with the model training data)
-        bit_score_grid_points : int, optional
-            The number of points to use for computing bit score. More steps lead to more accurate results. (default is 300)
-        bit_score_z_grid_method : str, optional
-            Method used to obtain the z score grid for bit score computation. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is None and uses z_estimation_method)
-        bit_score_start_z : int, optional
-            The z score used as the starting point for bit score computation. Computed automatically if not provided. (default is 'None')
-        bit_score_start_z_guessing_probabilities: list[float], optional
-            Custom guessing probabilities for each item. The same length as the number of items. Guessing is not supported for polytomously scored items and the probabilities for them will be ignored. (default is None and uses no guessing or, for multiple choice models, 1 over the number of item categories)
-        bit_score_start_z_guessing_iterations: int, optional
-            The number of iterations to use for approximating a minimum z when guessing is incorporated. (default is 10000)
-        bit_score_items: list[int], optional
-            The item indices for the items to use to compute the bit scores. (default is 'None' and uses all items)
-        Returns
-        -------
-        torch.Tensor or tuple[torch.Tensor, torch.Tensor]
-            A 2D tensor of latent scores, with latent variables as columns. If standard_errors is True, returns a tuple with the latent scores and the standard errors.
-        """
-        if scale not in ["bit", "z"]:
-            raise ValueError("Invalid scale. Choose either 'z' or 'bit'.")
-        if z_estimation_method not in ["NN", "ML", "EAP", "MAP"]:
-            raise ValueError("Invalid z_estimation_method. Choose either 'NN', 'ML', 'EAP' or 'MAP'.")
-        if standard_errors and (scale == "bit" or z_estimation_method != "ML"):
-            raise ValueError("Standard errors are only available for z scores with ML estimation.")
-
-        data = data.contiguous()
-        if data.dim() == 1:  # if we have only one observations
-            data = data.view(1, -1)
-
-        if z is None:
-            if self.algorithm.one_hot_encoded and z_estimation_method in ["NN", "ML", "MAP"]:
-                one_hot_data = one_hot_encode_test_data(data, self.model.item_categories, encode_missing=self.model.model_missing)
-                if isinstance(self.algorithm, AEIRT):
-                    z = self.algorithm.z_scores(one_hot_data).clone()
-                else:
-                    z = torch.zeros(one_hot_data.shape[0], self.model.latent_variables).float()
-            
-            data = self.algorithm.fix_missing_values(data)
 
-            logger.info("%s estimation of z scores.", z_estimation_method)
-            if not self.algorithm.one_hot_encoded and z_estimation_method in ["NN", "ML", "MAP"]:
-                z = self.algorithm.z_scores(data).clone()
-            if z_estimation_method in ["ML", "MAP"]:
-                z = self._ml_map_z_scores(data, z, z_estimation_method, learning_rate=lbfgs_learning_rate, device=ml_map_device)
-            elif z_estimation_method == "EAP":
-                z = self._eap_z_scores(data, eap_z_integration_points)
-
-        if scale == "z":
-            if standard_errors:
-                fisher_info = self.information(z, item=False, scale = "z", degrees=None)
-                se = 1/torch.einsum('...ii->...i', fisher_info).sqrt()
-                return z, se
-            return z
-        elif scale == "bit":
-            if bit_score_z_grid_method is None:
-                bit_score_z_grid_method = z_estimation_method
-            return self.bit_scores_from_z(
-                z=z,
-                start_z=bit_score_start_z,
-                population_z=bit_score_population_z,
-                one_dimensional=bit_score_one_dimensional,
-                z_estimation_method=bit_score_z_grid_method,
-                grid_points=bit_score_grid_points,
-                items=bit_score_items,
-                start_z_guessing_probabilities=bit_score_start_z_guessing_probabilities,
-                start_z_guessing_iterations=bit_score_start_z_guessing_iterations
-            )[0]
-
-    @torch.inference_mode(False)
-    def _ml_map_z_scores(
-        self, 
-        data: torch.Tensor, 
-        encoder_z_scores:torch.Tensor = None,
-        z_estimation_method: str = "ML",
-        learning_rate: float = 0.3,
-        device: str = "cuda" if torch.cuda.is_available() else "cpu"
-    ) -> torch.Tensor:
-        """
-        Get the latent scores from test data using an already fitted model.
-
-        Parameters
-        ----------
-        data: torch.Tensor
-            A 2D tensor with test data. Columns are items and rows are respondents
-        encoder_z_scores: torch.Tensor
-            A 2D tensor with the z scores of the training data. Columns are latent variables and rows are respondents.
-        z_estimation_method: str, optional
-            Method used to obtain the z scores. Can be 'ML', 'MAP' for maximum likelihood or maximum a posteriori respectively. (default is 'ML')
-        learning_rate: float, optional
-            The learning rate to use for the LBFGS optimizer. (default is 0.3)
-        device: str, optional
-            The device to use for computation. Can be 'cpu' or 'cuda'. (default is "cuda" if available else "cpu")
-        
-        Returns
-        -------
-        torch.Tensor
-            A torch.Tensor with the z scores. The columns are latent variables and rows are respondents.
-        """
-        try:
-            if self.algorithm.training_z_scores is None:
-                raise ValueError("Please fit the model before computing latent scores.")
-                
-            if z_estimation_method == "MAP": # Approximate prior
-                train_z_scores = self.algorithm.training_z_scores
-                # Center the data and compute the covariance matrix.
-                mean_centered_z_scores = train_z_scores - train_z_scores.mean(dim=0)
-                cov_matrix = mean_centered_z_scores.T @ mean_centered_z_scores / (train_z_scores.shape[0] - 1)
-                # Create prior (multivariate normal distribution).
-                prior_density = MultivariateNormal(torch.zeros(train_z_scores.shape[1]), cov_matrix)
-
-            # Ensure decoder parameters gradients are not updated
-            self.model.requires_grad_(False)
-
-            if encoder_z_scores is None:
-                encoder_z_scores = torch.zeros(data.shape[0], self.model.latent_variables).float()
-
-            if device == "cuda":
-                self.model = self.model.to(device)
-                encoder_z_scores = encoder_z_scores.to(device)
-                data = data.to(device)
-                max_iter = 30
-            else:
-                max_iter = 20
-
-            # Initial guess for the z_scores are the outputs from the encoder
-            optimized_z_scores = encoder_z_scores.clone().detach().requires_grad_(True)
-
-            optimizer = torch.optim.LBFGS([optimized_z_scores], lr = learning_rate)
-            loss_history = []
-            tolerance = 1e-8
-
-            def closure():
-                optimizer.zero_grad()
-                logits = self.model(optimized_z_scores)
-                if z_estimation_method == "MAP": # maximize -log likelihood - log prior
-                    loss = -self.model.log_likelihood(data, logits, loss_reduction = "sum") - prior_density.log_prob(optimized_z_scores).sum()
-                else: # maximize -log likelihood for ML
-                    loss = -self.model.log_likelihood(data, logits, loss_reduction = "sum")
-                loss.backward()
-                return loss
-
-            for i in range(max_iter):
-                optimizer.step(closure)
-                with torch.no_grad():
-                    logits = self.model(optimized_z_scores)
-                    if z_estimation_method == "MAP": # maximize -log likelihood - log prior
-                        loss = -self.model.log_likelihood(data, logits, loss_reduction = "sum") - prior_density.log_prob(optimized_z_scores).sum()
-                    else: # maximize -log likelihood for ML
-                        loss = -self.model.log_likelihood(data, logits, loss_reduction = "sum")
-                    loss = loss.item()
-
-                denominator = data.numel()
-                dynamic_print(f'Iteration {i+1}: Current Loss = {loss}')
-                if len(loss_history) > 0 and abs(loss - loss_history[-1]) / denominator < tolerance:
-                    logger.info("Converged at iteration %s.", i+1)
-                    break
-
-                loss_history.append(loss)
-        except Exception as e:
-            logger.error("Error in %s iteration %s: %s", z_estimation_method, i+1, e)
-            raise e
-        finally:
-            # Reset requires_grad for decoder parameters if we want to train decoder later
-            self.model = self.model.to("cpu")
-            optimized_z_scores = optimized_z_scores.detach().to("cpu")
-            self.model.requires_grad_(True)
-        return optimized_z_scores
-    
-    @torch.inference_mode()
-    def _eap_z_scores(self, data: torch.Tensor, grid_points: int = None) -> torch.Tensor:
-        """
-        Get the latent z scores from test data using an already fitted model.
-
-        Parameters
-        ----------
-        data: torch.Tensor
-            A 2D tensor with test data. Columns are items and rows are respondents
-        grid_points: int, optional
-            The number of grid points for each latent variable. (default is 'None' and uses a function of the number of latent variables)
-        
-        Returns
-        -------
-        torch.Tensor
-            A torch.Tensor with the z scores. The columns are latent variables and rows are respondents.
-        """
-        if self.algorithm.training_z_scores is None:
-            raise ValueError("Please fit the model before computing latent scores.")
-
-        # Get grid for integration.
-        train_z_scores = self.algorithm.training_z_scores
-        if grid_points is None:
-            if train_z_scores.shape[1] > 4:
-                raise ValueError("EAP is not implemented for more than 4 latent variables because of large integration grid.")
-            grid_points = {
-                1: 200,
-                2: 15,
-                3: 7,
-                4: 5
-            }.get(train_z_scores.shape[1], 100)
-            
-        z_grid = self._z_grid(train_z_scores, grid_size=grid_points)
-        
-        # Center the data and compute the covariance matrix.
-        mean_centered_z_scores = train_z_scores - train_z_scores.mean(dim=0)
-        cov_matrix = mean_centered_z_scores.T @ mean_centered_z_scores / (train_z_scores.shape[0] - 1)
-        # Create prior (multivariate normal distribution).
-        prior_density = MultivariateNormal(torch.zeros(train_z_scores.shape[1]), cov_matrix)
-        # Compute log of the prior.
-        log_prior = prior_density.log_prob(z_grid)
-
-        # Compute the log likelihood.
-        logits = self.model(z_grid)
-        replicated_data = data.repeat_interleave(z_grid.shape[0], dim=0)
-        replicated_logits = torch.cat([logits] * data.shape[0], dim=0)
-        replicated_z_grid = torch.cat([z_grid] * data.shape[0], dim=0)
-        log_prior = torch.cat([log_prior] * data.shape[0], dim=0)
-        grid_log_likelihoods = self.model.log_likelihood(replicated_data, replicated_logits, loss_reduction = "none")
-        grid_log_likelihoods = grid_log_likelihoods.view(-1, data.shape[1]).sum(dim=1) # sum likelihood over items
-
-        # Approximate integration integral(p(x|z)*p(z)dz)
-        # p(x|z)p(z) / sum(p(x|z)p(z)) needs to sum to 1 for each respondent response pattern.
-        log_posterior = (log_prior + grid_log_likelihoods).view(-1, z_grid.shape[0]) # each row is one respondent
-        # convert to float 64 to prevent 0 probabilities
-        exp_log_posterior = log_posterior.to(dtype=torch.float64).exp()
-        posterior = (exp_log_posterior.T / exp_log_posterior.sum(dim=1)).T.view(-1, 1) # transform to one column
-
-        # Get expected z
-        posterior_times_z = replicated_z_grid * posterior
-        expected_z = posterior_times_z.reshape(-1, z_grid.shape[0], posterior_times_z.shape[1])
-        return expected_z.sum(dim=1).to(dtype=torch.float32)
-
-    @torch.inference_mode()
-    def _z_grid(self, z_scores: torch.Tensor, grid_size: int = None):
-        """
-        Returns a new z score tensor covering a large range of latent variable values in a grid.
-        
-        Parameters
-        ----------
-        z_scores: torch.Tensor
-            The input test scores. Typically obtained from the training data.
-        grid_size: int
-            The number of grid points for each latent variable.
-        
-        Returns
-        -------
-        torch.Tensor
-            A tensor with all combinations of latent variable values. Latent variables as columns.
-        """
-        if grid_size is None:
-            grid_size = int(1e7 / (100 ** z_scores.shape[1]))
-        min_vals, _ = z_scores.min(dim=0)
-        max_vals, _ = z_scores.max(dim=0)
-        # add / remove 0.25 times the diff minus max and min in the training data
-        plus_minus = (max_vals-min_vals) * 0.25
-        min_vals = min_vals - plus_minus
-        max_vals = max_vals + plus_minus
-
-        # Using linspace to generate a range between min and max for each latent variable
-        grids = [torch.linspace(min_val, max_val, grid_size) for min_val, max_val in zip(min_vals, max_vals)]
-
-        # Use torch.cartesian_prod to generate all combinations of the tensors in grid
-        result = torch.cartesian_prod(*grids)
-        # Ensure result is always a 2D tensor even with 1 latent variable
-        return result.view(-1, z_scores.shape[1])
-
-    def bit_score_starting_z(
+    def bit_score_starting_theta(
         self,
-        z_estimation_method: str = "ML",
+        theta_estimation: str = "ML",
         ml_map_device: str = "cuda" if torch.cuda.is_available() else "cpu",
         lbfgs_learning_rate: float = 0.3,
         items: list[int] = None,
         start_all_incorrect: bool = False,
-        train_z: torch.Tensor = None,
+        train_theta: torch.Tensor = None,
         guessing_probabilities: list[float] = None,
         guessing_iterations: int = 10000,
     ):
         """
-        Computes the starting z score from which to compute bit scores.
+        Computes the starting theta score from which to compute bit scores.
         
         Parameters
         ----------
-        z_estimation_method : str, optional
-            Method used to obtain the z scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
+        theta_estimation : str, optional
+            Method used to obtain the theta scores. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
         ml_map_device: str, optional
             For ML and MAP. The device to use for computation. Can be 'cpu' or 'cuda'. (default is "cuda" if available else "cpu")
         lbfgs_learning_rate: float, optional
             For ML and MAP. The learning rate to use for the LBFGS optimizer. (default is 0.3)
         items: list[int], optional
             The item indices for the items to use to compute the bit scores. (default is None and uses all items)
         start_all_incorrect: bool, optional
-            Whether to compute the starting z scores based incorrect responses. If false, starting z is computed based on relationships between each latent variable and the item responses. (default is False)
-        train_z : torch.Tensor, optional
-            A 2D tensor with the training data z scores. Used to estimate relationships between z and getting the items correct when start_all_incorrect is False. Columns are latent variables and rows are respondents. (default is None and uses encoder z scores from the model training data)
+            Whether to compute the starting theta scores based incorrect responses. If false, starting theta is computed based on relationships between each latent variable and the item responses. (default is False)
+        train_theta : torch.Tensor, optional
+            A 2D tensor with the training data theta scores. Used to estimate relationships between theta and getting the items correct when start_all_incorrect is False. Columns are latent variables and rows are respondents. (default is None and uses encoder theta scores from the model training data)
         guessing_probabilities: list[float], optional
             The guessing probability for each item. The same length as the number of items. Guessing is not supported for polytomously scored items and the probabilities for them will be ignored. (default is None and uses no guessing or, for multiple choice models, 1 over the number of item categories)
         guessing_iterations: int, optional
-            The number of iterations to use for approximating a minimum z when guessing is incorporated. (default is 200)
-        
+            The number of iterations to use for approximating a minimum theta when guessing is incorporated. (default is 200)
         
         Returns
         -------
         torch.Tensor
-            A tensor with all the starting z values.
+            A tensor with all the starting theta values.
         """
         items = items or list(range(len(self.model.modeled_item_responses)))
         mc_correct = torch.tensor(self.model.mc_correct) if self.model.mc_correct else None
         if not all(isinstance(item, int) for item in items):
             raise ValueError("items must be a list of integers.")
         
         if guessing_probabilities:
@@ -486,42 +73,47 @@
 
         selected_item_categories = [self.model.item_categories[i] for i in items]
 
         if guessing_probabilities is None and mc_correct is not None:
             guessing_probabilities = [1 / categories for categories in selected_item_categories]
 
         if not start_all_incorrect:
-            if train_z is None:
-                train_z = self.algorithm.training_z_scores
+            if train_theta is None:
+                if isinstance(self.model.algorithm, (AE, VAE)):
+                    train_theta = self.model.algorithm.training_theta_scores
+                elif isinstance(self.model.algorithm, MML):
+                    mvn = MultivariateNormal(torch.zeros(self.model.latent_variables), self.model.algorithm.covariance_matrix)
+                    train_theta = mvn.sample((4000,)).to(dtype=torch.float32)
+
             # Which latent variables are inversely related to the test scores?
-            item_sum_scores = self.model.expected_scores(train_z, return_item_scores=False)
-            test_weights = linear_regression(train_z, item_sum_scores.reshape(-1, 1))[1:]
+            item_sum_scores = self.model.expected_scores(train_theta, return_item_scores=False)
+            test_weights = linear_regression(train_theta, item_sum_scores.reshape(-1, 1))[1:]
             inverted_scale = torch.where(test_weights < 0, torch.tensor(-1), torch.tensor(1)).reshape(-1)
             
             # Which latent variables are positively related to the item scores?
-            directions = self.model.item_z_relationship_directions(train_z)
-            item_z_positive = (inverted_scale * directions) >= 0 # Invert item relationship if overall test relationship is inverted
+            directions = self.model.item_theta_relationship_directions(train_theta)
+            item_theta_positive = (inverted_scale * directions) >= 0 # Invert item relationship if overall test relationship is inverted
 
         if guessing_probabilities is None:
             if start_all_incorrect:
-                logger.info("Computing z for all incorrect responses to get minimum bit score.")
-                starting_z = self.latent_scores(torch.zeros((1, len(items))).float(), scale="z", z_estimation_method=z_estimation_method, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
+                logger.info("Computing theta for all incorrect responses to get minimum bit score.")
+                starting_theta = self.model.latent_scores(torch.zeros((1, len(items))).float(), theta_estimation=theta_estimation, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
             else:
                 # Get minimum score in relation to each latent variable
                 min_sum_score = torch.zeros((len(items), self.model.latent_variables))
                 if self.model.model_missing:
-                    min_sum_score[~item_z_positive] = (torch.tensor(selected_item_categories) - 2).view(-1, 1).float().repeat(1, self.model.latent_variables)[~item_z_positive]
+                    min_sum_score[~item_theta_positive] = (torch.tensor(selected_item_categories) - 2).view(-1, 1).float().repeat(1, self.model.latent_variables)[~item_theta_positive]
                 else:
-                    min_sum_score[~item_z_positive] = (torch.tensor(selected_item_categories) - 1).view(-1, 1).float().repeat(1, self.model.latent_variables)[~item_z_positive]
+                    min_sum_score[~item_theta_positive] = (torch.tensor(selected_item_categories) - 1).view(-1, 1).float().repeat(1, self.model.latent_variables)[~item_theta_positive]
 
-                # get the minimum z scores based on the sum scores
-                starting_z = torch.zeros((1, self.model.latent_variables)).float()
-                for z in range(self.model.latent_variables):
-                    logger.info("Computing minimum bit score z for latent variable %s.", z+1)
-                    starting_z[:, z] = self.latent_scores(min_sum_score.float()[:, z], scale="z", z_estimation_method=z_estimation_method, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)[:, z]
+                # get the minimum theta scores based on the sum scores
+                starting_theta = torch.zeros((1, self.model.latent_variables)).float()
+                for theta in range(self.model.latent_variables):
+                    logger.info("Computing minimum bit score theta for latent variable %s.", theta+1)
+                    starting_theta[:, theta] = self.model.latent_scores(min_sum_score.float()[:, theta], theta_estimation=theta_estimation, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)[:, theta]
         else:
             if mc_correct is None:
                 selected_correct = torch.ones(len(items))
                 random_data = random_guessing_data(selected_item_categories, guessing_iterations, guessing_probabilities)
             else:
                 selected_correct = mc_correct.index_select(0, torch.tensor(items))
                 random_data = random_guessing_data(
@@ -529,519 +121,441 @@
                     guessing_iterations,
                     guessing_probabilities,
                     selected_correct
                 )
 
             if start_all_incorrect:
                 # With one-dimensional bit scores, guessing for all items makes sense
-                logger.info("Approximating z from random guessing data to get minimum bit score.")
-                guessing_z = self.latent_scores(random_data, scale="z", z_estimation_method=z_estimation_method, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
+                logger.info("Approximating theta from random guessing data to get minimum bit score.")
+                guessing_theta = self.model.latent_scores(random_data, theta_estimation=theta_estimation, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
             else:
                 # Random for positively related and set to correct for others
-                guessing_z = torch.zeros(random_data.shape[0], self.model.latent_variables)
-                for z in range(self.model.latent_variables):
-                    random_data_z = random_data.clone()
-                    random_data_z[:, ~item_z_positive[:, z]] = selected_correct[~item_z_positive[:, z]].float() - 1
-                    logger.info("Approximating minimum bit score z from random guessing data for latent variable %s.", z+1)
-                    guessing_z[:, z] = self.latent_scores(random_data_z, scale="z", z_estimation_method=z_estimation_method, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)[:, z]
+                guessing_theta = torch.zeros(random_data.shape[0], self.model.latent_variables)
+                for theta in range(self.model.latent_variables):
+                    random_data_theta = random_data.clone()
+                    random_data_theta[:, ~item_theta_positive[:, theta]] = selected_correct[~item_theta_positive[:, theta]].float() - 1
+                    logger.info("Approximating minimum bit score theta from random guessing data for latent variable %s.", theta+1)
+                    guessing_theta[:, theta] = self.model.latent_scores(random_data_theta, theta_estimation=theta_estimation, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)[:, theta]
 
-            starting_z = guessing_z.detach().median(dim=0).values.reshape(1, self.model.latent_variables)
+            starting_theta = guessing_theta.detach().median(dim=0).values.reshape(1, self.model.latent_variables)
 
-        return starting_z
+        return starting_theta
 
 
     @torch.inference_mode()
-    def bit_scores_from_z(
+    def bit_scores_from_theta(
         self,
-        z: torch.Tensor,
-        start_z: torch.Tensor = None,
-        population_z: torch.Tensor = None,
+        theta: torch.Tensor,
+        start_theta: torch.Tensor = None,
+        population_theta: torch.Tensor = None,
         one_dimensional: bool = False,
-        z_estimation_method: str = "ML",
+        theta_estimation: str = "ML",
         ml_map_device: str = "cuda" if torch.cuda.is_available() else "cpu",
         lbfgs_learning_rate: float = 0.3,
         grid_points: int = 300,
         items: list[int] = None,
-        start_z_guessing_probabilities: list[float] = None,
-        start_z_guessing_iterations: int = 10000,
+        start_theta_guessing_probabilities: list[float] = None,
+        start_theta_guessing_iterations: int = 10000,
     ) -> tuple[torch.Tensor, torch.Tensor]:
         """
-        Computes the bit scores from z scores.
+        Computes the bit scores from theta scores.
 
         Parameters
         ----------
-        z : torch.Tensor
+        theta : torch.Tensor
             A 2D tensor. Columns are latent variables and rows are respondents.
-        start_z : torch.Tensor, optional
+        start_theta : torch.Tensor, optional
             A one row 2D tensor with bit score starting values of each latent variable. Estimated automatically if not provided. (default is None)
-        population_z : torch.Tensor, optional
-            A 2D tensor with z scores of the population. Used to estimate relationships between each z and sum scores. Columns are latent variables and rows are respondents. (default is None and uses z_estimation_method with the model training data)
+        population_theta : torch.Tensor, optional
+            A 2D tensor with theta scores of the population. Used to estimate relationships between each theta and sum scores. Columns are latent variables and rows are respondents. (default is None and uses theta_estimation with the model training data)
         one_dimensional: bool, optional
-            Whether to estimate one combined bit score for a multidimensional model. (default is True)
-        z_estimation_method : str, optional
-            Method used to obtain the z score grid for bit score computation. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
+            Whether to estimate one combined bit score for a multidimensional self.model. (default is True)
+        theta_estimation : str, optional
+            Method used to obtain the theta score grid for bit score computation. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
         ml_map_device: str, optional
             For ML and MAP. The device to use for computation. Can be 'cpu' or 'cuda'. (default is "cuda" if available else "cpu")
         lbfgs_learning_rate: float, optional
             For ML and MAP. The learning rate to use for the LBFGS optimizer. (default is 0.3)
         grid_points : int, optional
             The number of points to use for computing bit score. More steps lead to more accurate results. (default is 300)
         items: list[int], optional
             The item indices for the items to use to compute the bit scores. (default is None and uses all items)
-        start_z_guessing_probabilities: list[float], optional
-            The guessing probability for each item if start_z is None. The same length as the number of items. Guessing is not supported for polytomously scored items and the probabilities for them will be ignored. (default is None and uses no guessing or, for multiple choice models, 1 over the number of item categories)
-        start_z_guessing_iterations: int, optional
-            The number of iterations to use for approximating a minimum z when guessing is incorporated. (default is 10000)
+        start_theta_guessing_probabilities: list[float], optional
+            The guessing probability for each item if start_theta is None. The same length as the number of items. Guessing is not supported for polytomously scored items and the probabilities for them will be ignored. (default is None and uses no guessing or, for multiple choice models, 1 over the number of item categories)
+        start_theta_guessing_iterations: int, optional
+            The number of iterations to use for approximating a minimum theta when guessing is incorporated. (default is 10000)
         
         Returns
         -------
         tuple[torch.Tensor, torch.Tensor]
-            A 2D tensor with bit score scale scores for each respondent across the rows together with another tensor with start_z.
+            A 2D tensor with bit score scale scores for each respondent across the rows together with another tensor with start_theta.
         """
         if grid_points <= 0:
             raise ValueError("steps must be a positive integer")
-        if start_z is not None and start_z.shape != (1, self.model.latent_variables):
-            raise ValueError(f"start_z must be a one row tensor with shape (1, {self.model.latent_variables}).")
-        if z_estimation_method not in ["NN", "ML", "EAP", "MAP"]:
-            raise ValueError("Invalid bit_score_z_grid_method. Choose either 'NN', 'ML', 'EAP' or 'MAP'.")
+        if start_theta is not None and start_theta.shape != (1, self.model.latent_variables):
+            raise ValueError(f"start_theta must be a one row tensor with shape (1, {self.model.latent_variables}).")
+        if theta_estimation not in ["NN", "ML", "EAP", "MAP"]:
+            raise ValueError("Invalid bit_score_theta_grid_method. Choose either 'NN', 'ML', 'EAP' or 'MAP'.")
         if items is None:
             items = list(range(len(self.model.modeled_item_responses)))
         elif not isinstance(items, list) or not all(isinstance(item, int) for item in items):
             raise ValueError("items must be a list of integers.")
         
-        if population_z is None:
-            if z_estimation_method != "NN":
-                logger.info("Estimating population z scores needed for bit score computation.")
-                population_z = self.latent_scores(self.algorithm.train_data, scale="z", z_estimation_method=z_estimation_method, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
+        if population_theta is None:
+            if theta_estimation != "NN":
+                logger.info("Estimating population theta scores needed for bit score computation.")
+                population_theta = self.model.latent_scores(self.model.algorithm.train_data, theta_estimation=theta_estimation, ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate)
             else:
-                logger.info("Using traning data z scores as population z scores for bit score computation.")
-                population_z = self.algorithm.training_z_scores
-
-        if start_z is None:
-            start_z = self.bit_score_starting_z(
-                z_estimation_method=z_estimation_method,
+                if isinstance(self.model.algorithm, (AE, VAE)):
+                    logger.info("Using traning data theta scores as population theta scores for bit score computation.")
+                    population_theta = self.model.algorithm.training_theta_scores
+                elif isinstance(self.model.algorithm, MML):
+                    logger.info("Sampling from multivariate normal as population theta scores for bit score computation.")
+                    mvn = MultivariateNormal(torch.zeros(self.model.latent_variables), self.model.algorithm.covariance_matrix)
+                    population_theta = mvn.sample((4000,)).to(dtype=torch.float32)
+
+        if start_theta is None:
+            start_theta = self.bit_score_starting_theta(
+                theta_estimation=theta_estimation,
                 items=items,
                 start_all_incorrect=one_dimensional,
-                train_z=population_z,
-                guessing_probabilities=start_z_guessing_probabilities,
-                guessing_iterations=start_z_guessing_iterations,
+                train_theta=population_theta,
+                guessing_probabilities=start_theta_guessing_probabilities,
+                guessing_iterations=start_theta_guessing_iterations,
             )
 
-        inverted_scales = self._inverted_scales(population_z)
-        z_adjusted, train_z_adjusted, start_z_adjusted = self._anti_invert_and_adjust_z_scores(z, population_z, start_z, inverted_scales)
-        grid_start, grid_end, _ = self._get_grid_boundaries(train_z_adjusted, start_z_adjusted)
+        inverted_scales = self._inverted_scales(population_theta)
+        theta_adjusted, train_theta_adjusted, start_theta_adjusted = self._anti_invert_and_adjust_theta_scores(theta, population_theta, start_theta, inverted_scales)
+        grid_start, grid_end, _ = self._get_grid_boundaries(train_theta_adjusted, start_theta_adjusted)
         
         if one_dimensional:
             bit_scores = self._compute_1d_bit_scores(
-                z_adjusted,
-                start_z_adjusted,
+                theta_adjusted,
+                start_theta_adjusted,
                 grid_start,
                 grid_end,
                 inverted_scales,
                 grid_points
             )
         else:
             bit_scores = self._compute_multi_dimensional_bit_scores(
-                z_adjusted,
-                start_z_adjusted,
-                train_z_adjusted,
+                theta_adjusted,
+                start_theta_adjusted,
+                train_theta_adjusted,
                 grid_start,
                 grid_end,
                 inverted_scales,
                 grid_points
             )
         
-        return bit_scores, start_z
-    
+        return bit_scores, start_theta
+
     @torch.inference_mode(False)
     def bit_score_gradients(
         self,
-        z: torch.Tensor,
+        theta: torch.Tensor,
         h: float = None,
-        independent_z: int = None,
-        start_z: torch.Tensor = None,
-        population_z: torch.Tensor = None,
+        independent_theta: int = None,
+        start_theta: torch.Tensor = None,
+        population_theta: torch.Tensor = None,
         one_dimensional: bool = False,
-        z_estimation_method: str = "ML",
+        theta_estimation: str = "ML",
         ml_map_device: str = "cuda" if torch.cuda.is_available() else "cpu",
         lbfgs_learning_rate: float = 0.3,
         grid_points: int = 300,
         items: list[int] = None,
-        start_z_guessing_probabilities: list[float] = None,
-        start_z_guessing_iterations: int = 10000,
+        start_theta_guessing_probabilities: list[float] = None,
+        start_theta_guessing_iterations: int = 10000,
     ) -> torch.Tensor:
-        """
-        Computes the gradients of the bit scores with respect to the input z scores using the central difference method: 
+        r"""
+        Computes the gradients of the bit scores with respect to the input theta scores using the central difference method: 
         .. math ::
 
-            f^{\\prime}(z) \\approx \\frac{f(z+h)-f(z-h)}{2 h}
+            f^{\prime}(theta) \approx \frac{f(theta+h)-f(theta-h)}{2 h}
 
         Parameters
         ----------
-        z : torch.Tensor
-            A 2D tensor containing latent variable z scores. Each column represents one latent variable.
+        theta : torch.Tensor
+            A 2D tensor containing latent variable theta scores. Each column represents one latent variable.
         h : float, optional
-            The step size for the central difference method. (default is uses the difference between the smaller and upper outlier limits (computed using the interquantile range rule) of the training z scores divided by 1000)
-        independent_z : int, optional
-            The latent variable to differentiate with respect to. (default is None and computes gradients with respect to z)
-        start_z : torch.Tensor, optional
+            The step size for the central difference method. (default is uses the difference between the smaller and upper outlier limits (computed using the interquantile range rule) of the training theta scores divided by 1000)
+        independent_theta : int, optional
+            The latent variable to differentiate with respect to. (default is None and computes gradients with respect to theta)
+        start_theta : torch.Tensor, optional
             A one row 2D tensor with bit score starting values of each latent variable. Estimated automatically if not provided. (default is None)
-        population_z : torch.Tensor, optional
-            A 2D tensor with z scores of the population. Used to estimate relationships between each z and sum scores. Columns are latent variables and rows are respondents. (default is None and uses z_estimation_method with the model training data)
+        population_theta : torch.Tensor, optional
+            A 2D tensor with theta scores of the population. Used to estimate relationships between each theta and sum scores. Columns are latent variables and rows are respondents. (default is None and uses theta_estimation with the model training data)
         one_dimensional: bool, optional
-            Whether to estimate one combined bit score for a multidimensional model. (default is True)
-        z_estimation_method : str, optional
-            Method used to obtain the z score grid for bit score computation. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
+            Whether to estimate one combined bit score for a multidimensional self.model. (default is True)
+        theta_estimation : str, optional
+            Method used to obtain the theta score grid for bit score computation. Can be 'NN', 'ML', 'EAP' or 'MAP' for neural network, maximum likelihood, expected a posteriori or maximum a posteriori respectively. (default is 'ML')
         ml_map_device: str, optional
             For ML and MAP. The device to use for computation. Can be 'cpu' or 'cuda'. (default is "cuda" if available else "cpu")
         lbfgs_learning_rate: float, optional
             For ML and MAP. The learning rate to use for the LBFGS optimizer. (default is 0.3)
         grid_points : int, optional
             The number of points to use for computing bit score. More steps lead to more accurate results. (default is 300)
         items: list[int], optional
             The item indices for the items to use to compute the bit scores. (default is None and uses all items)
-        start_z_guessing_probabilities: list[float], optional
-            The guessing probability for each item if start_z is None. The same length as the number of items. Guessing is not supported for polytomously scored items and the probabilities for them will be ignored. (default is None and uses no guessing or, for multiple choice models, 1 over the number of item categories)
-        start_z_guessing_iterations: int, optional
-            The number of iterations to use for approximating a minimum z when guessing is incorporated. (default is 10000)
+        start_theta_guessing_probabilities: list[float], optional
+            The guessing probability for each item if start_theta is None. The same length as the number of items. Guessing is not supported for polytomously scored items and the probabilities for them will be ignored. (default is None and uses no guessing or, for multiple choice models, 1 over the number of item categories)
+        start_theta_guessing_iterations: int, optional
+            The number of iterations to use for approximating a minimum theta when guessing is incorporated. (default is 10000)
 
         Returns
         -------
         torch.Tensor
-            A torch tensor with the gradients for each z score. Dimensions are (z rows, bit scores, z scores) where the last two dimensions represent the jacobian.
-            If independent_z is provided, the tensor has dimensions (z rows, bit scores).
+            A torch tensor with the gradients for each theta score. Dimensions are (theta rows, bit scores, theta scores) where the last two dimensions represent the jacobian.
+            If independent_theta is provided, the tensor has dimensions (theta rows, bit scores).
         """
-        if start_z is None:
-            start_z = self.bit_score_starting_z(
-                z_estimation_method=z_estimation_method,
+        if start_theta is None:
+            start_theta = self.bit_score_starting_theta(
+                theta_estimation=theta_estimation,
                 items=items,
                 start_all_incorrect=one_dimensional,
-                train_z=population_z,
-                guessing_probabilities=start_z_guessing_probabilities,
-                guessing_iterations=start_z_guessing_iterations,
+                train_theta=population_theta,
+                guessing_probabilities=start_theta_guessing_probabilities,
+                guessing_iterations=start_theta_guessing_iterations,
             )
 
-        q1_q3 = torch.quantile(self.algorithm.training_z_scores, torch.tensor([0.25, 0.75]), dim=0)
+        if hasattr(self.model.algorithm, "training_theta_scores") and self.model.algorithm.training_theta_scores is not None:
+        # if isinstance(self.algorithm, (AE, VAE)):
+            q1_q3 = torch.quantile(self.model.algorithm.training_theta_scores, torch.tensor([0.25, 0.75]), dim=0)
+        else:
+        # elif isinstance(self.algorithm, MML):
+            q1_q3 = torch.tensor([-0.6745, 0.6745]).unsqueeze(1).expand(-1, self.model.latent_variables)
+
+        
         iqr = q1_q3[1] - q1_q3[0]
         lower_bound = q1_q3[0] - 1.5 * iqr
         upper_bound = q1_q3[1] + 1.5 * iqr
         h = (upper_bound - lower_bound) / 1000
-        z_low = z-h
-        z_high = z+h
-        if independent_z is None:
-            gradients = torch.zeros(z.shape[0], z.shape[1], z.shape[1])
-            for latent_variable in range(z.shape[1]):
-                z_low_var = torch.cat((z[:, :latent_variable], z_low[:, latent_variable].view(-1, 1), z[:, latent_variable+1:]), dim=1)
-                z_high_var = torch.cat((z[:, :latent_variable], z_high[:, latent_variable].view(-1, 1), z[:, latent_variable+1:]), dim=1)
-                bit_scores_low = self.bit_scores_from_z(
-                    z_low_var, start_z = start_z, population_z=population_z, one_dimensional=one_dimensional, z_estimation_method=z_estimation_method,
+        theta_low = theta-h
+        theta_high = theta+h
+        if independent_theta is None:
+            gradients = torch.zeros(theta.shape[0],theta.shape[1],theta.shape[1])
+            for latent_variable in range(theta.shape[1]):
+                theta_low_var = torch.cat((theta[:, :latent_variable], theta_low[:, latent_variable].view(-1, 1), theta[:, latent_variable+1:]), dim=1)
+                theta_high_var = torch.cat((theta[:, :latent_variable], theta_high[:, latent_variable].view(-1, 1), theta[:, latent_variable+1:]), dim=1)
+                bit_scores_low = self.bit_scores_from_theta(
+                    theta_low_var, start_theta = start_theta, population_theta=population_theta, one_dimensional=one_dimensional, theta_estimation=theta_estimation,
                     ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate, grid_points=grid_points, items=items
                 )[0]
-                bit_scores_high = self.bit_scores_from_z(
-                    z_high_var, start_z = start_z, population_z=population_z, one_dimensional=one_dimensional, z_estimation_method=z_estimation_method,
+                bit_scores_high = self.bit_scores_from_theta(
+                    theta_high_var, start_theta = start_theta, population_theta=population_theta, one_dimensional=one_dimensional, theta_estimation=theta_estimation,
                     ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate, grid_points=grid_points, items=items
                 )[0]
                 gradients[:, latent_variable, :] = (bit_scores_high - bit_scores_low) / (2 * h[latent_variable])
         else:
-            z_low_var = torch.cat((z[:, :independent_z-1], z_low[:, independent_z-1].view(-1, 1), z[:, independent_z:]), dim=1)
-            z_high_var = torch.cat((z[:, :independent_z-1], z_high[:, independent_z-1].view(-1, 1), z[:, independent_z:]), dim=1)
-            bit_scores_low = self.bit_scores_from_z(
-                z_low_var, start_z = start_z, population_z=population_z, one_dimensional=one_dimensional, z_estimation_method=z_estimation_method,
+            theta_low_var = torch.cat((theta[:, :independent_theta-1], theta_low[:, independent_theta-1].view(-1, 1), theta[:, independent_theta:]), dim=1)
+            theta_high_var = torch.cat((theta[:, :independent_theta-1], theta_high[:, independent_theta-1].view(-1, 1), theta[:, independent_theta:]), dim=1)
+            bit_scores_low = self.bit_scores_from_theta(
+                theta_low_var, start_theta = start_theta, population_theta=population_theta, one_dimensional=one_dimensional, theta_estimation=theta_estimation,
                 ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate, grid_points=grid_points, items=items
             )[0]
-            bit_scores_high = self.bit_scores_from_z(
-                z_high_var, start_z = start_z, population_z=population_z, one_dimensional=one_dimensional, z_estimation_method=z_estimation_method,
+            bit_scores_high = self.bit_scores_from_theta(
+                theta_high_var, start_theta = start_theta, population_theta=population_theta, one_dimensional=one_dimensional, theta_estimation=theta_estimation,
                 ml_map_device=ml_map_device, lbfgs_learning_rate=lbfgs_learning_rate, grid_points=grid_points, items=items
             )[0]
-            gradients = (bit_scores_high - bit_scores_low) / (2 * h[independent_z-1])
+            gradients = (bit_scores_high - bit_scores_low) / (2 * h[independent_theta-1])
 
         return gradients
 
+
     @torch.inference_mode(False)
-    def expected_item_score_slopes(
+    def bit_expected_item_score_slopes(
         self,
-        z: torch.Tensor,
-        scale: str = 'z',
+        theta: torch.Tensor,
         bit_scores: torch.Tensor = None,
         rescale_by_item_score: bool = True,
         **kwargs
     ) -> torch.Tensor:
         """
-        Computes the slope of the expected item scores, averaged over the sample in z. Similar to loadings in traditional factor analysis. For each separate latent variable, the slope is computed as the average of the slopes of the expected item scores for each item, using the median z scores for the other latent variables.
+        Computes the slope of the expected item scores with respect to the bit scores, averaged over the sample intheta. Similar to loadings in traditional factor analysis. For each separate latent variable, the slope is computed as the average of the slopes of the expected item scores for each item, using the median theta scores for the other latent variables.
 
         Parameters
         ----------
-        z : torch.Tensor, optional
-            A 2D tensor with latent z scores from the population of interest. Each row represents one respondent, and each column represents a latent variable. If not provided, uses the training z scores. (default is None)
+        theta : torch.Tensor, optional
+            A 2D tensor with latent theta scores from the population of interest. Each row represents one respondent, and each column represents a latent variable. If not provided, uses the training theta scores. (default is None)
         scale : str, optional
-            The latent trait scale to differentiate with respect to. Can be 'bit' or 'z'. 
-            'bit' is only a linear approximation for multidimensional models since multiple z scores can lead to the same bit scores, 
-            and thus there are no unique derivatives of the item scores with respect to the bit scores for multidimensional models. (default is 'z')
+            The latent trait scale to differentiate with respect to. Can be 'bit' or 'theta'. 
+            'bit' is only a linear approximation for multidimensional models since multiple theta scores can lead to the same bit scores, 
+            and thus there are no unique derivatives of the item scores with respect to the bit scores for multidimensional models. (default is 'theta')
         bit_scores: torch.Tensor, optional
-            A 2D tensor with bit scores corresponding to the z scores. If not provided, computes the bit scores from the z scores. (default is None)
+            A 2D tensor with bit scores corresponding to the theta scores. If not provided, computes the bit scores from the theta scores. (default is None)
         rescale_by_item_score : bool, optional
             Whether to rescale the expected items scores to have a max of one by dividing by the max item score. (default is True)
         **kwargs
             Additional keyword arguments for the bit_score_gradients method.
 
         Returns
         -------
         torch.Tensor
             A tensor with the expected item score slopes.
         """
-        if z.shape[0] < 2:
-            raise ValueError("z must have at least 2 rows.")
-        if z.requires_grad:
-            z.requires_grad_(False)
+        if theta.shape[0] < 2:
+            raise ValueError("theta must have at least 2 rows.")
+        if theta.requires_grad:
+            theta.requires_grad_(False)
 
-        if scale == 'bit' and self.model.latent_variables > 1:
-            expected_item_sum_scores = self.model.expected_scores(z, return_item_scores=True).detach()
+        if self.model.latent_variables > 1:
+            expected_item_sum_scores = self.model.expected_scores(theta, return_item_scores=True).detach()
             if not self.model.mc_correct and rescale_by_item_score:
                 expected_item_sum_scores = expected_item_sum_scores / (torch.tensor(self.model.modeled_item_responses) - 1)
             if bit_scores is None:
-                bit_scores = self.bit_scores_from_z(z)[0]
+                bit_scores = self.bit_scores_from_theta(theta)[0]
             # item score slopes for each item
             mean_slopes = linear_regression(bit_scores, expected_item_sum_scores).t()[:, 1:]
         else:
-            median, _ = torch.median(z, dim=0)
-            mean_slopes = torch.zeros(z.shape[0], len(self.model.modeled_item_responses), z.shape[1])
-            for latent_variable in range(z.shape[1]):
-                z_scores = median.repeat(z.shape[0], 1)
-                z_scores[:, latent_variable], _ = z[:, latent_variable].sort()
-                z_scores.requires_grad_(True)
-                expected_item_sum_scores = self.model.expected_scores(z_scores, return_item_scores=True)
+            median, _ = torch.median(theta, dim=0)
+            mean_slopes = torch.zeros(theta.shape[0], len(self.model.modeled_item_responses),theta.shape[1])
+            for latent_variable in range(theta.shape[1]):
+                theta_scores = median.repeat(theta.shape[0], 1)
+                theta_scores[:, latent_variable], _ = theta[:, latent_variable].sort()
+                theta_scores.requires_grad_(True)
+                expected_item_sum_scores = self.model.expected_scores(theta_scores, return_item_scores=True)
                 if not self.model.mc_correct and rescale_by_item_score:
                     expected_item_sum_scores = expected_item_sum_scores / (torch.tensor(self.model.modeled_item_responses) - 1)
 
                 # item score slopes for each item
                 for item in range(expected_item_sum_scores.shape[1]):
-                    if z_scores.grad is not None:
-                        z_scores.grad.zero_()
+                    if theta_scores.grad is not None:
+                        theta_scores.grad.zero_()
                     expected_item_sum_scores[:, item].sum().backward(retain_graph=True)
-                    mean_slopes[:, item, latent_variable] = z_scores.grad[:, latent_variable]
+                    mean_slopes[:, item, latent_variable] = theta_scores.grad[:, latent_variable]
 
-            if scale == 'bit' and self.model.latent_variables == 1:
-                dbit_dz = self.bit_score_gradients(z, independent_z=1, **kwargs)
-                # divide by the derivative of the bit scores with respect to the z scores
+            if self.model.latent_variables == 1:
+                dbit_dtheta = self.bit_score_gradients(theta, independent_theta=1, **kwargs)
+                # divide by the derivative of the bit scores with respect to the theta scores
                 # to get the expected item score slopes with respect to the bit scores
-                mean_slopes = torch.einsum('ab...,a...->ab...', mean_slopes, 1/dbit_dz)
+                mean_slopes = torch.einsum("ab...,a...->ab...", mean_slopes, 1/dbit_dtheta)
             else:
                 mean_slopes = mean_slopes.mean(dim=0)
 
         return mean_slopes
 
-    def information(self, z: torch.Tensor, item: bool = True, scale: str = "z", degrees: list[int] = None, **kwargs) -> torch.Tensor:
-        """
-        Calculate the Fisher information matrix (FIM) for the z scores (or the information in the direction supplied by degrees).
+
+    def bit_information(self, theta: torch.Tensor, item: bool = True, degrees: list[int] = None, **kwargs) -> torch.Tensor:
+        r"""
+        Calculate the Fisher information matrix (FIM) for the theta corresponding bit scores (or the information in the direction supplied by degrees).
 
         Parameters
         ----------
-        z : torch.Tensor
-            A 2D tensor containing latent variable z scores for which to compute the information. Each column represents one latent variable.
+        theta : torch.Tensor
+            A 2D tensor containing latent variable theta scores for which to compute the information. Each column represents one latent variable.
         item : bool, optional
             Whether to compute the information for each item (True) or for the test as a whole (False). (default is True)
-        scale: str, optional
-            The grouping method scale, which can either be 'bit' or 'z'. (default is 'z')
         degrees : list[int], optional
             For multidimensional models. A list of angles in degrees between 0 and 90, one for each latent variable. Specifies the direction in which to compute the information. (default is None and returns the full FIM)
         **kwargs : dict, optional
             Additional keyword arguments to be passed to the bit_score_gradients method if scale is 'bit'. See :meth:`bit_score_gradients` for details.
             
         Returns
         -------
         torch.Tensor
-            A tensor with the information for each z score. Dimensions are:
+            A tensor with the information for each theta score. Dimensions are:
             
-            - By default: (z rows, items, FIM rows, FIM columns).
-            - If degrees are specified: (z rows, items).
-            - If item is False: (z rows, FIM rows, FIM columns).
-            - If degrees are specified and item is False: (z rows).
+            - By default: (theta rows, items, FIM rows, FIM columns).
+            - If degrees are specified: (theta rows, items).
+            - If item is False: (theta rows, FIM rows, FIM columns).
+            - If degrees are specified and item is False: (theta rows).
 
         Notes
         -----
         In the context of IRT, the Fisher information matrix measures the amount of information
         that a test taker's responses :math:`X` carries about the latent variable(s)
-        :math:`\\mathbf{z}`.
+        :math:`\mathbf{\theta}`.
 
         The formula for the Fisher information matrix in the case of multiple parameters is:
 
         .. math::
 
-            I(\\mathbf{z}) = E\\left[ \\left(\\frac{\\partial \\ell(X; \\mathbf{z})}{\\partial \\mathbf{z}}\\right) \\left(\\frac{\\partial \\ell(X; \\mathbf{z})}{\\partial \\mathbf{z}}\\right)^T \\right] = -E\\left[\\frac{\\partial^2 \\ell(X; \\mathbf{z})}{\\partial \\mathbf{z} \\partial \\mathbf{z}^T}\\right]
+            I(\mathbf{\theta}) = E\left[ \left(\frac{\partial \ell(X; \mathbf{\theta})}{\partial \mathbf{\theta}}\right) \left(\frac{\partial \ell(X; \mathbf{\theta})}{\partial \mathbf{\theta}}\right)^T \right] = -E\left[\frac{\partial^2 \ell(X; \mathbf{\theta})}{\partial \mathbf{\theta} \partial \mathbf{\theta}^T}\right]
 
         Where:
 
-        - :math:`I(\\mathbf{z})` is the Fisher Information Matrix.
-        - :math:`\ell(X; \\mathbf{z})` is the log-likelihood of :math:`X`, given the latent variable vector :math:`\\mathbf{z}`.
-        - :math:`\\frac{\\partial \\ell(X; \\mathbf{z})}{\\partial \\mathbf{z}}` is the gradient vector of the first derivatives of the log-likelihood of :math:`X` with respect to :math:`\\mathbf{z}`.
-        - :math:`\\frac{\\partial^2 \\log f(X; \\mathbf{z})}{\\partial \\mathbf{z} \\partial \\mathbf{z}^T}` is the Hessian matrix of the second derivatives of the log-likelihood of :math:`X` with respect to :math:`\\mathbf{z}`.
+        - :math:`I(\mathbf{\theta})` is the Fisher Information Matrix.
+        - :math:`\ell(X; \mathbf{\theta})` is the log-likelihood of :math:`X`, given the latent variable vector :math:`\mathbf{\theta}`.
+        - :math:`\frac{\partial \ell(X; \mathbf{\theta})}{\partial \mathbf{\theta}}` is the gradient vector of the first derivatives of the log-likelihood of :math:`X` with respect to :math:`\mathbf{\theta}`.
+        - :math:`\frac{\partial^2 \log f(X; \mathbf{\theta})}{\partial \mathbf{\theta} \partial \mathbf{\theta}^T}` is the Hessian matrix of the second derivatives of the log-likelihood of :math:`X` with respect to :math:`\mathbf{\theta}`.
         
         For additional details, see :cite:t:`Chang2017`.
         """
         if degrees is not None and len(degrees) != self.model.latent_variables:
             raise ValueError("There must be one degree for each latent variable.")
 
-        probabilities = self.model.item_probabilities(z.clone())
-        gradients = self.model.probability_gradients(z).detach()
-        if scale == "bit":
-            bit_z_gradients = self.bit_score_gradients(z, one_dimensional=False, **kwargs)
-            # we divide by diagonal of the bit score gradients (the gradients in the direction of the bit score corresponding z scores)
-            bit_z_gradients_diag = torch.einsum('...ii->...i', bit_z_gradients)
-            gradients = (gradients.permute(1, 2, 0, 3) / bit_z_gradients_diag).permute(2, 0, 1, 3)
+        probabilities = self.model.item_probabilities(theta.clone())
+        gradients = self.model.probability_gradients(theta).detach()
+        bit_theta_gradients = self.bit_score_gradients(theta, one_dimensional=False, **kwargs)
+        # we divide by diagonal of the bit score gradients (the gradients in the direction of the bit score corresponding theta scores)
+        bit_theta_gradients_diag = torch.einsum("...ii->...i", bit_theta_gradients)
+        gradients = (gradients.permute(1, 2, 0, 3) / bit_theta_gradients_diag).permute(2, 0, 1, 3)
 
         # squared gradient matrices for each latent variable
         # Uses einstein summation with batch permutation ...
         squared_grad_matrices = torch.einsum("...i,...j->...ij", gradients, gradients)
         information_matrices = squared_grad_matrices / probabilities.unsqueeze(-1).unsqueeze(-1).expand_as(squared_grad_matrices)
         information_matrices = information_matrices.nansum(dim=2) # sum over item categories
 
-        if degrees is not None and z.shape[1] > 1:
+        if degrees is not None and theta.shape[1] > 1:
             cos_degrees = torch.tensor(degrees).float().deg2rad_().cos_()
-            # For each z and item: Matrix multiplication cos_degrees^T @ information_matrix @ cos_degrees
-            information = torch.einsum('i,...ij,j->...', cos_degrees, information_matrices, cos_degrees)
+            # For each theta and item: Matrix multiplication cos_degrees^T @ information_matrix @ cos_degrees
+            information = torch.einsum("i,...ij,j->...", cos_degrees, information_matrices, cos_degrees)
         else:
             information = information_matrices
 
         if item:
             return information
         else:
             return information.nansum(dim=1) # sum over items
 
-    def _inverted_scales(self, train_z):
+    def _compute_1d_bit_scores(self, theta_adjusted, start_theta_adjusted, grid_start, grid_end, inverted_scale, grid_points):
         """
-        Compute a tensor with information about whether each latent variable is positively or negatively related to the test scores.
+        Computes the 1D bit scores for the given input theta scores.
 
         Parameters
         ----------
-        train_z : torch.Tensor
-            The training data in the latent space.
-
-        Returns
-        -------
-        torch.Tensor
-            A one row tensor with elements corresponding to latent variables. 1's for positive and -1's for negative relationships.
-
-        Notes
-        -----
-        If the neural network is set to handle multiple choice correct answers, 
-        the method computes the scores based on the correct responses. 
-        Otherwise, it simply sums up the training data. 
-        The method then performs a linear regression between the latent variables 
-        and the scores, and inverts the scales based on the linear weights.
-        """
-        scores = self.model.expected_scores(train_z).sum(dim=1).reshape(-1, 1)
-        linear_weights = linear_regression(train_z, scores)[1:]
-        inverted_scale = torch.where(linear_weights < 0, torch.tensor(-1), torch.tensor(1)).reshape(1, -1)
-        return inverted_scale
-
-    def _anti_invert_and_adjust_z_scores(self, z, train_z, start_z, inverted_scale):
-        """
-        Adjust the input and training z scores based on the starting z scores and the inverted scale.
-
-        Parameters
-        ----------
-        z : torch.Tensor
-            The input z scores.
-        train_z : torch.Tensor
-            The training z scores.
-        start_z : torch.Tensor
-            The starting z scores.
-        inverted_scale : torch.Tensor
-            The inverted scale.
-
-        Returns
-        -------
-        tuple of torch.Tensor
-            The adjusted input z scores, the adjusted training z scores and the adjusted starting z scores.
-
-        Notes
-        -----
-        The method first anti-inverts the z scores by multiplying them with the inverted scale. 
-        Then, If the anti-inverted z scores are smaller than the starting z scores, we set them to the starting z scores.
-        """
-        start_z_adjusted = start_z * inverted_scale
-        z_adjusted = torch.max(z * inverted_scale, start_z_adjusted)
-        train_z_adjusted = torch.max(train_z * inverted_scale, start_z_adjusted)
-
-        return z_adjusted, train_z_adjusted, start_z_adjusted
-
-    def _get_grid_boundaries(self, train_z_adjusted: torch.tensor, start_z_adjusted):
-        """
-        Determines the start and end points of the grid used for computing bit scores.
-
-        Parameters
-        ----------
-        train_z_adjusted : torch.Tensor
-            A 2D array containing the adjusted z scores of the training data. Each row represents one respondent, and each column represents a latent variable.
-        start_z_adjusted : torch.Tensor
-            A 1 row tensor containing starting z scores for the bit scores.
-
-        Returns
-        -------
-        grid_start : torch.Tensor
-            A 1D tensor containing the start points of the grid for each latent variable.
-        grid_end : torch.Tensor
-            A 1D tensor containing the end points of the grid for each latent variable.
-        start_is_outlier : torch.Tensor
-            A 1 row boolean tensor where each column corresponds to one latent variable. True if the starting z score is an outlier.
-        """        
-        outlier_detector = OutlierDetector(factor=4)
-        start_is_outlier = outlier_detector.is_outlier(start_z_adjusted, data=train_z_adjusted, lower=True)[0, :]
-        if any(start_is_outlier):
-            smallest_non_outlier = outlier_detector.smallest_largest_non_outlier(train_z_adjusted, smallest=True)
-            grid_start = torch.max(start_z_adjusted, smallest_non_outlier)
-        else:
-            grid_start = start_z_adjusted
-        grid_end = outlier_detector.smallest_largest_non_outlier(train_z_adjusted, smallest=False)
-        return grid_start, grid_end, start_is_outlier
-
-    def _compute_1d_bit_scores(self, z_adjusted, start_z_adjusted, grid_start, grid_end, inverted_scale, grid_points):
-        """
-        Computes the 1D bit scores for the given input z scores.
-
-        Parameters
-        ----------
-        z_adjusted : torch.Tensor
-            The adjusted z-scores. A 2D tensor.
-        start_z_adjusted : torch.Tensor
-            The adjusted z-scores for the starting point. A one row tensor.
+        theta_adjusted : torch.Tensor
+            The adjusted theta-scores. A 2D tensor.
+        start_theta_adjusted : torch.Tensor
+            The adjusted theta-scores for the starting point. A one row tensor.
         grid_start : torch.Tensor
             The start of the grid. A one row tensor.
         grid_end : torch.Tensor
             The end of the grid. A one row tensor.
         inverted_scale : torch.Tensor
             The inverted scale. A one row tensor with -1 for latent variables inversely related to the test scores and 1 for others.
         grid_points : int
             The number of grid points.
 
         Returns
         -------
         torch.Tensor
             The computed 1D bit scores.
         """
-        # Limit all z_scores to be within the grid range
-        z_adjusted_capped = torch.clamp(z_adjusted, grid_start, grid_end)
+        # Limit all theta_scores to be within the grid range
+        theta_adjusted_capped = torch.clamp(theta_adjusted, grid_start, grid_end)
         
         grid_linespace = torch.linspace(0, 1, steps=grid_points).unsqueeze(-1)
         # Use broadcasting to compute the grid
-        grid = grid_start + (grid_linespace * (z_adjusted_capped - grid_start).unsqueeze(1))
+        grid = grid_start + (grid_linespace * (theta_adjusted_capped - grid_start).unsqueeze(1))
 
-        # set the entire grid for those below the grid to their z scores
-        below_grid_start_mask = z_adjusted < grid_start
-        grid = torch.where(below_grid_start_mask.unsqueeze(1), z_adjusted.unsqueeze(1), grid)
+        # set the entire grid for those below the grid to their theta scores
+        below_grid_start_mask = theta_adjusted < grid_start
+        grid = torch.where(below_grid_start_mask.unsqueeze(1), theta_adjusted.unsqueeze(1), grid)
 
-        # Ensure all values are larger than start_z_adjusted
-        grid = torch.maximum(grid, start_z_adjusted)
+        # Ensure all values are larger than start_theta_adjusted
+        grid = torch.maximum(grid, start_theta_adjusted)
 
-        # set the last slot in each grid to the outliers z scores
-        grid[:, -1, :] = torch.where(z_adjusted > grid_end, z_adjusted, grid[:, -1])
-        # set the first slot in each grid to the start_z_adjusted (required when z_adjusted is an outlier)
-        grid[:, 0, :] = start_z_adjusted.squeeze()
+        # set the last slot in each grid to the outliers theta scores
+        grid[:, -1, :] = torch.where(theta_adjusted > grid_end, theta_adjusted, grid[:, -1])
+        # set the first slot in each grid to the start_theta_adjusted (required when theta_adjusted is an outlier)
+        grid[:, 0, :] = start_theta_adjusted.squeeze()
 
-        # convert back to non-inverted z scale and compute grid entropies
+        # convert back to non-inverted theta scale and compute grid entropies
         grid = grid.view(-1, grid.shape[2]) * inverted_scale
         output = self.model(grid)
         entropies = output_to_item_entropy(output, self.model.modeled_item_responses)
         # the goal is to get the entropies to the dimensions required for bit_score_distance
         # we need to transpose for view to order them correctly
         # and change positioning of each dimension in the end using permute
         entropies = (
@@ -1054,69 +568,159 @@
         diff = torch.abs(entropies - torch.roll(entropies, shifts=1, dims=2))
         # Note that for each sub-tensor in the third dimension, the first element will
         # be the difference with the last element of the previous sub-tensor because
         # of the roll function. We set this to 0
         diff[:, :, 0] = 0
         return diff.sum(dim=(1, 2)).unsqueeze(1)
 
-    def _compute_multi_dimensional_bit_scores(self, z_adjusted, start_z_adjusted, train_z_adjusted, grid_start, grid_end, inverted_scale, grid_points):
+    def _compute_multi_dimensional_bit_scores(self, theta_adjusted, start_theta_adjusted, train_theta_adjusted, grid_start, grid_end, inverted_scale, grid_points):
         """
-        Computes the multi-dimensional bit scores for the given input z scores.
+        Computes the multi-dimensional bit scores for the given input theta scores.
 
         Parameters
         -----------
-        z_adjusted : torch.Tensor
-            The input z scores.
-        start_z_adjusted : torch.Tensor
-            The minimum z score to be used in the grid. A one row tensor.
-        train_z_adjusted : torch.Tensor
-            The z scores of the training data. Used for computing the median of each latent variable.
+        theta_adjusted : torch.Tensor
+            The input theta scores.
+        start_theta_adjusted : torch.Tensor
+            The minimum theta score to be used in the grid. A one row tensor.
+        train_theta_adjusted : torch.Tensor
+            The theta scores of the training data. Used for computing the median of each latent variable.
         grid_start : float
             The minimum value of the grid. A one row tensor.
         grid_end : float
             The maximum value of the grid. A one row tensor.
         inverted_scale : torch.Tensor
             The inverted scale. A one row tensor with -1 for latent variables inversely related to the test scores and 1 for others.
         grid_points : int
             The number of points in the grid.
 
         Returns
         --------
         bit_scores : torch.Tensor
-            The multi-dimensional bit scores for the input z scores.
+            The multi-dimensional bit scores for the input theta scores.
         """
         # Construct grid
         ratio = torch.linspace(0, 1, steps=grid_points).view(-1, 1)
         grid = (1 - ratio) * grid_start + ratio * grid_end
-        # Add z scores to the grid and sort the columns
-        grid = torch.cat([grid, z_adjusted], dim=0)
-        # set all z scores smaller than start_z_adjusted to start_z_adjusted
-        grid = torch.max(grid, start_z_adjusted)
-        # set the first slot in each grid to the start_z_adjusted
-        # required when any value in z_adjusted is an outlier
-        grid[0, :] = start_z_adjusted
+        # Add theta scores to the grid and sort the columns
+        grid = torch.cat([grid, theta_adjusted], dim=0)
+        # set all theta scores smaller than start_theta_adjusted to start_theta_adjusted
+        grid = torch.max(grid, start_theta_adjusted)
+        # set the first slot in each grid to the start_theta_adjusted
+        # required when any value in theta_adjusted is an outlier
+        grid[0, :] = start_theta_adjusted
 
         grid, sorted_indices = torch.sort(grid, dim=0)
         # Fill each column in grid we are not not computing bit scores for with the median
-        median, _ = torch.median(train_z_adjusted, dim=0)
-        bit_scores = torch.zeros_like(z_adjusted)
-        for z_var in range(grid.shape[1]):
+        median, _ = torch.median(train_theta_adjusted, dim=0)
+        bit_scores = torch.zeros_like(theta_adjusted)
+        for theta_var in range(grid.shape[1]):
             # Only compute once per unique value
-            unique_grid, inverse_indices = grid[:, z_var].unique(return_inverse=True)
+            unique_grid, inverse_indices = grid[:, theta_var].unique(return_inverse=True)
             latent_variable_grid = median.repeat(unique_grid.shape[0], 1)
-            latent_variable_grid[:, z_var] = unique_grid
+            latent_variable_grid[:, theta_var] = unique_grid
 
-            # Convert back to non-inverted z scale and compute grid entropies
+            # Convert back to non-inverted theta scale and compute grid entropies
             output = self.model(latent_variable_grid * inverted_scale)
             entropies = output_to_item_entropy(output, self.model.modeled_item_responses)
 
             # Compute the absolute difference between each grid point entropy and the previous one
             diff = torch.zeros_like(entropies)
             diff[1:,:] = torch.abs(entropies[:-1, :] - entropies[1:, :])
 
             # cummulative sum over grid points and then sum the item scores
             bit_score_grid = diff.sum(dim=1).cumsum(dim=0)
 
-            # add duplicates, unsort and take only the bit scores for the input z scores
-            bit_scores[:, z_var] = bit_score_grid[inverse_indices][torch.sort(sorted_indices[:, z_var])[1]][-z_adjusted.shape[0]:]
+            # add duplicates, unsort and take only the bit scores for the input theta scores
+            bit_scores[:, theta_var] = bit_score_grid[inverse_indices][torch.sort(sorted_indices[:, theta_var])[1]][-theta_adjusted.shape[0]:]
             
         return bit_scores
+
+
+    def _inverted_scales(self, train_theta):
+        """
+        Compute a tensor with information about whether each latent variable is positively or negatively related to the test scores.
+
+        Parameters
+        ----------
+        train_theta : torch.Tensor
+            The training data in the latent space.
+
+        Returns
+        -------
+        torch.Tensor
+            A one row tensor with elements corresponding to latent variables. 1's for positive and -1's for negative relationships.
+
+        Notes
+        -----
+        If the neural network is set to handle multiple choice correct answers, 
+        the method computes the scores based on the correct responses. 
+        Otherwise, it simply sums up the training data. 
+        The method then performs a linear regression between the latent variables 
+        and the scores, and inverts the scales based on the linear weights.
+        """
+        scores = self.model.expected_scores(train_theta).sum(dim=1).reshape(-1, 1)
+        linear_weights = linear_regression(train_theta, scores)[1:]
+        inverted_scale = torch.where(linear_weights < 0, torch.tensor(-1), torch.tensor(1)).reshape(1, -1)
+        return inverted_scale
+
+    def _anti_invert_and_adjust_theta_scores(self, theta, train_theta, start_theta, inverted_scale):
+        """
+        Adjust the input and training theta scores based on the starting theta scores and the inverted scale.
+
+        Parameters
+        ----------
+        theta : torch.Tensor
+            The input theta scores.
+        train_theta : torch.Tensor
+            The training theta scores.
+        start_theta : torch.Tensor
+            The starting theta scores.
+        inverted_scale : torch.Tensor
+            The inverted scale.
+
+        Returns
+        -------
+        tuple of torch.Tensor
+            The adjusted input theta scores, the adjusted training theta scores and the adjusted starting theta scores.
+
+        Notes
+        -----
+        The method first anti-inverts the theta scores by multiplying them with the inverted scale. 
+        Then, If the anti-inverted theta scores are smaller than the starting theta scores, we set them to the starting theta scores.
+        """
+        start_theta_adjusted = start_theta * inverted_scale
+        theta_adjusted = torch.max(theta * inverted_scale, start_theta_adjusted)
+        train_theta_adjusted = torch.max(train_theta * inverted_scale, start_theta_adjusted)
+
+        return theta_adjusted, train_theta_adjusted, start_theta_adjusted
+
+
+    def _get_grid_boundaries(self, train_theta_adjusted: torch.Tensor, start_theta_adjusted):
+        """
+        Determines the start and end points of the grid used for computing bit scores.
+
+        Parameters
+        ----------
+        train_theta_adjusted : torch.Tensor
+            A 2D array containing the adjusted theta scores of the training data. Each row represents one respondent, and each column represents a latent variable.
+        start_theta_adjusted : torch.Tensor
+            A 1 row tensor containing starting theta scores for the bit scores.
+
+        Returns
+        -------
+        grid_start : torch.Tensor
+            A 1D tensor containing the start points of the grid for each latent variable.
+        grid_end : torch.Tensor
+            A 1D tensor containing the end points of the grid for each latent variable.
+        start_is_outlier : torch.Tensor
+            A 1 row boolean tensor where each column corresponds to one latent variable. True if the starting theta score is an outlier.
+        """        
+        outlier_detector = OutlierDetector(factor=4)
+        start_is_outlier = outlier_detector.is_outlier(start_theta_adjusted, data=train_theta_adjusted, lower=True)[0, :]
+        if any(start_is_outlier):
+            smallest_non_outlier = outlier_detector.smallest_largest_non_outlier(train_theta_adjusted, smallest=True)
+            grid_start = torch.max(start_theta_adjusted, smallest_non_outlier)
+        else:
+            grid_start = start_theta_adjusted
+        grid_end = outlier_detector.smallest_largest_non_outlier(train_theta_adjusted, smallest=False)
+        return grid_start, grid_end, start_is_outlier
```

### Comparing `irtorch-0.0.4/irtorch/latent_variable_functions.py` & `irtorch-0.1.0/irtorch/latent_variable_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import torch
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 def interp(x_new, x, y):
     """
     Linear interpolation function with simple linear extrapolation at edges
 
     Parameters
     ----------
```

### Comparing `irtorch-0.0.4/irtorch/layers.py` & `irtorch-0.1.0/irtorch/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import torch
 from torch import nn
 import torch.nn.functional as F
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 class SoftplusLinear(nn.Module):
     """
     A linear layer with positive weights ensured using the softplus function. Should be more stable than squaring and maintains gradients in contrast to clipping/abs.
     """
 
     def __init__(
@@ -123,34 +123,34 @@
         else:
             weight[self.free_weight] = self.raw_weight_param
         bias[self.free_bias] = self.bias_param
         output = F.linear(x, weight, bias)
         return output
 
 class NegationLayer(nn.Module):
-    def __init__(self, item_z_relationships: torch.Tensor, inputs_per_items: int, zero_outputs: torch.Tensor):
+    def __init__(self, item_theta_relationships: torch.Tensor, inputs_per_items: int, zero_outputs: torch.Tensor):
         """
         Parameters
         ----------
-        item_z_relationships : torch.Tensor
+        item_theta_relationships : torch.Tensor
             An integer tensor of shape (items,) that determines for which weights should be trained. Mostly used for training multidimensional IRT models for which each item or item category has a separate network and some of the item/latent variable relationships are set to be 0.
         inputs_per_items : int
             Number of inputs per item. One weight for all inputs per item.
         zero_outputs : torch.Tensor
             A boolean tensor of shape (out_features,) that determines which outputs should be 0. Typically used for the final layer for IRT models with polytomously scored items where different items have differing number of response categories. Items with fewer categories should set the outputs for nonexisting categories to 0.
         """
         super().__init__()
 
         self.inputs_per_items = inputs_per_items
-        self.item_z_relationships = item_z_relationships
+        self.item_theta_relationships = item_theta_relationships
         self.zero_outputs = zero_outputs
-        self.zero_weights = (1-item_z_relationships).repeat_interleave(inputs_per_items).bool()
-        self.register_buffer("weight", torch.zeros(item_z_relationships.numel() * inputs_per_items))
+        self.zero_weights = (1-item_theta_relationships).repeat_interleave(inputs_per_items).bool()
+        self.register_buffer("weight", torch.zeros(item_theta_relationships.numel() * inputs_per_items))
         # One weight for each item related to the latent variable
-        self.weight_param = nn.Parameter(torch.Tensor(sum(item_z_relationships).item()))
+        self.weight_param = nn.Parameter(torch.Tensor(sum(item_theta_relationships).item()))
         self.reset_parameters()
 
     def reset_parameters(self):
         nn.init.zeros_(self.weight_param)
 
     def forward(self, x: torch.Tensor):
         # break the gradients for weights for non-used categories
@@ -163,11 +163,11 @@
     def all_item_weights(self):
         """
         Returns
         -------
         weight : torch.Tensor
             All layer weights, including the unused ones.
         """
-        weights = torch.zeros(self.item_z_relationships.numel())
-        mask = (1 - self.item_z_relationships).bool()
+        weights = torch.zeros(self.item_theta_relationships.numel())
+        mask = (1 - self.item_theta_relationships).bool()
         weights[~mask] = self.weight_param
         return weights
```

### Comparing `irtorch-0.0.4/irtorch/load_dataset.py` & `irtorch-0.1.0/irtorch/load_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 from importlib import resources
 import torch
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 def swedish_national_mathematics_2() -> torch.Tensor:
     """
     Load the second Swedish National Mathematics dataset.
 
     Returns
     -------
     torch.Tensor
         The loaded dataset.
     """
     try:
-        file_path = resources.files('irtorch') / 'datasets' / 'national_mathematics' / 'mathematics_2.pt'
+        file_path = resources.files("irtorch") / "datasets" / "national_mathematics" / "mathematics_2.pt"
         data = torch.load(file_path)
     except Exception as e:
         raise RuntimeError("Failed to load data") from e
     return data
 
 def swedish_national_mathematics_1() -> torch.Tensor:
     """
@@ -26,15 +26,15 @@
 
     Returns
     -------
     torch.Tensor
         The loaded dataset.
     """
     try:
-        file_path = resources.files('irtorch') / 'datasets' / 'national_mathematics' / 'mathematics_1.pt'
+        file_path = resources.files("irtorch") / "datasets" / "national_mathematics" / "mathematics_1.pt"
         data = torch.load(file_path)
     except Exception as e:
         raise RuntimeError("Failed to load data") from e
     return data
 
 def swedish_sat_verbal() -> tuple[torch.Tensor, list[int]]:
     """
@@ -42,21 +42,21 @@
 
     Returns
     -------
     tuple (torch.Tensor, list[int])
         A tuple containing the loaded dataset and the correct item responses.
     """
     try:
-        file_path = resources.files('irtorch') / 'datasets' / 'swedish_sat' / 'swesat22b_nominal_verb.pt'
+        file_path = resources.files("irtorch") / "datasets" / "swedish_sat" / "swesat22b_nominal_verb.pt"
         data = torch.load(file_path)
     except Exception as e:
         raise RuntimeError("Failed to load data") from e
 
     try:
-        with resources.files('irtorch').joinpath('datasets/swedish_sat/swesat22b_verb_correct.txt').open('r', encoding='utf-8') as file:
+        with resources.files("irtorch").joinpath("datasets/swedish_sat/swesat22b_verb_correct.txt").open("r", encoding="utf-8") as file:
             correct_category = file.read().replace("\n", "")
             correct_category = [int(char) for char in correct_category if char.isdigit()]
     except Exception as e:
         raise RuntimeError("Failed to load correct item responses") from e
 
     return data - 1, correct_category
 
@@ -66,21 +66,21 @@
 
     Returns
     -------
     tuple (torch.Tensor, list[int])
         A tuple containing the loaded dataset and the correct item responses.
     """
     try:
-        file_path = resources.files('irtorch') / 'datasets' / 'swedish_sat' / 'swesat22b_nominal_quant.pt'
+        file_path = resources.files("irtorch") / "datasets" / "swedish_sat" / "swesat22b_nominal_quant.pt"
         data = torch.load(file_path)
     except Exception as e:
         raise RuntimeError("Failed to load data") from e
 
     try:
-        with resources.files('irtorch').joinpath('datasets/swedish_sat/swesat22b_quant_correct.txt').open('r', encoding='utf-8') as file:
+        with resources.files("irtorch").joinpath("datasets/swedish_sat/swesat22b_quant_correct.txt").open("r", encoding="utf-8") as file:
             correct_category = file.read().replace("\n", "")
             correct_category = [int(char) for char in correct_category if char.isdigit()]
     except Exception as e:
         raise RuntimeError("Failed to load correct item responses") from e
 
     return data - 1, correct_category
 
@@ -127,14 +127,14 @@
 
     Returns
     -------
     torch.Tensor
         The loaded dataset.
     """
     try:
-        file_path = resources.files('irtorch') / 'datasets' / 'big_five' / 'big_five.pt'
+        file_path = resources.files("irtorch") / "datasets" / "big_five" / "big_five.pt"
         data = torch.load(file_path)
     except Exception as e:
         raise RuntimeError("Failed to load data") from e
 
-    data[data == 0] = float('nan')
+    data[data == 0] = float("nan")
     return data - 1
```

### Comparing `irtorch-0.0.4/irtorch/models/generalized_partial_credit.py` & `irtorch-0.1.0/irtorch/models/two_parameter_logistic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,96 +1,98 @@
 import pandas as pd
 import torch
 import torch.nn as nn
 from irtorch.models.base_irt_model import BaseIRTModel
 
-class GeneralizedPartialCredit(BaseIRTModel):
-    """
-    Generalized Partial Credit IRT model.
+class TwoParameterLogistic(BaseIRTModel):
+    r"""
+    Two parametric logistic (2PL) IRT model.
 
     Parameters
     ----------
     latent_variables : int
         Number of latent variables.
-    item_categories : list[int]
-        Number of categories for each item. One integer for each item. Missing responses exluded.
-    item_z_relationships : torch.Tensor, optional
+    items : int
+        Number of items.
+    item_theta_relationships : torch.Tensor, optional
         A boolean tensor of shape (items, latent_variables). If specified, the model will have connections between latent dimensions and items where the tensor is True. If left out, all latent variables and items are related (Default: None)
+    
+    Notes
+    -----
+    For an item :math:`j`, the model defines the probability for responding correctly as:
+
+    .. math::
+
+        \frac{
+            \exp(\mathbf{a}_j^\top \mathbf{\theta} + d_j)
+        }{
+            1+\exp(\mathbf{a}_j^\top \mathbf{\theta} + d_j)
+        },
+
+    where:
+
+    - :math:`\mathbf{\theta}` is a vector of latent variables.
+    - :math:`\mathbf{a}_j` is a vector of weights for item :math:`j`.
+    - :math:`d_j` is the bias term for item :math:`j`.
     """
     def __init__(
         self,
         latent_variables: int,
-        item_categories: list[int],
-        item_z_relationships: torch.Tensor = None,
+        items: int,
+        item_theta_relationships: torch.Tensor = None
     ):
-        super().__init__(latent_variables=latent_variables, item_categories=item_categories)
-        if item_z_relationships is not None:
-            if item_z_relationships.shape != (len(item_categories), latent_variables):
+        super().__init__(latent_variables=latent_variables, item_categories = [2] * items)
+        if item_theta_relationships is not None:
+            if item_theta_relationships.shape != (items, latent_variables):
                 raise ValueError(
-                    f"latent_item_connections must have shape ({len(item_categories)}, {latent_variables})."
+                    f"latent_item_connections must have shape ({items}, {latent_variables})."
                 )
-            assert(item_z_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
-            assert(torch.all(item_z_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
+            assert(item_theta_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
+            assert(torch.all(item_theta_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
 
-        self.output_size = self.items * self.max_item_responses
+        self.output_size = self.items * 2
+        self.weight_param = nn.Parameter(torch.zeros(item_theta_relationships.sum().int()))
+        self.bias_param = nn.Parameter(torch.zeros(self.items))
 
-        free_weights = torch.ones(self.items, latent_variables)
-        self.register_buffer("gpc_weight_multiplier", torch.arange(0, self.max_item_responses).repeat(self.items))
-        if item_z_relationships is not None:
-            for item, item_cat in enumerate(self.modeled_item_responses):
-                free_weights[item, :] = item_z_relationships[item, :]
-
-        self.weight_param = nn.Parameter(torch.zeros(free_weights.sum().int()))
-
-        number_of_bias_parameters = sum(self.modeled_item_responses) - self.items
-        self.bias_param = nn.Parameter(torch.zeros(number_of_bias_parameters))
-        first_category = torch.zeros(self.items, self.max_item_responses)
+        first_category = torch.zeros(self.items, 2)
         first_category[:, 0] = 1.0
         first_category = first_category.reshape(-1)
-        missing_category = torch.zeros(self.items, self.max_item_responses)
-        for item, item_cat in enumerate(self.modeled_item_responses):
-            missing_category[item, item_cat:self.max_item_responses] = 1.0
-        missing_category = missing_category.reshape(-1)
-        free_bias = (1 - first_category) * (1 - missing_category)
-        self.register_buffer("free_weights", free_weights.bool())
+
+        free_bias = 1 - first_category
+        self.register_buffer("free_weights", item_theta_relationships.bool())
         self.register_buffer("free_bias", free_bias.bool())
-        self.register_buffer("missing_category", missing_category.bool())
         self.register_buffer("first_category", first_category.bool())
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         nn.init.normal_(self.weight_param, mean=1., std=0.01)
         nn.init.zeros_(self.bias_param)
     
-    def forward(self, z: torch.Tensor) -> torch.Tensor:
+    def forward(self, theta: torch.Tensor) -> torch.Tensor:
         """
         Forward pass of the model.
 
         Parameters
         ----------
-        z : torch.Tensor
+        theta : torch.Tensor
             2D tensor with latent variables. Rows are respondents and latent variables are columns. 
 
         Returns
         -------
         output : torch.Tensor
             2D tensor. Rows are respondents and columns are item category logits.
         """
-        bias = torch.zeros(self.output_size, device=z.device)
+        bias = torch.zeros(self.output_size, device=theta.device)
         bias[self.free_bias] = self.bias_param
         
-        weights = torch.zeros(self.items, self.latent_variables, device=z.device)
+        weights = torch.zeros(self.items, self.latent_variables, device=theta.device)
         weights[self.free_weights] = self.weight_param
-        weighted_z = torch.matmul(z, weights.T).repeat_interleave(self.max_item_responses, dim=1)
-        weighted_z *= self.gpc_weight_multiplier
-
-        output = weighted_z + bias
-        # stop gradients from flowing through the missing categories
-        output[:, self.missing_category] = -torch.inf
+        weighted_theta = torch.matmul(theta, weights.T).repeat_interleave(self.max_item_responses, dim=1)
 
+        output = weighted_theta + bias
         output[:, self.first_category] = 0
 
         return output
 
     def item_parameters(self, irt_format = False) -> pd.DataFrame:
         """
         Get the item parameters for a fitted model.
@@ -101,44 +103,45 @@
             Only for unidimensional models. Whether to return the item parameters in traditional IRT format. Otherwise returns weights and biases. (default is False)
 
         Returns
         -------
         pd.DataFrame
             A dataframe with the item parameters.
         """
-        biases = torch.zeros(self.output_size)
-        biases[self.free_bias] = self.bias_param
-        biases = biases.reshape(-1, self.max_item_responses)
-
+        if irt_format and self.latent_variables > 1:
+            raise ValueError("IRT format is only available for unidimensional models.")
+        
+        biases = self.bias_param
+        biases = biases.reshape(-1, 1)
         weights = torch.zeros(self.items, self.latent_variables)
         weights[self.free_weights] = self.weight_param
 
         weights_df = pd.DataFrame(weights.detach().numpy())
-        if irt_format and self.latent_variables == 1:
+        if irt_format:
             weights_df.columns = [f"a{i+1}" for i in range(weights.shape[1])]
-            biases_df = pd.DataFrame(-(weights*biases).detach()[:, 1:].numpy())
+            biases_df = pd.DataFrame(-(weights*biases).detach().numpy())
         else:
             weights_df.columns = [f"w{i+1}" for i in range(weights.shape[1])]
             biases_df = pd.DataFrame(biases.detach().numpy())
             
-        biases_df.columns = [f"b{i+1}" for i in range(biases_df.shape[1])]
+        biases_df.columns = ["b1"]
         parameters = pd.concat([weights_df, biases_df], axis=1)
 
         return parameters
 
     @torch.inference_mode()
-    def item_z_relationship_directions(self, z:torch.Tensor = None) -> torch.Tensor:
+    def item_theta_relationship_directions(self, theta:torch.Tensor = None) -> torch.Tensor:
         """
         Get the relationship directions between each item and latent variable for a fitted model.
 
         Parameters
         ----------
-        z : torch.Tensor, optional
+        theta : torch.Tensor, optional
             Not needed for this model. (default is None)
-
+            
         Returns
         -------
         torch.Tensor
             A 2D tensor with the relationships between the items and latent variables. Items are rows and latent variables are columns.
         """
         weights = torch.zeros(self.items, self.latent_variables)
         weights[self.free_weights] = self.weight_param
```

### Comparing `irtorch-0.0.4/irtorch/models/monotone_nn.py` & `irtorch-0.1.0/irtorch/models/monotone_nn.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,100 +2,110 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from irtorch.models.base_irt_model import BaseIRTModel
 from irtorch.layers import SoftplusLinear, NegationLayer
 from irtorch.activation_functions import BoundedELU
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 class MonotoneNN(BaseIRTModel):
-    """
+    r"""
     Nonparametric Monotone Neural Network IRT model.
-    The model is a feedforward neural network with a separate monotone nonparametric latent variable weight function for each item or item category.
+    The model is a feedforward neural network separate monotone functions for each item or item category.
 
     If mc_correct is specified, the latent variable effect for the correct item response is a cumulative sum of the effects for the other possible item responses to ensure monotonicity. This model is also referred to as the Monotone Multiple Choice Neural Network (MMCNN) model.
     
     If mc_correct is not specified, the item response categories are treated as ordered, and the latent variable effect for an item response category is the cumulative sum of the effects for the lower categories.
 
     Parameters
     ----------
-    latent_variables : int
-        Number of latent variables.
-    item_categories : list[int]
-        Number of categories for each item. One integer for each item. Missing responses exluded.
+    latent_variables : int, optional
+        Number of latent variables. (default is 1)
+    data: torch.Tensor, optional
+        A 2D torch tensor with test data. Used to automatically compute item_categories. Columns are items and rows are respondents. (default is None)
+    item_categories : list[int], optional
+        Number of categories for each item. One integer for each item. Missing responses exluded. (default is None)
     hidden_dim : list[int]
         Number of neurons in each hidden layer. For separate='items' or separate='categories', each element is the number of neurons for each separate item or category. For separate='none', each element is the number of neurons for each layer. Needs to be a multiple of 3 is when use_bounded_activation=True and a multiple of 2 when use_bounded_activation=False.
     model_missing : bool, optional
         Whether to model missing item responses as separate item response categories. (Default: False)
     mc_correct : list[int], optional
         The correct response category for each item. (Default: None)
     separate : str, optional
         Whether to fit separate latent trait weight functions for items or items categories. Can be 'items' or 'categories'. 
         Note that 'categories' results in a more flexible model with more parameters. (Default: 'categories')
-    item_z_relationships : torch.Tensor, optional
+    item_theta_relationships : torch.Tensor, optional
         A boolean tensor of shape (items, latent_variables). If specified, the model will have connections between latent dimensions and items where the tensor is True. If left out, all latent variables and items are related (Default: None)
     negative_latent_variable_item_relationships : bool, optional
         Whether to allow for negative latent variable item relationships. (Default: True)
     use_bounded_activation : bool, optional
         Whether to use bounded activation functions. (Default: True)
 
     Notes
     -----
-    For an item :math:`j` with :math:`m=0, 1, 2, \\ldots, M_j` possible item responses/scores, the model defines the probability for responding with a score of :math:`x` as follows (selecting response option :math:`x` for multiple choice items):
+    For an item :math:`j` with :math:`m=0, 1, 2, \ldots, M_j` possible item responses/scores, the model defines the probability for responding with a score of :math:`x` as follows (selecting response option :math:`x` for multiple choice items):
 
     .. math::
 
-        P(X_j=x | \\mathbf{z}) = \\frac{
-            \\exp(z_{jx}(\\mathbf{z}))
+        P(X_j=x | \mathbf{\theta}) = \frac{
+            \exp(\delta_{jx}(\mathbf{\theta}))
         }{
-            \\sum_{m=0}^{M_j}
-                \\exp(z_{jm}(\\mathbf{z}))
+            \sum_{m=0}^{M_j}
+                \exp(\delta_{jm}(\mathbf{\theta}))
         },
 
     where:
 
-    - :math:`\\mathbf{z}` is a vector of latent variables.
+    - :math:`\mathbf{\theta}` is a vector of latent variables.
     - When mc_correct is not specified: 
-        - :math:`z_{jm}(\\mathbf{z}) = \\sum_{c=0}^{m}\\text{monotone}_{jc}(\\mathbf{z}) - b_{jm}`.
+        - :math:`\delta_{jm}(\mathbf{\theta}) = \sum_{c=0}^{m}\text{monotone}_{jc}(\mathbf{\theta}) + b_{jm}`.
     - When mc_correct is specified:
-        - :math:`z_{jm}(\\mathbf{z}) = \\text{monotone}_{jm}(\\mathbf{z}) - b_{jm}` for all incorrect response options, and :math:`z_{jm}(\\mathbf{z}) = \\sum_{c=0}^{M_j}\\text{monotone}_{jc}(\\mathbf{z}) - b_{jm}` for the correct response option.
-    - :math:`\\text{monotone}_{jm}(\\mathbf{z})` is a monotonic neural network with ELU based activation functions as per :cite:t:`Runje2023`.
+        - :math:`\delta_{jm}(\mathbf{\theta}) = \text{monotone}_{jm}(\mathbf{\theta}) + b_{jm}` for all incorrect response options, and :math:`\delta_{jm}(\mathbf{\theta}) = \sum_{c=0}^{M_j}\text{monotone}_{jc}(\mathbf{\theta}) + b_{jm}` for the correct response option.
+    - :math:`\text{monotone}_{jm}(\mathbf{\theta})` is a monotonic neural network with ELU based activation functions as per :cite:t:`Runje2023`.
     """
     def __init__(
         self,
-        latent_variables: int,
-        item_categories: list[int],
-        hidden_dim: list[int],
+        latent_variables: int = 1,
+        data: torch.Tensor = None,
+        item_categories: list[int] = None,
+        hidden_dim: list[int] = None,
         model_missing: bool = False,
         mc_correct: list[int] = None,
-        item_z_relationships: torch.Tensor = None,
+        item_theta_relationships: torch.Tensor = None,
         separate: str = "categories",
         negative_latent_variable_item_relationships: bool = True,
         use_bounded_activation: bool = True
     ):
+        if item_categories is None:
+            if data is None:
+                raise ValueError("Either an instantiated model, item_categories or data must be provided to initialize the model.")
+            else:
+                # replace nan with -inf to get max
+                item_categories = (torch.where(~data.isnan(), data, torch.tensor(float('-inf'))).max(dim=0).values + 1).int().tolist()
+                
         super().__init__(latent_variables, item_categories, mc_correct, model_missing)
-        if item_z_relationships is not None:
-            if item_z_relationships.shape != (len(item_categories), latent_variables):
+        if item_theta_relationships is not None:
+            if item_theta_relationships.shape != (len(item_categories), latent_variables):
                 raise ValueError(
                     f"latent_item_connections must have shape ({len(item_categories)}, {latent_variables})."
                 )
-            assert(item_z_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
-            assert(torch.all(item_z_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
+            assert(item_theta_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
+            assert(torch.all(item_theta_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
         else:
-            item_z_relationships = torch.tensor([[True] * latent_variables] * self.items, dtype=torch.bool)
+            item_theta_relationships = torch.tensor([[True] * latent_variables] * self.items, dtype=torch.bool)
         if hidden_dim is None:
             hidden_dim = [3]
         else:
             if use_bounded_activation and not all(x % 3 == 0 for x in hidden_dim):
                 raise ValueError("hidden_dim must be a multiple of 3 when use_bounded_activation=True")
             if not use_bounded_activation and not all(x % 2 == 0 for x in hidden_dim):
                 raise ValueError("hidden_dim must be a multiple of 2 when use_bounded_activation=False")
 
-        self.item_z_relationships = item_z_relationships
+        self.item_theta_relationships = item_theta_relationships
         self.separate = separate
         self.hidden_layers = len(hidden_dim)
         self.output_length = self.items * self.max_item_responses
         self.negative_latent_variable_item_relationships = negative_latent_variable_item_relationships
         self.use_bounded_activation = use_bounded_activation
         self.hidden_out_dim = hidden_dim[-1]
         if separate == "items":
@@ -114,99 +124,99 @@
         for item, item_cat in enumerate(self.modeled_item_responses):
             missing_categories[item, item_cat:self.max_item_responses] = 1
         missing_categories = missing_categories.reshape(-1)
         self.register_buffer("missing_categories", missing_categories.bool())
         self.register_buffer("free_bias", (1 - missing_categories).bool())
         self.bias_param = nn.Parameter(torch.zeros(sum(self.modeled_item_responses)))
 
-        for z_dim in range(latent_variables):
-            zero_outputs = 1 - item_z_relationships[:, z_dim].int()
+        for theta_dim in range(latent_variables):
+            zero_outputs = 1 - item_theta_relationships[:, theta_dim].int()
 
             # Input layer
             input_dim = 1
             if separate == "items":
                 output_dim = self.items * hidden_dim[0]
-                layer_zero_out = zero_outputs.repeat_interleave(hidden_dim[0])
+                layer_thetaero_out = zero_outputs.repeat_interleave(hidden_dim[0])
             elif separate == "categories":
                 output_dim = self.output_length * hidden_dim[0]
                 # missing categories output 0
                 missing_category_out = missing_categories.repeat_interleave(hidden_dim[0]).int()
-                layer_zero_out = zero_outputs.repeat_interleave(hidden_dim[0] * self.max_item_responses)
-                layer_zero_out = torch.bitwise_or(missing_category_out, layer_zero_out)
+                layer_thetaero_out = zero_outputs.repeat_interleave(hidden_dim[0] * self.max_item_responses)
+                layer_thetaero_out = torch.bitwise_or(missing_category_out, layer_thetaero_out)
 
-            self.add_module(f"linear0_dim{z_dim}", SoftplusLinear(input_dim, output_dim, zero_outputs=layer_zero_out))
+            self.add_module(f"linear0_dim{theta_dim}", SoftplusLinear(input_dim, output_dim, zero_outputs=layer_thetaero_out))
 
             # Hidden layers
             for i in range(1, len(hidden_dim)):
                 if separate == "items":
                     output_dim = self.items * hidden_dim[i]
-                    layer_zero_out = zero_outputs.repeat_interleave(hidden_dim[i])
+                    layer_thetaero_out = zero_outputs.repeat_interleave(hidden_dim[i])
                     separate_inputs = torch.tensor([hidden_dim[i - 1]] * self.items)
                     separate_outputs = torch.tensor([hidden_dim[i]] * self.items)
                     input_dim = hidden_dim[i - 1] * self.items
                 if separate == "categories":
                     output_dim = self.output_length * hidden_dim[i]
                     missing_category_out = missing_categories.repeat_interleave(hidden_dim[i]).int()
-                    layer_zero_out = zero_outputs.repeat_interleave(hidden_dim[i] * self.max_item_responses)
+                    layer_thetaero_out = zero_outputs.repeat_interleave(hidden_dim[i] * self.max_item_responses)
                     # missing categories output 0
-                    layer_zero_out = torch.bitwise_or(missing_category_out, layer_zero_out)
+                    layer_thetaero_out = torch.bitwise_or(missing_category_out, layer_thetaero_out)
                     separate_inputs = torch.tensor([hidden_dim[i - 1]] * self.output_length)
                     separate_outputs = torch.tensor([hidden_dim[i]] * self.output_length)
                     input_dim = hidden_dim[i - 1] * self.output_length
 
-                self.add_module(f"linear{i}_dim{z_dim}", SoftplusLinear(
+                self.add_module(f"linear{i}_dim{theta_dim}", SoftplusLinear(
                     input_dim,
                     output_dim,
                     separate_inputs=separate_inputs,
                     separate_outputs=separate_outputs,
-                    zero_inputs=getattr(self, f"linear{i-1}_dim{z_dim}").zero_outputs,
-                    zero_outputs=layer_zero_out,
+                    zero_inputs=getattr(self, f"linear{i-1}_dim{theta_dim}").zero_outputs,
+                    zero_outputs=layer_thetaero_out,
                 ))
 
             if negative_latent_variable_item_relationships:
                 inputs_per_items = 1 if separate == "items" else self.max_item_responses
                 missing_cats = self.missing_categories if separate == "categories" else torch.zeros(self.items, dtype=torch.bool)
                 item_relationships = 1 - zero_outputs
                 self.add_module(
-                    f"negation_dim{z_dim}",
+                    f"negation_dim{theta_dim}",
                     NegationLayer(
-                        item_z_relationships=item_relationships,
+                        item_theta_relationships=item_relationships,
                         inputs_per_items=inputs_per_items,
                         zero_outputs=missing_cats
                     )
                 )
 
-    def forward(self, z: torch.Tensor) -> torch.Tensor:
+    def forward(self, theta: torch.Tensor) -> torch.Tensor:
         latent_variable_outputs = []
         for latent_variable in range(self.latent_variables):
-            layer_out = self._modules[f'linear0_dim{latent_variable}'](z[:, latent_variable].unsqueeze(1))
+            layer_out = self._modules[f"linear0_dim{latent_variable}"](theta[:, latent_variable].unsqueeze(1))
 
             layer_out = self.split_activation(layer_out)
             for i in range(1, self.hidden_layers):
-                layer_out = self._modules[f'linear{i}_dim{latent_variable}'](layer_out)
+                layer_out = self._modules[f"linear{i}_dim{latent_variable}"](layer_out)
                 layer_out = self.split_activation(layer_out)
 
             layer_out = layer_out.reshape(-1, self.separations, self.hidden_out_dim).sum(dim=2)
 
             if self.negative_latent_variable_item_relationships:
-                layer_out = self._modules[f'negation_dim{latent_variable}'](layer_out)
+                layer_out = self._modules[f"negation_dim{latent_variable}"](layer_out)
 
             latent_variable_outputs.append(layer_out)
         
         out = torch.stack(latent_variable_outputs, dim=-1).sum(dim=-1)
 
         if self.separate == "items":
             out = out.repeat_interleave(self.max_item_responses, dim=1)
 
         if self.mc_correct_output_idx is None:
             out = out.view(out.shape[0], -1, self.max_item_responses).cumsum(dim=2).reshape(out.shape[0], -1)
         else:
             out[:, self.mc_correct_output_idx] = out.view(out.shape[0], -1, self.max_item_responses).sum(dim=2)
 
-        bias = torch.zeros(self.output_length, device=z.device)
+        bias = torch.zeros(self.output_length, device=theta.device)
         bias[self.free_bias] = self.bias_param
         out += bias
         out[:, self.missing_categories] = -torch.inf
         return out
 
     def split_activation(self, x: torch.Tensor) -> torch.Tensor:
         """
@@ -247,15 +257,15 @@
         torch.Tensor
             3D torch tensor with dimensions (respondents, items, item categories).
         """
         reshaped_output = output.reshape(-1, self.max_item_responses)
         return F.softmax(reshaped_output, dim=1).reshape(output.shape[0], self.items, self.max_item_responses)
 
 
-    def item_z_relationship_directions(self, *args) -> torch.Tensor:
+    def item_theta_relationship_directions(self, *args) -> torch.Tensor:
         """
         Get the relationship directions between each item and latent variable for a fitted model.
 
         Returns
         -------
         torch.Tensor
             A 2D tensor with the relationships between the items and latent variables. Items are rows and latent variables are columns.
```

### Comparing `irtorch-0.0.4/irtorch/models/nominal_response.py` & `irtorch-0.1.0/irtorch/models/generalized_partial_credit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,83 @@
 import pandas as pd
 import torch
 import torch.nn as nn
 from irtorch.models.base_irt_model import BaseIRTModel
 
-class NominalResponse(BaseIRTModel):
-    """
-    Nominal response IRT model.
+class GeneralizedPartialCredit(BaseIRTModel):
+    r"""
+    Generalized Partial Credit IRT model.
 
     Parameters
     ----------
     latent_variables : int
         Number of latent variables.
+    data: torch.Tensor, optional
+        A 2D torch tensor with test data. Used to automatically compute item_categories. Columns are items and rows are respondents. (default is None)
     item_categories : list[int]
         Number of categories for each item. One integer for each item. Missing responses exluded.
-    item_z_relationships : torch.Tensor, optional
+    item_theta_relationships : torch.Tensor, optional
         A boolean tensor of shape (items, latent_variables). If specified, the model will have connections between latent dimensions and items where the tensor is True. If left out, all latent variables and items are related (Default: None)
-    model_missing : bool, optional
-        Whether to model missing item responses as separate item response categories. (Default: False)
-    mc_correct : list[int], optional
-        The correct response category for each item. If specified, the logits for the correct responses are cumulative logits. (Default: None)
-    reference_category : bool, optional
-        Whether to use the first category as an unparameterized reference category. (Default: False and uses the original parameterization given by Bock(1972))
+
+    Notes
+    -----
+    For an item :math:`j` with :math:`m=0, 1, 2, \ldots, M_j` possible item scores, the model defines the probability for responding with a score of :math:`x` as follows (selecting response option :math:`x` for multiple choice items):
+
+    .. math::
+
+        P(X_j=x | \mathbf{\theta}) = \begin{cases}
+            \dfrac{1}
+            {1+\sum_{g=1}^{M_i}\exp \left(g\mathbf{a}_{j}^\top \mathbf{\theta} + \sum_{m=1}^gd_{jm}\right)}, & \text{if } x = 0\\
+            \dfrac{\exp \left( x\mathbf{a}_{j}^\top \mathbf{\theta}+\sum_{m=1}^{x}d_{jm}\right)}
+            {1+\sum_{g=1}^{M_i}\exp \left(g\mathbf{a}_{j}^\top \mathbf{\theta} + \sum_{m=1}^gd_{jm}\right)}, & \text{otherwise}
+        \end{cases}
+
+    where:
+
+    - :math:`\mathbf{\theta}` is a vector of latent variables.
+    - :math:`\mathbf{a}_{j}` is a vector of weights for item :math:`j`.
+    - :math:`d_{jm}` is the bias term for item :math:`j` and response category :math:`m`.
     """
     def __init__(
         self,
-        latent_variables: int,
-        item_categories: list[int],
-        item_z_relationships: torch.Tensor = None,
-        model_missing: bool = False,
-        mc_correct: list[int] = None,
-        reference_category: bool = False
+        latent_variables: int = 1,
+        data: torch.Tensor = None,
+        item_categories: list[int] = None,
+        item_theta_relationships: torch.Tensor = None,
     ):
-        super().__init__(latent_variables=latent_variables, item_categories=item_categories, model_missing=model_missing, mc_correct=mc_correct)
-        if item_z_relationships is not None:
-            if item_z_relationships.shape != (len(item_categories), latent_variables):
+        if item_categories is None:
+            if data is None:
+                raise ValueError("Either an instantiated model, item_categories or data must be provided to initialize the model.")
+            else:
+                # replace nan with -inf to get max
+                item_categories = (torch.where(~data.isnan(), data, torch.tensor(float('-inf'))).max(dim=0).values + 1).int().tolist()
+
+        super().__init__(latent_variables=latent_variables, item_categories=item_categories)
+        if item_theta_relationships is not None:
+            if item_theta_relationships.shape != (len(item_categories), latent_variables):
                 raise ValueError(
                     f"latent_item_connections must have shape ({len(item_categories)}, {latent_variables})."
                 )
-            assert(item_z_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
-            assert(torch.all(item_z_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
+            assert(item_theta_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
+            assert(torch.all(item_theta_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
 
         self.output_size = self.items * self.max_item_responses
 
-        free_weights = torch.zeros(self.items, self.max_item_responses, latent_variables)
-        for item, item_cat in enumerate(self.modeled_item_responses):
-            start_1 = 1 if reference_category else 0
-            if item_z_relationships is not None:
-                free_weights[item, start_1:item_cat, :] = item_z_relationships[item, :]
-            else:
-                free_weights[item, start_1:item_cat, :] = 1.0
+        free_weights = torch.ones(self.items, latent_variables)
+        self.register_buffer("gpc_weight_multiplier", torch.arange(0, self.max_item_responses).repeat(self.items))
+        if item_theta_relationships is not None:
+            for item, item_cat in enumerate(self.modeled_item_responses):
+                free_weights[item, :] = item_theta_relationships[item, :]
 
-        free_weights = free_weights.reshape(-1, latent_variables)
         self.weight_param = nn.Parameter(torch.zeros(free_weights.sum().int()))
 
-        number_of_bias_parameters = sum(self.modeled_item_responses) if not reference_category else sum(self.modeled_item_responses) - self.items
+        number_of_bias_parameters = sum(self.modeled_item_responses) - self.items
         self.bias_param = nn.Parameter(torch.zeros(number_of_bias_parameters))
         first_category = torch.zeros(self.items, self.max_item_responses)
-        if reference_category:
-            first_category[:, 0] = 1.0
+        first_category[:, 0] = 1.0
         first_category = first_category.reshape(-1)
         missing_category = torch.zeros(self.items, self.max_item_responses)
         for item, item_cat in enumerate(self.modeled_item_responses):
             missing_category[item, item_cat:self.max_item_responses] = 1.0
         missing_category = missing_category.reshape(-1)
         free_bias = (1 - first_category) * (1 - missing_category)
         self.register_buffer("free_weights", free_weights.bool())
@@ -70,36 +86,37 @@
         self.register_buffer("first_category", first_category.bool())
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         nn.init.normal_(self.weight_param, mean=1., std=0.01)
         nn.init.zeros_(self.bias_param)
     
-    def forward(self, z: torch.Tensor) -> torch.Tensor:
+    def forward(self, theta: torch.Tensor) -> torch.Tensor:
         """
         Forward pass of the model.
 
         Parameters
         ----------
-        z : torch.Tensor
+        theta : torch.Tensor
             2D tensor with latent variables. Rows are respondents and latent variables are columns. 
 
         Returns
         -------
         output : torch.Tensor
             2D tensor. Rows are respondents and columns are item category logits.
         """
-        bias = torch.zeros(self.output_size, device=z.device)
+        bias = torch.zeros(self.output_size, device=theta.device)
         bias[self.free_bias] = self.bias_param
         
-        weights = torch.zeros(self.output_size, self.latent_variables, device=z.device)
+        weights = torch.zeros(self.items, self.latent_variables, device=theta.device)
         weights[self.free_weights] = self.weight_param
-        weighted_z = torch.matmul(z, weights.T)
+        weighted_theta = torch.matmul(theta, weights.T).repeat_interleave(self.max_item_responses, dim=1)
+        weighted_theta *= self.gpc_weight_multiplier
 
-        output = weighted_z + bias
+        output = weighted_theta + bias
         # stop gradients from flowing through the missing categories
         output[:, self.missing_category] = -torch.inf
 
         output[:, self.first_category] = 0
 
         return output
 
@@ -117,42 +134,42 @@
         pd.DataFrame
             A dataframe with the item parameters.
         """
         biases = torch.zeros(self.output_size)
         biases[self.free_bias] = self.bias_param
         biases = biases.reshape(-1, self.max_item_responses)
 
-        weights = torch.zeros(self.output_size, self.latent_variables)
+        weights = torch.zeros(self.items, self.latent_variables)
         weights[self.free_weights] = self.weight_param
-        weights = weights.reshape(-1, self.max_item_responses * self.latent_variables)
 
         weights_df = pd.DataFrame(weights.detach().numpy())
         if irt_format and self.latent_variables == 1:
-            biases_df = pd.DataFrame(-(weights*biases).detach().numpy())
-            weights_df.columns = [f"a{i+1}{j+1}" for i in range(self.latent_variables) for j in range(int(weights.shape[1]/self.latent_variables))]
+            weights_df.columns = [f"a{i+1}" for i in range(weights.shape[1])]
+            biases_df = pd.DataFrame(-(weights*biases).detach()[:, 1:].numpy())
         else:
+            weights_df.columns = [f"w{i+1}" for i in range(weights.shape[1])]
             biases_df = pd.DataFrame(biases.detach().numpy())
-            weights_df.columns = [f"w{i+1}{j+1}" for i in range(self.latent_variables) for j in range(int(weights.shape[1]/self.latent_variables))]
             
         biases_df.columns = [f"b{i+1}" for i in range(biases_df.shape[1])]
         parameters = pd.concat([weights_df, biases_df], axis=1)
 
         return parameters
 
     @torch.inference_mode()
-    def item_z_relationship_directions(self, z:torch.Tensor = None) -> torch.Tensor:
+    def item_theta_relationship_directions(self, theta:torch.Tensor = None) -> torch.Tensor:
         """
         Get the relationship directions between each item and latent variable for a fitted model.
 
         Parameters
         ----------
-        z : torch.Tensor, optional
-            Only needed for NR models. A 2D tensor with latent z scores from the population of interest. Each row represents one respondent, and each column represents a latent variable.
+        theta : torch.Tensor, optional
+            Not needed for this model. (default is None)
 
         Returns
         -------
         torch.Tensor
             A 2D tensor with the relationships between the items and latent variables. Items are rows and latent variables are columns.
         """
-        if z is None:
-            raise ValueError("z must be provided to get item to z relationships for NR models.")
-        return super().item_z_relationship_directions(z)
+        weights = torch.zeros(self.items, self.latent_variables)
+        weights[self.free_weights] = self.weight_param
+        return weights.sign().int()
+
```

### Comparing `irtorch-0.0.4/irtorch/models/one_parameter_logistic.py` & `irtorch-0.1.0/irtorch/models/one_parameter_logistic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 import pandas as pd
 import torch
 import torch.nn as nn
 from irtorch.models.base_irt_model import BaseIRTModel
 
 class OneParameterLogistic(BaseIRTModel):
-    """
+    r"""
     One parametric logistic (2PL) IRT model.
 
     Parameters
     ----------
     latent_variables : int
         Number of latent variables.
     items : int
         Number of items.
-    item_z_relationships : torch.Tensor, optional
+    item_theta_relationships : torch.Tensor, optional
         A boolean tensor of shape (items, latent_variables). If specified, the model will have connections between latent dimensions and items where the tensor is True. If left out, all latent variables and items are related (Default: None)
+    
+    Notes
+    -----
+    For an item :math:`j`, the model defines the probability for responding correctly as:
+
+    .. math::
+
+        \frac{
+            \exp(\mathbf{a}^\top \mathbf{\theta} + d_j)
+        }{
+            1+\exp(\mathbf{a}^\top \mathbf{\theta} + d_j)
+        },
+
+    where:
+
+    - :math:`\mathbf{\theta}` is a vector of latent variables.
+    - :math:`\mathbf{a}` is a vector of weights. This is the same for all items.
+    - :math:`d_j` is the bias term for item :math:`j`.
     """
     def __init__(
         self,
         latent_variables: int,
         items: int,
-        item_z_relationships: torch.Tensor = None
+        item_theta_relationships: torch.Tensor = None
     ):
         super().__init__(latent_variables=latent_variables, item_categories = [2] * items)
-        if item_z_relationships is not None:
-            if item_z_relationships.shape != (items, latent_variables):
+        if item_theta_relationships is not None:
+            if item_theta_relationships.shape != (items, latent_variables):
                 raise ValueError(
                     f"latent_item_connections must have shape ({items}, {latent_variables})."
                 )
-            assert(item_z_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
-            assert(torch.all(item_z_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
+            assert(item_theta_relationships.dtype == torch.bool), "latent_item_connections must be boolean type."
+            assert(torch.all(item_theta_relationships.sum(dim=1) > 0)), "all items must have a relationship with a least one latent variable."
 
         self.output_size = self.items * 2
         self.weight_param = nn.Parameter(torch.zeros(latent_variables))
         self.bias_param = nn.Parameter(torch.zeros(self.items))
 
         first_category = torch.zeros(self.items, 2)
         first_category[:, 0] = 1.0
@@ -45,33 +63,33 @@
         self.register_buffer("first_category", first_category.bool())
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         nn.init.normal_(self.weight_param, mean=1., std=0.01)
         nn.init.zeros_(self.bias_param)
     
-    def forward(self, z: torch.Tensor) -> torch.Tensor:
+    def forward(self, theta: torch.Tensor) -> torch.Tensor:
         """
         Forward pass of the model.
 
         Parameters
         ----------
-        z : torch.Tensor
+        theta : torch.Tensor
             2D tensor with latent variables. Rows are respondents and latent variables are columns. 
 
         Returns
         -------
         output : torch.Tensor
             2D tensor. Rows are respondents and columns are item category logits.
         """
-        bias = torch.zeros(self.output_size, device=z.device)
+        bias = torch.zeros(self.output_size, device=theta.device)
         bias[self.free_bias] = self.bias_param
-        weighted_z = (self.weight_param * z).sum(dim=1, keepdim=True)
+        weighted_theta = (self.weight_param * theta).sum(dim=1, keepdim=True)
 
-        output = weighted_z + bias
+        output = weighted_theta + bias
         output[:, self.first_category] = 0
 
         return output
 
     def item_parameters(self, irt_format = False) -> pd.DataFrame:
         """
         Get the item parameters for a fitted model.
@@ -103,21 +121,21 @@
             
         biases_df.columns = ["b1"]
         parameters = pd.concat([weights_df, biases_df], axis=1)
 
         return parameters
 
     @torch.inference_mode()
-    def item_z_relationship_directions(self, z:torch.Tensor = None) -> torch.Tensor:
+    def item_theta_relationship_directions(self, theta:torch.Tensor = None) -> torch.Tensor:
         """
         Get the relationship directions between each item and latent variable for a fitted model.
 
         Parameters
         ----------
-        z : torch.Tensor, optional
+        theta : torch.Tensor, optional
             Not needed for this model. (default is None)
             
         Returns
         -------
         torch.Tensor
             A 2D tensor with the relationships between the items and latent variables. Items are rows and latent variables are columns.
         """
```

### Comparing `irtorch-0.0.4/irtorch/outlier_detector.py` & `irtorch-0.1.0/irtorch/outlier_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import torch
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 class OutlierDetector:
     """
     A class for identifying and detecting outliers in a dataset.
     """
 
     def __init__(self, factor: int = 1.5):
@@ -148,16 +148,16 @@
         q1, q3 = torch.quantile(data, torch.tensor([0.25, 0.75]), dim=0, keepdim=True)
         iqr = q3 - q1
 
         # Calculate lower and upper bounds
         lower_bound = q1 - self.factor * iqr
         upper_bound = q3 + self.factor * iqr
 
-        # Mask the original data with the non-outliers mask and replace outliers with 'inf'/'-inf' (to ignore during min/max calculation)
+        # Mask the original data with the non-outliers mask and replace outliers with "inf"/"-inf" (to ignore during min/max calculation)
         non_outliers_mask = (data >= lower_bound) & (data <= upper_bound)
         if smallest:
-            masked_data = torch.where(non_outliers_mask, data, torch.full_like(data, float('inf')))
+            masked_data = torch.where(non_outliers_mask, data, torch.full_like(data, float("inf")))
         else:
-            masked_data = torch.where(non_outliers_mask, data, torch.full_like(data, float('-inf')))
+            masked_data = torch.where(non_outliers_mask, data, torch.full_like(data, float("-inf")))
         resulting_values, _ = torch.min(masked_data, dim=0) if smallest else torch.max(masked_data, dim=0)
 
         return resulting_values.unsqueeze(0)
```

### Comparing `irtorch-0.0.4/irtorch/quantile_mv_normal.py` & `irtorch-0.1.0/irtorch/quantile_mv_normal.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import torch
 from torch.distributions.multivariate_normal import MultivariateNormal
 from irtorch.latent_variable_functions import (
     quantile_transform,
     interp,
 )
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 class QuantileMVNormal:
     """
     Quantile multivariate normal approximation of a multivariate joint density function.
     """
 
     def __init__(self):
```

### Comparing `irtorch-0.0.4/irtorch/timer.py` & `irtorch-0.1.0/irtorch/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import torch, time, gc
 
-logger = logging.getLogger('irtorch')
+logger = logging.getLogger("irtorch")
 
 START_TIME = None
 
 def start_timer():
     """
     Start the timer for measuring execution time and memory usage.
     """
```

### Comparing `irtorch-0.0.4/irtorch/utils.py` & `irtorch-0.1.0/irtorch/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,14 +14,58 @@
     Returns
     ----------
     list
         A list of integers where each integer is the number of possible responses for the corresponding item.
     """
     return [int(data[~data.isnan().any(dim=1)][:, col].max()) + 1 for col in range(data.shape[1])]
 
+def impute_missing(data: torch.tensor, mc_correct: list[int] = None, item_categories: list[int] = None):
+    """
+    Impute missing values in the data. 
+    For multiple choice data for which missing is not modeled, imputes randomly from incorrect responses.
+    For non-multiple choice data, imputes missing values as 0.
+
+    Parameters
+    -----------
+    data : torch.Tensor
+        A 2D tensor where each row represents one respondent and each column represents an item.
+        The values should be the scores/possible responses on the items, starting from 0.
+        Missing item responses need to be coded as -1 or "nan".
+    mc_correct : list[int], optional
+        A list of integers where each integer is the correct response for the corresponding item. If None, the data is assumed to be non multiple choice (or dichotomously scored multiple choice with only 0's and 1's). (default is None)
+    item_categories : list[int], optional
+        A list of integers where each integer is the number of possible responses for the corresponding item. If None, the number of possible responses is calculated from the data. (default is None)
+
+    Returns
+    ----------
+    torch.Tensor
+        A 2D tensor with missing values imputed. Rows are respondents and columns are items.
+    """
+    if data.isnan().any():
+        data[data.isnan()] = -1
+
+    if mc_correct is None:
+        data[data==-1] = 0
+        return data
+    else: 
+        if item_categories is None:
+            item_categories = (torch.where(~data.isnan(), data, torch.tensor(float('-inf'))).max(dim=0).values + 1).int().tolist()
+        for col in range(data.shape[1]):
+            # Get the incorrect non-missing responses from the column
+            incorrect_responses = torch.arange(0, item_categories[col])
+            incorrect_responses = incorrect_responses[incorrect_responses != mc_correct[col]-1]
+
+            # Find the indices of -1 values in the column
+            missing_indices = (data[:, col] == -1).squeeze()
+
+            # randomly sample from the incorrect responses and replace missing
+            data[missing_indices, col] = incorrect_responses[torch.randint(0, incorrect_responses.size(0), (missing_indices.sum(),))].float()
+
+        return data
+
 def split_data(data, train_ratio=0.8, shuffle=True):
     """
     Splits a tensor into training and testing datasets.
 
     Parameters
     ----------
     data : torch.Tensor
```

### Comparing `irtorch-0.0.4/irtorch.egg-info/PKG-INFO` & `irtorch-0.1.0/irtorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irtorch
-Version: 0.0.4
+Version: 0.1.0
 Summary: IRTorch: An item response theory package for python.
 Home-page: https://github.com/joakimwallmark/irtorch
 Author: Joakim Wallmark
 Author-email: wallmark.joakim@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `irtorch-0.0.4/irtorch.egg-info/SOURCES.txt` & `irtorch-0.1.0/irtorch.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 LICENSE.txt
 README.md
 setup.py
 irtorch/__init__.py
 irtorch/_internal_utils.py
 irtorch/activation_functions.py
+irtorch/bit_scales.py
 irtorch/config.py
 irtorch/cross_validation.py
+irtorch/evaluation.py
 irtorch/gaussian_mixture_model.py
-irtorch/irt.py
-irtorch/irt_evaluator.py
-irtorch/irt_plotter.py
-irtorch/irt_scorer.py
 irtorch/latent_variable_functions.py
 irtorch/layers.py
 irtorch/load_dataset.py
 irtorch/outlier_detector.py
+irtorch/plotting.py
 irtorch/quantile_mv_normal.py
 irtorch/timer.py
 irtorch/utils.py
 irtorch.egg-info/PKG-INFO
 irtorch.egg-info/SOURCES.txt
 irtorch.egg-info/dependency_links.txt
 irtorch.egg-info/not-zip-safe
@@ -28,38 +27,39 @@
 irtorch/datasets/national_mathematics/mathematics_1.pt
 irtorch/datasets/national_mathematics/mathematics_2.pt
 irtorch/datasets/swedish_sat/swesat22b_nominal_quant.pt
 irtorch/datasets/swedish_sat/swesat22b_nominal_verb.pt
 irtorch/datasets/swedish_sat/swesat22b_quant_correct.txt
 irtorch/datasets/swedish_sat/swesat22b_verb_correct.txt
 irtorch/estimation_algorithms/__init__.py
-irtorch/estimation_algorithms/aeirt.py
+irtorch/estimation_algorithms/ae.py
 irtorch/estimation_algorithms/base_irt_algorithm.py
-irtorch/estimation_algorithms/vaeirt.py
+irtorch/estimation_algorithms/mml.py
+irtorch/estimation_algorithms/vae.py
 irtorch/estimation_algorithms/encoders/__init__.py
 irtorch/estimation_algorithms/encoders/base_encoder.py
 irtorch/estimation_algorithms/encoders/bounded_encoder.py
 irtorch/estimation_algorithms/encoders/standard_encoder.py
 irtorch/estimation_algorithms/encoders/variational_encoder.py
 irtorch/models/__init__.py
 irtorch/models/base_irt_model.py
 irtorch/models/generalized_partial_credit.py
 irtorch/models/monotone_nn.py
 irtorch/models/nominal_response.py
 irtorch/models/one_parameter_logistic.py
 irtorch/models/two_parameter_logistic.py
 tests/test_activation_functions.py
-tests/test_aeirt.py
+tests/test_ae.py
+tests/test_bit_scales.py
 tests/test_config.py
+tests/test_evaluation.py
 tests/test_gaussian_mixture_torch.py
 tests/test_integration.py
 tests/test_internal_utils.py
-tests/test_irt_evaluator.py
-tests/test_irt_plotter.py
-tests/test_irt_scorer.py
 tests/test_latent_variable_functions.py
 tests/test_layers.py
 tests/test_load_dataset.py
+tests/test_mml.py
 tests/test_outlier_detector.py
 tests/test_quantile_mv_normal.py
 tests/test_utils.py
-tests/test_vaeirt.py
+tests/test_vae.py
```

### Comparing `irtorch-0.0.4/setup.py` & `irtorch-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
-with open('README.md', 'r', encoding='utf-8') as f:
+with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="irtorch",
-    version="0.0.4",
+    version="0.1.0",
     description="IRTorch: An item response theory package for python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.10",
     url="https://github.com/joakimwallmark/irtorch",
     author="Joakim Wallmark",
     author_email="wallmark.joakim@gmail.com",
```

### Comparing `irtorch-0.0.4/tests/test_activation_functions.py` & `irtorch-0.1.0/tests/test_activation_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/tests/test_aeirt.py` & `irtorch-0.1.0/tests/test_mml.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,110 @@
 import pytest
 from unittest.mock import patch
-from utils import initialize_fit
 import torch
-from irtorch.estimation_algorithms import AEIRT
+from torch.distributions import MultivariateNormal
+from irtorch.estimation_algorithms import MML
 from irtorch.models import MonotoneNN
 
 
 # The @pytest.fixture decorator is used to create fixture methods.
 # This method is called once per test method that uses it, and its return value is passed to the test method as an argument.
 # pytest.fixture with params creates two fixtures, one for the CPU and one for the GPU.
 # The ids parameter is used to give the tests meaningful names
-class TestAEIRT:
+class TestMML:
     @pytest.fixture()
-    def algorithm(self, device, latent_variables, item_categories, data_loaders):
-        if device == "cuda" and not torch.cuda.is_available():
-            pytest.skip("GPU is not available.")
-
+    def irt_model(self, latent_variables, item_categories):
         model = MonotoneNN(
             latent_variables = latent_variables,
             item_categories = item_categories,
             hidden_dim = [3]
         )
-        algorithm = AEIRT(
-            model=model,
-            hidden_layers_encoder=[20],  # 1 hidden layer with 20 neurons
-            nonlinear_encoder=torch.nn.ELU()
-        )
+        return model
 
+    @pytest.fixture()
+    def algorithm(self, data_loaders):
+        algorithm = MML()
         algorithm.imputation_method = "zero"
         # Set DataLoaders from the fixture
         algorithm.data_loader, algorithm.validation_data_loader = data_loaders
-
-        initialize_fit(algorithm)
         return algorithm
 
-    def test_forward(self, algorithm: AEIRT, test_data):
-        output = algorithm.forward(test_data)
-        assert output.shape == (120, algorithm.model.max_item_responses * algorithm.model.items)
-
-    def test_latent_scores(self, algorithm: AEIRT, test_data):
-        output = algorithm.z_scores(test_data.to(next(algorithm.parameters()).device))
-        assert output.shape == (120, algorithm.model.latent_variables)
-
-    def test__train_step(self, algorithm: AEIRT):
+    def test__train_step(self, algorithm: MML, irt_model: MonotoneNN, test_data: torch.Tensor):
+        algorithm.optimizer = torch.optim.Adam(
+            list(irt_model.parameters()), lr=0.01, amsgrad=True
+        )
         previous_loss = float("inf")
-        for epoch in range(2):
-            loss = algorithm._train_step(epoch)
+        latent_grid = torch.linspace(-3, 3, 5).view(-1, 1)
+        latent_grid = latent_grid.expand(-1, irt_model.latent_variables).contiguous()
+        normal_dist = MultivariateNormal(
+            loc=torch.zeros(irt_model.latent_variables),
+            covariance_matrix=torch.eye(irt_model.latent_variables)
+        )
+        if latent_grid.size(1) > 1:
+            columns = [latent_grid[:, i] for i in range(latent_grid.size(1))]
+            latent_combos = torch.cartesian_prod(*columns)
+        else:
+            latent_combos = latent_grid
+
+        log_weights = normal_dist.log_prob(latent_combos)
+        latent_combos_rep = latent_combos.repeat_interleave(test_data.size(0), dim=0)
+        train_data_rep = test_data.repeat(latent_combos.size(0), 1)
+        log_weights_rep = log_weights.repeat_interleave(test_data.size(0), dim=0)
+
+
+        algorithm
+        for _ in range(2):
+            loss = algorithm._train_step(
+                irt_model,
+                train_data_rep,
+                latent_combos_rep,
+                log_weights_rep,
+                latent_combos.size(0)
+            )
             assert loss <= previous_loss  # Loss should decrease
             previous_loss = loss
 
-    def test__validation_step(self, algorithm: AEIRT):
-        log_likelihood = algorithm._validation_step()
-        assert isinstance(log_likelihood, float)
-        assert log_likelihood > 0
-
-    def test__impute_missing_zero(self, algorithm: AEIRT):
+    def test__impute_missing_thetaero(self, algorithm: MML, irt_model: MonotoneNN):
         a, b = 5, 5
         data = torch.full((a, b), 5)
         no_missing_mask = torch.full((a, b), 0)
         missing_mask = torch.tensor(
             [
                 [0, 0, 1, 0, 0],
                 [0, 1, 0, 0, 0],
                 [0, 0, 0, 0, 1],
                 [0, 0, 0, 0, 0],
                 [1, 1, 0, 0, 0],
             ]
         )
 
         algorithm.imputation_method = "zero"
-        imputed_data = algorithm._impute_missing(data, missing_mask)
+        imputed_data = algorithm._impute_missing(irt_model, data, missing_mask)
         assert torch.equal(
             imputed_data,
             torch.tensor(
                 [
                     [5, 5, 0, 5, 5],
                     [5, 0, 5, 5, 5],
                     [5, 5, 5, 5, 0],
                     [5, 5, 5, 5, 5],
                     [0, 0, 5, 5, 5],
                 ]
             ),
         )
-        imputed_data = algorithm._impute_missing(data, no_missing_mask)
+        imputed_data = algorithm._impute_missing(irt_model, data, no_missing_mask)
         assert torch.equal(imputed_data, data)
 
-    # The following is a test for the fit function of the AEIRTNeuralNet class
-    def test_fit(self, algorithm: AEIRT, test_data):
+    def test_fit(self, algorithm: MML, irt_model: MonotoneNN, test_data):
         # Mock the inner functions that would be called during training
         with patch.object(
             algorithm, "_train_step", return_value=torch.tensor(0.5)
-        ) as mocked_train_step, patch.object(
-            algorithm, "_validation_step", return_value=torch.tensor(0.5)
-        ) as mocked_validation_step:
+        ) as mocked_train_step:
             # Call fit function
             algorithm.fit(
+                model=irt_model,
                 train_data=test_data[0:100],
-                validation_data=test_data[100:120],
                 max_epochs=5
             )
 
             # Check if inner functions are called
             assert mocked_train_step.call_count == 5
-            assert mocked_validation_step.call_count == 5
```

### Comparing `irtorch-0.0.4/tests/test_config.py` & `irtorch-0.1.0/tests/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import logging
 from irtorch.config import set_verbosity
 
 def test_set_verbosity():
     # Test setting verbosity level 1
     set_verbosity(1)
-    assert logging.getLogger('irtorch').getEffectiveLevel() == logging.CRITICAL
+    assert logging.getLogger("irtorch").getEffectiveLevel() == logging.CRITICAL
 
     # Test setting verbosity level 2
     set_verbosity(2)
-    assert logging.getLogger('irtorch').getEffectiveLevel() == logging.ERROR
+    assert logging.getLogger("irtorch").getEffectiveLevel() == logging.ERROR
 
     # Test setting verbosity level 3
     set_verbosity(3)
-    assert logging.getLogger('irtorch').getEffectiveLevel() == logging.WARNING
+    assert logging.getLogger("irtorch").getEffectiveLevel() == logging.WARNING
 
     # Test setting verbosity level 4
     set_verbosity(4)
-    assert logging.getLogger('irtorch').getEffectiveLevel() == logging.INFO
+    assert logging.getLogger("irtorch").getEffectiveLevel() == logging.INFO
 
     # Test setting verbosity level 5
     set_verbosity(5)
-    assert logging.getLogger('irtorch').getEffectiveLevel() == logging.DEBUG
+    assert logging.getLogger("irtorch").getEffectiveLevel() == logging.DEBUG
 
     # Test setting invalid verbosity level
     try:
         set_verbosity(6)
     except ValueError as e:
         assert str(e) == "Invalid verbosity level. Level should be 1, 2, 3, 4 or 5."
```

### Comparing `irtorch-0.0.4/tests/test_gaussian_mixture_torch.py` & `irtorch-0.1.0/tests/test_gaussian_mixture_torch.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/tests/test_integration.py` & `irtorch-0.1.0/tests/test_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,38 +34,38 @@
 #         device=device
 #     )
     
 #     # Save models for other tests
 #     # model.save_model(f"tests/fitted_models/{model_type}_latent_variables{latent_variables}_{data_type}_{device}.pt")
 
 #     for name, param in model.model.state_dict().items():
-#         if 'free' not in name and 'missing_categories' not in name and not re.match(r'negation_dim\d+\.weight', name):
+#         if "free" not in name and "missing_categories" not in name and not re.match(r"negation_dim\d+\.weight", name):
 #             assert not torch.equal(initial_parameter_dict[name], param), f"Parameter {name} was not updated."
 
 # @pytest.mark.integration
 # def test_latent_scores(model: IRT, data, latent_variables):
-#     z_nn_scores = model.scorer.latent_scores(data, scale="z", z_estimation_method="NN")
-#     z_ml_scores = model.scorer.latent_scores(data, scale="z", z_estimation_method="ML")
-#     multi_bit_score_nn_scores = model.scorer.latent_scores(data, scale="bit", z_estimation_method="NN", bit_score_one_dimensional=False)
-#     multi_bit_score_ml_scores = model.scorer.latent_scores(data, scale="bit", z = z_ml_scores, z_estimation_method="ML", bit_score_population_z=z_ml_scores, bit_score_one_dimensional=False)
-#     one_bit_score_nn_scores = model.scorer.latent_scores(data, scale="bit", z_estimation_method="NN", bit_score_one_dimensional=True)
-#     one_bit_score_ml_scores = model.scorer.latent_scores(data, scale="bit", z = z_ml_scores, z_estimation_method="ML", bit_score_population_z=z_ml_scores, bit_score_one_dimensional=True)
+#     theta_nn_scores = model.scorer.latent_scores(data, theta_estimation="NN")
+#     theta_ml_scores = model.scorer.latent_scores(data, theta_estimation="ML")
+#     multi_bit_score_nn_scores = model.scorer.latent_scores(data, scale="bit", theta_estimation="NN", bit_score_one_dimensional=False)
+#     multi_bit_score_ml_scores = model.scorer.latent_scores(data, scale="bit", theta = theta_ml_scores, theta_estimation="ML", bit_score_population_theta=theta_ml_scores, bit_score_one_dimensional=False)
+#     one_bit_score_nn_scores = model.scorer.latent_scores(data, scale="bit", theta_estimation="NN", bit_score_one_dimensional=True)
+#     one_bit_score_ml_scores = model.scorer.latent_scores(data, scale="bit", theta = theta_ml_scores, theta_estimation="ML", bit_score_population_theta=theta_ml_scores, bit_score_one_dimensional=True)
 
 #     # TODO Add map and EAP again
-#     # multi_bit_score_map_scores = model.scorer.latent_scores(data, scale="bit", z_estimation_method="MAP", bit_score_one_dimensional=False)
-#     # multi_bit_score_eap_scores = model.scorer.latent_scores(data, scale="bit", z_estimation_method="EAP", bit_score_one_dimensional=False)
-#     # z_map_scores = model.scorer.latent_scores(data, scale="z", z_estimation_method="MAP")
-#     # z_eap_scores = model.scorer.latent_scores(data, scale="z", z_estimation_method="EAP")
-#     # one_bit_score_map_scores = model.scorer.latent_scores(data, scale="bit", z_estimation_method="MAP", bit_score_one_dimensional=True)
-#     # one_bit_score_eap_scores = model.scorer.latent_scores(data, scale="bit", z_estimation_method="EAP", bit_score_one_dimensional=True)
-
-#     assert z_nn_scores.shape == torch.Size([data.shape[0], latent_variables])
-#     assert z_ml_scores.shape == torch.Size([data.shape[0], latent_variables])
-#     # assert z_map_scores.shape == torch.Size([data.shape[0], latent_variables])
-#     # assert z_eap_scores.shape == torch.Size([data.shape[0], latent_variables])
+#     # multi_bit_score_map_scores = model.scorer.latent_scores(data, scale="bit", theta_estimation="MAP", bit_score_one_dimensional=False)
+#     # multi_bit_score_eap_scores = model.scorer.latent_scores(data, scale="bit", theta_estimation="EAP", bit_score_one_dimensional=False)
+#     # theta_map_scores = model.scorer.latent_scores(data, theta_estimation="MAP")
+#     # theta_eap_scores = model.scorer.latent_scores(data, theta_estimation="EAP")
+#     # one_bit_score_map_scores = model.scorer.latent_scores(data, scale="bit", theta_estimation="MAP", bit_score_one_dimensional=True)
+#     # one_bit_score_eap_scores = model.scorer.latent_scores(data, scale="bit", theta_estimation="EAP", bit_score_one_dimensional=True)
+
+#     assert theta_nn_scores.shape == torch.Size([data.shape[0], latent_variables])
+#     assert theta_ml_scores.shape == torch.Size([data.shape[0], latent_variables])
+#     # assert theta_map_scores.shape == torch.Size([data.shape[0], latent_variables])
+#     # assert theta_eap_scores.shape == torch.Size([data.shape[0], latent_variables])
 #     assert multi_bit_score_nn_scores.shape == torch.Size([data.shape[0], latent_variables])
 #     assert multi_bit_score_ml_scores.shape == torch.Size([data.shape[0], latent_variables])
 #     # assert multi_bit_score_map_scores.shape == torch.Size([data.shape[0], latent_variables])
 #     # assert multi_bit_score_eap_scores.shape == torch.Size([data.shape[0], latent_variables])
 #     assert one_bit_score_nn_scores.shape == torch.Size([data.shape[0], 1])
 #     assert one_bit_score_ml_scores.shape == torch.Size([data.shape[0], 1])
 #     # assert one_bit_score_map_scores.shape == torch.Size([data.shape[0], 1])
@@ -73,76 +73,76 @@
 
 #     for latent_var in range(latent_variables):
 #         # Remove duplicates and check spearman correlation
 #         # and use is close and not equal two for when we have an uneven amount of perfectly negatively correlated values
 #         sorted_scores, indices = multi_bit_score_nn_scores[:, latent_var].sort()
 #         unique_a, counts = sorted_scores.unique(sorted=True, return_counts = True)
 #         first_occurrences = torch.cumsum(counts, dim=0) - counts
-#         unique_b = z_nn_scores[indices, latent_var][first_occurrences]
+#         unique_b = theta_nn_scores[indices, latent_var][first_occurrences]
 #         corr = spearman_correlation(unique_a, unique_b)
 #         assert (torch.isclose(corr, torch.tensor(1.0), atol = 1e-5) or torch.isclose(corr, torch.tensor(-1.0), atol = 1e-5))
 #         sorted_scores, indices = multi_bit_score_ml_scores[:,latent_var].sort()
 #         unique_a, counts = sorted_scores.unique(sorted=True, return_counts = True)
 #         first_occurrences = torch.cumsum(counts, dim=0) - counts
-#         unique_b = z_ml_scores[indices, latent_var][first_occurrences]
+#         unique_b = theta_ml_scores[indices, latent_var][first_occurrences]
 #         corr = spearman_correlation(unique_a, unique_b)
 #         assert (torch.isclose(corr, torch.tensor(1.0), atol = 1e-5) or torch.isclose(corr, torch.tensor(-1.0), atol = 1e-5))
 #         # sorted_scores, indices = multi_bit_score_map_scores[:,latent_var].sort()
 #         # unique_a, counts = sorted_scores.unique(sorted=True, return_counts = True)
 #         # first_occurrences = torch.cumsum(counts, dim=0) - counts
-#         # unique_b = z_map_scores[indices, latent_var][first_occurrences]
+#         # unique_b = theta_map_scores[indices, latent_var][first_occurrences]
 #         # corr = spearman_correlation(unique_a, unique_b)
 #         # assert (torch.isclose(corr, torch.tensor(1.0), atol = 1e-5) or torch.isclose(corr, torch.tensor(-1.0), atol = 1e-5))
 #         # sorted_scores, indices = multi_bit_score_eap_scores[:,latent_var].sort()
 #         # unique_a, counts = sorted_scores.unique(sorted=True, return_counts = True)
 #         # first_occurrences = torch.cumsum(counts, dim=0) - counts
-#         # unique_b = z_eap_scores[indices, latent_var][first_occurrences]
+#         # unique_b = theta_eap_scores[indices, latent_var][first_occurrences]
 #         # corr = spearman_correlation(unique_a, unique_b)
 #         # assert (torch.isclose(corr, torch.tensor(1.0), atol = 1e-5) or torch.isclose(corr, torch.tensor(-1.0), atol = 1e-5))
 
 #     if latent_variables == 1:
 #         assert torch.allclose(one_bit_score_nn_scores, multi_bit_score_nn_scores, atol=1e-01)
 #         assert torch.allclose(one_bit_score_ml_scores, multi_bit_score_ml_scores, atol=1e-01)
 #         # assert torch.allclose(one_bit_score_map_scores, multi_bit_score_map_scores, atol=1e-01)
 #         # assert torch.allclose(one_bit_score_eap_scores, multi_bit_score_eap_scores, atol=1e-01)
 
 # @pytest.mark.integration
 # def test_plot_item_probabilities(model: IRT, latent_variables):
-#     model.plot_item_probabilities(10, scale = "z")
-#     model.plot_item_probabilities(12, scale = "z", group_fit_groups=8, plot_group_fit=True)
+#     model.plot_item_probabilities(10, scale = "theta")
+#     model.plot_item_probabilities(12, scale = "theta", group_fit_groups=8, plot_group_fit=True)
 #     model.plot_item_probabilities(12, scale = "entropy", steps=40, group_fit_groups=8, plot_group_fit=True)
 #     model.plot_item_probabilities(12, scale = "entropy", steps=40)
 #     if latent_variables > 1:
-#         model.plot_item_probabilities(10, scale = "z", latent_variables=(2, ))
-#         model.plot_item_probabilities(10, scale = "z", latent_variables=(1, 2))
+#         model.plot_item_probabilities(10, scale = "theta", latent_variables=(2, ))
+#         model.plot_item_probabilities(10, scale = "theta", latent_variables=(1, 2))
 #         if latent_variables == 2:
 #             with pytest.raises(TypeError):
-#                 model.plot_item_probabilities(10, scale = "z", latent_variables=(2, ), fixed_zs=(1, 0.5))
+#                 model.plot_item_probabilities(10, scale = "theta", latent_variables=(2, ), fixed_thetas=(1, 0.5))
 #         else:
-#             model.plot_item_probabilities(10, scale = "z", latent_variables=(1, 2), fixed_zs=(1, ))
+#             model.plot_item_probabilities(10, scale = "theta", latent_variables=(1, 2), fixed_thetas=(1, ))
 
 #     # TODO add bit scores plots
 
 # @pytest.mark.integration
-# def test_bit_score_starting_z(model: IRT):
+# def test_bit_score_starting_theta(model: IRT):
 #     guessing_probabilities = [0.5] * len(model.scorer.algorithm.model.modeled_item_responses)
 
 #     # Test with no guessing (or default guessing for multiple choice)
-#     starting_z = model.scorer.bit_score_starting_z(guessing_iterations=200)
-#     assert starting_z.shape == (1, model.model.latent_variables)
+#     starting_theta = model.scorer.bit_score_starting_theta(guessing_iterations=200)
+#     assert starting_theta.shape == (1, model.model.latent_variables)
 
 #     # Test with guessing for dichotomous items
-#     starting_z = model.scorer.bit_score_starting_z(guessing_probabilities=guessing_probabilities, guessing_iterations=200)
-#     assert starting_z.shape == (1, model.model.latent_variables)
+#     starting_theta = model.scorer.bit_score_starting_theta(guessing_probabilities=guessing_probabilities, guessing_iterations=200)
+#     assert starting_theta.shape == (1, model.model.latent_variables)
 
 #     # Test with guessing and MC correct
 #     model.scorer.algorithm.model.mc_correct = [1] * len(model.scorer.algorithm.model.modeled_item_responses)
-#     starting_z = model.scorer.bit_score_starting_z(guessing_probabilities=guessing_probabilities, guessing_iterations=200)
-#     assert starting_z.shape == (1, model.model.latent_variables)
+#     starting_theta = model.scorer.bit_score_starting_theta(guessing_probabilities=guessing_probabilities, guessing_iterations=200)
+#     assert starting_theta.shape == (1, model.model.latent_variables)
 #     model.scorer.algorithm.model.mc_correct = None
 
 # @pytest.mark.integration
 # def test_probability_gradients(model: IRT, latent_variables):
 #     # This makes sure we can run torch.vmap inside probability_gradients, as it is not compatible with some tensor operations
-#     z = torch.randn((40, latent_variables))
-#     gradients = model.model.probability_gradients(z)
-#     assert gradients.shape == torch.Size([z.shape[0], model.model.items, model.model.max_item_responses, model.model.latent_variables])
+#     theta = torch.randn((40, latent_variables))
+#     gradients = model.model.probability_gradients(theta)
+#     assert gradients.shape == torch.Size([theta.shape[0], model.model.items, model.model.max_item_responses, model.model.latent_variables])
```

### Comparing `irtorch-0.0.4/tests/test_internal_utils.py` & `irtorch-0.1.0/tests/test_internal_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,15 @@
     linear_regression,
     is_jupyter,
     dynamic_print,
     conditional_score_distribution,
     sum_incorrect_probabilities,
     entropy,
     output_to_item_entropy,
-    impute_missing,
-    random_guessing_data
+    random_guessing_data,
 )
 
 @pytest.fixture(scope="module")
 def logits(device):
     return torch.tensor(
         [
             [
@@ -56,20 +55,20 @@
         ]
     ).to(device)
 
 
 def test_is_jupyter():
     assert is_jupyter() is False
 
-def testdynamic_print(capsys):
+def test_dynamic_print(capsys):
     dynamic_print("arg1\narg2")
 
     # Capture the output again after calling dynamic_print
     captured_output = capsys.readouterr()
-    assert captured_output.out == '\rarg1\narg2 '
+    assert captured_output.out == "\rarg1\narg2 "
 
     dynamic_print("Hello World!")
     captured_output = capsys.readouterr()
 
     assert captured_output.out == "\rHello World! "
 
 def test_linear_regression():
@@ -188,31 +187,14 @@
     entropies = output_to_item_entropy(output, item_categories)
     assert entropies.shape == (100, 5)
 
     # Test with invalid input (length of item_categories is not equal to the second dimension of output divided by the sum of item_categories)
     with pytest.raises(ValueError):
         output_to_item_entropy(output, [2, 2, 3, 2, 2])
 
-def test_impute_missing():
-    data = torch.tensor([[1, 2, 1, -1], [-1, float('nan'), 0, 2], [-1, float('nan'), 1, 2]])
-    # mc_correct is corresponds to correct item category and not correct score (2 means score 1 is correct)
-    mc_correct = [2, 3, 2, 3]
-    imputed_data = impute_missing(data = data.clone())
-    assert (imputed_data == torch.tensor([[1, 2, 1, 0], [0, 0, 0, 2], [0, 0, 1, 2]])).all()
-
-    imputed_data = impute_missing(data = data, mc_correct=mc_correct, item_categories=[3, 3, 2, 3])
-    missing_mask = torch.logical_or(data == -1, data.isnan())
-    assert (imputed_data[missing_mask] > -1).all() # all missing are replaced
-    assert (imputed_data[~missing_mask] == data[~missing_mask]).all() # non missing are still the same
-    assert imputed_data[0, 3] != 2 # we did not replace with true values
-    assert imputed_data[1, 0] != 1
-    assert imputed_data[1, 1] != 2
-    assert imputed_data[2, 0] != 1
-    assert imputed_data[2, 1] != 2
-
 def test_random_guessing_data():
     # Test non multiple choice data
     item_categories = [2, 2, 2, 2, 4]
     guessing_probabilities = [0.6, 0.6, 0.6, 0.6, 0.5]
     data = random_guessing_data(item_categories, 100, guessing_probabilities)
     assert data.shape == (100, 5)
     assert data.min() == 0
```

### Comparing `irtorch-0.0.4/tests/test_irt_evaluator.py` & `irtorch-0.1.0/tests/test_evaluation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 from unittest.mock import MagicMock, patch
 import torch
 from torch.nn.functional import softmax
 import pytest
-from irtorch.irt_evaluator import IRTEvaluator, IRTScorer
-from irtorch.estimation_algorithms import BaseIRTAlgorithm
+from irtorch.evaluation import Evaluation
+from irtorch.bit_scales import BitScales
+from irtorch.estimation_algorithms import AE
 from irtorch.models import BaseIRTModel
 from irtorch.quantile_mv_normal import QuantileMVNormal
-
+from irtorch.gaussian_mixture_model import GaussianMixtureModel
 
 @pytest.fixture
-def irt_evaluator(latent_variables):
-    # Create a mock instance of AEIRTNeuralNet
+def algorithm(latent_variables):
     item_categories = [2, 3]
-    mock_algorithm = MagicMock(spec=BaseIRTAlgorithm)
+    mock_algorithm = MagicMock(spec=AE)
     mock_algorithm.one_hot_encoded = False
     mock_algorithm.train_data = torch.cat(
         [
             torch.randint(0, item_cat, (30, 1))
             for item_cat in item_categories
         ],
         dim=1,
     )
-    mock_algorithm.training_z_scores = torch.randn(30, latent_variables)
+    mock_algorithm.training_theta_scores = torch.randn(30, latent_variables)
+    # Mock theta_scores method based on input
+    def theta_scores_mock(input_tensor):
+        theta_scores = torch.randn(input_tensor.shape[0], latent_variables)
+        return theta_scores
 
-    # Mock fix_missing_values method 
-    def fix_missing_values_mock(input_tensor):
-        return input_tensor
+    mock_algorithm.theta_scores = MagicMock(side_effect=theta_scores_mock)
+    return mock_algorithm
 
-    mock_algorithm.fix_missing_values = MagicMock(side_effect=fix_missing_values_mock)
+@pytest.fixture
+def bit_scales():
+    mock_bit_scales = MagicMock(spec=BitScales)
+    # Mock bit_score_distance method based on input
+    def bit_scores_from_theta_mock(theta, **kwargs):
+        return torch.randn(theta.shape[0],theta.shape[1]).abs() * 10, torch.randn(1,theta.shape[1])
+    
+    mock_bit_scales.bit_scores_from_theta = MagicMock(side_effect=bit_scores_from_theta_mock)
+    return mock_bit_scales
+
+@pytest.fixture
+def irt_model(latent_variables, algorithm: AE, bit_scales: BitScales):
+    item_categories = [2, 3]
 
     def model_forward_mock(input_tensor: torch.Tensor):
         logits = [
             torch.randn(input_tensor.shape[0], category)
             for category in item_categories
         ]
         return torch.cat(logits, dim=1)
@@ -39,363 +54,368 @@
     # Mock item_probabilities method based on input
     def item_probabilities_mock(input_tensor):
         logits = torch.randn(input_tensor.shape[0], len(item_categories), max(item_categories))
         for item_id, item_cats in enumerate(item_categories):
             logits[:, item_id, item_cats:] = -torch.inf
         return torch.softmax(logits, dim = 2)
     
+    # Mock theta_scores method based on input
+    def latent_scores(data, **kwargs):
+        theta_scores = torch.randn(data.shape[0], latent_variables)
+        return theta_scores
+    
     mock_model = MagicMock(spec=BaseIRTModel, side_effect=model_forward_mock)
+    mock_model.algorithm = algorithm
+    mock_model.bit_scales = bit_scales
     mock_model.item_probabilities = MagicMock(side_effect=item_probabilities_mock)
+    mock_model.latent_scores = MagicMock(side_effect=latent_scores)
     mock_model.item_categories = item_categories
     mock_model.modeled_item_responses = item_categories
     mock_model.model_missing = False
     mock_model.mc_correct = None
     mock_model.latent_variables = latent_variables
 
-    # Mock z_scores method based on input
-    def z_scores_mock(input_tensor):
-        z_scores = torch.randn(input_tensor.shape[0], latent_variables)
-        return z_scores
-
-    mock_algorithm.z_scores = MagicMock(side_effect=z_scores_mock)
-    # Create a mock instance of IRTScorer
-    mock_scorer = MagicMock(spec=IRTScorer)
+    return mock_model
 
-    # Mock z_scores method based on input
-    def latent_scores(data, **kwargs):
-        z_scores = torch.randn(data.shape[0], latent_variables)
-        return z_scores
-
-    # Mock bit_score_distance method based on input
-    def bit_scores_from_z_mock(z, **kwargs):
-        return torch.randn(z.shape[0], z.shape[1]).abs() * 10, torch.randn(1, z.shape[1])
-
-    # Mock min_max_z_for_integration_mock
-    def min_max_z_for_integration_mock(z):
-        z_min = z.min(dim=0)[0]
-        z_max = z.max(dim=0)[0]
-        z_stds = z.std(dim=0)
-        return z_min - z_stds, z_max + z_stds
-
-    # Mock latent density pdf function
-    def pdf_mock(z):
-        return torch.rand(z.shape[0])
-    mock_scorer.latent_scores = MagicMock(side_effect=latent_scores)
-    mock_scorer.bit_scores_from_z = MagicMock(side_effect=bit_scores_from_z_mock)
-    mock_scorer.min_max_z_for_integration = MagicMock(
-        side_effect=min_max_z_for_integration_mock
-    )
-    mock_scorer.latent_density = QuantileMVNormal()
-    mock_scorer.latent_density.pdf = MagicMock(side_effect=pdf_mock)
-    return IRTEvaluator(mock_model, mock_algorithm, mock_scorer)
+@pytest.fixture
+def evaluation(irt_model: BaseIRTModel):
+    def pdf_mock(theta):
+        return torch.rand(theta.shape[0])
+
+    evaluation = Evaluation(irt_model)
+    evaluation.latent_density = QuantileMVNormal()
+    evaluation.latent_density.pdf = MagicMock(side_effect=pdf_mock)
 
+    return evaluation
 
-# add test for the _evaluate_data_z_input method
-def test_evaluate_data_z_input(irt_evaluator: IRTEvaluator):
+# add test for the _evaluate_data_theta_input method
+def test__evaluate_data_theta_input(evaluation: Evaluation):
     # Create some synthetic test data
     data = torch.cat(
         [
             torch.randint(0, item_cat, (30, 1))
-            for item_cat in irt_evaluator.model.item_categories
+            for item_cat in evaluation.model.item_categories
         ],
         dim=1,
     )
 
-    # Call the method with data and z as None
-    result_data, result_z = irt_evaluator._evaluate_data_z_input(data, None, 'NN')
+    # Call the method with data and theta as None
+    result_data, result_theta = evaluation._evaluate_data_theta_input(data, None, "NN")
 
-    # Check the shape of the output data and z
+    # Check the shape of the output data and theta
     assert result_data.shape == data.shape
-    assert result_z.shape == irt_evaluator.algorithm.training_z_scores.shape
+    assert result_theta.shape == evaluation.model.algorithm.training_theta_scores.shape
 
     # Call the method with data as None
-    result_data, result_z = irt_evaluator._evaluate_data_z_input(None, None, 'NN')
+    result_data, result_theta = evaluation._evaluate_data_theta_input(None, None, "NN")
 
-    # Check the shape of the output data and z
-    assert result_data.shape == irt_evaluator.algorithm.train_data.shape
-    assert result_z.shape == irt_evaluator.algorithm.training_z_scores.shape
-
-def test_probabilities_from_grouped_z(irt_evaluator: IRTEvaluator, latent_variables):
-    # Create some synthetic z scores
-    grouped_z = (
+    # Check the shape of the output data and theta
+    assert result_data.shape == evaluation.model.algorithm.train_data.shape
+    assert result_theta.shape == evaluation.model.algorithm.training_theta_scores.shape
+
+def test_probabilities_from_grouped_theta(evaluation: Evaluation, latent_variables):
+    # Create some synthetic theta scores
+    grouped_theta = (
         torch.randn(10, latent_variables),
         torch.randn(10, latent_variables),
         torch.randn(10, latent_variables),
     )
 
     # Call the method
-    probabilities = irt_evaluator._grouped_z_probabilities(grouped_z)
+    probabilities = evaluation._grouped_theta_probabilities(grouped_theta)
     assert probabilities.shape == (3, 2, 3)
     assert torch.allclose(probabilities.sum(dim=2), torch.ones(probabilities.shape[0], probabilities.shape[1]), atol=1e-7)
 
-def test_probabilities_from_grouped_data(irt_evaluator: IRTEvaluator):
+def test_probabilities_from_grouped_data(evaluation: Evaluation):
     # Create synthetic test data groups
     grouped_data = (
         torch.cat(
             [
                 torch.randint(0, item_cat, (5, 1))
-                for item_cat in irt_evaluator.model.item_categories
+                for item_cat in evaluation.model.item_categories
             ],
             dim=1,
         ),
         torch.cat(
             [
                 torch.randint(0, item_cat, (5, 1))
-                for item_cat in irt_evaluator.model.item_categories
+                for item_cat in evaluation.model.item_categories
             ],
             dim=1,
         ),
         torch.cat(
             [
                 torch.randint(0, item_cat, (5, 1))
-                for item_cat in irt_evaluator.model.item_categories
+                for item_cat in evaluation.model.item_categories
             ],
             dim=1,
         ),
     )
 
     # Call the method
-    probabilities = irt_evaluator._grouped_data_probabilities(grouped_data)
+    probabilities = evaluation._grouped_data_probabilities(grouped_data)
 
     assert probabilities.shape == torch.Size([3, 2, 3])
     assert torch.allclose(probabilities.sum(dim=2), torch.ones_like(probabilities[:, :, 0]), atol=1e-7)
 
-@pytest.mark.parametrize("scale", ["bit", "z"])
-def test_latent_group_probabilities(irt_evaluator: IRTEvaluator, scale):
+@pytest.mark.parametrize("scale", ["bit", "theta"])
+def test_latent_group_probabilities(evaluation: Evaluation, scale):
     # Create some synthetic test data
     data = torch.cat(
         [
             torch.randint(0, item_cat, (30, 1))
-            for item_cat in irt_evaluator.model.item_categories
+            for item_cat in evaluation.model.item_categories
         ],
         dim=1,
     )
 
     groups = 3
     (
         grouped_data_probabilities,
         grouped_model_probabilities,
         group_averages,
-    ) = irt_evaluator.latent_group_probabilities(
+    ) = evaluation.latent_group_probabilities(
         groups=groups, data=data, scale=scale, latent_variable=1
     )
 
     # Check the number of groups
     assert grouped_data_probabilities.shape == grouped_model_probabilities.shape
     assert grouped_data_probabilities.shape == torch.Size([3, 2, 3])
     assert torch.allclose(grouped_data_probabilities.sum(dim=2), torch.ones_like(grouped_data_probabilities[:, :, 0]), atol=1e-7)
     assert torch.allclose(grouped_model_probabilities.sum(dim=2), torch.ones_like(grouped_model_probabilities[:, :, 0]), atol=1e-7)
     assert group_averages.shape == (groups,)
 
     if scale == "bit":
         # check if bit score was called
-        irt_evaluator.scorer.bit_scores_from_z.assert_called_once()
+        evaluation.model.bit_scales.bit_scores_from_theta.assert_called_once()
 
-def test_group_fit_residuals(irt_evaluator: IRTEvaluator):
+def test_group_fit_residuals(evaluation: Evaluation):
     data = torch.cat(
         [
             torch.randint(0, item_cat, (30, 1))
-            for item_cat in irt_evaluator.model.item_categories
+            for item_cat in evaluation.model.item_categories
         ],
         dim=1,
     )
 
-    residuals, mid_points = irt_evaluator.group_fit_residuals(data=data, groups=3, latent_variable=1)
+    residuals, mid_points = evaluation.group_fit_residuals(data=data, groups=3, latent_variable=1)
 
     assert residuals.shape == (3, 2, 3)
     assert mid_points.shape == (3,)
-    assert irt_evaluator.model.item_probabilities.call_count == 3
+    assert evaluation.model.item_probabilities.call_count == 3
 
 @pytest.mark.parametrize(
     "latent_density_method", ["data", "encoder sampling", "qmvn", "gmm"]
 )
-def test_sum_score_probabilities(irt_evaluator: IRTEvaluator, latent_density_method):
+def test_sum_score_probabilities(evaluation: Evaluation, latent_density_method):
+    # mock _cv_gaussian_mixture_model method
+    def _cv_gaussian_mixture_model_mock(data, cv_n_components):
+        return GaussianMixtureModel(n_components=cv_n_components[0], n_features=data.shape[1])
+    
+    evaluation._cv_gaussian_mixture_model = MagicMock(side_effect=_cv_gaussian_mixture_model_mock)
+    
     if latent_density_method == "encoder sampling":
         with pytest.raises(ValueError):
-            total_score_probs = irt_evaluator.sum_score_probabilities(
+            total_score_probs = evaluation.sum_score_probabilities(
                 latent_density_method=latent_density_method
             )
     else:
-        total_score_probs = irt_evaluator.sum_score_probabilities(
+        total_score_probs = evaluation.sum_score_probabilities(
             latent_density_method=latent_density_method, trapezoidal_segments=5
         )
-        # We should have 4 scores since we have
-        # mock_neuralnet.decoder.modeled_item_responses = [2, 3]
+        # We should have 4 scores since we have modeled_item_responses = [2, 3]
         assert total_score_probs.shape == (4,)
         # They should add up to 1
         assert torch.isclose(total_score_probs.sum(), torch.tensor(1.0), atol=1e-6)
 
-def test_log_likelihood(irt_evaluator: IRTEvaluator):
+def test_log_likelihood(evaluation: Evaluation):
     # Create synthetic test data
     data = torch.cat(
         [
             torch.randint(0, item_cat, (30, 1))
-            for item_cat in irt_evaluator.model.item_categories
+            for item_cat in evaluation.model.item_categories
         ],
         dim=1,
     )
 
     # Mock log_likelihood method
     def log_likelihood_mock(data, output, loss_reduction):
         t1 = torch.tensor([-0.5, -1.0]).repeat(data.shape[0] // 2)
         t2 = torch.tensor([-0.1, -0.2]).repeat(data.shape[0] - (data.shape[0] // 2))
         return torch.cat([t1, t2])
 
-    irt_evaluator.model.log_likelihood = MagicMock(side_effect=log_likelihood_mock)
+    evaluation.model.log_likelihood = MagicMock(side_effect=log_likelihood_mock)
 
     # latent_group_fit
     # Test with default parameters
-    group_mean_likelihoods = irt_evaluator.group_fit_log_likelihood(data=data)
+    group_mean_likelihoods = evaluation.group_fit_log_likelihood(data=data)
     assert group_mean_likelihoods.shape == (10,)  # Default number of groups is 10
     assert group_mean_likelihoods.dtype == torch.float32
     assert torch.allclose(group_mean_likelihoods[:5], torch.full((5,), -1.5)) # first half of groups
     assert torch.allclose(group_mean_likelihoods[5:], torch.full((5,), -0.3)) # second half of groups
     # Test with specified parameters
-    group_mean_likelihoods = irt_evaluator.group_fit_log_likelihood(groups=5, latent_variable=1, data=data, z_estimation_method="ML")
+    group_mean_likelihoods = evaluation.group_fit_log_likelihood(groups=5, latent_variable=1, data=data, theta_estimation="ML")
     assert group_mean_likelihoods.shape == (5,)  # We specified 5 groups
     assert group_mean_likelihoods.dtype == torch.float32
     assert torch.allclose(group_mean_likelihoods[:2], torch.full((2,), -1.5)) # first half of groups
     assert torch.allclose(group_mean_likelihoods[2], torch.full((1,), -0.9)) # first half of groups
     assert torch.allclose(group_mean_likelihoods[3:], torch.full((2,), -0.3)) # second half of groups
 
     # respondent level
     # Test with default parameters
-    person_likelihoods = irt_evaluator.log_likelihood(data=data, reduction="sum", level="respondent")
+    person_likelihoods = evaluation.log_likelihood(data=data, reduction="sum", level="respondent")
     assert person_likelihoods.shape == (30,)  # We have 30 respondents
     assert person_likelihoods.dtype == torch.float32
     assert torch.allclose(person_likelihoods[:15], torch.full((15,), -1.5)) # first half of respondents
     assert torch.allclose(person_likelihoods[15:], torch.full((15,), -0.3)) # second half of respondents
 
     # item level
     # Test with default parameters
-    item_likelihoods = irt_evaluator.log_likelihood(data=data, reduction="mean", level="item")
+    item_likelihoods = evaluation.log_likelihood(data=data, reduction="mean", level="item")
     assert item_likelihoods.shape == (2,)  # We have 2 items
     assert item_likelihoods.dtype == torch.float32
     assert torch.isclose(item_likelihoods[0], torch.tensor(-0.3))
     assert torch.isclose(item_likelihoods[1], torch.tensor(-0.6))
 
 
-def test_accuracy(irt_evaluator: IRTEvaluator):
+def test_accuracy(evaluation: Evaluation):
     # Create synthetic test data
     data = torch.cat(
         [
             torch.randint(0, item_cat, (30, 1))
-            for item_cat in irt_evaluator.model.item_categories
+            for item_cat in evaluation.model.item_categories
         ],
         dim=1,
     )
 
     # Mock probabilities
-    def item_probabilities_mock(z):
+    def item_probabilities_mock(theta):
         # static 3D tensor with dimensions (respondents, items, item categories)
-        t1 = torch.tensor(([0.55, 0.45, 0.0], [0.2, 0.35, 0.45])).unsqueeze(0).repeat(z.shape[0] // 2, 1, 1)
-        t2 = torch.tensor(([0.15, 0.85, 0.0], [0.6, 0.05, 0.35])).unsqueeze(0).repeat(z.shape[0] - (z.shape[0] // 2), 1, 1)
+        t1 = torch.tensor(([0.55, 0.45, 0.0], [0.2, 0.35, 0.45])).unsqueeze(0).repeat(theta.shape[0] // 2, 1, 1)
+        t2 = torch.tensor(([0.15, 0.85, 0.0], [0.6, 0.05, 0.35])).unsqueeze(0).repeat(theta.shape[0] - (theta.shape[0] // 2), 1, 1)
         return torch.cat([t1, t2])
 
-    irt_evaluator.model.item_probabilities = MagicMock(side_effect=item_probabilities_mock)
+    evaluation.model.item_probabilities = MagicMock(side_effect=item_probabilities_mock)
 
     # overall
-    accuracy = irt_evaluator.accuracy(data=data, level="all")
+    accuracy = evaluation.accuracy(data=data, level="all")
     assert accuracy.shape == ()  # We have 30 respondents
     assert accuracy.dtype == torch.float32
     assert torch.all((accuracy >= 0) & (accuracy <= 1)), "All values are not between 0 and 1"
     
     # respondent level
-    accuracy = irt_evaluator.accuracy(data=data, level="respondent")
+    accuracy = evaluation.accuracy(data=data, level="respondent")
     assert accuracy.shape == (30,)  # We have 30 respondents
     assert accuracy.dtype == torch.float32
     assert torch.all((accuracy >= 0) & (accuracy <= 1)), "All values are not between 0 and 1"
 
     # item level
-    item_likelihoods = irt_evaluator.accuracy(data=data, level="item")
+    item_likelihoods = evaluation.accuracy(data=data, level="item")
     assert item_likelihoods.shape == (2,)  # We have 2 items
     assert item_likelihoods.dtype == torch.float32
     assert torch.all((accuracy >= 0) & (accuracy <= 1)), "All values are not between 0 and 1"
 
 
-def test_residuals(irt_evaluator: IRTEvaluator):
+def test_residuals(evaluation: Evaluation):
     # Create synthetic test data
     data = torch.tensor(
         (
             [0, 2],
             [1, 1],
             [1, 0],
             [0, 1],
             [0, 2],
         )
     ).float()
 
     # Mock probabilities
-    def item_probabilities_mock(z):
+    def item_probabilities_mock(theta):
         # static 3D tensor with dimensions (respondents, items, item categories)
-        t1 = torch.tensor(([0.55, 0.45, 0.0], [0.2, 0.35, 0.45])).unsqueeze(0).repeat(z.shape[0] // 2, 1, 1)
-        t2 = torch.tensor(([0.15, 0.85, 0.0], [0.6, 0.05, 0.35])).unsqueeze(0).repeat(z.shape[0] - (z.shape[0] // 2), 1, 1)
+        t1 = torch.tensor(([0.55, 0.45, 0.0], [0.2, 0.35, 0.45])).unsqueeze(0).repeat(theta.shape[0] // 2, 1, 1)
+        t2 = torch.tensor(([0.15, 0.85, 0.0], [0.6, 0.05, 0.35])).unsqueeze(0).repeat(theta.shape[0] - (theta.shape[0] // 2), 1, 1)
         return torch.cat([t1, t2])
 
-    irt_evaluator.model.item_probabilities = MagicMock(side_effect=item_probabilities_mock)
+    evaluation.model.item_probabilities = MagicMock(side_effect=item_probabilities_mock)
     # For scored tests, we actual vs model expected scores
 
 
     # For MC tests, we have residuals for each MC option
-    irt_evaluator.model.mc_correct = [0, 2]
+    evaluation.model.mc_correct = [0, 2]
     # non-averaged
-    residuals = irt_evaluator.residuals(data=data)
+    residuals = evaluation.residuals(data=data)
     assert residuals.shape == (5, 2)  # We have 30 respondents
     assert torch.allclose(residuals, torch.tensor([
         [0.4500, 0.5500],
         [0.5500, 0.6500],
         [0.1500, 0.4000],
         [0.8500, 0.9500],
         [0.8500, 0.6500]]
     )), "Residuals are not correct"
 
     # overall
-    residuals = irt_evaluator.residuals(data=data, average_over="everything")
+    residuals = evaluation.residuals(data=data, average_over="everything")
     assert residuals.shape == ()  # We have 30 respondents
     assert torch.isclose(residuals, torch.tensor(0.6050)), "Residuals are not correct"
 
     # respondent level
-    residuals = irt_evaluator.residuals(data=data, average_over="items")
+    residuals = evaluation.residuals(data=data, average_over="items")
     assert residuals.shape == (5,)  # We have 5 respondents
     assert torch.allclose(residuals, torch.tensor([0.5000, 0.6000, 0.2750, 0.9000, 0.7500])), "Residuals are not correct"
 
     # item level
-    residuals = irt_evaluator.residuals(data=data, average_over="respondents")
+    residuals = evaluation.residuals(data=data, average_over="respondents")
     assert residuals.shape == (2,)  # We have 2 items
     assert torch.allclose(residuals, torch.tensor([0.5700, 0.6400])), "Residuals are not correct"
 
-def test_infit_outfit(irt_evaluator: IRTEvaluator):
+def test_infit_outfit(evaluation: Evaluation):
     data = torch.tensor([[0, 2], [1, 1]]).float()
-    z = torch.randn(2, irt_evaluator.model.latent_variables)
+    theta = torch.randn(2, evaluation.model.latent_variables)
 
-    def item_probabilities_mock(z):
+    def item_probabilities_mock(theta):
         return torch.tensor([[[0.55, 0.45, 0.0], [0.2, 0.35, 0.45]], [[0.15, 0.85, 0.0], [0.6, 0.05, 0.35]]])
 
     
-    irt_evaluator.model.item_probabilities = MagicMock(side_effect=item_probabilities_mock)
+    evaluation.model.item_probabilities = MagicMock(side_effect=item_probabilities_mock)
     
-    def expected_scores_mock(z, **kwargs):
+    def expected_scores_mock(theta, **kwargs):
         return torch.tensor(([0.45, 0.35 + 2 * 0.45], [0.85, 0.05+2 * 0.35]))
 
-    irt_evaluator.model.expected_scores = MagicMock(side_effect=expected_scores_mock)
+    evaluation.model.expected_scores = MagicMock(side_effect=expected_scores_mock)
 
-    infit, outfit = irt_evaluator.infit_outfit(data, z, level = 'item')
+    infit, outfit = evaluation.infit_outfit(data, theta, level = "item")
     assert torch.allclose(infit, torch.tensor([0.6000000, 0.4237288])), "Infit is incorrect"
     assert torch.allclose(outfit, torch.tensor([0.4973261, 0.5139347])), "Outfit is incorrect"
 
-    infit, outfit = irt_evaluator.infit_outfit(data, z, level = 'respondent')
+    infit, outfit = evaluation.infit_outfit(data, theta, level = "respondent")
     assert torch.allclose(infit, torch.tensor([0.9161677, 0.0837438])), "Infit is incorrect"
     assert torch.allclose(outfit, torch.tensor([0.8878143, 0.1234465])), "Outfit is incorrect"
 
-    def expected_scores_mock_mc(z, **kwargs):
+    def expected_scores_mock_mc(theta, **kwargs):
         return torch.tensor(([0.55, 0.45], [0.15, 0.35]))
 
-    irt_evaluator.model.expected_scores = MagicMock(side_effect=expected_scores_mock_mc)
+    evaluation.model.expected_scores = MagicMock(side_effect=expected_scores_mock_mc)
 
-    irt_evaluator.model.mc_correct = [1, 3]
-    infit, outfit = irt_evaluator.infit_outfit(data, z, level = 'item')
+    evaluation.model.mc_correct = [1, 3]
+    infit, outfit = evaluation.infit_outfit(data, theta, level = "item")
     assert torch.allclose(infit, torch.tensor([0.6000000, 0.8947369])), "Infit is incorrect"
     assert torch.allclose(outfit, torch.tensor([0.4973262, 0.8803419])), "Outfit is incorrect"
 
-    infit, outfit = irt_evaluator.infit_outfit(data, z, level = 'respondent')
+    infit, outfit = evaluation.infit_outfit(data, theta, level = "respondent")
     assert torch.allclose(infit, torch.tensor([1.0202020, 0.4084507])), "Infit is incorrect"
     assert torch.allclose(outfit, torch.tensor([1.0202019, 0.3574660])), "Outfit is incorrect"
+
+@pytest.mark.parametrize("cv_n_components", [[1], [1, 2, 3]])
+def test__cv_gaussian_mixture_model(evaluation: Evaluation, cv_n_components):
+    data = torch.randn(100, evaluation.model.latent_variables)
+
+    with patch.object(GaussianMixtureModel, "fit") as mock_fit, patch.object(GaussianMixtureModel, "__call__") as mock_call:
+        mock_fit.return_value = None
+        mock_call.return_value = torch.tensor(1.0)
+
+        gmm = evaluation._cv_gaussian_mixture_model(data, cv_n_components)
+
+    assert isinstance(gmm, GaussianMixtureModel)
+    assert gmm.n_components == cv_n_components[0]
+    assert gmm.n_features == data.shape[1]
+    mock_fit.assert_called()
+    if len(cv_n_components) > 1:
+        assert mock_call.call_count == len(cv_n_components) * 5  # 5-fold cross-validation
```

### Comparing `irtorch-0.0.4/tests/test_latent_variable_functions.py` & `irtorch-0.1.0/tests/test_latent_variable_functions.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/tests/test_layers.py` & `irtorch-0.1.0/tests/test_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     assert torch.all(original_weights != sp_linear.raw_weight_param), "Free weights should have changed"
     assert torch.all(original_bias != sp_linear.bias_param), "Free weights should have changed"
 
 
 def test_NegationLayer_forward():
     neg_layer = NegationLayer(
-        item_z_relationships=torch.tensor([1, 0, 1]),
+        item_theta_relationships=torch.tensor([1, 0, 1]),
         inputs_per_items=3,
         zero_outputs=torch.tensor([0, 0, 1, 0, 0, 0, 0, 0, 1]).bool(),
     )
     with torch.no_grad():
         neg_layer.weight_param[0].fill_(2)
         neg_layer.weight_param[1].fill_(-1)
 
@@ -91,15 +91,15 @@
         [ 4.,  4., 0., 0.,  0.,  0., -2., -2., 0.],
         [ 2.,  2., 0., 0.,  0.,  0.,  -1.,  -1., 0.],
         [-2., -2., 0., 0.,  0.,  0.,  1.,  1., 0.]
     ]))
 
 def test_NegationLayer_all_item_weights():
     neg_layer = NegationLayer(
-        item_z_relationships=torch.tensor([1, 0, 1]),
+        item_theta_relationships=torch.tensor([1, 0, 1]),
         inputs_per_items=3,
         zero_outputs=torch.tensor([0, 0, 1, 0, 0, 0, 0, 0, 1]).bool(),
     )
     with torch.no_grad():
         neg_layer.weight_param[0].fill_(2)
         neg_layer.weight_param[1].fill_(-1)
```

### Comparing `irtorch-0.0.4/tests/test_load_dataset.py` & `irtorch-0.1.0/tests/test_load_dataset.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/tests/test_outlier_detector.py` & `irtorch-0.1.0/tests/test_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/tests/test_quantile_mv_normal.py` & `irtorch-0.1.0/tests/test_quantile_mv_normal.py`

 * *Files identical despite different names*

### Comparing `irtorch-0.0.4/tests/test_utils.py` & `irtorch-0.1.0/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,32 @@
 import pytest
 import torch
-from irtorch.utils import get_item_categories, one_hot_encode_test_data, decode_one_hot_test_data, split_data
+from irtorch.utils import get_item_categories, one_hot_encode_test_data, decode_one_hot_test_data, split_data, impute_missing
 
 def test_get_item_categories(test_data, item_categories):
     result = get_item_categories(test_data)
     assert result == item_categories
 
+def test_impute_missing():
+    data = torch.tensor([[1, 2, 1, -1], [-1, float("nan"), 0, 2], [-1, float("nan"), 1, 2]])
+    # mc_correct is corresponds to correct item category and not correct score (2 means score 1 is correct)
+    mc_correct = [2, 3, 2, 3]
+    imputed_data = impute_missing(data = data.clone())
+    assert (imputed_data == torch.tensor([[1, 2, 1, 0], [0, 0, 0, 2], [0, 0, 1, 2]])).all()
+
+    imputed_data = impute_missing(data = data, mc_correct=mc_correct, item_categories=[3, 3, 2, 3])
+    missing_mask = torch.logical_or(data == -1, data.isnan())
+    assert (imputed_data[missing_mask] > -1).all() # all missing are replaced
+    assert (imputed_data[~missing_mask] == data[~missing_mask]).all() # non missing are still the same
+    assert imputed_data[0, 3] != 2 # we did not replace with true values
+    assert imputed_data[1, 0] != 1
+    assert imputed_data[1, 1] != 2
+    assert imputed_data[2, 0] != 1
+    assert imputed_data[2, 1] != 2
+
 def test_one_hot_encode_test_data(device):
     # Define a small tensor of test scores and a list of maximum scores
     #
     scores = (
         torch.tensor([[0, 1, 2], [1, 2, 3], [2, 0, float("nan")], [2, 0, -1]])
         .float()
         .to(device)
```

