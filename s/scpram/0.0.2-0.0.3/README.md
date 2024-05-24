# Comparing `tmp/scpram-0.0.2.tar.gz` & `tmp/scpram-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scpram-0.0.2.tar", last modified: Thu Dec  7 09:25:54 2023, max compression
+gzip compressed data, was "scpram-0.0.3.tar", last modified: Fri May 24 05:35:12 2024, max compression
```

## Comparing `scpram-0.0.2.tar` & `scpram-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-12-07 09:25:54.145128 scpram-0.0.2/
--rw-rw-rw-   0        0        0     1067 2023-12-07 08:45:57.000000 scpram-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2331 2023-12-07 09:25:54.144124 scpram-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-11-16 07:21:55.000000 scpram-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-12-07 09:25:54.118264 scpram-0.0.2/scpram/
--rw-rw-rw-   0        0        0      150 2023-11-15 12:47:31.000000 scpram-0.0.2/scpram/__init__.py
--rw-rw-rw-   0        0        0     1717 2023-11-15 03:17:40.000000 scpram-0.0.2/scpram/data_process.py
--rw-rw-rw-   0        0        0     3735 2023-11-15 12:53:20.000000 scpram-0.0.2/scpram/dataset.py
--rw-rw-rw-   0        0        0    17928 2023-12-07 08:52:37.000000 scpram-0.0.2/scpram/evaluate.py
--rw-rw-rw-   0        0        0    12269 2023-11-15 14:28:10.000000 scpram-0.0.2/scpram/models.py
--rw-rw-rw-   0        0        0     5367 2023-11-15 07:39:11.000000 scpram-0.0.2/scpram/utils.py
--rw-rw-rw-   0        0        0       21 2023-12-07 09:24:16.000000 scpram-0.0.2/scpram/version.py
-drwxrwxrwx   0        0        0        0 2023-12-07 09:25:54.144124 scpram-0.0.2/scpram.egg-info/
--rw-rw-rw-   0        0        0     2331 2023-12-07 09:25:54.000000 scpram-0.0.2/scpram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-12-07 09:25:54.000000 scpram-0.0.2/scpram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-07 09:25:54.000000 scpram-0.0.2/scpram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-12-07 09:25:54.000000 scpram-0.0.2/scpram.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-12-07 09:25:54.000000 scpram-0.0.2/scpram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-07 09:25:54.145128 scpram-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2537 2023-12-07 09:25:17.000000 scpram-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:12.674011 scpram-0.0.3/
+-rw-rw-rw-   0        0        0     1067 2023-12-07 08:45:57.000000 scpram-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2331 2024-05-24 05:35:12.672436 scpram-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3910 2024-04-06 07:33:30.000000 scpram-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:12.646126 scpram-0.0.3/scpram/
+-rw-rw-rw-   0        0        0      150 2023-11-15 12:47:31.000000 scpram-0.0.3/scpram/__init__.py
+-rw-rw-rw-   0        0        0     1717 2023-11-15 03:17:40.000000 scpram-0.0.3/scpram/data_process.py
+-rw-rw-rw-   0        0        0     3735 2023-11-15 12:53:20.000000 scpram-0.0.3/scpram/dataset.py
+-rw-rw-rw-   0        0        0    17928 2023-12-07 08:52:37.000000 scpram-0.0.3/scpram/evaluate.py
+-rw-rw-rw-   0        0        0    12290 2024-05-24 05:35:07.000000 scpram-0.0.3/scpram/models.py
+-rw-rw-rw-   0        0        0     5367 2023-11-15 07:39:11.000000 scpram-0.0.3/scpram/utils.py
+-rw-rw-rw-   0        0        0       21 2023-12-07 09:24:16.000000 scpram-0.0.3/scpram/version.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:35:12.671931 scpram-0.0.3/scpram.egg-info/
+-rw-rw-rw-   0        0        0     2331 2024-05-24 05:35:12.000000 scpram-0.0.3/scpram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-24 05:35:12.000000 scpram-0.0.3/scpram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 05:35:12.000000 scpram-0.0.3/scpram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2024-05-24 05:35:12.000000 scpram-0.0.3/scpram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 05:35:12.000000 scpram-0.0.3/scpram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 05:35:12.674011 scpram-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2537 2024-05-24 05:35:00.000000 scpram-0.0.3/setup.py
```

### Comparing `scpram-0.0.2/LICENSE` & `scpram-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scpram-0.0.2/PKG-INFO` & `scpram-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpram
-Version: 0.0.2
+Version: 0.0.3
 Summary: scPRAM accurately predicts single-cell gene expression perturbation response based on attention mechanism
 Home-page: https://github.com/jiang-q19/scPRAM
 Author: Qun Jiang
 License: MIT Licence
 Keywords: single cell,perturbation,attention,optimal transport
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scpram-0.0.2/scpram/data_process.py` & `scpram-0.0.3/scpram/data_process.py`

 * *Files identical despite different names*

### Comparing `scpram-0.0.2/scpram/dataset.py` & `scpram-0.0.3/scpram/dataset.py`

 * *Files identical despite different names*

### Comparing `scpram-0.0.2/scpram/evaluate.py` & `scpram-0.0.3/scpram/evaluate.py`

 * *Files identical despite different names*

### Comparing `scpram-0.0.2/scpram/models.py` & `scpram-0.0.3/scpram/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             Normal(0, 1)
         ).sum(dim=1)
         loss_rec = ((x - x_hat) ** 2).sum(dim=1)
 
         return x_hat, loss_rec, loss_kl
 
     def get_latent_adata(self, adata):
