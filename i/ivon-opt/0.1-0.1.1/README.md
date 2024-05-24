# Comparing `tmp/ivon-opt-0.1.tar.gz` & `tmp/ivon_opt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivon-opt-0.1.tar", last modified: Wed Feb 28 05:39:46 2024, max compression
+gzip compressed data, was "ivon_opt-0.1.1.tar", last modified: Fri May 24 19:57:27 2024, max compression
```

## Comparing `ivon-opt-0.1.tar` & `ivon_opt-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 pnickl    (1000) pnickl    (1000)        0 2024-02-28 05:39:46.945060 ivon-opt-0.1/
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)    35149 2024-02-27 06:50:44.000000 ivon-opt-0.1/LICENSE
--rw-r--r--   0 pnickl    (1000) pnickl    (1000)     3971 2024-02-28 05:39:46.945060 ivon-opt-0.1/PKG-INFO
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)     3454 2024-02-28 05:38:46.000000 ivon-opt-0.1/README.md
-drwxrwxr-x   0 pnickl    (1000) pnickl    (1000)        0 2024-02-28 05:39:46.941060 ivon-opt-0.1/ivon/
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)       44 2024-02-27 06:50:44.000000 ivon-opt-0.1/ivon/__init__.py
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)    10613 2024-02-28 04:40:33.000000 ivon-opt-0.1/ivon/_ivon.py
-drwxrwxr-x   0 pnickl    (1000) pnickl    (1000)        0 2024-02-28 05:39:46.945060 ivon-opt-0.1/ivon_opt.egg-info/
--rw-r--r--   0 pnickl    (1000) pnickl    (1000)     3971 2024-02-28 05:39:46.000000 ivon-opt-0.1/ivon_opt.egg-info/PKG-INFO
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)      185 2024-02-28 05:39:46.000000 ivon-opt-0.1/ivon_opt.egg-info/SOURCES.txt
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)        1 2024-02-28 05:39:46.000000 ivon-opt-0.1/ivon_opt.egg-info/dependency_links.txt
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)        5 2024-02-28 05:39:46.000000 ivon-opt-0.1/ivon_opt.egg-info/top_level.txt
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)       38 2024-02-28 05:39:46.945060 ivon-opt-0.1/setup.cfg
--rw-rw-r--   0 pnickl    (1000) pnickl    (1000)      883 2024-02-28 05:28:29.000000 ivon-opt-0.1/setup.py
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-24 19:57:27.605216 ivon_opt-0.1.1/
+-rw-rw-r--   0 ys        (1000) ys        (1000)    35149 2024-05-24 19:18:06.000000 ivon_opt-0.1.1/LICENSE
+-rw-r--r--   0 ys        (1000) ys        (1000)     4312 2024-05-24 19:57:27.605216 ivon_opt-0.1.1/PKG-INFO
+-rw-rw-r--   0 ys        (1000) ys        (1000)     3793 2024-05-24 19:18:06.000000 ivon_opt-0.1.1/README.md
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-24 19:57:27.605216 ivon_opt-0.1.1/ivon/
+-rw-rw-r--   0 ys        (1000) ys        (1000)       44 2024-05-24 19:18:06.000000 ivon_opt-0.1.1/ivon/__init__.py
+-rw-rw-r--   0 ys        (1000) ys        (1000)    10610 2024-05-24 19:18:42.000000 ivon_opt-0.1.1/ivon/_ivon.py
+drwxrwxr-x   0 ys        (1000) ys        (1000)        0 2024-05-24 19:57:27.605216 ivon_opt-0.1.1/ivon_opt.egg-info/
+-rw-r--r--   0 ys        (1000) ys        (1000)     4312 2024-05-24 19:57:27.000000 ivon_opt-0.1.1/ivon_opt.egg-info/PKG-INFO
+-rw-rw-r--   0 ys        (1000) ys        (1000)      185 2024-05-24 19:57:27.000000 ivon_opt-0.1.1/ivon_opt.egg-info/SOURCES.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)        1 2024-05-24 19:57:27.000000 ivon_opt-0.1.1/ivon_opt.egg-info/dependency_links.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)        5 2024-05-24 19:57:27.000000 ivon_opt-0.1.1/ivon_opt.egg-info/top_level.txt
+-rw-rw-r--   0 ys        (1000) ys        (1000)       38 2024-05-24 19:57:27.605216 ivon_opt-0.1.1/setup.cfg
+-rw-rw-r--   0 ys        (1000) ys        (1000)      885 2024-05-24 19:19:44.000000 ivon_opt-0.1.1/setup.py
```

### Comparing `ivon-opt-0.1/LICENSE` & `ivon_opt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ivon-opt-0.1/PKG-INFO` & `ivon_opt-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ivon-opt
-Version: 0.1
+Version: 0.1.1
 Summary: An optimizer for neural networks based on variational learning
 Home-page: https://github.com/team-approx-bayes/ivon
 Author: IVON Team
 Author-email: ivonteam@googlegroups.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Improved Variational Online Newton (IVON)
