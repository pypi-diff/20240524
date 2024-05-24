# Comparing `tmp/dna_se-0.0.9.tar.gz` & `tmp/DNA_SE-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dna_se-0.0.9.tar", last modified: Thu May  9 08:12:03 2024, max compression
+gzip compressed data, was "DNA_SE-0.1.0.tar", last modified: Fri May 24 06:01:03 2024, max compression
```

## Comparing `dna_se-0.0.9.tar` & `DNA_SE-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 08:12:03.000000 dna_se-0.0.9/
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 08:12:03.000000 dna_se-0.0.9/DNA_SE/
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     5216 2024-05-09 07:43:23.000000 dna_se-0.0.9/DNA_SE/DNA_SE.py
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       25 2024-05-08 12:46:34.000000 dna_se-0.0.9/DNA_SE/__init__.py
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 08:12:03.000000 dna_se-0.0.9/DNA_SE.egg-info/
--rw-r--r--   0 r12user2  (1003) r12user2  (1003)     5202 2024-05-09 08:12:03.000000 dna_se-0.0.9/DNA_SE.egg-info/PKG-INFO
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      186 2024-05-09 08:12:03.000000 dna_se-0.0.9/DNA_SE.egg-info/SOURCES.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        1 2024-05-09 08:12:03.000000 dna_se-0.0.9/DNA_SE.egg-info/dependency_links.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        7 2024-05-09 08:12:03.000000 dna_se-0.0.9/DNA_SE.egg-info/top_level.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1091 2024-05-08 12:46:34.000000 dna_se-0.0.9/LICENSE.txt
--rw-r--r--   0 r12user2  (1003) r12user2  (1003)     5202 2024-05-09 08:12:03.000000 dna_se-0.0.9/PKG-INFO
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     4783 2024-05-09 08:11:12.000000 dna_se-0.0.9/README.md
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       38 2024-05-09 08:12:03.000000 dna_se-0.0.9/setup.cfg
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      686 2024-05-09 08:11:19.000000 dna_se-0.0.9/setup.py
+drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/
+drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/DNA_SE/
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     6251 2024-05-23 19:16:22.000000 DNA_SE-0.1.0/DNA_SE/DNA_SE.py
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)       25 2024-05-08 12:46:34.000000 DNA_SE-0.1.0/DNA_SE/__init__.py
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      208 2024-05-23 18:18:05.000000 DNA_SE-0.1.0/DNA_SE/image.py
+drwxrwxr-x   0 qsliu     (1003) qsliu     (1003)        0 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/DNA_SE.egg-info/
+-rw-r--r--   0 qsliu     (1003) qsliu     (1003)     5202 2024-05-24 06:01:03.000000 DNA_SE-0.1.0/DNA_SE.egg-info/PKG-INFO
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      202 2024-05-24 06:01:03.000000 DNA_SE-0.1.0/DNA_SE.egg-info/SOURCES.txt
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)        1 2024-05-24 06:01:03.000000 DNA_SE-0.1.0/DNA_SE.egg-info/dependency_links.txt
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)        7 2024-05-24 06:01:03.000000 DNA_SE-0.1.0/DNA_SE.egg-info/top_level.txt
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     1091 2024-05-08 12:46:34.000000 DNA_SE-0.1.0/LICENSE.txt
+-rw-r--r--   0 qsliu     (1003) qsliu     (1003)     5202 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/PKG-INFO
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)     4783 2024-05-09 08:11:12.000000 DNA_SE-0.1.0/README.md
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)       38 2024-05-24 06:01:03.453419 DNA_SE-0.1.0/setup.cfg
+-rw-rw-r--   0 qsliu     (1003) qsliu     (1003)      686 2024-05-24 06:00:00.000000 DNA_SE-0.1.0/setup.py
```

### Comparing `dna_se-0.0.9/DNA_SE/DNA_SE.py` & `DNA_SE-0.1.0/DNA_SE/DNA_SE.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import torch
 from torch import nn
 from torch.optim import Adam
 import torch.utils.data as Data
 import numpy as np
-import torch.nn.functional as F     
+import torch.nn.functional as F    
+import matplotlib.pyplot as plt
+from matplotlib.animation import FuncAnimation 
 