-        device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+        device = self.device
         x = Tensor(adata.to_df().values).to(device)
         latent_z = self.encode(x)[0].cpu().detach().numpy()
         latent_adata = sc.AnnData(X=latent_z, obs=adata.obs.copy())
         return latent_adata
 
     def get_loss(self, x):
         x_hat, loss_rec, loss_kl = self.forward(x)
@@ -114,14 +114,15 @@
             pbar.set_description("Training Epoch {}".format(epoch))
             for idx, x in enumerate(train_loader):
                 x = x.to(device)
                 loss_rec, loss_kl = self.get_loss(x)
                 SCPRAM_loss = (0.5 * loss_rec + 0.5 * (loss_kl * self.kl_weight)).mean()
                 optim_SCPRAM.zero_grad()
                 SCPRAM_loss.backward()
+                torch.nn.utils.clip_grad_norm(self.parameters(), 10)
                 optim_SCPRAM.step()
             pbar.set_postfix(SCPRAM_loss=SCPRAM_loss.item(), recon_loss=loss_rec.mean().item(),
                              kl_loss=loss_kl.mean().item())
 
     def ot_predict(self, adata_train, cell_to_pred, key_dic):
         '''
         The optimal transport mapping is used directly to predict the expression state after perturbation
```

### Comparing `scpram-0.0.2/scpram/utils.py` & `scpram-0.0.3/scpram/utils.py`

 * *Files identical despite different names*

### Comparing `scpram-0.0.2/scpram.egg-info/PKG-INFO` & `scpram-0.0.3/scpram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scpram
-Version: 0.0.2
+Version: 0.0.3
 Summary: scPRAM accurately predicts single-cell gene expression perturbation response based on attention mechanism
 Home-page: https://github.com/jiang-q19/scPRAM
 Author: Qun Jiang
 License: MIT Licence
 Keywords: single cell,perturbation,attention,optimal transport
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scpram-0.0.2/setup.py` & `scpram-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name="scpram",
-    version="0.0.2",
+    version="0.0.3",
     description="scPRAM accurately predicts single-cell gene expression perturbation response based on attention mechanism",
     long_description="With the rapid advancement of single-cell sequencing technology, we are gradually enabled to delve into the cellular re-sponses to various external perturbations at the gene expression level. However, obtaining perturbed samples in certain scenarios may be considerably challenging, and the substantial costs associated with sequencing also curtail the feasibil-ity of large-scale experimentation. A repertoire of methodologies has been employed for forecasting perturbative re-sponses in single-cell gene expression. However, existing methods only focus on predictions at the average level and do not capture the heterogeneity at the single-cell resolution effectively. Here we present scPRAM, a method for predicting Perturbation Responses in single-cell gene expression based on At-tention Mechanisms. Leveraging variational autoencoders and optimal transport, scPRAM aligns cell states before and after perturbation, followed by accurate prediction of gene expression responses to perturbations for unseen cell types through attention mechanisms. Experiments on multiple real perturbation datasets involving drug treatments and bacteri-al infections demonstrate that scPRAM attains heightened accuracy in perturbation prediction across cell types, species, and individuals, surpassing existing methodologies. Furthermore, scPRAM demonstrates outstanding capability in identi-fying differentially expressed genes under perturbation, capturing heterogeneity in perturbation responses across spe-cies, and maintaining stability in the presence of data noise and sample size variations.",
     license="MIT Licence",
     url="https://github.com/jiang-q19/scPRAM",
     author="Qun Jiang",
     classifiers=[
         "Programming Language :: Python :: 3.8",
```

