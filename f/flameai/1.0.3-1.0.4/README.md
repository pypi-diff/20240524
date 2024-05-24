# Comparing `tmp/flameai-1.0.3.tar.gz` & `tmp/flameai-1.0.4.tar.gz`

## Comparing `flameai-1.0.3.tar` & `flameai-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,23 @@
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/__main__.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/_env.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/cmd.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/metrics.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/mining.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/plot.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/preprocessing.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/train.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 flameai-1.0.3/src/flameai/util.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 flameai-1.0.3/tests/test_metrics.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 flameai-1.0.3/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.3/LICENSE
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 flameai-1.0.3/README.md
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 flameai-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 flameai-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 flameai-1.0.4/.flake8
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 flameai-1.0.4/noxfile.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 flameai-1.0.4/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/__main__.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/_env.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/cmd.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/metrics.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/mining.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/plot.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/preprocessing.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/train.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 flameai-1.0.4/src/flameai/util.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_metrics.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_mining.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_plot.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_preprocessing.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 flameai-1.0.4/tests/test_train.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 flameai-1.0.4/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 flameai-1.0.4/README.md
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 flameai-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 flameai-1.0.4/PKG-INFO
```

### Comparing `flameai-1.0.3/src/flameai/cmd.py` & `flameai-1.0.4/src/flameai/cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import subprocess
+
 import click
 
-from .util import set_logger
 from ._env import check_hive_env
+from .util import set_logger
 
 
 logger = set_logger()
 
 
 @click.command()
 @click.option('-n', '--name', default='World', help='Name to greet')
@@ -27,16 +28,16 @@
     else:
         command = f'hive -f {file_name}.hql > {file_name}.csv'
         logger.info(f'Run `{command}`')
 
         try:
             res = subprocess.run(command, shell=True, text=True)
             if res.returncode != 0:
-                logger.warning(f'Failed to execute query.')
+                logger.warning('Failed to execute query.')
                 logger.error(f'Error: {res.stderr}')
                 logger.error(f'returncode: {res.returncode}')
         except Exception as e:
             logger.error(f'An Error occurred: {e}')
 
 
 if __name__ == "__main__":
-    hive_cli()
+    hive_cli()
```

### Comparing `flameai-1.0.3/src/flameai/metrics.py` & `flameai-1.0.4/src/flameai/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import numpy as np
-import pandas as pd
+from enum import Enum
+from typing import Any, Optional, Tuple
+
 import sklearn.metrics
 
-from enum import Enum
-from typing import Tuple, Optional, Any
 from .train import gen_threshold
 
 
 class Metric(Enum):
     ACCURACY = sklearn.metrics.accuracy_score
     PRECISION = sklearn.metrics.precision_score
     RECALL = sklearn.metrics.recall_score
@@ -17,17 +16,17 @@
 def lgb_feature_importance(gbm) -> None:
     """
     Calculate the importance of features in a LightGBM model.
 
     :param gbm: The trained LightGBM model.
     """
     items = [(k, v) for k, v in zip(gbm.feature_name(), gbm.feature_importance())]
-    sorted_items = sorted(items, key = lambda e: e[1], reverse = True)
+    sorted_items = sorted(items, key=lambda e: e[1], reverse=True)
     for i, (k, v) in enumerate(sorted_items):
-        print(f'[rank {i+1}] {k}: {v}')
+        print(f'[rank {i + 1}] {k}: {v}')
 
 
 def eval_continuous(y_true, y_pred) -> None:
     """
     This function evaluates the performance of a regression model by calculating
     the Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R2) score.
 
@@ -39,52 +38,54 @@
     r2_score = sklearn.metrics.r2_score(y_true, y_pred)
 
     print(f'mae: {mae:.5f}')
     print(f'mse: {mse:.5f}')
     print(f'r2_score: {r2_score:.5f}')
 
 
-def eval_binary(y_true,
-                y_pred,
-                threshold: Optional[float] = None,
-                metric: Metric = Metric.F1_SCORE,
-                n_trials: int = 200,
-                ret: bool = False
-    ) -> Optional[Tuple[Any, float]]:
+def eval_binary(
+    y_true,
+    y_pred,
+    threshold: Optional[float] = None,
+    metric: Metric = Metric.F1_SCORE,
+    n_trials: int = 200,
+    ret: bool = False
+) -> Optional[Tuple[Any, float]]:
     """
     Evaluate a binary classification task.
 
     :param y_true: An array of the true values.
     :param y_pred: An array of the model's predictions.
     :param threshold: The threshold determines whether a case is positive or negative.
                       If the predicted probability is greater than the threshold,
                       it is classified as a positive case. If the threshold is None,
                       the optuna package will be used to calculate the optimal threshold.
     :param metric: The metric used to evaluate the model. Default is Metric.F1_SCORE.
     :param n_trials: The number of trials for threshold generation. Default is 200.