-def dnase(p, Oi, BATCHSIZE, EPOCH, M, B, input_dim, hidden_dim, output_dim, K_func, C_func, psi_func, depth, activation = 'tanh', device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
+def dna(p, Oi, BATCHSIZE, EPOCH, M, B, input_dim, hidden_dim, output_dim, K_func, C_func, depth, psi_func = None, esti_mask = False, activation = 'tanh', device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')):
     
     '''
     p: int, the number of features X
     Oi: np.array, the observed data
     BATCHSIZE: int, the batch size
     EPOCH: int, the number of epochs
     M: int, the Monte Carlo number of data points for t
@@ -39,28 +41,27 @@
     class MyModel(nn.Module):
         def __init__(self, input_dim, hidden_dim, output_dim, depth, activation):
             super(MyModel, self).__init__()
             layers = []
             for i in range(depth):
                 if i == 0:
                     layers.append(nn.Linear(input_dim, hidden_dim))
+                    if activation == 'relu':
+                        layers.append(nn.ReLU())
+                    elif activation == 'sigmoid':
+                        layers.append(nn.Sigmoid())
+                    elif activation == 'tanh':
+                        layers.append(nn.Tanh())
+                    else:
+                        raise ValueError("Unsupported activation function.")
                 elif i == depth - 1:
                     layers.append(nn.Linear(hidden_dim, output_dim))
                 else:
                     layers.append(nn.Linear(hidden_dim, hidden_dim))
-                    
-                if activation == 'relu':
-                    layers.append(nn.ReLU())
-                elif activation == 'sigmoid':
-                    layers.append(nn.Sigmoid())
-                elif activation == 'tanh':
-                    layers.append(nn.Tanh())
-                else:
-                    raise ValueError("Unsupported activation function.")
-                    
+                     
             self.layers = nn.ModuleList(layers)
             
         def forward(self, x):
             for layer in self.layers:
                 x = layer(x)
             return x
 
@@ -86,44 +87,77 @@
     train_loader = Data.DataLoader(dataset=train_data, batch_size=BATCHSIZE, shuffle=True)
     
     # set parameters and optimizer
     Parameters_b = model_b.parameters() # ,{"params":beta.parameters()}]
     optimizer_b = torch.optim.Adam(Parameters_b, lr=1e-3)
     Parameters_beta = beta.parameters()
     optimizer_beta = torch.optim.Adam(Parameters_beta, lr=1e-2)
+    losses = []
+    epochs = []
     
     for epoch in range(EPOCH):
         for step, (t_train, _) in enumerate(train_loader):
             
-            s = torch.linspace(min(Oi),max(Oi),M).reshape(M,1).to(device)
-            t = t_train[..., -1]  
+            t = torch.linspace(int(min(Oi)),int(max(Oi)),M).reshape(M,1).to(device)
+            s = t_train[..., -1].reshape(BATCHSIZE,1).to(device)
+            ones_M = torch.ones(M,1).to(device)
 
             def loss_function_integral(s, t, Oi, beta, model_b):
                 
-                inter_left = torch.sum(K_func(s,t,Oi,beta)*model_b(s,Oi))
-                inter_right = C_func(t,Oi,beta) + model_b(t,Oi)
-                return torch.mean(torch.sum((inter_left - inter_right)**2))
+                inter_left = torch.mean(K_func(s,t,Oi,beta)*torch.kron(ones_M,model_b(s)).reshape(M,BATCHSIZE), dim=1).reshape(M,1)
+                inter_right = C_func(t,Oi,beta) + model_b(t)
+                return torch.mean((inter_left - inter_right)**2)
             
             optimizer_b.zero_grad()
             loss_integral = loss_function_integral(s, t, Oi, beta, model_b)
             loss_integral.backward()
             optimizer_b.step()
+
             
-            if step % 5 == 0:
+            if step % 5 == 0 and esti_mask == 1:
                 
                 def loss_function_estimate(Oi, beta, model_b):
                 
                     return torch.mean(psi_func(Oi, beta, model_b)**2)
             
                 optimizer_beta.zero_grad()
                 loss_estimate = loss_function_estimate(Oi, beta, model_b)
                 loss_estimate.backward()
                 optimizer_beta.step()
 
-        if epoch % 100 == 0:
+        if epoch % 100 == 0 and esti_mask == 1:
             print(f'Epoch {epoch}: loss = {loss_estimate.item()}')
-    return model_b, beta.data(), optimizer_b, optimizer_beta
+        if epoch % 1 == 0 and esti_mask == 0:
+            print(f'Epoch {epoch}: loss = {loss_integral.item()}')
+            losses.append(loss_integral.item())
+            epochs.append(epoch)
+
+    if esti_mask == 1:
+        return model_b, beta.data()
+    else:
+        return model_b
+
+# a simple example
+p = 1
+Oi = torch.rand(1000,1)
+BATCHSIZE = 100
+EPOCH = 200
+M = 1000
+B = 10000
+input_dim = 1
+output_dim = 1
+hidden_dim = 5
+depth = 2
+ones_B = torch.ones(BATCHSIZE,1).to(torch.device('cuda' if torch.cuda.is_available() else 'cpu'))
+
+def K_func(x,y,Oi,b):
+    return y * torch.kron(ones_B,x).reshape(BATCHSIZE,M)
+def C_func(x,Oi,b):
+    return -torch.exp(x)
+output = dna(p, Oi, BATCHSIZE, EPOCH, M, B, input_dim, hidden_dim, output_dim, K_func, C_func, depth)
+print(output)
+
 '''
 beta.data() is used to get the value of beta
 '''
 
 # Path: DNA-SE/package/DNA_SE/DNA_SE.py
```

### Comparing `dna_se-0.0.9/DNA_SE.egg-info/PKG-INFO` & `DNA_SE-0.1.0/DNA_SE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: DNA_SE
-Version: 0.0.9
+Name: DNA-SE
+Version: 0.1.0
 Summary: A small example package
 Home-page: https://github.com/liuqs111/DNA-SE
 Author: Qinshuo
 Author-email: u3008680@connect.hku.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dna_se-0.0.9/LICENSE.txt` & `DNA_SE-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dna_se-0.0.9/PKG-INFO` & `DNA_SE-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DNA_SE
-Version: 0.0.9
+Version: 0.1.0
 Summary: A small example package
 Home-page: https://github.com/liuqs111/DNA-SE
 Author: Qinshuo
 Author-email: u3008680@connect.hku.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dna_se-0.0.9/README.md` & `DNA_SE-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dna_se-0.0.9/setup.py` & `DNA_SE-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DNA_SE", # Replace with your own username
-    version="0.0.9",
+    version="0.1.0",
     author="Qinshuo",
     author_email="u3008680@connect.hku.hk",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liuqs111/DNA-SE",
     packages=setuptools.find_packages(),
```

