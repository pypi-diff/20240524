# Comparing `tmp/nlpx-1.0.9.tar.gz` & `tmp/nlpx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.0.9.tar", last modified: Fri May 24 06:07:22 2024, max compression
+gzip compressed data, was "nlpx-1.1.0.tar", last modified: Fri May 24 06:10:30 2024, max compression
```

## Comparing `nlpx-1.0.9.tar` & `nlpx-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:07:22.573403 nlpx-1.0.9/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 06:07:22.572321 nlpx-1.0.9/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.9/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:07:22.557758 nlpx-1.0.9/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.9/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:07:22.570839 nlpx-1.0.9/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.9/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2638 2024-05-24 04:23:40.000000 nlpx-1.0.9/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)     3769 2024-05-24 06:07:07.000000 nlpx-1.0.9/nlpx/models/_trainer.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.9/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:07:22.566349 nlpx-1.0.9/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 06:07:22.000000 nlpx-1.0.9/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 06:07:22.000000 nlpx-1.0.9/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 06:07:22.000000 nlpx-1.0.9/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.9/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 06:07:22.000000 nlpx-1.0.9/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 06:07:22.573681 nlpx-1.0.9/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 06:07:13.000000 nlpx-1.0.9/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:10:30.812320 nlpx-1.1.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 06:10:30.811585 nlpx-1.1.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:10:30.800556 nlpx-1.1.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.0/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:10:30.810844 nlpx-1.1.0/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.1.0/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2638 2024-05-24 04:23:40.000000 nlpx-1.1.0/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)     3811 2024-05-24 06:10:27.000000 nlpx-1.1.0/nlpx/models/_trainer.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.1.0/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 06:10:30.806826 nlpx-1.1.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 06:10:30.000000 nlpx-1.1.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 06:10:30.000000 nlpx-1.1.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 06:10:30.000000 nlpx-1.1.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.1.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 06:10:30.000000 nlpx-1.1.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 06:10:30.812563 nlpx-1.1.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 06:10:27.000000 nlpx-1.1.0/setup.py
```

### Comparing `nlpx-1.0.9/PKG-INFO` & `nlpx-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.0.9
+Version: 1.1.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.0.9/nlpx/models/_text_cnn.py` & `nlpx-1.1.0/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.9/nlpx/models/_trainer.py` & `nlpx-1.1.0/nlpx/models/_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from torch.optim.lr_scheduler import CosineAnnealingLR
 from sklearn.model_selection import train_test_split
 
 
 class Trainer:
 
 	def __init__(self, model, train_set, eval_set, collate_fn=None,
-				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max=10,
+				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max=None,
 				 batch_size=8, eval_batch_size=16,
 				 num_workers=4, num_eval_workers=2,
 				 early_stopping_rounds=10,  # 早停，等10轮决策，评价指标不在变化，停止
 				 device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
 		self.model = model.to(device)
 		self.train_loader = DataLoader(dataset=train_set, batch_size=batch_size,
 									   num_workers=num_workers, shuffle=True, collate_fn=collate_fn)
@@ -26,27 +26,29 @@
 
 	def train(self):
 		cnt = 0
 		cnt2 = 0
 		best_acc = 0.0
 		last_acc = 0.0
 		best_model = None
-		scheduler = CosineAnnealingLR(self.optimizer, T_max=self.T_max)
+		if self.T_max:
+			scheduler = CosineAnnealingLR(self.optimizer, T_max=self.T_max)
 		for epoch in range(self.max_iter):
 			total = 0.0
 			losses = 0.0
 			correct = 0.0
 			self.model.train()
 			for x, y in self.train_loader:
 				x, y = x.to(self.device), y.to(self.device)
 				loss, logits = self.model(x, y)
 				self.optimizer.zero_grad()
 				loss.backward()
 				self.optimizer.step()
-				scheduler.step()
+				if self.T_max:
+					scheduler.step()
 
 				losses += loss.item()
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
 			val_loss, val_acc = self.eval()
 			print('epoch-{}/{}  lr: {:.6f}, train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
@@ -87,15 +89,15 @@
 				total += len(y)
 		return losses / total, correct / total
 
 
 class SimpleTrainer(Trainer):
 
 	def __init__(self, model, X, y, eval_size=0.2, random_state=None, collate_fn=None,
-				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max=10,
+				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max=None,
 				 batch_size=8, eval_batch_size=16,
 				 num_workers=4, num_eval_workers=2,
 				 early_stopping_rounds=10,  # 早停，等10轮决策，评价指标不在变化，停止
 				 device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
 		X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=eval_size, random_state=random_state)
 		super().__init__(model,
 						 TensorDataset(X_train, y_train),
```

### Comparing `nlpx-1.0.9/nlpx/text_token.py` & `nlpx-1.1.0/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.9/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.0/nlpx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.0.9
+Version: 1.1.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.0.9/setup.py` & `nlpx-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.9',
+    version='1.1.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