-    :param ret: A flag to indicate if the function should return the predicted labels and threshold. Default is False.
+    :param ret: A flag to indicate if the function should return the predicted
+                labels and threshold. Default is False.
     :return: If ret is True, the function returns the predicted labels and threshold.
     """
 
     # Metrics that can be directly calculated using y_pred
-    auc = sklearn.metrics.roc_auc_score(y_true = y_true, y_score = y_pred)
-    log_loss = sklearn.metrics.log_loss(y_true = y_true, y_pred = y_pred)
+    auc = sklearn.metrics.roc_auc_score(y_true=y_true, y_score=y_pred)
+    log_loss = sklearn.metrics.log_loss(y_true=y_true, y_pred=y_pred)
 
     # If the threshold does not exist, obtain it
     if threshold is None:
         threshold = gen_threshold(y_true, y_pred, metric, n_trials)
 
     y_label = [1 if e > threshold else 0 for e in y_pred]
 
     # Metrics that require the predicted labels (y_label)
-    acc = sklearn.metrics.accuracy_score(y_true = y_true, y_pred = y_label)
-    precision = sklearn.metrics.precision_score(y_true = y_true, y_pred = y_label)
-    recall = sklearn.metrics.recall_score(y_true = y_true, y_pred = y_label)
-    f1 = sklearn.metrics.f1_score(y_true = y_true, y_pred = y_label)
-    cm = sklearn.metrics.confusion_matrix(y_true = y_true, y_pred = y_label)
+    acc = sklearn.metrics.accuracy_score(y_true=y_true, y_pred=y_label)
+    precision = sklearn.metrics.precision_score(y_true=y_true, y_pred=y_label)
+    recall = sklearn.metrics.recall_score(y_true=y_true, y_pred=y_label)
+    f1 = sklearn.metrics.f1_score(y_true=y_true, y_pred=y_label)
+    cm = sklearn.metrics.confusion_matrix(y_true=y_true, y_pred=y_label)
     tn, fp, fn, tp = cm.ravel()
 
     print(f'threshold: {threshold:.5f}')
     print(f'accuracy: {acc:.5f}')
     print(f'precision: {precision:.5f}')
     print(f'recall: {recall:.5f}')
     print(f'f1_score: {f1:.5f}')
@@ -93,8 +94,8 @@
     print(f'True Positive (TP): {tp}')
     print(f'True Negative (TN): {tn}')
     print(f'False Positive (FP): {fp}')
     print(f'False Negative (FN): {fn}')
     print(f'confusion matrix:\n{cm}')
 
     if ret:
-        return y_label, threshold
+        return y_label, threshold
```

### Comparing `flameai-1.0.3/src/flameai/plot.py` & `flameai-1.0.4/src/flameai/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-import pandas as pd
-import sklearn.metrics
 import matplotlib.pyplot as plt
+import pandas as pd
 import seaborn as sns
+import sklearn.metrics
 
 
 def roc_curve(y_true, y_score) -> None:
     """
     Plot the ROC curve.
 
     :param y_true: An array of true binary labels.
     :param y_score: An array of predicted probabilities.
     """
-    fpr, tpr, thresholds = sklearn.metrics.roc_curve(y_true = y_true, y_score = y_score)
-    auc = sklearn.metrics.roc_auc_score(y_true = y_true, y_score = y_score)
+    fpr, tpr, thresholds = sklearn.metrics.roc_curve(y_true=y_true, y_score=y_score)
+    auc = sklearn.metrics.roc_auc_score(y_true=y_true, y_score=y_score)
     print(f'AUC: {auc:.5f}')
 
-    plt.figure(figsize = (8, 6))
+    plt.figure(figsize=(8, 6))
     plt.plot(fpr, tpr, label='ROC curve (AUC = {:.2f})'.format(auc))
 
     plt.title('Receiver Operating Characteristic (ROC) Curve')
     plt.xlabel('False Positive Rate (FPR)')
     plt.ylabel('True Positive Rate (TPR)')
     plt.legend(loc="lower right")
-    plt.grid(True, linestyle = 'dashed', alpha = 0.5)
+    plt.grid(True, linestyle='dashed', alpha=0.5)
 
     plt.show()
 
 
 def confusion_matrix(y_true, y_label) -> None:
     """
     Generates and plots a confusion matrix of a classification model.
 
     :param y_true: An array of true binary labels.
     :param y_label: An array of labels predicted by the model.
     """
-    cm = sklearn.metrics.confusion_matrix(y_true = y_true, y_pred = y_label)
-    cm_matrix = pd.DataFrame(data = cm,
-                             columns = ['Predict Negative:0', 'Predict Positive:1'], 
-                             index = ['Actual Negative:0', 'Actual Positive:1'])
-    sns.heatmap(cm_matrix, annot = True, fmt = 'd', cmap = 'YlGnBu')
+    cm = sklearn.metrics.confusion_matrix(y_true=y_true, y_pred=y_label)
+    cm_matrix = pd.DataFrame(data=cm,
+                             columns=['Predict Negative:0', 'Predict Positive:1'],
+                             index=['Actual Negative:0', 'Actual Positive:1'])
+    sns.heatmap(cm_matrix, annot=True, fmt='d', cmap='YlGnBu')
+
+    plt.show()
```

### Comparing `flameai-1.0.3/src/flameai/preprocessing.py` & `flameai-1.0.4/src/flameai/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import math
 import numpy as np
 import pandas as pd
 import sklearn.preprocessing
-import torch
 
 
 def label_encoder(df: pd.DataFrame) -> pd.DataFrame:
     """
     Encode categorical features (String) into integers (int).
     """
     cat_feats = [col for col in df.columns if df[col].dtypes == np.dtype('object')]
@@ -23,15 +21,15 @@
     total_positive_samples = sum(y_train)
     total_negative_samples = len(y_train) - sum(y_train)
     scale_pos_weight = total_negative_samples / total_positive_samples
     return scale_pos_weight
 
 
 class DataLoader:
-    def __init__(self, lst: list = []):
+    def __init__(self, lst: list):
         self.i = 0
         self._data = lst
 
     @property
     def data(self):
         return self._data
 
@@ -45,20 +43,7 @@
 
     def __next__(self):
         if self.i < len(self._data):
             self.i += 1
             return self._data[self.i - 1]
         else:
             raise StopIteration
-
-
-def data_iter(data: list, batch_size: int) -> DataLoader:
-    """Split the original input data list into batches."""
-    lst = []
-    batch_num = math.floor(len(data) / batch_size)
-    for i in range(batch_num):
-        start, end = batch_size * i, batch_size * (i + 1)
-        X = torch.tensor([e[0] for e in data[start:end]])
-        y = torch.tensor([e[1] for e in data[start:end]])
-        lst.append((X, y))
-
-    return DataLoader(lst)
```

### Comparing `flameai-1.0.3/src/flameai/train.py` & `flameai-1.0.4/src/flameai/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from typing import Optional
+
 import numpy as np
-import scipy
-import sklearn.metrics
 import optuna
+import scipy
 
 
 class AdaptiveLearningRate:
     """Customized learning rate decay"""
+
     def __init__(self,
                  learning_rate: float = 0.3,
                  decay_rate: float = 0.9,
-                 patience: int = 10
-        ) -> None:
+                 patience: int = 10) -> None:
         self.learning_rate = learning_rate
         self.decay_rate = decay_rate
         self.patience = patience
         self.best_score = float('inf')
         self.wait_count = 0
 
     def callback(self, env):
@@ -29,15 +30,18 @@
 
         # If there has been no improvement for 'patience' attempts
         # Decay the learning rate
         if self.wait_count >= self.patience:
             pre = self.learning_rate
             self.learning_rate *= self.decay_rate
             if env.params.get('verbose', 0) >= 0:
-                print(f"Learning rate ==> {self.learning_rate:.3f} (-{pre - self.learning_rate:.4f})")
+                print(
+                    f"Learning rate ==> {self.learning_rate:.3f} "
+                    f"(-{pre - self.learning_rate:.4f})"
+                )
             self.wait_count = 0  # Reset wait_count
 
         # Update the learning rate
         env.model.params['learning_rate'] = self.learning_rate
 
 
 def gen_threshold(y_true, y_pred, metric, n_trials: int) -> float:
@@ -48,27 +52,27 @@
     # Set the logging level to ERROR
     verbose = optuna.logging.get_verbosity()
     optuna.logging.set_verbosity(optuna.logging.ERROR)
 
     def objective(trial):
         t = trial.suggest_float('threshold', 0.0, 1.0)
         y_label = [1 if e > t else 0 for e in y_pred]
-        return metric(y_true = y_true, y_pred = y_label)
+        return metric(y_true=y_true, y_pred=y_label)
 
-    study = optuna.create_study(direction = 'maximize')
-    study.optimize(objective, n_trials = n_trials)
+    study = optuna.create_study(direction='maximize')
+    study.optimize(objective, n_trials=n_trials)
     best_params = study.best_params
 
     # Restore the original logging level
     optuna.logging.set_verbosity(verbose)
 
     return best_params['threshold']
 
 
-def gen_threshold_cdf(y_pred, rate: float, interval: int = 100) -> float:
+def gen_threshold_cdf(y_pred, rate: float, interval: int = 100) -> Optional[float]:
     """
     Finds the optimal threshold based on the desired proportion of negative samples (label 0)
 
     :param y_pred: An array of predicted probabilities.
     :param rate: The proportion of negative samples.
     :param interval: The number of intervals.
     :return: The optimal threshold.
