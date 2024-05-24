# Comparing `tmp/mag_net_hub-0.0.6.tar.gz` & `tmp/mag_net_hub-0.0.8.tar.gz`

## Comparing `mag_net_hub-0.0.6.tar` & `mag_net_hub-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/requirements.txt
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/__init__.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/loss.py
--rw-r--r--   0        0        0    20384 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/paderborn.py
--rw-r--r--   0        0        0    14852 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/sydney.py
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt
--rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt
--rw-r--r--   0        0        0    44502 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt
--rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C90.pt
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C92.pt
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C94.pt
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C95.pt
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3E6.pt
--rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3F4.pt
--rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/77.pt
--rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/78.pt
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/79.pt
--rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/ML95S.pt
--rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N27.pt
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N30.pt
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N49.pt
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N87.pt
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/src_py/magnethub/models/sydney/T37.pt
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/tests/test_paderborn.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/tests/test_sydney.py
--rw-r--r--   0        0        0  1524230 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/LICENSE
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/README.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 mag_net_hub-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/__init__.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/loss.py
+-rw-r--r--   0        0        0    20384 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/paderborn.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/sydney.py
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44451 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44349 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt
+-rw-r--r--   0        0        0    44170 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt
+-rw-r--r--   0        0        0    44502 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt
+-rw-r--r--   0        0        0    44400 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3C90.pt
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3C92.pt
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3C94.pt
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3C95.pt
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3E6.pt
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3F4.pt
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/77.pt
+-rw-r--r--   0        0        0     6930 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/78.pt
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/79.pt
+-rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/ML95S.pt
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/N27.pt
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/N30.pt
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/N49.pt
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/N87.pt
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/src_py/magnethub/models/sydney/T37.pt
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/tests/test_paderborn.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/tests/test_sydney.py
+-rw-r--r--   0        0        0  1524230 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/README.md
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 mag_net_hub-0.0.8/PKG-INFO
```

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/loss.py` & `mag_net_hub-0.0.8/src_py/magnethub/loss.py`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/paderborn.py` & `mag_net_hub-0.0.8/src_py/magnethub/paderborn.py`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/sydney.py` & `mag_net_hub-0.0.8/src_py/magnethub/sydney.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-File contains the model according to the Paderborn University approach for the magnet challenge.
+File contains the model according to the Sydney University approach for the magnet challenge.
 
 Source: https://github.com/moetomg/magnet-engine
 """
 import torch
 import numpy as np
 from scipy.signal import savgol_filter
 
@@ -20,91 +20,90 @@
     "T37": "T37.pt",
     "N27": "N27.pt",
     "N30": "N30.pt",
     "N49": "N49.pt",
     "N87": "N87.pt",
     "ML95S": "ML95S.pt",
 }
-
 # Material normalization data (1.B 2.H 3.F 4.T 5.dB/dt)
 normsDict ={"77":  [[-2.63253458e-19,  7.47821754e-02],
                     [-7.60950004e-18,  1.10664739e+01],
-                    [5.24678898e+00,  2.89351404e-01],
-                    [5.87473793e+01,  2.40667381e+01],
-                    [6.16727829e+00,  3.83645439e+01]],
-            "78":  [[5.67033925e-19,  7.22424510e-02],
+                    [ 5.24678898e+00,  2.89351404e-01],
+                    [ 5.87473793e+01,  2.40667381e+01],
+                    [ 6.16727829e+00,  3.83645439e+01]],
+            "78":  [[ 5.67033925e-19,  7.22424510e-02],
                     [-1.54283684e-16,  1.15338828e+01],
-                    [5.23810768e+00,  2.89979160e-01],
-                    [5.87434082e+01,  2.40685291e+01],
-                    [6.09561586e+00,  3.81356049e+01]],
-            "79":  [[1.70344847e-13,  9.41321492e-02],
+                    [ 5.23810768e+00,  2.89979160e-01],
+                    [ 5.87434082e+01,  2.40685291e+01],
+                    [ 6.09561586e+00,  3.81356049e+01]],
+            "79":  [[ 1.70344847e-13,  9.41321492e-02],
                     [-4.54025068e-02,  3.20463941e+01],
-                    [5.21954346e+00,  2.66715437e-01],
-                    [5.52068787e+01,  2.37196522e+01],
-                    [6.77422905e+00,  3.90895233e+01]],
-            "N27": [[7.52738469e-19,  7.48951129e-02],
+                    [ 5.21954346e+00,  2.66715437e-01],
+                    [ 5.52068787e+01,  2.37196522e+01],
+                    [ 6.77422905e+00,  3.90895233e+01]],
+            "N27": [[ 7.52738469e-19,  7.48951129e-02],
                     [-8.97477366e-17,  1.47606605e+01],
-                    [5.24649334e+00,  2.89964765e-01],
-                    [5.87355194e+01,  2.40766029e+01],
-                    [6.17841434e+00,  3.84738274e+01]],
-            "N30": [[1.43320465e-19,  6.56044649e-02],
+                    [ 5.24649334e+00,  2.89964765e-01],
+                    [ 5.87355194e+01,  2.40766029e+01],
+                    [ 6.17841434e+00,  3.84738274e+01]],
+            "N30": [[ 1.43320465e-19,  6.56044649e-02],
                     [-1.57874135e-16,  1.09083332e+01],
-                    [5.31786680e+00,  2.78960317e-01],
-                    [5.86466904e+01,  2.40616817e+01],
-                    [7.01255989e+00,  4.09709969e+01]],
+                    [ 5.31786680e+00,  2.78960317e-01],
+                    [ 5.86466904e+01,  2.40616817e+01],
+                    [ 7.01255989e+00,  4.09709969e+01]],
             "N49": [[-8.99073580e-19,  8.94479227e-02],
-                    [4.15423721e-16,  3.70622618e+01],
-                    [5.25545311e+00,  3.00384015e-01],
-                    [5.94716339e+01,  2.44349327e+01],
-                    [6.75209475e+00,  3.91901703e+01]],
-            "N87": [[1.72051200e-13,  6.26231476e-02],
-                    [4.02299992e-02,  7.61060358e+00],
-                    [5.26309967e+00,  2.87137657e-01],
-                    [5.83059006e+01,  2.40639057e+01],
-                    [6.53078842e+00,  3.93127785e+01]],
-            "3E6": [[1.01579639e-18,  7.04261607e-02],
-                    [2.34374135e-16,  7.21573964e+00],
-                    [5.34307003e+00,  2.66708523e-01],
-                    [5.86578026e+01,  2.40552864e+01],
-                    [7.23155785e+00,  4.15975838e+01]],
+                    [ 4.15423721e-16,  3.70622618e+01],
+                    [ 5.25545311e+00,  3.00384015e-01],
+                    [ 5.94716339e+01,  2.44349327e+01],
+                    [ 6.75209475e+00,  3.91901703e+01]],           
+            "N87": [[ 1.72051200e-13,  6.26231476e-02],
+                    [ 4.02299992e-02,  7.61060358e+00],
+                    [ 5.26309967e+00,  2.87137657e-01],
+                    [ 5.83059006e+01,  2.40639057e+01],
+                    [ 6.53078842e+00,  3.93127785e+01]],
+            "3E6": [[ 1.01579639e-18,  7.04261607e-02],
+                    [ 2.34374135e-16,  7.21573964e+00],
+                    [ 5.34307003e+00,  2.66708523e-01],
+                    [ 5.86578026e+01,  2.40552864e+01],
+                    [ 7.23155785e+00,  4.15975838e+01]],
             "3F4": [[-1.75200068e-19,  5.98892952e-02],
                     [-9.48865199e-18,  4.74414811e+01],
-                    [5.14398336e+00,  3.04210454e-01],
-                    [5.76523476e+01,  2.43824081e+01],
-                    [6.23030663e+00,  3.64991379e+01]],
-            "T37": [[1.72051200e-13,  6.26231476e-02],
-                    [4.02299992e-02,  7.61060358e+00],
-                    [5.26309967e+00,  2.87137657e-01],
-                    [5.83059006e+01,  2.40639057e+01],
-                    [6.53078842e+00,  3.93127785e+01]],
+                    [ 5.14398336e+00,  3.04210454e-01],
+                    [ 5.76523476e+01,  2.43824081e+01],
+                    [ 6.23030663e+00,  3.64991379e+01]],
+            "T37": [[ 1.72051200e-13,  6.26231476e-02],
+                    [ 4.02299992e-02,  7.61060358e+00],
+                    [ 5.26309967e+00,  2.87137657e-01],
+                    [ 5.83059006e+01,  2.40639057e+01],
+                    [ 6.53078842e+00,  3.93127785e+01]],
             "3C90":[[-3.27923689e-19,  6.56109348e-02],
-                    [6.99196716e-17,  1.26583787e+01],
-                    [5.19875193e+00,  2.68499136e-01],
-                    [5.86049919e+01,  2.40574703e+01],
-                    [6.29652929e+00,  3.84585190e+01]],
+                    [ 6.99196716e-17,  1.26583787e+01],
+                    [ 5.19875193e+00,  2.68499136e-01],
+                    [ 5.86049919e+01,  2.40574703e+01],
+                    [ 6.29652929e+00,  3.84585190e+01]],
             "3C92":[[-2.35520104e-13,  6.53518693e-02],
-                    [1.18689366e-01,  1.23585692e+01],
-                    [5.16579533e+00,  2.73998171e-01],
-                    [5.84305267e+01,  2.40970516e+01],
-                    [5.88209248e+00,  3.69935722e+01]],
-            "3C94":[[1.21232679e-19,  7.44383659e-02],
+                    [ 1.18689366e-01,  1.23585692e+01],
+                    [ 5.16579533e+00,  2.73998171e-01],
+                    [ 5.84305267e+01,  2.40970516e+01],
+                    [ 5.88209248e+00,  3.69935722e+01]],
+            "3C94":[[ 1.21232679e-19,  7.44383659e-02],
                     [-2.19613879e-17,  1.18042579e+01],
-                    [5.22766781e+00,  2.68348873e-01],
-                    [5.87128143e+01,  2.40769634e+01],
-                    [6.53718996e+00,  3.91955910e+01]],
-            "3C95":[[5.64116728e-14,  7.90115297e-02],
-                    [1.11898437e-01,  1.29696641e+01],
-                    [5.18842697e+00,  2.69014776e-01],
-                    [5.86223640e+01,  2.40957470e+01],
-                    [6.25767517e+00,  3.84026108e+01]],
+                    [ 5.22766781e+00,  2.68348873e-01],
+                    [ 5.87128143e+01,  2.40769634e+01],
+                    [ 6.53718996e+00,  3.91955910e+01]],
+            "3C95":[[ 5.64116728e-14,  7.90115297e-02],
+                    [ 1.11898437e-01,  1.29696641e+01],
+                    [ 5.18842697e+00,  2.69014776e-01],
+                    [ 5.86223640e+01,  2.40957470e+01],
+                    [ 6.25767517e+00,  3.84026108e+01]],
            "ML95S":[[-1.53185180e-13,  1.15827541e-01],
-                    [3.84426934e-01,  4.45061606e+01],
-                    [5.21606445e+00,  2.65364528e-01],
-                    [5.70770302e+01,  2.44398289e+01],
-                    [7.30377579e+00,  4.04136391e+01]],
+                    [ 3.84426934e-01,  4.45061606e+01],
+                    [ 5.21606445e+00,  2.65364528e-01],
+                    [ 5.70770302e+01,  2.44398289e+01],
+                    [ 7.30377579e+00,  4.04136391e+01]],
              }
 
 # %% Initialize model
 class SydneyModel:
     """The Sydney model."""
 
     def __init__(self, mdl_path, material):
@@ -118,36 +117,42 @@
         state_dict = torch.load(mdl_path, map_location=self.device)
         self.mdl.load_state_dict(state_dict,strict=True)
         
     
     def __call__(self, data_B, data_F, data_T):
         """Call method."""
         # ----------------------------------------------------------- batch execution  
-        # if isinstance(data_F, np.ndarray):
-
         # 1.Get dataloader
+        if data_B.ndim == 1:
+            data_B = np.array(data_B).reshape(1, -1)
+
         loader = get_dataloader(data_B,data_F,data_T,self.mdl.norm)
 
         # 2.Validate the models
         data_P = torch.Tensor([]).to(self.device)  # Allocate memory to store loss density
 
         with torch.no_grad():
             # Start model evaluation explicitly
             self.mdl.eval()
             for inputs, vars in loader:
                     Pv, h_series = self.mdl(inputs.to(self.device), vars.to(self.device))
 
                     data_P = torch.cat((data_P,Pv.to(self.device)),dim=0)
         data_P, h_series = data_P.cpu().numpy(), h_series.cpu().numpy()
+        
+        # 3.Return results 
         if data_P.size == 1:
             data_P = data_P.item()
         if h_series.ndim == 1:
             h_series = h_series.reshape(1, -1)
+            
         return data_P, h_series
 
+    
+
 class MMINet(torch.nn.Module):
     """
     Magnetization mechanism-determined neural network.
 
     Parameters:
     - hidden_size: number of eddy current slices (RNN neuron)
     - operator_size: number of operators
@@ -231,15 +236,15 @@
         Pv = torch.trapz(H, B, axis=1)*(10**(var[:, 0:1]*self.norm[2][1]+self.norm[2][0]))
 
         # Return results
         H = savgol_filter(H.detach().to("cpu").numpy(), window_length=7, polyorder=2,axis=1)
         H = torch.from_numpy(H).view(batch_size,-1,1)
         real_H = torch.cat((H[:, -self.n_init:, :],H[:, :-self.n_init, :]), dim=1)
         return torch.flatten(Pv).cpu(), real_H[:, :, 0].cpu()
-
+    
 class StopOperatorCell():
     """
     MMINN Sub-layer: Static hysteresis prediction using stop operators.
 
     Parameters:
     - operator_size: number of operator
     """
@@ -253,16 +258,15 @@
         return torch.max(-a,torch.min(a,X))
     
     def __call__(self, dB, state):
         """Update operator of each time step."""
         r = self.operator_thre.to(dB.device) 
         output = self.sslu((dB + state)/r)*r
         return output.float()
-
-
+  
 class EddyCell(torch.nn.Module):
     """
     MMINN subsubnetwork: Dynamic hysteresis prediction.
 
     Parameters:
     - input_size: feature size
     - hidden_size: number of hidden units (eddy current layers)
@@ -308,20 +312,22 @@
     data_T
          T data
     norm : list 
          B/F/T normalization data
     n_init : int
          Additional points for computing the history magnetization
     """
+    
     # Data pre-process 
     # 1. Down-sample to 128 points 
     seq_length = 128
-    cols = np.array(range(0,1023,8))
-    data_B = data_B[:, cols]
 
+    cols = np.array(range(0,data_B.shape[1],round(data_B.shape[1]/seq_length)))
+    data_B = data_B[:, cols]
+    
     # 2. Add extra points for initial magnetization calculation 
     data_length = seq_length + n_init
     data_B = np.hstack((data_B,data_B[:,1:1+n_init]))
 
     # 3. Format data into tensors 
     B = torch.from_numpy(data_B).view(-1, data_length, 1).float()
     if np.isscalar(data_F):
@@ -331,15 +337,15 @@
     T = torch.from_numpy(data_T).view(-1, 1).float()
     F = torch.from_numpy(np.log10(data_F)).view(-1,1).float()
 
     # 4. Data Normalization 
     in_B = (B-norm[0][0])/norm[0][1]
     in_F = (F-norm[2][0])/norm[2][1]
     in_T = (T-norm[3][0])/norm[3][1]
-
+    
     # 5. Extra features 
     in_dB = torch.diff(in_B,dim=1)                     # Flux density change
     in_dB = torch.cat((in_dB[:, 0:1, :], in_dB), dim=1)
     
     dB_dt = in_dB*(seq_length*F.reshape(-1, 1, 1))
     in_dB_dt = (dB_dt-norm[4][0])/norm[4][1]        # Flux density change rate
     
@@ -367,17 +373,17 @@
     dB : torch_like (batch, data_length)
          Flux density changes at each t
     Bmax: torch_like (batch)
          Max flux density of each cycle
     Bmin: torch_like (batch)
          Min flux density of each cycle
     operator_size: int
-         TBD
+         The number of operators 
     max_out_H:
-         TBD
+         The maximum output of field strength
     """
     # 1. Parameter setting
     batch = dB.shape[0]
     state = torch.zeros((batch, operator_size))
     operator_thre = torch.pow(torch.arange(1, operator_size+1, dtype=torch.float)/operator_size+1, torch.tensor(3.0)).view(1, -1)*max_out_H
 
     # 2. Iterate each excitation for the operator inital state computation
```

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3C90_experiment_1b4d8_model_f3915868_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3C92_experiment_ea1fe_model_72510647_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3C94_experiment_56441_model_55693612_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3C95_experiment_ad6ec_model_046383a5_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3E6_experiment_a7817_model_a1035e58_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_3F4_experiment_c234d_model_2d43b97d_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_77_experiment_268ae_model_5b7c92ed_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_78_experiment_e5297_model_77fbd758_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_79_experiment_45989_model_7227af72_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_A_experiment_c9cfe_model_d893c778_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_B_experiment_c9cfe_model_b6a920cc_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_C_experiment_c9cfe_model_c1ced7b6_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_D_experiment_c9cfe_model_11672810_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_E_experiment_c9cfe_model_5ae50f9e_p.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_ML95S_experiment_1c978_model_883a5d2f_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_N27_experiment_8b7f0_model_20954a2a_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_N30_experiment_5a78c_model_6bd86623_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_N49_experiment_27442_model_d6234a32_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_N87_experiment_985cb_model_d51b0f7e_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/paderborn/cnn_T37_experiment_a084a_model_fb31325e_seed_0_fold_0.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C90.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3C90.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C92.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3C95.pt`

 * *Files 22% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7074 bytes, number of entries: 10
--rw----     0.0 fat      749 bl stor 80-000-00 00:00 MMINN_Material A/data.pkl
--rw----     0.0 fat        6 bl stor 80-000-00 00:00 MMINN_Material A/byteorder
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 MMINN_Material A/data/0
--rw----     0.0 fat        4 bl stor 80-000-00 00:00 MMINN_Material A/data/1
--rw----     0.0 fat      480 bl stor 80-000-00 00:00 MMINN_Material A/data/2
--rw----     0.0 fat     3600 bl stor 80-000-00 00:00 MMINN_Material A/data/3
--rw----     0.0 fat      120 bl stor 80-000-00 00:00 MMINN_Material A/data/4
--rw----     0.0 fat        4 bl stor 80-000-00 00:00 MMINN_Material A/data/5
--rw----     0.0 fat        2 bl stor 80-000-00 00:00 MMINN_Material A/version
--rw----     0.0 fat       40 bl stor 80-000-00 00:00 MMINN_Material A/.data/serialization_id
+-rw----     0.0 fat      749 bl stor 80-000-00 00:00 MMINN_Material C/data.pkl
+-rw----     0.0 fat        6 bl stor 80-000-00 00:00 MMINN_Material C/byteorder
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 MMINN_Material C/data/0
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 MMINN_Material C/data/1
+-rw----     0.0 fat      480 bl stor 80-000-00 00:00 MMINN_Material C/data/2
+-rw----     0.0 fat     3600 bl stor 80-000-00 00:00 MMINN_Material C/data/3
+-rw----     0.0 fat      120 bl stor 80-000-00 00:00 MMINN_Material C/data/4
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 MMINN_Material C/data/5
+-rw----     0.0 fat        2 bl stor 80-000-00 00:00 MMINN_Material C/version
+-rw----     0.0 fat       40 bl stor 80-000-00 00:00 MMINN_Material C/.data/serialization_id
 10 files, 5133 bytes uncompressed, 5133 bytes compressed:  0.0%
```

