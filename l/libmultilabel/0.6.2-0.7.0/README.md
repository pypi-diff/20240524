# Comparing `tmp/libmultilabel-0.6.2.tar.gz` & `tmp/libmultilabel-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmultilabel-0.6.2.tar", last modified: Thu Mar  7 06:42:56 2024, max compression
+gzip compressed data, was "libmultilabel-0.7.0.tar", last modified: Fri May 24 13:44:56 2024, max compression
```

## Comparing `libmultilabel-0.6.2.tar` & `libmultilabel-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:42:56.519261 libmultilabel-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-07 06:42:56.519261 libmultilabel-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:42:56.511261 libmultilabel-0.6.2/libmultilabel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:42:56.515261 libmultilabel-0.6.2/libmultilabel/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/linear/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23267 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/linear/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/linear/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/linear/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/linear/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/linear/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:42:56.515261 libmultilabel-0.6.2/libmultilabel/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9092 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:42:56.515261 libmultilabel-0.6.2/libmultilabel/nn/networks/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/networks/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/networks/bert_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/networks/caml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/networks/kim_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10107 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/networks/labelwise_attention_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/networks/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/networks/xml_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/libmultilabel/nn/nn_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 06:42:56.519261 libmultilabel-0.6.2/libmultilabel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-07 06:42:56.000000 libmultilabel-0.6.2/libmultilabel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-07 06:42:56.000000 libmultilabel-0.6.2/libmultilabel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 06:42:56.000000 libmultilabel-0.6.2/libmultilabel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-07 06:42:56.000000 libmultilabel-0.6.2/libmultilabel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-07 06:42:56.000000 libmultilabel-0.6.2/libmultilabel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-07 06:42:51.000000 libmultilabel-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-07 06:42:56.519261 libmultilabel-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:56.412392 libmultilabel-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 13:44:56.412392 libmultilabel-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:56.408392 libmultilabel-0.7.0/libmultilabel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:56.408392 libmultilabel-0.7.0/libmultilabel/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/linear/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23377 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/linear/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/linear/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/linear/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/linear/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/linear/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:56.412392 libmultilabel-0.7.0/libmultilabel/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33501 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/attentionxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17420 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8993 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:56.412392 libmultilabel-0.7.0/libmultilabel/nn/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/networks/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/networks/bert_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/networks/caml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/networks/kim_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/networks/labelwise_attention_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/networks/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/networks/xml_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/libmultilabel/nn/nn_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:44:56.412392 libmultilabel-0.7.0/libmultilabel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 13:44:56.000000 libmultilabel-0.7.0/libmultilabel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-24 13:44:56.000000 libmultilabel-0.7.0/libmultilabel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:44:56.000000 libmultilabel-0.7.0/libmultilabel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-24 13:44:56.000000 libmultilabel-0.7.0/libmultilabel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 13:44:56.000000 libmultilabel-0.7.0/libmultilabel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-24 13:44:50.000000 libmultilabel-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-24 13:44:56.412392 libmultilabel-0.7.0/setup.cfg
```

### Comparing `libmultilabel-0.6.2/LICENSE` & `libmultilabel-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/PKG-INFO` & `libmultilabel-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.6.2
-Summary: A library for multi-label text classification
+Version: 0.7.0
+Summary: A library for multi-class and multi-label classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.1
```

### Comparing `libmultilabel-0.6.2/README.md` & `libmultilabel-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# LibMultiLabel — a Library for Multi-class and Multi-label Text Classification
+# LibMultiLabel — a Library for Multi-class and Multi-label Classification
 
 LibMultiLabel is a library for binary, multi-class, and multi-label classification. It has the following functionalities
 
 - end-to-end services from raw texts to final evaluation/analysis
 - support for common neural network architectures and linear classifiers
 - easy hyper-parameter selection
