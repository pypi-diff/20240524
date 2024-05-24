# Comparing `tmp/ood_detectors-0.0.8.tar.gz` & `tmp/ood_detectors-0.0.9.tar.gz`

## Comparing `ood_detectors-0.0.8.tar` & `ood_detectors-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/docki.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/requirements.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/requirements_dev.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/__init__.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/ema.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/eval_utils.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/likelihood.py
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/losses.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/models.py
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/ood_utils.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/ops_utils.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/plot_utils.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/residual.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/sde.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/src/ood_detectors/train.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/tests/init_test.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/LICENSE
--rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/README.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ood_detectors-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/docki.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/requirements_dev.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/__init__.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/ema.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/eval_utils.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/likelihood.py
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/losses.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/models.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/ood_utils.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/ops_utils.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/plot_utils.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/residual.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/sde.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/src/ood_detectors/train.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/tests/init_test.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/README.md
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 ood_detectors-0.0.9/PKG-INFO
```

### Comparing `ood_detectors-0.0.8/docki.yaml` & `ood_detectors-0.0.9/docki.yaml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/.github/workflows/publish.yml` & `ood_detectors-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/ema.py` & `ood_detectors-0.0.9/src/ood_detectors/ema.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/eval_utils.py` & `ood_detectors-0.0.9/src/ood_detectors/eval_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/likelihood.py` & `ood_detectors-0.0.9/src/ood_detectors/likelihood.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         """
         return self.model.state_dict()
 
     def fit(self, dataset, n_epochs, batch_size, 
             num_workers=0,
             update_fn=None, 
             verbose=True,
+            collate_fn=None,
             ):
         """Trains the model on the given dataset.
 
         Args:
             dataset (object): The dataset object containing the training data.
             n_epochs (int): The number of epochs to train the model.
             batch_size (int): The batch size for training.
@@ -108,31 +109,31 @@
                 sde=self.sde,
                 model=self.model,
                 optimizer=self.optimizer,
             )
         else:
             update_fn = update_fn(sde=self.sde, model=self.model, optimizer=self.optimizer)
 
-        return train.train(dataset, self.model, update_fn, n_epochs, batch_size, self.device, num_workers, verbose=verbose)
+        return train.train(dataset, self.model, update_fn, n_epochs, batch_size, self.device, num_workers, verbose=verbose, collate_fn=collate_fn)
 
-    def predict(self, dataset, batch_size, num_workers=0, verbose=True):
+    def predict(self, dataset, batch_size, num_workers=0, verbose=True, collate_fn=None):
         """Performs inference on the given dataset.
 
         Args:
             dataset (object): The dataset object containing the test data.
             batch_size (int): The batch size for inference.
             num_workers (int): The number of worker processes for data loading. Default is 0.
             verbose (bool): Whether to print inference progress. Default is True.
 
         Returns:
             dict: A dictionary containing the likelihood scores for the test data.
 
         """
         likelihood_fn = ood_utils.get_likelihood_fn(self.sde)
-        return train.inference(dataset, self.model, likelihood_fn, batch_size, self.device, num_workers, verbose)
+        return train.inference(dataset, self.model, likelihood_fn, batch_size, self.device, num_workers, verbose, collate_fn=collate_fn)
     
     def __call__(self, *args, **kwargs):
         """Calls the predict method.
 
         Args:
             *args: Variable length argument list.
             **kwargs: Arbitrary keyword arguments.
```

### Comparing `ood_detectors-0.0.8/src/ood_detectors/losses.py` & `ood_detectors-0.0.9/src/ood_detectors/losses.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/models.py` & `ood_detectors-0.0.9/src/ood_detectors/models.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/ood_utils.py` & `ood_detectors-0.0.9/src/ood_detectors/ood_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/ops_utils.py` & `ood_detectors-0.0.9/src/ood_detectors/ops_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/plot_utils.py` & `ood_detectors-0.0.9/src/ood_detectors/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/residual.py` & `ood_detectors-0.0.9/src/ood_detectors/residual.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
 
     def __init__(self, dims=512, u=0):
         self.dims = dims
         self.u = u
         self.name = "Residual"
 
-    def fit(self, data, *args, **kwargs):
+    def fit(self, data, *args, collate_fn=None, **kwargs):
         """
         Fit the Residual model to the given data.
 
         Args:
             data (array-like or torch.Tensor or torch.utils.data.DataLoader): Input data for fitting the model.
             *args: Additional positional arguments.
             **kwargs: Additional keyword arguments.