#### zipnote «TEMP»/diffoscope_fvi51vcn_/tmpet2bec24_.zip

```diff
@@ -1,31 +1,31 @@
-Filename: MMINN_Material A/data.pkl
+Filename: MMINN_Material C/data.pkl
 Comment: 
 
-Filename: MMINN_Material A/byteorder
+Filename: MMINN_Material C/byteorder
 Comment: 
 
-Filename: MMINN_Material A/data/0
+Filename: MMINN_Material C/data/0
 Comment: 
 
-Filename: MMINN_Material A/data/1
+Filename: MMINN_Material C/data/1
 Comment: 
 
-Filename: MMINN_Material A/data/2
+Filename: MMINN_Material C/data/2
 Comment: 
 
-Filename: MMINN_Material A/data/3
+Filename: MMINN_Material C/data/3
 Comment: 
 
-Filename: MMINN_Material A/data/4
+Filename: MMINN_Material C/data/4
 Comment: 
 
-Filename: MMINN_Material A/data/5
+Filename: MMINN_Material C/data/5
 Comment: 
 
-Filename: MMINN_Material A/version
+Filename: MMINN_Material C/version
 Comment: 
 
-Filename: MMINN_Material A/.data/serialization_id
+Filename: MMINN_Material C/.data/serialization_id
 Comment: 
 
 Zip file comment:
```

