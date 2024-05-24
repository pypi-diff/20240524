# Comparing `tmp/nlpx-1.0.0.tar.gz` & `tmp/nlpx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.0.0.tar", last modified: Fri May 24 03:33:32 2024, max compression
+gzip compressed data, was "nlpx-1.0.1.tar", last modified: Fri May 24 04:05:24 2024, max compression
```

## Comparing `nlpx-1.0.0.tar` & `nlpx-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:33:32.793537 nlpx-1.0.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 03:33:32.792742 nlpx-1.0.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:33:32.783513 nlpx-1.0.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.0/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:33:32.791689 nlpx-1.0.0/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.0/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2639 2024-05-24 03:18:24.000000 nlpx-1.0.0/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)     3681 2024-05-24 03:25:51.000000 nlpx-1.0.0/nlpx/models/_trainer.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.0/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:33:32.788964 nlpx-1.0.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 03:33:32.000000 nlpx-1.0.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 03:33:32.000000 nlpx-1.0.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 03:33:32.000000 nlpx-1.0.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 03:26:25.000000 nlpx-1.0.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 03:33:32.000000 nlpx-1.0.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 03:33:32.793789 nlpx-1.0.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 03:33:23.000000 nlpx-1.0.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:05:24.094104 nlpx-1.0.1/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:05:24.093423 nlpx-1.0.1/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.1/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:05:24.079415 nlpx-1.0.1/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.1/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:05:24.091709 nlpx-1.0.1/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.1/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2639 2024-05-24 03:18:24.000000 nlpx-1.0.1/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)     3666 2024-05-24 04:05:18.000000 nlpx-1.0.1/nlpx/models/_trainer.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.1/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:05:24.086858 nlpx-1.0.1/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 04:05:24.094374 nlpx-1.0.1/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 04:05:18.000000 nlpx-1.0.1/setup.py
```

### Comparing `nlpx-1.0.0/nlpx/models/_text_cnn.py` & `nlpx-1.0.1/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.0/nlpx/models/_trainer.py` & `nlpx-1.0.1/nlpx/models/_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 	def __init__(self, model, train_set, eval_set, collate_fn=None,
 				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001,
 				 batch_size=8, eval_batch_size=16,
 				 num_workers=4, num_eval_workers=2,
 				 early_stopping_rounds=10,  # 早停，等10轮决策，评价指标不在变化，停止
 				 device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
-		self.model = model.to(self.device)
+		self.model = model.to(device)
 		self.train_loader = DataLoader(dataset=train_set, batch_size=batch_size,
 									   num_workers=num_workers, shuffle=True, collate_fn=collate_fn)
 		self.eval_loader = DataLoader(dataset=eval_set, batch_size=eval_batch_size,
 									  num_workers=num_eval_workers, collate_fn=collate_fn)
 		self.max_iter = max_iter
 		self.optimizer = optimizer(model.parameters(), lr=learning_rate)
 		self.early_stopping_rounds = early_stopping_rounds
@@ -66,15 +66,15 @@
 			last_acc = val_acc
 			cnt += 1
 			if epoch > 5 and (
 					cnt > self.early_stopping_rounds or cnt2 > self.early_stopping_rounds):  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
 				print("Early stopping at epoch-{}/{}".format(epoch + 1, self.max_iter))
 				break
 
-		return best_model, best_acc
+		return best_model
 
 	def eval(self):
 		total = 0.0
 		losses = 0.0
 		correct = 0.0
 		self.model.eval()
 		with torch.no_grad():
```

### Comparing `nlpx-1.0.0/nlpx/text_token.py` & `nlpx-1.0.1/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.0/setup.py` & `nlpx-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.0',
+    version='1.0.1',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