@@ -77,12 +81,11 @@
     kde = scipy.stats.gaussian_kde(y_pred)
     pdf = kde.evaluate(xx)
     cdf = np.cumsum(pdf) * (xx[1] - xx[0])
 
     px = 0
     for x, y in zip(xx, cdf):
         if y > rate:
-            xa = (px + x) / 2
-            break
+            return (px + x) / 2
         px = x
 
-    return xa
+    return None
```

### Comparing `flameai-1.0.3/src/flameai/util.py` & `flameai-1.0.4/src/flameai/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,61 @@
-import os
 import logging
+import os
+
 import pandas as pd
 
 
-def gen_abspath(dir: str, rel_path: str) -> str:
+def gen_abspath(directory: str, rel_path: str) -> str:
     """
     Generate the absolute path by combining the given directory with a relative path.
 
-    :param dir: The specified directory, which can be either an absolute or a relative path.
+    :param directory: The specified directory, which can be either an absolute or a relative path.
     :param rel_path: The relative path with respect to the 'dir'.
-    :return: The resulting absolute path formed by concatenating the absolute directory and the relative path.
+    :return: The resulting absolute path formed by concatenating the absolute directory
+             and the relative path.
     """
-    abs_dir = os.path.abspath(dir)
+    abs_dir = os.path.abspath(directory)
     return os.path.join(abs_dir, rel_path)
 
 
