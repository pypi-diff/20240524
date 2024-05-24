# Comparing `tmp/nlpx-1.0.4.tar.gz` & `tmp/nlpx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.0.4.tar", last modified: Fri May 24 04:35:12 2024, max compression
+gzip compressed data, was "nlpx-1.0.5.tar", last modified: Fri May 24 04:57:56 2024, max compression
```

## Comparing `nlpx-1.0.4.tar` & `nlpx-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:35:12.147931 nlpx-1.0.4/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:35:12.147205 nlpx-1.0.4/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.4/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:35:12.129420 nlpx-1.0.4/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.4/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:35:12.146025 nlpx-1.0.4/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.4/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2638 2024-05-24 04:23:40.000000 nlpx-1.0.4/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)     3716 2024-05-24 04:35:08.000000 nlpx-1.0.4/nlpx/models/_trainer.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.4/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:35:12.138866 nlpx-1.0.4/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:35:11.000000 nlpx-1.0.4/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 04:35:11.000000 nlpx-1.0.4/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:35:11.000000 nlpx-1.0.4/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.4/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 04:35:11.000000 nlpx-1.0.4/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 04:35:12.148218 nlpx-1.0.4/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 04:35:08.000000 nlpx-1.0.4/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:57:56.316197 nlpx-1.0.5/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:57:56.314778 nlpx-1.0.5/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.5/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:57:56.303394 nlpx-1.0.5/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.5/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:57:56.313691 nlpx-1.0.5/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.5/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2638 2024-05-24 04:23:40.000000 nlpx-1.0.5/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)     3716 2024-05-24 04:57:51.000000 nlpx-1.0.5/nlpx/models/_trainer.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.5/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:57:56.309054 nlpx-1.0.5/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:57:56.000000 nlpx-1.0.5/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 04:57:56.000000 nlpx-1.0.5/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:57:56.000000 nlpx-1.0.5/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.5/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 04:57:56.000000 nlpx-1.0.5/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 04:57:56.317999 nlpx-1.0.5/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 04:57:51.000000 nlpx-1.0.5/setup.py
```

### Comparing `nlpx-1.0.4/PKG-INFO` & `nlpx-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.0.4/nlpx/models/_text_cnn.py` & `nlpx-1.0.5/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.4/nlpx/models/_trainer.py` & `nlpx-1.0.5/nlpx/models/_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 				scheduler.step()
 
 				losses += loss.item()
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
 			val_loss, val_acc = self.eval()
-			print('epoch-{}/{}  train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}, lr: {:.4f}'.format(
+			print('epoch-{}/{}  train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}, lr: {:.8f}'.format(
 				epoch + 1, self.max_iter, losses / total, correct / total, val_loss, val_acc, self.optimizer.param_groups[0]['lr']
 			))
 			if epoch > 5 and val_acc > best_acc:
 				best_acc = val_acc
 				best_model = self.model
 
 			if val_acc >= best_acc:  # val_acc提升
```

### Comparing `nlpx-1.0.4/nlpx/text_token.py` & `nlpx-1.0.5/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.4/nlpx.egg-info/PKG-INFO` & `nlpx-1.0.5/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.0.4/setup.py` & `nlpx-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.4',
+    version='1.0.5',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

