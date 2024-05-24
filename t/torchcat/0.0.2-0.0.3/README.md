# Comparing `tmp/torchcat-0.0.2.tar.gz` & `tmp/torchcat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchcat-0.0.2.tar", last modified: Wed May 22 13:40:24 2024, max compression
+gzip compressed data, was "torchcat-0.0.3.tar", last modified: Fri May 24 02:52:32 2024, max compression
```

## Comparing `torchcat-0.0.2.tar` & `torchcat-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:40:24.471046 torchcat-0.0.2/
--rw-rw-rw-   0        0        0    17765 2024-05-21 13:29:45.000000 torchcat-0.0.2/License
--rw-rw-rw-   0        0        0      278 2024-05-22 13:40:24.468394 torchcat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-05-21 13:35:58.000000 torchcat-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 13:40:24.471046 torchcat-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      415 2024-05-22 13:39:51.000000 torchcat-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:40:24.462389 torchcat-0.0.2/torchcat/
--rw-rw-rw-   0        0        0     1978 2024-05-22 13:30:42.000000 torchcat-0.0.2/torchcat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:40:24.468394 torchcat-0.0.2/torchcat.egg-info/
--rw-rw-rw-   0        0        0      278 2024-05-22 13:40:24.000000 torchcat-0.0.2/torchcat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2024-05-22 13:40:24.000000 torchcat-0.0.2/torchcat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:40:24.000000 torchcat-0.0.2/torchcat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 13:40:24.000000 torchcat-0.0.2/torchcat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-22 13:40:24.000000 torchcat-0.0.2/torchcat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 02:52:32.213183 torchcat-0.0.3/
+-rw-rw-rw-   0        0        0    17765 2024-05-21 13:29:45.000000 torchcat-0.0.3/License
+-rw-rw-rw-   0        0        0      285 2024-05-24 02:52:32.213183 torchcat-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2024-05-21 13:35:58.000000 torchcat-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 02:52:32.213183 torchcat-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      528 2024-05-24 02:51:40.000000 torchcat-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 02:52:32.206206 torchcat-0.0.3/torchcat/
+-rw-rw-rw-   0        0        0     2242 2024-05-23 10:04:24.000000 torchcat-0.0.3/torchcat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 02:52:32.212186 torchcat-0.0.3/torchcat.egg-info/
+-rw-rw-rw-   0        0        0      285 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 02:52:32.000000 torchcat-0.0.3/torchcat.egg-info/top_level.txt
```

### Comparing `torchcat-0.0.2/License` & `torchcat-0.0.3/License`

 * *Files identical despite different names*

### Comparing `torchcat-0.0.2/torchcat/__init__.py` & `torchcat-0.0.3/torchcat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import numpy as np
 from torchsummary import summary
 
 
 class Cat:
     def __init__(self, model, loss_fn=None, optimizer=None):
-        # 模型、损失函数、优化器、GPU 标志
+        # 训练日志、模型、损失函数、优化器、GPU 标志
         self.model = model
         self.loss_fn = loss_fn
         self.optimizer = optimizer
         self.GPU_FLAG = str(next(model[0].parameters()).device)
+        self.log = {'train loss': [], 'train acc': [], 'valid loss': [], 'valid acc': []}
+
         if (loss_fn and optimizer) is None:
-            print('未检测到损失函数或优化器，别担心，这并不影响你炼丹🙂')
+            print('未检测到损失函数或优化器，这将会影响到你的模型训练🙂')
 
     # 训练
     def train(self, train_set, epochs):
-        if not self.model.training:
-            self.model.train()
+        self.model.train()
         for epoch in range(1, epochs+1):
             loss_temp = []  # 储存一个批次内的损失值
             for x, y in train_set:
                 self.optimizer.zero_grad()
                 pred = self.model(x)
                 loss = self.loss_fn(pred, y)
                 loss_temp.append(loss.item())
                 loss.backward()
                 self.optimizer.step()
-            print(f'Epoch {epoch}/{epochs} Loss: {np.mean(loss_temp):.6f}')
+            loss_mean = np.mean(loss_temp)
+            # 记录、输出训练日志
+            self.log['train loss'].append(loss_mean)
+            print(f'Epoch {epoch}/{epochs} Loss: {loss_mean:.6f}')
 
     # 验证
     def valid(self, valid_set):
-        if self.model.training:
-            self.model.eval()
+        self.model.eval()
         acc_temp = []       # 储存一个批次内的准确率、损失值
         loss_temp = []
         for x, y in valid_set:
             pred = self.model(x)
             loss_temp.append(self.loss_fn(pred, y).item())  # 计算验证集 loss
             acc_temp.append(np.mean(pred.detach().numpy().argmax(-1) == y))  # 计算验证集 accuracy
         print(f'Loss: {np.mean(loss_temp):.6f}')
@@ -45,9 +48,15 @@
         # 判断GPU是否可用
         if self.GPU_FLAG == 'cpu':
             device = 'cpu'
         else:
             device = 'cuda'
         summary(self.model, input_size, device=device)
 
+    def train(self):
+        self.model.train()
+
+    def eval(self):
+        self.model.eval()
+
     def __call__(self, x):
         return self.model(x)
```

