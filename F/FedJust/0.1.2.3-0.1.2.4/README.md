# Comparing `tmp/fedjust-0.1.2.3.tar.gz` & `tmp/fedjust-0.1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedjust-0.1.2.3.tar", max compression
+gzip compressed data, was "fedjust-0.1.2.4.tar", max compression
```

## Comparing `fedjust-0.1.2.3.tar` & `fedjust-0.1.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2024-04-29 21:08:19.328339 fedjust-0.1.2.3/FedJust/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-29 21:08:19.328339 fedjust-0.1.2.3/FedJust/aggregators/aggregator.py
--rw-r--r--   0        0        0     1442 2024-05-02 14:42:59.238594 fedjust-0.1.2.3/FedJust/aggregators/fedopt_aggregator.py
--rw-r--r--   0        0        0     1515 2024-05-02 14:35:56.655748 fedjust-0.1.2.3/FedJust/files/archive.py
--rw-r--r--   0        0        0     1721 2024-04-29 21:08:19.328339 fedjust-0.1.2.3/FedJust/files/handlers.py
--rw-r--r--   0        0        0     2187 2024-04-29 21:08:19.328339 fedjust-0.1.2.3/FedJust/files/loggers.py
--rw-r--r--   0        0        0    17018 2024-05-16 12:12:29.810973 fedjust-0.1.2.3/FedJust/model/federated_model.py
--rw-r--r--   0        0        0     5910 2024-04-29 21:13:37.832090 fedjust-0.1.2.3/FedJust/node/federated_node.py
--rw-r--r--   0        0        0     3335 2024-05-01 12:25:08.143947 fedjust-0.1.2.3/FedJust/operations/evaluations.py
--rw-r--r--   0        0        0     3430 2024-04-29 21:08:19.332339 fedjust-0.1.2.3/FedJust/operations/orchestrations.py
--rw-r--r--   0        0        0     6205 2024-05-01 12:56:19.110407 fedjust-0.1.2.3/FedJust/simulation/adaptive_optimizer_simulation.py
--rw-r--r--   0        0        0    10659 2024-04-29 21:08:19.332339 fedjust-0.1.2.3/FedJust/simulation/simulation.py
--rw-r--r--   0        0        0      824 2024-05-01 12:07:32.211788 fedjust-0.1.2.3/FedJust/utils/computations.py
--rw-r--r--   0        0        0     3091 2024-04-29 21:08:19.332339 fedjust-0.1.2.3/README.md
--rw-r--r--   0        0        0      428 2024-05-16 12:33:46.988040 fedjust-0.1.2.3/pyproject.toml
--rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 fedjust-0.1.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-29 21:08:19.328339 fedjust-0.1.2.4/FedJust/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-29 21:08:19.328339 fedjust-0.1.2.4/FedJust/aggregators/aggregator.py
+-rw-r--r--   0        0        0     1442 2024-05-02 14:42:59.238594 fedjust-0.1.2.4/FedJust/aggregators/fedopt_aggregator.py
+-rw-r--r--   0        0        0     1515 2024-05-02 14:35:56.655748 fedjust-0.1.2.4/FedJust/files/archive.py
+-rw-r--r--   0        0        0     1721 2024-04-29 21:08:19.328339 fedjust-0.1.2.4/FedJust/files/handlers.py
+-rw-r--r--   0        0        0     2187 2024-04-29 21:08:19.328339 fedjust-0.1.2.4/FedJust/files/loggers.py
+-rw-r--r--   0        0        0    17171 2024-05-22 11:50:33.002404 fedjust-0.1.2.4/FedJust/model/federated_model.py
+-rw-r--r--   0        0        0     5910 2024-04-29 21:13:37.832090 fedjust-0.1.2.4/FedJust/node/federated_node.py
+-rw-r--r--   0        0        0     2694 2024-05-22 11:52:41.204209 fedjust-0.1.2.4/FedJust/operations/evaluations.py
+-rw-r--r--   0        0        0     3430 2024-04-29 21:08:19.332339 fedjust-0.1.2.4/FedJust/operations/orchestrations.py
+-rw-r--r--   0        0        0     6205 2024-05-01 12:56:19.110407 fedjust-0.1.2.4/FedJust/simulation/adaptive_optimizer_simulation.py
+-rw-r--r--   0        0        0    10659 2024-04-29 21:08:19.332339 fedjust-0.1.2.4/FedJust/simulation/simulation.py
+-rw-r--r--   0        0        0      824 2024-05-01 12:07:32.211788 fedjust-0.1.2.4/FedJust/utils/computations.py
+-rw-r--r--   0        0        0     3091 2024-04-29 21:08:19.332339 fedjust-0.1.2.4/README.md
+-rw-r--r--   0        0        0      428 2024-05-24 12:32:49.533113 fedjust-0.1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3666 1970-01-01 00:00:00.000000 fedjust-0.1.2.4/PKG-INFO
```

### Comparing `fedjust-0.1.2.3/FedJust/aggregators/aggregator.py` & `fedjust-0.1.2.4/FedJust/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/aggregators/fedopt_aggregator.py` & `fedjust-0.1.2.4/FedJust/aggregators/fedopt_aggregator.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/files/archive.py` & `fedjust-0.1.2.4/FedJust/files/archive.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/files/handlers.py` & `fedjust-0.1.2.4/FedJust/files/handlers.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/files/loggers.py` & `fedjust-0.1.2.4/FedJust/files/loggers.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/model/federated_model.py` & `fedjust-0.1.2.4/FedJust/model/federated_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -351,14 +351,15 @@
         Returns
         -------
             Tuple[float, float]: loss and accuracy on the test set.
         """
         # Try: to place net on device directly during the evaluation stage.
         self.net.to(self.device)
         self.net.eval()
+        evaluation_results = {}
         criterion = torch.nn.CrossEntropyLoss()
         test_loss = 0
         correct = 0
         total = 0
         y_pred = []
         y_true = []
         losses = []
@@ -374,65 +375,60 @@
                 test_loss = criterion(output, targets).item()
                 losses.append(test_loss)
                 pred = output.argmax(dim=1, keepdim=True)
                 correct += pred.eq(targets.view_as(pred)).sum().item()
                 y_pred.append(pred)
                 y_true.append(targets)
 
-        test_loss = np.mean(test_loss)
-        accuracy = correct / total
+        evaluation_results['test_loss'] = np.mean(losses)
+        evaluation_results['accuracy'] = correct / total
 
         y_true = [item.item() for sublist in y_true for item in sublist]
         y_pred = [item.item() for sublist in y_pred for item in sublist]
 
-        f1score = f1_score(y_true, y_pred, average="macro")
-        precision = precision_score(y_true, y_pred, average="macro")
-        recall = recall_score(y_true, y_pred, average="macro")
+        evaluation_results['f1score'] = f1_score(y_true, y_pred, average="macro")
+        evaluation_results['precision'] = precision_score(y_true, y_pred, average="macro")
+        evaluation_results['recall'] = recall_score(y_true, y_pred, average="macro")
 
         cm = confusion_matrix(y_true, y_pred)
         cm = cm.astype("float") / cm.sum(axis=1)[:, np.newaxis]
         accuracy_per_class = cm.diagonal()
+        accuracy_per_class_expanded = {
+            f'accuracy_per_{class_id}': value for class_id, value in enumerate(accuracy_per_class)
+        }
+        evaluation_results.update(accuracy_per_class_expanded)
+
+        # true_positives = np.diag(cm)
+        # num_classes = len(list(set(y_true)))
+
+        # false_positives = []
+        # for i in range(num_classes):
+        #     false_positives.append(sum(cm[:,i]) - cm[i,i])
+
+        # false_negatives = []
+        # for i in range(num_classes):
+        #     false_negatives.append(sum(cm[i,:]) - cm[i,i])
+
+        # true_negatives = []
+        # for i in range(num_classes):
+        #     temp = np.delete(cm, i, 0)   # delete ith row
+        #     temp = np.delete(temp, i, 1)  # delete ith column
+        #     true_negatives.append(sum(sum(temp)))
+
+        # denominator = [sum(x) for x in zip(false_positives, true_negatives)]
+        # false_positive_rate = [num/den for num, den in zip(false_positives, denominator)]
+
+        # denominator = [sum(x) for x in zip(true_positives, false_negatives)]
+        # true_positive_rate = [num/den for num, den in zip(true_positives, denominator)]
+
+        # # # Emptying the cuda_cache
+        # # if torch.cuda.is_available():
+        # #     torch.cuda.empty_cache()
 
-        true_positives = np.diag(cm)
-        num_classes = len(list(set(y_true)))
-
-        false_positives = []
-        for i in range(num_classes):
-            false_positives.append(sum(cm[:,i]) - cm[i,i])
-
-        false_negatives = []
-        for i in range(num_classes):
-            false_negatives.append(sum(cm[i,:]) - cm[i,i])
-
-        true_negatives = []
-        for i in range(num_classes):
-            temp = np.delete(cm, i, 0)   # delete ith row
-            temp = np.delete(temp, i, 1)  # delete ith column
-            true_negatives.append(sum(sum(temp)))
-
-        denominator = [sum(x) for x in zip(false_positives, true_negatives)]
-        false_positive_rate = [num/den for num, den in zip(false_positives, denominator)]
-
-        denominator = [sum(x) for x in zip(true_positives, false_negatives)]
-        true_positive_rate = [num/den for num, den in zip(true_positives, denominator)]
-
-        # # Emptying the cuda_cache
-        # if torch.cuda.is_available():
-        #     torch.cuda.empty_cache()
-
-        return (
-                test_loss,
-                accuracy,
-                f1score,
-                precision,
-                recall,
-                accuracy_per_class,
-                true_positive_rate,
-                false_positive_rate
-                )
+        return evaluation_results
 
 
     # def quick_evaluate(self) -> tuple[float, float]:
     #     """Quicker version of the evaluate_model(function) 
     #     Validate the network on the local test set returning only the loss and accuracy.
         
     #     Parameters