#### Comparing `MMINN_Material A/data.pkl` & `MMINN_Material C/data.pkl`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C94.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3C94.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3C95.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/N30.pt`

 * *Files 27% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7074 bytes, number of entries: 10
--rw----     0.0 fat      749 bl stor 80-000-00 00:00 MMINN_Material C/data.pkl
--rw----     0.0 fat        6 bl stor 80-000-00 00:00 MMINN_Material C/byteorder
--rw----     0.0 fat      128 bl stor 80-000-00 00:00 MMINN_Material C/data/0
--rw----     0.0 fat        4 bl stor 80-000-00 00:00 MMINN_Material C/data/1
--rw----     0.0 fat      480 bl stor 80-000-00 00:00 MMINN_Material C/data/2
--rw----     0.0 fat     3600 bl stor 80-000-00 00:00 MMINN_Material C/data/3
--rw----     0.0 fat      120 bl stor 80-000-00 00:00 MMINN_Material C/data/4
--rw----     0.0 fat        4 bl stor 80-000-00 00:00 MMINN_Material C/data/5
--rw----     0.0 fat        2 bl stor 80-000-00 00:00 MMINN_Material C/version
--rw----     0.0 fat       40 bl stor 80-000-00 00:00 MMINN_Material C/.data/serialization_id
+Zip file size: 6940 bytes, number of entries: 10
+-rw----     0.0 fat      749 bl stor 80-000-00 00:00 MMINN_N30/data.pkl
+-rw----     0.0 fat        6 bl stor 80-000-00 00:00 MMINN_N30/byteorder
+-rw----     0.0 fat      128 bl stor 80-000-00 00:00 MMINN_N30/data/0
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 MMINN_N30/data/1
+-rw----     0.0 fat      480 bl stor 80-000-00 00:00 MMINN_N30/data/2
+-rw----     0.0 fat     3600 bl stor 80-000-00 00:00 MMINN_N30/data/3
+-rw----     0.0 fat      120 bl stor 80-000-00 00:00 MMINN_N30/data/4
+-rw----     0.0 fat        4 bl stor 80-000-00 00:00 MMINN_N30/data/5
+-rw----     0.0 fat        2 bl stor 80-000-00 00:00 MMINN_N30/version
+-rw----     0.0 fat       40 bl stor 80-000-00 00:00 MMINN_N30/.data/serialization_id
 10 files, 5133 bytes uncompressed, 5133 bytes compressed:  0.0%