-def read_csv(file_path: str,
-             sep: str = ',',
-             header: int = 0,
-             on_bad_lines: str = 'warn',
-             encoding: str = 'utf-8',
-             dtype: dict = None
-    ) -> pd.DataFrame:
+def read_csv(
+    file_path: str,
+    sep: str = ',',
+    header: int = 0,
+    on_bad_lines: str = 'warn',
+    encoding: str = 'utf-8',
+    dtype: dict = None
+) -> pd.DataFrame:
     """
     Read a CSV file from the specified path.
     """
     return pd.read_csv(file_path,
-                       header = header,
-                       sep = sep,
-                       on_bad_lines = on_bad_lines,
-                       encoding = encoding,
-                       dtype = dtype)
+                       header=header,
+                       sep=sep,
+                       on_bad_lines=on_bad_lines,
+                       encoding=encoding,
+                       dtype=dtype)
 
 
-def set_logger(name: str = 'flameai', level: int = logging.WARNING):
+def set_logger(name: str = 'FlameAI', level: int = logging.WARNING):
     """
     Set up the logger for the application.
     """
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
 
     # Create stream_handler and set level
     stream_handler = logging.StreamHandler()
     stream_handler.setLevel(level)
 
     # Create formatter
     formatter = logging.Formatter(
-        fmt = '%(asctime)s %(levelname)s [%(name)s]: (%(module)s:%(funcName)s(%(lineno)d)) - %(message)s',
-        datefmt = '%Y-%m-%d %H:%M:%S'
+        fmt='%(asctime)s %(levelname)s [%(name)s]: '
+            '(%(module)s:%(funcName)s(%(lineno)d)) - %(message)s',
+        datefmt='%Y-%m-%d %H:%M:%S'
     )
     stream_handler.setFormatter(formatter)  # add formatter to stream_handler
 
     # add stream_handler to logger
     logger.addHandler(stream_handler)
 