```

### Comparing `libmultilabel-0.6.2/libmultilabel/common_utils.py` & `libmultilabel-0.7.0/libmultilabel/common_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/linear/data_utils.py` & `libmultilabel-0.7.0/libmultilabel/linear/data_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/linear/linear.py` & `libmultilabel-0.7.0/libmultilabel/linear/linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,21 @@
     "train_thresholding",
     "train_cost_sensitive",
     "train_cost_sensitive_micro",
     "train_binary_and_multiclass",
     "predict_values",
     "get_topk_labels",
     "get_positive_labels",
+    "FlatModel",
 ]
 
 
 class FlatModel:
+    """A model returned from a training function."""
+
     def __init__(
         self,
         name: str,
         weights: np.matrix,
         bias: float,
         thresholds: float | np.ndarray,
         multiclass: bool,
@@ -615,15 +618,15 @@
         bias=bias,
         thresholds=thresholds,
         multiclass=multiclass,
     )
 
 
 def predict_values(model, x: sparse.csr_matrix) -> np.ndarray:
-    """Calculates the decision values associated with x.
+    """Calculates the decision values associated with x, equivalent to model.predict_values(x).
 
     Args:
         model: A model returned from a training function.
         x (sparse.csr_matrix): A matrix with dimension number of instances * number of features.
 
     Returns:
         np.ndarray: A matrix with dimension number of instances * number of classes.
```

### Comparing `libmultilabel-0.6.2/libmultilabel/linear/metrics.py` & `libmultilabel-0.7.0/libmultilabel/linear/metrics.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/linear/preprocessor.py` & `libmultilabel-0.7.0/libmultilabel/linear/preprocessor.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/linear/tree.py` & `libmultilabel-0.7.0/libmultilabel/linear/tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import scipy.sparse as sparse
 import sklearn.cluster
 import sklearn.preprocessing
 from tqdm import tqdm
 
 from . import linear
 