@@ -43,26 +43,29 @@
             list: An empty list.
 
         """
         if isinstance(data, (list, tuple)):
             data = np.array(data)
         elif isinstance(data, torch.Tensor):
             data = data.cpu().numpy()
-        elif isinstance(data, torch.utils.data.DataLoader):
-            data = np.vstack([x.cpu().numpy() for x, _ in data])
+        elif isinstance(data, torch.utils.data.Dataset):
+            if collate_fn is None:
+                data = np.vstack([x.cpu().numpy() for x, *_ in data])
+            else:
+                data = np.vstack([collate_fn([d])[0].cpu().numpy() for d in data])
 
         ec = EmpiricalCovariance(assume_centered=True)
         ec.fit(data - self.u)
         eig_vals, eigen_vectors = np.linalg.eig(ec.covariance_)
         self.ns = np.ascontiguousarray(
             (eigen_vectors.T[np.argsort(eig_vals * -1)[self.dims :]]).T
         )
         return []
 
-    def predict(self, data, *args, **kwargs):
+    def predict(self, data, *args, collate_fn=None, **kwargs):
         """
         Predict the outlier scores for the given data.
 
         Args:
             data (array-like or torch.Tensor or torch.utils.data.DataLoader): Input data for predicting the outlier scores.
             *args: Additional positional arguments.
             **kwargs: Additional keyword arguments.
@@ -71,16 +74,19 @@
             numpy.ndarray: Outlier scores for the input data.
 
         """
         if isinstance(data, (list, tuple)):
             data = np.array(data)
         elif isinstance(data, torch.Tensor):
             data = data.cpu().numpy()
-        elif isinstance(data, torch.utils.data.DataLoader):
-            data = np.vstack([x.cpu().numpy() for x, _ in data])
+        elif isinstance(data, torch.utils.data.Dataset):
+            if collate_fn is None:
+                data = np.vstack([x.cpu().numpy() for x, *_ in data])
+            else:
+                data = np.vstack([collate_fn([d])[0].cpu().numpy() for d in data])
 
         return np.linalg.norm((data - self.u) @ self.ns, axis=-1)
 
     def __call__(self, *args, **kwargs):
         return self.predict(*args, **kwargs)
 
     def to(self, device):
```

### Comparing `ood_detectors-0.0.8/src/ood_detectors/sde.py` & `ood_detectors-0.0.9/src/ood_detectors/sde.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/src/ood_detectors/train.py` & `ood_detectors-0.0.9/src/ood_detectors/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import torch
 import tqdm
 
-def train(dataset, model, update_fn, n_epochs, batch_size, device, num_workers=0, verbose=True, tw=None, lrs=True):
+def train(dataset, model, update_fn, n_epochs, batch_size, device, num_workers=0, verbose=True, tw=None, collate_fn=None):
     """
     Trains a model on a given dataset for a specified number of epochs.
 
     Args:
         dataset (torch.utils.data.Dataset): The training dataset.
         model (torch.nn.Module): The model to be trained.
         update_fn (callable): The function that updates the model parameters.
@@ -19,16 +19,18 @@
         lrs (bool, optional): Whether to use learning rate scheduling. Defaults to True.
 
     Returns:
         list: A list of average epoch losses.
     """
     if verbose:
         print(f'Training for {n_epochs} epochs...')
-      
-    data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=True, num_workers=num_workers, drop_last=True)
+    if collate_fn is None:
+        data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=True, num_workers=num_workers, drop_last=True)
+    else:
+        data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=True, num_workers=num_workers, drop_last=True, collate_fn=collate_fn)
     if verbose:
         epochs = tqdm.trange(n_epochs)
     else:
         epochs = range(n_epochs)
     avg_epoch_loss = []
     model.train()
     for epoch in epochs:
@@ -47,15 +49,15 @@
             tw.add_scalar('Loss/train', epoch_loss, epoch)
         # Print the averaged training loss so far.
         if verbose:
             epochs.set_description('Average Loss: {:5f}'.format(avg_loss / num_items))
     return avg_epoch_loss
 
 
-def inference(dataset, model, ode_likelihood, batch_size, device, num_workers=0, verbose=True):
+def inference(dataset, model, ode_likelihood, batch_size, device, num_workers=0, verbose=True, collate_fn=None):
     """
     Performs inference using a trained model on a given dataset.
 
     Args:
         dataset (torch.utils.data.Dataset): The dataset for inference.
         model (torch.nn.Module): The trained model.
         ode_likelihood (callable): The function that computes the likelihood.
@@ -63,15 +65,18 @@
         device (torch.device): The device to run the inference on.
         num_workers (int, optional): The number of workers for data loading. Defaults to 0.
         verbose (bool, optional): Whether to display inference progress. Defaults to True.
 
     Returns:
         numpy.ndarray: An array of inference scores.
     """
-    data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=True, num_workers=num_workers)
+    if collate_fn is None:
+        data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=True, num_workers=num_workers)
+    else:
+        data_loader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, shuffle=True, num_workers=num_workers, collate_fn=collate_fn)
     all_bpds = 0.
     all_items = 0
     score_id = []
     if verbose:
         data_iter = tqdm.tqdm(data_loader)
     else:
         data_iter = data_loader
```

### Comparing `ood_detectors-0.0.8/LICENSE` & `ood_detectors-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/README.md` & `ood_detectors-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/pyproject.toml` & `ood_detectors-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.8/PKG-INFO` & `ood_detectors-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ood_detectors
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/Arty-Facts/ood_detectors#readme
 Project-URL: Issues, https://github.com/Arty-Facts/ood_detectors/issues
 Project-URL: Source, https://github.com/Arty-Facts/ood_detectors
 Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>, Yifan Ding <yifan.ding@liu.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