-    return logger
+    return logger
```

### Comparing `flameai-1.0.3/LICENSE` & `flameai-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flameai-1.0.3/README.md` & `flameai-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -78,14 +78,35 @@
 # or install from local wheel
 # `pip install dist/flameai-[VERSION]-py3-none-any.whl`
 
 # uninstall
 pip uninstall flameai
 ```
 
+Test:
+
+```
+# install pytest
+pip install pytest
+
+# run tests
+pytest
+```
+
+Lint:
+
+```
+# install flake8 and flake8-import-order
+pip install flake8
+pip install flake8-import-order
+
+# lint
+flake8 --import-order-style google
+```
+
 ## Development
 
 Build:
 
 ```bash
 python3 -m pip install --upgrade build
```

### Comparing `flameai-1.0.3/pyproject.toml` & `flameai-1.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flameai"
-version = "1.0.3"
+version = "1.0.4"
 description = "Deep Learning Toolkit."
 readme = "README.md"
 keywords = [
   "deep learning",
   "flameai",
 ]
 license = { text = "Apache-2.0" }
 authors = [
   { name = "luochang" },
   { email = "luochang212@gmail.com" },
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 dependencies = [
-  "numpy>=1.26.4",
-  "pandas>=2.2.0",
-  "scipy>=1.13.0",
-  "scikit-learn>=1.5.0",
-  "matplotlib>=3.8.4",
+  "numpy>=1.24.4",
+  "pandas>=2.0.3",
+  "scipy>=1.10.1",
+  "scikit-learn>=1.3.2",
+  "matplotlib>=3.7.5",
   "seaborn>=0.13.2",
   "optuna>=3.6.1",
   "click>=8.1.7",
-  "torch>=2.2.2",
 ]
 classifiers = [
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: MacOS",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
   "Operating System :: Unix",
```

### Comparing `flameai-1.0.3/PKG-INFO` & `flameai-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flameai
-Version: 1.0.3
+Version: 1.0.4
 Summary: Deep Learning Toolkit.
 Project-URL: repository, https://github.com/luochang212/flameai
 Project-URL: bug-tracker, https://github.com/luochang212/flameai/issues
 Project-URL: documentation, https://luochang212.github.io/posts/flameai
 Author: luochang
 Author-email: luochang212@gmail.com
 License: Apache-2.0
@@ -17,24 +17,23 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: click>=8.1.7
-Requires-Dist: matplotlib>=3.8.4
-Requires-Dist: numpy>=1.26.4
+Requires-Dist: matplotlib>=3.7.5
+Requires-Dist: numpy>=1.24.4
 Requires-Dist: optuna>=3.6.1
-Requires-Dist: pandas>=2.2.0
-Requires-Dist: scikit-learn>=1.5.0
-Requires-Dist: scipy>=1.13.0
+Requires-Dist: pandas>=2.0.3
+Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: scipy>=1.10.1
 Requires-Dist: seaborn>=0.13.2
-Requires-Dist: torch>=2.2.2
 Description-Content-Type: text/markdown
 
 # 🔥 FlameAI
 
 Deep Learning Toolkit.
 
 ## Installation
@@ -113,14 +112,35 @@
 # or install from local wheel
 # `pip install dist/flameai-[VERSION]-py3-none-any.whl`
 
 # uninstall
 pip uninstall flameai
 ```
 
+Test:
+
+```
+# install pytest
+pip install pytest
+
+# run tests
+pytest
+```
+
+Lint:
+
+```
+# install flake8 and flake8-import-order
+pip install flake8
+pip install flake8-import-order
+
+# lint
+flake8 --import-order-style google
+```
+
 ## Development
 
 Build:
 
 ```bash
 python3 -m pip install --upgrade build
```