-__all__ = ["train_tree"]
+__all__ = ["train_tree", "TreeModel"]
 
 
 class Node:
     def __init__(
         self,
         label_map: np.ndarray,
         children: list[Node],
@@ -34,14 +34,16 @@
         visit(self)
         # Stops if self.children is empty, i.e. self is a leaf node
         for child in self.children:
             child.dfs(visit)
 
 
 class TreeModel:
+    """A model returned from train_tree."""
+
     def __init__(
         self,
         root: Node,
         flat_model: linear.FlatModel,
         weight_map: np.ndarray,
     ):
         self.name = "tree"
```

### Comparing `libmultilabel-0.6.2/libmultilabel/linear/utils.py` & `libmultilabel-0.7.0/libmultilabel/linear/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     with open(checkpoint_path, "wb") as f:
         pickle.dump(
             {
                 "preprocessor": preprocessor,
                 "model": model,
             },
             f,
+            protocol=pickle.HIGHEST_PROTOCOL,
         )
 
 
 def load_pipeline(checkpoint_path: str) -> tuple[Preprocessor, Any]:
     """Loads preprocessor and model from checkpoint_path.
 
     Args:
```

### Comparing `libmultilabel-0.6.2/libmultilabel/logging.py` & `libmultilabel-0.7.0/libmultilabel/logging.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/data_utils.py` & `libmultilabel-0.7.0/libmultilabel/nn/data_utils.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/metrics.py` & `libmultilabel-0.7.0/libmultilabel/nn/metrics.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/model.py` & `libmultilabel-0.7.0/libmultilabel/nn/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -151,22 +151,26 @@
         Args:
             batch (dict): A batch of text and label.
             batch_idx (int): Index of current batch.
 
         Returns:
             dict: Top k label indexes and the prediction scores.
         """
-        _, pred_logits = self.shared_step(batch)
+        pred_logits = self(batch)
         pred_scores = pred_logits.detach().cpu().numpy()
         k = self.save_k_predictions
         top_k_idx = argsort_top_k(pred_scores, k, axis=1)
         top_k_scores = np.take_along_axis(pred_scores, top_k_idx, axis=1)
 
         return {"top_k_pred": top_k_idx, "top_k_pred_scores": top_k_scores}
 
+    def forward(self, batch):
+        """compute predicted logits"""
+        return self.network(batch)["logits"]
+
     def print(self, *args, **kwargs):
         """Prints only from process 0 and not in silent mode. Use this in any
         distributed mode to log only once."""
 
         if not self.silent:
             # print() in LightningModule to print only from process 0
             super().print(*args, **kwargs)
@@ -174,37 +178,34 @@
 
 class Model(MultiLabelModel):
     """A class that implements `MultiLabelModel` for initializing and training a neural network.
 
     Args:
         classes (list): List of class names.
         word_dict (torchtext.vocab.Vocab): A vocab object which maps tokens to indices.
-        embed_vecs (torch.Tensor): The pre-trained word vectors of shape (vocab_size, embed_dim).
         network (nn.Module): Network (i.e., CAML, KimCNN, or XMLCNN).
         loss_function (str, optional): Loss function name (i.e., binary_cross_entropy_with_logits,
             cross_entropy). Defaults to 'binary_cross_entropy_with_logits'.
         log_path (str): Path to a directory holding the log files and models.
     """
 
     def __init__(
         self,
         classes,
         word_dict,
-        embed_vecs,
         network,
         loss_function="binary_cross_entropy_with_logits",
         log_path=None,
         **kwargs
     ):
         super().__init__(num_classes=len(classes), log_path=log_path, **kwargs)
         self.save_hyperparameters(
             ignore=["log_path"]
         )  # If log_path is saved, loading the checkpoint will cause an error since each experiment has unique log_path (result_dir).
         self.word_dict = word_dict
-        self.embed_vecs = embed_vecs
         self.classes = classes
         self.network = network
         self.configure_loss_function(loss_function)
 
     def configure_loss_function(self, loss_function):
         assert hasattr(
             F, loss_function
@@ -220,12 +221,11 @@
             batch (dict): A batch of text and label.
 
         Returns:
             loss (torch.Tensor): Loss between target and predict logits.
             pred_logits (torch.Tensor): The predict logits (batch_size, num_classes).
         """
         target_labels = batch["label"]
-        outputs = self.network(batch)
-        pred_logits = outputs["logits"]
+        pred_logits = self(batch)
         loss = self.loss_function(pred_logits, target_labels.float())
 
         return loss, pred_logits
```

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/networks/__init__.py` & `libmultilabel-0.7.0/libmultilabel/nn/networks/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .caml import CAML
 from .kim_cnn import KimCNN
 from .xml_cnn import XMLCNN
 from .labelwise_attention_networks import BiGRULWAN
 from .labelwise_attention_networks import BiLSTMLWAN
 from .labelwise_attention_networks import BiLSTMLWMHAN
 from .labelwise_attention_networks import CNNLWAN
+from .labelwise_attention_networks import AttentionXML_0, AttentionXML_1
 
 
 def get_init_weight_func(init_weight):
     def init_weight_func(m):
         if isinstance(m, nn.Linear) or isinstance(m, nn.Conv1d) or isinstance(m, nn.Conv2d):
             getattr(nn.init, init_weight + "_")(m.weight)
```

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/networks/bert.py` & `libmultilabel-0.7.0/libmultilabel/nn/networks/bert.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/networks/bert_attention.py` & `libmultilabel-0.7.0/libmultilabel/nn/networks/bert_attention.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/networks/caml.py` & `libmultilabel-0.7.0/libmultilabel/nn/networks/caml.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/networks/kim_cnn.py` & `libmultilabel-0.7.0/libmultilabel/nn/networks/kim_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/networks/labelwise_attention_networks.py` & `libmultilabel-0.7.0/libmultilabel/nn/networks/labelwise_attention_networks.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     Embedding,
     GRUEncoder,
     LSTMEncoder,
     CNNEncoder,
     LabelwiseAttention,
     LabelwiseMultiHeadAttention,
     LabelwiseLinearOutput,
+    PartialLabelwiseAttention,
+    MultilayerLinearOutput,
 )
 
 
 class LabelwiseAttentionNetwork(ABC, nn.Module):
     """Base class for Labelwise Attention Network
 
     Args:
@@ -262,7 +264,74 @@
     def forward(self, input):
         # (batch_size, sequence_length, embed_dim)
         x = self.embedding(input["text"])
         x = self.encoder(x)  # (batch_size, sequence_length, hidden_dim)
         x, _ = self.attention(x)  # (batch_size, num_classes, hidden_dim)
         x = self.output(x)  # (batch_size, num_classes)
         return {"logits": x}
+
+
+class AttentionXML_0(nn.Module):
+    def __init__(
+        self,
+        embed_vecs,
+        num_classes: int,
+        rnn_dim: int,
+        linear_size: list,
+        freeze_embed_training: bool = False,
+        rnn_layers: int = 1,
+        embed_dropout: float = 0.2,
+        encoder_dropout: float = 0,
+        post_encoder_dropout: float = 0.5,
+    ):
+        super().__init__()
+        self.embedding = Embedding(embed_vecs, freeze=freeze_embed_training, dropout=embed_dropout)
+        self.encoder = LSTMEncoder(embed_vecs.shape[1], rnn_dim // 2, rnn_layers, encoder_dropout, post_encoder_dropout)
+        self.attention = LabelwiseAttention(rnn_dim, num_classes)
+        self.output = MultilayerLinearOutput([rnn_dim] + linear_size, 1)
+
+    def forward(self, inputs):
+        x = inputs["text"]
+        # the index of padding is 0
+        masks = x != 0
+        lengths = masks.sum(dim=1)
+        masks = masks[:, : lengths.max()]
+
+        x = self.embedding(x)[:, : lengths.max()]  # batch_size, length, embedding_size
+        x = self.encoder(x, lengths)  # batch_size, length, hidden_size
+        x, _ = self.attention(x)  # batch_size, num_classes, hidden_size
+        x = self.output(x)  # batch_size, num_classes
+        return {"logits": x}
+
+
+class AttentionXML_1(nn.Module):
+    def __init__(
+        self,
+        embed_vecs,
+        num_classes: int,
+        rnn_dim: int,
+        linear_size: list,
+        freeze_embed_training: bool = False,
+        rnn_layers: int = 1,
+        embed_dropout: float = 0.2,
+        encoder_dropout: float = 0,
+        post_encoder_dropout: float = 0.5,
+    ):
+        super().__init__()
+        self.embedding = Embedding(embed_vecs, freeze=freeze_embed_training, dropout=embed_dropout)
+        self.encoder = LSTMEncoder(embed_vecs.shape[1], rnn_dim // 2, rnn_layers, encoder_dropout, post_encoder_dropout)
+        self.attention = PartialLabelwiseAttention(rnn_dim, num_classes)
+        self.output = MultilayerLinearOutput([rnn_dim] + linear_size, 1)
+
+    def forward(self, inputs):
+        x = inputs["text"]
+        labels_selected = inputs["labels_selected"]
+        # the index of padding is 0
+        masks = x != 0
+        lengths = masks.sum(dim=1)
+        masks = masks[:, : lengths.max()]
+
+        x = self.embedding(x)[:, : lengths.max()]  # batch_size, length, embedding_size
+        x = self.encoder(x, lengths)  # batch_size, length, hidden_size
+        x, _ = self.attention(x, labels_selected)  # batch_size, sample_size, hidden_size
+        x = self.output(x)  # batch_size, sample_size
+        return {"logits": x}
```

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/networks/modules.py` & `libmultilabel-0.7.0/libmultilabel/nn/networks/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,7 +206,39 @@
 
     def __init__(self, input_size, num_classes):
         super(LabelwiseLinearOutput, self).__init__()
         self.output = nn.Linear(input_size, num_classes)
 
     def forward(self, input):
         return (self.output.weight * input).sum(dim=-1) + self.output.bias
+
+
+class PartialLabelwiseAttention(nn.Module):
+    """Similar to LabelwiseAttention.
+    What makes the class different from LabelwiseAttention is that only the weights of selected labels will be
+    updated in a single iteration.
+    """
+
+    def __init__(self, hidden_size, num_classes):
+        super().__init__()
+        self.attention = nn.Embedding(num_classes + 1, hidden_size)
+
+    def forward(self, inputs, labels_selected):
+        attn_inputs = inputs.transpose(1, 2)  # batch_size, hidden_dim, length
+        attn_weights = self.attention(labels_selected)  # batch_size, sample_size, hidden_dim
+        attention = attn_weights @ attn_inputs  # batch_size, sample_size, length
+        attention = F.softmax(attention, -1)  # batch_size, sample_size, length
+        logits = attention @ inputs  # batch_size, sample_size, hidden_dim
+        return logits, attention
+
+
+class MultilayerLinearOutput(nn.Module):
+    def __init__(self, linear_size, output_size):
+        super().__init__()
+        self.linears = nn.ModuleList(nn.Linear(in_s, out_s) for in_s, out_s in zip(linear_size[:-1], linear_size[1:]))
+        self.output = nn.Linear(linear_size[-1], output_size)
+
+    def forward(self, inputs):
+        linear_out = inputs
+        for linear in self.linears:
+            linear_out = F.relu(linear(linear_out))
+        return torch.squeeze(self.output(linear_out), -1)
```

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/networks/xml_cnn.py` & `libmultilabel-0.7.0/libmultilabel/nn/networks/xml_cnn.py`

 * *Files identical despite different names*

### Comparing `libmultilabel-0.6.2/libmultilabel/nn/nn_utils.py` & `libmultilabel-0.7.0/libmultilabel/nn/nn_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
     if init_weight is not None:
         init_weight = networks.get_init_weight_func(init_weight=init_weight)
         network.apply(init_weight)
 
     model = Model(
         classes=classes,
         word_dict=word_dict,
-        embed_vecs=embed_vecs,
         network=network,
         log_path=log_path,
         learning_rate=learning_rate,
         optimizer=optimizer,
         momentum=momentum,
         weight_decay=weight_decay,
         lr_scheduler=lr_scheduler,
```

### Comparing `libmultilabel-0.6.2/libmultilabel.egg-info/PKG-INFO` & `libmultilabel-0.7.0/libmultilabel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: libmultilabel
-Version: 0.6.2
-Summary: A library for multi-label text classification
+Version: 0.7.0
+Summary: A library for multi-class and multi-label classification
 Home-page: https://github.com/ASUS-AICS/LibMultiLabel
 Author: LibMultiLabel Team
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ASUS-AICS/LibMultiLabel/issues
 Project-URL: Documentation, https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 Project-URL: Source Code, https://github.com/ASUS-AICS/LibMultiLabel/
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.1
```

### Comparing `libmultilabel-0.6.2/libmultilabel.egg-info/SOURCES.txt` & `libmultilabel-0.7.0/libmultilabel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 libmultilabel/linear/data_utils.py
 libmultilabel/linear/linear.py
 libmultilabel/linear/metrics.py
 libmultilabel/linear/preprocessor.py
 libmultilabel/linear/tree.py
 libmultilabel/linear/utils.py
 libmultilabel/nn/__init__.py
+libmultilabel/nn/attentionxml.py
 libmultilabel/nn/data_utils.py
 libmultilabel/nn/metrics.py
 libmultilabel/nn/model.py
 libmultilabel/nn/nn_utils.py
 libmultilabel/nn/networks/__init__.py
 libmultilabel/nn/networks/bert.py
 libmultilabel/nn/networks/bert_attention.py
```

### Comparing `libmultilabel-0.6.2/setup.cfg` & `libmultilabel-0.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = libmultilabel
-version = 0.6.2
+version = 0.7.0
 author = LibMultiLabel Team
 license = MIT License
 license_file = LICENSE
-description = A library for multi-label text classification
+description = A library for multi-class and multi-label classification
 long_description = See documentation here: https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 url = https://github.com/ASUS-AICS/LibMultiLabel
 project_urls = 
 	Bug Tracker = https://github.com/ASUS-AICS/LibMultiLabel/issues
 	Documentation = https://www.csie.ntu.edu.tw/~cjlin/libmultilabel
 	Source Code = https://github.com/ASUS-AICS/LibMultiLabel/
 classifiers =
```