```

### Comparing `fedjust-0.1.2.3/FedJust/node/federated_node.py` & `fedjust-0.1.2.4/FedJust/node/federated_node.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/operations/evaluations.py` & `fedjust-0.1.2.4/FedJust/operations/evaluations.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,47 +27,28 @@
     log_to_screen: bool (default to False)
         Boolean flag whether we want to log the results to the screen.
     
     Returns
     -------
         None"""
     try:
-        (
-            loss,
-            accuracy,
-            fscore,
-            precision,
-            recall,
-            test_accuracy_per_class,
-            true_positive_rate,
-            false_positive_rate
-        ) = model.evaluate_model()
-        metrics = {"epoch": iteration,
-                    "node": model.node_name,
-                    "loss":loss, 
-                    "accuracy": accuracy, 
-                    "fscore": fscore, 
-                    "precision": precision,
-                    "recall": recall, 
-                    "test_accuracy_per_class": test_accuracy_per_class, 
-                    "true_positive_rate": true_positive_rate,
-                    "false_positive_rate": false_positive_rate,
-                    "epoch": iteration}
+        evaluation_results = model.evaluate_model()
+        evaluation_results['node_id'] = model.node_name
         if log_to_screen == True:
             pass
             #logger.info(f"Evaluating model after iteration {iteration} on node {model.node_name}. Results: {metrics}")
     except Exception as e:
         logger.warning(f"Unable to compute metrics. {e}")
     path = os.path.join(save_path)
     with open(path, 'a+', newline='') as saved_file:
-            writer = csv.DictWriter(saved_file, list(metrics.keys()))
+            writer = csv.DictWriter(saved_file, list(evaluation_results.keys()))
             # If the file does not exist, it will create it and write the header.
             if os.path.getsize(path) == 0:
                 writer.writeheader()
-            writer.writerow(metrics)
+            writer.writerow(evaluation_results)
 
 
 def automatic_node_evaluation(
     iteration: int, 
     nodes: dict[int: FederatedNode],
     save_path: str,
     logger = None,
```

### Comparing `fedjust-0.1.2.3/FedJust/operations/orchestrations.py` & `fedjust-0.1.2.4/FedJust/operations/orchestrations.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/simulation/adaptive_optimizer_simulation.py` & `fedjust-0.1.2.4/FedJust/simulation/adaptive_optimizer_simulation.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/simulation/simulation.py` & `fedjust-0.1.2.4/FedJust/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/FedJust/utils/computations.py` & `fedjust-0.1.2.4/FedJust/utils/computations.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/README.md` & `fedjust-0.1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.2.3/PKG-INFO` & `fedjust-0.1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedJust
-Version: 0.1.2.3
+Version: 0.1.2.4
 Summary: 
 Author: Scolpe
 Author-email: 63779111+Scolpe@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

