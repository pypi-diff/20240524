# Comparing `tmp/flameai-1.0.2.tar.gz` & `tmp/flameai-1.0.3.tar.gz`

## Comparing `flameai-1.0.2.tar` & `flameai-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/__main__.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/_env.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/cmd.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/metrics.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/mining.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/plot.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/preprocessing.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/train.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/util.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 flameai-1.0.2/tests/test_metrics.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 flameai-1.0.2/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.2/LICENSE
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 flameai-1.0.2/README.md
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 flameai-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 flameai-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/__main__.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/_env.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/cmd.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/metrics.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/mining.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/plot.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/preprocessing.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/train.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/util.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 flameai-1.0.3/tests/test_metrics.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 flameai-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 flameai-1.0.3/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 flameai-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 flameai-1.0.3/PKG-INFO
```

### Comparing `flameai-1.0.2/src/flameai/_env.py` & `flameai-1.0.3/src/flameai/_env.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.2/src/flameai/cmd.py` & `flameai-1.0.3/src/flameai/cmd.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.2/src/flameai/metrics.py` & `flameai-1.0.3/src/flameai/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import numpy as np
 import pandas as pd
 import sklearn.metrics
 
+from enum import Enum
 from typing import Tuple, Optional, Any
 from .train import gen_threshold
 
 
+class Metric(Enum):
+    ACCURACY = sklearn.metrics.accuracy_score
+    PRECISION = sklearn.metrics.precision_score
+    RECALL = sklearn.metrics.recall_score
+    F1_SCORE = sklearn.metrics.f1_score
+
+
 def lgb_feature_importance(gbm) -> None:
     """
     Calculate the importance of features in a LightGBM model.
 
     :param gbm: The trained LightGBM model.
     """
     items = [(k, v) for k, v in zip(gbm.feature_name(), gbm.feature_importance())]
@@ -34,38 +42,40 @@
     print(f'mse: {mse:.5f}')
     print(f'r2_score: {r2_score:.5f}')
 
 
 def eval_binary(y_true,
                 y_pred,
                 threshold: Optional[float] = None,
+                metric: Metric = Metric.F1_SCORE,
                 n_trials: int = 200,
                 ret: bool = False
     ) -> Optional[Tuple[Any, float]]:
     """
     Evaluate a binary classification task.
 
     :param y_true: An array of the true values.
     :param y_pred: An array of the model's predictions.
     :param threshold: The threshold determines whether a case is positive or negative.
                       If the predicted probability is greater than the threshold,
                       it is classified as a positive case. If the threshold is None,
                       the optuna package will be used to calculate the optimal threshold.
+    :param metric: The metric used to evaluate the model. Default is Metric.F1_SCORE.
     :param n_trials: The number of trials for threshold generation. Default is 200.
     :param ret: A flag to indicate if the function should return the predicted labels and threshold. Default is False.
     :return: If ret is True, the function returns the predicted labels and threshold.
     """
 
     # Metrics that can be directly calculated using y_pred
     auc = sklearn.metrics.roc_auc_score(y_true = y_true, y_score = y_pred)
     log_loss = sklearn.metrics.log_loss(y_true = y_true, y_pred = y_pred)
 
     # If the threshold does not exist, obtain it
     if threshold is None:
-        threshold = gen_threshold(y_true, y_pred, n_trials)
+        threshold = gen_threshold(y_true, y_pred, metric, n_trials)
 
     y_label = [1 if e > threshold else 0 for e in y_pred]
 
     # Metrics that require the predicted labels (y_label)
     acc = sklearn.metrics.accuracy_score(y_true = y_true, y_pred = y_label)
     precision = sklearn.metrics.precision_score(y_true = y_true, y_pred = y_label)
     recall = sklearn.metrics.recall_score(y_true = y_true, y_pred = y_label)
```

### Comparing `flameai-1.0.2/src/flameai/plot.py` & `flameai-1.0.3/src/flameai/plot.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.2/src/flameai/preprocessing.py` & `flameai-1.0.3/src/flameai/preprocessing.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.2/src/flameai/train.py` & `flameai-1.0.3/src/flameai/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,33 +36,32 @@
                 print(f"Learning rate ==> {self.learning_rate:.3f} (-{pre - self.learning_rate:.4f})")
             self.wait_count = 0  # Reset wait_count
 
         # Update the learning rate
         env.model.params['learning_rate'] = self.learning_rate
 
 
-def gen_threshold(y_true, y_pred, n_trials):
+def gen_threshold(y_true, y_pred, metric, n_trials: int) -> float:
     """
-    Aiming to maximize the f1_score, find the optimal threshold.
+    Finds the optimal threshold based on the desired metric
     """
 
     # Set the logging level to ERROR
     verbose = optuna.logging.get_verbosity()
     optuna.logging.set_verbosity(optuna.logging.ERROR)
 
-    def f1_objective(trial):
+    def objective(trial):
         t = trial.suggest_float('threshold', 0.0, 1.0)
         y_label = [1 if e > t else 0 for e in y_pred]
-        f1 = sklearn.metrics.f1_score(y_true=y_true, y_pred=y_label)
-        return f1
-    
-    f1_study = optuna.create_study(direction='maximize')
-    f1_study.optimize(f1_objective, n_trials=n_trials)
-    best_params = f1_study.best_params
-    
+        return metric(y_true = y_true, y_pred = y_label)
+
+    study = optuna.create_study(direction = 'maximize')
+    study.optimize(objective, n_trials = n_trials)
+    best_params = study.best_params
+
     # Restore the original logging level
     optuna.logging.set_verbosity(verbose)
 
     return best_params['threshold']
 
 
 def gen_threshold_cdf(y_pred, rate: float, interval: int = 100) -> float:
```

### Comparing `flameai-1.0.2/src/flameai/util.py` & `flameai-1.0.3/src/flameai/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
              encoding: str = 'utf-8',
              dtype: dict = None
     ) -> pd.DataFrame:
     """
     Read a CSV file from the specified path.
     """
     return pd.read_csv(file_path,
-                       header=header,
-                       sep=sep,
-                       on_bad_lines=on_bad_lines,
-                       encoding=encoding,
-                       dtype=dtype)
+                       header = header,
+                       sep = sep,
+                       on_bad_lines = on_bad_lines,
+                       encoding = encoding,
+                       dtype = dtype)
 
 
 def set_logger(name: str = 'flameai', level: int = logging.WARNING):
     """
     Set up the logger for the application.
     """
     logger = logging.getLogger(name)
```

### Comparing `flameai-1.0.2/LICENSE` & `flameai-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flameai-1.0.2/README.md` & `flameai-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `flameai-1.0.2/pyproject.toml` & `flameai-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flameai"
-version = "1.0.2"
+version = "1.0.3"
 description = "Deep Learning Toolkit."
 readme = "README.md"
 keywords = [
   "deep learning",
   "flameai",
 ]
 license = { text = "Apache-2.0" }
```

### Comparing `flameai-1.0.2/PKG-INFO` & `flameai-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flameai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Deep Learning Toolkit.
 Project-URL: repository, https://github.com/luochang212/flameai
 Project-URL: bug-tracker, https://github.com/luochang212/flameai/issues
 Project-URL: documentation, https://luochang212.github.io/posts/flameai
 Author: luochang
 Author-email: luochang212@gmail.com
 License: Apache-2.0
```