```

#### zipnote «TEMP»/diffoscope_fvi51vcn_/tmpzy0f6fav_.zip

```diff
@@ -1,31 +1,31 @@
-Filename: MMINN_Material C/data.pkl
+Filename: MMINN_N30/data.pkl
 Comment: 
 
-Filename: MMINN_Material C/byteorder
+Filename: MMINN_N30/byteorder
 Comment: 
 
-Filename: MMINN_Material C/data/0
+Filename: MMINN_N30/data/0
 Comment: 
 
-Filename: MMINN_Material C/data/1
+Filename: MMINN_N30/data/1
 Comment: 
 
-Filename: MMINN_Material C/data/2
+Filename: MMINN_N30/data/2
 Comment: 
 
-Filename: MMINN_Material C/data/3
+Filename: MMINN_N30/data/3
 Comment: 
 
-Filename: MMINN_Material C/data/4
+Filename: MMINN_N30/data/4
 Comment: 
 
-Filename: MMINN_Material C/data/5
+Filename: MMINN_N30/data/5
 Comment: 
 
-Filename: MMINN_Material C/version
+Filename: MMINN_N30/version
 Comment: 
 
-Filename: MMINN_Material C/.data/serialization_id
+Filename: MMINN_N30/.data/serialization_id
 Comment: 
 
 Zip file comment:
```

#### Comparing `MMINN_Material C/data.pkl` & `MMINN_N30/data.pkl`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3E6.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3E6.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/3F4.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/3F4.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/77.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/77.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/78.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/78.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/79.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/79.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/ML95S.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/ML95S.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N27.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/N27.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N49.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/N49.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/N87.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/N87.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/src_py/magnethub/models/sydney/T37.pt` & `mag_net_hub-0.0.8/src_py/magnethub/models/sydney/T37.pt`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/tests/test_paderborn.py` & `mag_net_hub-0.0.8/tests/test_paderborn.py`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/tests/test_sydney.py` & `mag_net_hub-0.0.8/tests/test_sydney.py`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv` & `mag_net_hub-0.0.8/tests/test_files/unit_test_data_ploss_at_450kWpm3.csv`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/.gitignore` & `mag_net_hub-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/LICENSE` & `mag_net_hub-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/README.md` & `mag_net_hub-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mag_net_hub-0.0.6/pyproject.toml` & `mag_net_hub-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mag-net-hub"
-version = "0.0.6"
+version = "0.0.8"
 authors = [
     { name = "Wilhelm Kirchgässner" },
 ]
 description = "MagNet Toolkit - Certified Models of the MagNet Challenge"
 readme = "README.md"
 requires-python = "~=3.10"
 classifiers = [
@@ -68,8 +68,8 @@
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 skip-magic-trailing-comma = false
-line-ending = "auto"
+line-ending = "auto"
```

### Comparing `mag_net_hub-0.0.6/PKG-INFO` & `mag_net_hub-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: mag-net-hub
-Version: 0.0.6
+Version: 0.0.8
 Summary: MagNet Toolkit - Certified Models of the MagNet Challenge
 Project-URL: Homepage, https://github.com/upb-lea/mag-net-hub
 Project-URL: Issues, https://github.com/upb-lea/mag-net-hub/issues
 Author: Wilhelm Kirchgässner
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.10
 Requires-Dist: joblib>=1.3.2
-Requires-Dist: pandas>=2.0.3
+Requires-Dist: pandas>=2
 Requires-Dist: scipy
 Requires-Dist: torch>=2.0.1
 Requires-Dist: torchinfo>=1.8.0
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
```