+[![Downloads](https://static.pepy.tech/badge/ivon-opt)](https://pepy.tech/project/ivon-opt) [![Downloads](https://static.pepy.tech/badge/ivon-opt/month)](https://pepy.tech/project/ivon-opt)
 
 We provide code of the IVON optimizer to train deep neural networks, along with a usage guide and small-scale examples.
 
 **Variational Learning is Effective for Large Deep Networks**  
 *Y. Shen\*, N. Daheim\*, B. Cong, P. Nickl, G.M. Marconi, C. Bazan, R. Yokota, I. Gurevych, D. Cremers, M.E. Khan, T. Möllenhoff*\
 Paper: https://arxiv.org/abs/2402.17641
 
@@ -28,29 +29,31 @@
 
 **Dependencies**
 
 Install PyTorch as described [here](https://pytorch.org/get-started/locally/): `pip3 install torch --index-url https://download.pytorch.org/whl/cu118`
 
 ## Usage guide
 
+In Appendix A of the [paper](https://arxiv.org/abs/2402.17641), we provide practical guidelines for choosing IVON hyperparameters.
+
 **Training loop**
 
 In the code snippet below we demonstrate the difference in the implementation of the training loop of the IVON optimizer compared to standard optimizers like SGD or Adam.
 The standard setting for weight sampling during training is to use one MC sample (`train_samples=1`).
 
 ```diff
 import torch
 +import ivon
 
 train_loader = torch.utils.data.DataLoader(train_dataset) 
 test_loader = torch.utils.data.DataLoader(test_dataset) 
 model = MLP()
 
 -optimizer = torch.optim.Adam(model.parameters())
-+optimizer = ivon.IVON(model.parameters())
++optimizer = ivon.IVON(model.parameters(), lr=0.1, ess=len(train_dataset))
 
 for X, y in train_loader:
 
 +    for _ in range(train_samples):
 +       with optimizer.sampled_params(train=True)
             optimizer.zero_grad()
             logit = model(X)
@@ -60,22 +63,23 @@
     optimizer.step()
 ```
 
 **Prediction**
 
 There are two different ways of using the variational posterior of IVON for prediction:
 
-(1) Predicting at the mean of the variational posterior (fast)
+(1) IVON can be used like standard optimizers:
 
 ```
 for X, y in test_loader:
     logit = model(X)
     _, prediction = logit.max(1)
 ```
-(2) Predicting with Bayesian model averaging obtained by drawing a total of `test_samples` weight samples from the variational posterior (slower, but better inference with multiple weight samples)
+
+(2) A better way is to do posterior averaging. We can draw a total of `test_samples` weights from a Gaussian, predict with each one and average the predictions to obtain predictive probabilities. 
 
 ```
 for X, y in test_loader:
     sampled_probs = []
     for i in range(test_samples):
         with optimizer.sampled_params():
             sampled_logit = model(X)
@@ -83,20 +87,20 @@
     prob = torch.mean(torch.stack(sampled_probs), dim=0)
     _, prediction = prob.max(1)
 ```
 
 ## Examples
 
 We include three Google Colab notebooks to demonstrate the usage of the IVON optimizers on small-scale problems.
-1. [2-D Logistic Regression](https://colab.research.google.com/drive/1o2XFJA8UbCiAUEKbiGFsNCwuvhZdFFfg?usp=sharing)
-    - SGD finds the mode of the weight posterior, while IVON converges to a region that is more robust to perturbation.
+1. [MNIST image classification](https://colab.research.google.com/drive/1Q6MdLxmvR5Q1I2NbVXLCgGTDuP1m79tV?usp=sharing)
+    - We compare IVON to an SGD baseline.
 2. [1-D Regression](https://colab.research.google.com/drive/1GcCCRfiZ6u7OwkYS46LGIAQKLnGL8Ae7?usp=sharing)
     - IVON captures uncertainty in regions with little data. AdamW fails at this task.
-3. [MNIST image classification](https://colab.research.google.com/drive/1Q6MdLxmvR5Q1I2NbVXLCgGTDuP1m79tV?usp=sharing)
-    - We compare IVON to an SGD baseline.
+3. [2-D Logistic Regression](https://colab.research.google.com/drive/1o2XFJA8UbCiAUEKbiGFsNCwuvhZdFFfg?usp=sharing)
+    - SGD finds the mode of the weight posterior, while IVON converges to a region that is more robust to perturbation.
 
 ## How to cite
 
 ```
 @article{shen2024variational,
       title={Variational Learning is Effective for Large Deep Networks}, 
       author={Yuesong Shen and Nico Daheim and Bai Cong and Peter Nickl and Gian Maria Marconi and Clement Bazan and Rio Yokota and Iryna Gurevych and Daniel Cremers and Mohammad Emtiyaz Khan and Thomas Möllenhoff},
```

### Comparing `ivon-opt-0.1/README.md` & `ivon_opt-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Improved Variational Online Newton (IVON)
+[![Downloads](https://static.pepy.tech/badge/ivon-opt)](https://pepy.tech/project/ivon-opt) [![Downloads](https://static.pepy.tech/badge/ivon-opt/month)](https://pepy.tech/project/ivon-opt)
 
 We provide code of the IVON optimizer to train deep neural networks, along with a usage guide and small-scale examples.
 
 **Variational Learning is Effective for Large Deep Networks**  
 *Y. Shen\*, N. Daheim\*, B. Cong, P. Nickl, G.M. Marconi, C. Bazan, R. Yokota, I. Gurevych, D. Cremers, M.E. Khan, T. Möllenhoff*\
 Paper: https://arxiv.org/abs/2402.17641
 
@@ -13,29 +14,31 @@
 
 **Dependencies**
 
 Install PyTorch as described [here](https://pytorch.org/get-started/locally/): `pip3 install torch --index-url https://download.pytorch.org/whl/cu118`
 
 ## Usage guide
 
+In Appendix A of the [paper](https://arxiv.org/abs/2402.17641), we provide practical guidelines for choosing IVON hyperparameters.
+
 **Training loop**
 
 In the code snippet below we demonstrate the difference in the implementation of the training loop of the IVON optimizer compared to standard optimizers like SGD or Adam.
 The standard setting for weight sampling during training is to use one MC sample (`train_samples=1`).
 
 ```diff
 import torch
 +import ivon
 
 train_loader = torch.utils.data.DataLoader(train_dataset) 
 test_loader = torch.utils.data.DataLoader(test_dataset) 
 model = MLP()
 
 -optimizer = torch.optim.Adam(model.parameters())
-+optimizer = ivon.IVON(model.parameters())
++optimizer = ivon.IVON(model.parameters(), lr=0.1, ess=len(train_dataset))
 
 for X, y in train_loader:
 
 +    for _ in range(train_samples):
 +       with optimizer.sampled_params(train=True)
             optimizer.zero_grad()
             logit = model(X)
@@ -45,22 +48,23 @@
     optimizer.step()
 ```
 
 **Prediction**
 
 There are two different ways of using the variational posterior of IVON for prediction:
 
-(1) Predicting at the mean of the variational posterior (fast)
+(1) IVON can be used like standard optimizers:
 
 ```
 for X, y in test_loader:
     logit = model(X)
     _, prediction = logit.max(1)
 ```
-(2) Predicting with Bayesian model averaging obtained by drawing a total of `test_samples` weight samples from the variational posterior (slower, but better inference with multiple weight samples)
+
+(2) A better way is to do posterior averaging. We can draw a total of `test_samples` weights from a Gaussian, predict with each one and average the predictions to obtain predictive probabilities. 
 
 ```
 for X, y in test_loader:
     sampled_probs = []
     for i in range(test_samples):
         with optimizer.sampled_params():
             sampled_logit = model(X)
@@ -68,20 +72,20 @@
     prob = torch.mean(torch.stack(sampled_probs), dim=0)
     _, prediction = prob.max(1)
 ```
 
 ## Examples
 
 We include three Google Colab notebooks to demonstrate the usage of the IVON optimizers on small-scale problems.
-1. [2-D Logistic Regression](https://colab.research.google.com/drive/1o2XFJA8UbCiAUEKbiGFsNCwuvhZdFFfg?usp=sharing)
-    - SGD finds the mode of the weight posterior, while IVON converges to a region that is more robust to perturbation.
+1. [MNIST image classification](https://colab.research.google.com/drive/1Q6MdLxmvR5Q1I2NbVXLCgGTDuP1m79tV?usp=sharing)
+    - We compare IVON to an SGD baseline.
 2. [1-D Regression](https://colab.research.google.com/drive/1GcCCRfiZ6u7OwkYS46LGIAQKLnGL8Ae7?usp=sharing)
     - IVON captures uncertainty in regions with little data. AdamW fails at this task.
-3. [MNIST image classification](https://colab.research.google.com/drive/1Q6MdLxmvR5Q1I2NbVXLCgGTDuP1m79tV?usp=sharing)
-    - We compare IVON to an SGD baseline.
+3. [2-D Logistic Regression](https://colab.research.google.com/drive/1o2XFJA8UbCiAUEKbiGFsNCwuvhZdFFfg?usp=sharing)
+    - SGD finds the mode of the weight posterior, while IVON converges to a region that is more robust to perturbation.
 
 ## How to cite
 
 ```
 @article{shen2024variational,
       title={Variational Learning is Effective for Large Deep Networks}, 
       author={Yuesong Shen and Nico Daheim and Bai Cong and Peter Nickl and Gian Maria Marconi and Clement Bazan and Rio Yokota and Iryna Gurevych and Daniel Cremers and Mohammad Emtiyaz Khan and Thomas Möllenhoff},
```

### Comparing `ivon-opt-0.1/ivon/_ivon.py` & `ivon_opt-0.1.1/ivon/_ivon.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         for group in self.param_groups:
             for p in group["params"]:
                 if p is None:
                     continue
 
                 p_slice = slice(offset, offset + p.numel())
 
-                p.data = param_avg[p_slice].view(*p.shape)
+                p.data = param_avg[p_slice].view(p.shape)
                 if train:
                     if p.requires_grad:
                         param_grads.append(p.grad.flatten())
                     else:
                         param_grads.append(torch.zeros_like(p).flatten())
                 offset += p.numel()
         assert offset == self._numel  # sanity check
@@ -211,15 +211,15 @@
                     continue
 
                 p_avg = p.data.flatten()
                 numel = p.numel()
                 p_noise = noise_sample[offset : offset + numel]
 
                 param_avgs.append(p_avg)
-                p.data = (p_avg + p_noise).view(*p.shape)
+                p.data = (p_avg + p_noise).view(p.shape)
                 goffset += numel
                 offset += numel
             assert goffset == group["numel"]  # sanity check
         assert offset == self._numel  # sanity check
 
         return torch.cat(param_avgs, 0), torch.cat(noise_samples, 0)
 
@@ -264,15 +264,15 @@
             )
 
             # update params
             pg_offset = 0
             for p in group["params"]:
                 if p is not None:
                     p.data = param_avg[pg_offset : pg_offset + p.numel()].view(
-                        *p.shape
+                        p.shape
                     )
                     pg_offset += p.numel()
             assert pg_offset == group["numel"]  # sanity check
             offset += group["numel"]
         assert offset == self._numel  # sanity check
 
     @staticmethod
```

### Comparing `ivon-opt-0.1/ivon_opt.egg-info/PKG-INFO` & `ivon_opt-0.1.1/ivon_opt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ivon-opt
-Version: 0.1
+Version: 0.1.1
 Summary: An optimizer for neural networks based on variational learning
 Home-page: https://github.com/team-approx-bayes/ivon
 Author: IVON Team
 Author-email: ivonteam@googlegroups.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Improved Variational Online Newton (IVON)
+[![Downloads](https://static.pepy.tech/badge/ivon-opt)](https://pepy.tech/project/ivon-opt) [![Downloads](https://static.pepy.tech/badge/ivon-opt/month)](https://pepy.tech/project/ivon-opt)
 
 We provide code of the IVON optimizer to train deep neural networks, along with a usage guide and small-scale examples.
 
 **Variational Learning is Effective for Large Deep Networks**  
 *Y. Shen\*, N. Daheim\*, B. Cong, P. Nickl, G.M. Marconi, C. Bazan, R. Yokota, I. Gurevych, D. Cremers, M.E. Khan, T. Möllenhoff*\
 Paper: https://arxiv.org/abs/2402.17641
 
@@ -28,29 +29,31 @@
 
 **Dependencies**
 
 Install PyTorch as described [here](https://pytorch.org/get-started/locally/): `pip3 install torch --index-url https://download.pytorch.org/whl/cu118`
 
 ## Usage guide
 
+In Appendix A of the [paper](https://arxiv.org/abs/2402.17641), we provide practical guidelines for choosing IVON hyperparameters.
+
 **Training loop**
 
 In the code snippet below we demonstrate the difference in the implementation of the training loop of the IVON optimizer compared to standard optimizers like SGD or Adam.
 The standard setting for weight sampling during training is to use one MC sample (`train_samples=1`).
 
 ```diff
 import torch
 +import ivon
 
 train_loader = torch.utils.data.DataLoader(train_dataset) 
 test_loader = torch.utils.data.DataLoader(test_dataset) 
 model = MLP()
 
 -optimizer = torch.optim.Adam(model.parameters())
-+optimizer = ivon.IVON(model.parameters())
++optimizer = ivon.IVON(model.parameters(), lr=0.1, ess=len(train_dataset))
 
 for X, y in train_loader:
 
 +    for _ in range(train_samples):
 +       with optimizer.sampled_params(train=True)
             optimizer.zero_grad()
             logit = model(X)
@@ -60,22 +63,23 @@
     optimizer.step()
 ```
 
 **Prediction**
 
 There are two different ways of using the variational posterior of IVON for prediction:
 
-(1) Predicting at the mean of the variational posterior (fast)
+(1) IVON can be used like standard optimizers:
 
 ```
 for X, y in test_loader:
     logit = model(X)
     _, prediction = logit.max(1)
 ```
-(2) Predicting with Bayesian model averaging obtained by drawing a total of `test_samples` weight samples from the variational posterior (slower, but better inference with multiple weight samples)
+
+(2) A better way is to do posterior averaging. We can draw a total of `test_samples` weights from a Gaussian, predict with each one and average the predictions to obtain predictive probabilities. 
 
 ```
 for X, y in test_loader:
     sampled_probs = []
     for i in range(test_samples):
         with optimizer.sampled_params():
             sampled_logit = model(X)
@@ -83,20 +87,20 @@
     prob = torch.mean(torch.stack(sampled_probs), dim=0)
     _, prediction = prob.max(1)
 ```
 
 ## Examples
 
 We include three Google Colab notebooks to demonstrate the usage of the IVON optimizers on small-scale problems.
-1. [2-D Logistic Regression](https://colab.research.google.com/drive/1o2XFJA8UbCiAUEKbiGFsNCwuvhZdFFfg?usp=sharing)
-    - SGD finds the mode of the weight posterior, while IVON converges to a region that is more robust to perturbation.
+1. [MNIST image classification](https://colab.research.google.com/drive/1Q6MdLxmvR5Q1I2NbVXLCgGTDuP1m79tV?usp=sharing)
+    - We compare IVON to an SGD baseline.
 2. [1-D Regression](https://colab.research.google.com/drive/1GcCCRfiZ6u7OwkYS46LGIAQKLnGL8Ae7?usp=sharing)
     - IVON captures uncertainty in regions with little data. AdamW fails at this task.
-3. [MNIST image classification](https://colab.research.google.com/drive/1Q6MdLxmvR5Q1I2NbVXLCgGTDuP1m79tV?usp=sharing)
-    - We compare IVON to an SGD baseline.
+3. [2-D Logistic Regression](https://colab.research.google.com/drive/1o2XFJA8UbCiAUEKbiGFsNCwuvhZdFFfg?usp=sharing)
+    - SGD finds the mode of the weight posterior, while IVON converges to a region that is more robust to perturbation.
 
 ## How to cite
 
 ```
 @article{shen2024variational,
       title={Variational Learning is Effective for Large Deep Networks}, 
       author={Yuesong Shen and Nico Daheim and Bai Cong and Peter Nickl and Gian Maria Marconi and Clement Bazan and Rio Yokota and Iryna Gurevych and Daniel Cremers and Mohammad Emtiyaz Khan and Thomas Möllenhoff},
```

### Comparing `ivon-opt-0.1/setup.py` & `ivon_opt-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ivon-opt",
-    version="0.1",
+    version="0.1.1",
     url="https://github.com/team-approx-bayes/ivon",
     packages=find_packages(),
     description="An optimizer for neural networks based on variational learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     license='GPLv3+',
```

