# Comparing `tmp/nlpx-1.0.1.tar.gz` & `tmp/nlpx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.0.1.tar", last modified: Fri May 24 04:05:24 2024, max compression
+gzip compressed data, was "nlpx-1.0.2.tar", last modified: Fri May 24 04:22:21 2024, max compression
```

## Comparing `nlpx-1.0.1.tar` & `nlpx-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:05:24.094104 nlpx-1.0.1/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:05:24.093423 nlpx-1.0.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.1/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:05:24.079415 nlpx-1.0.1/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.1/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:05:24.091709 nlpx-1.0.1/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.1/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2639 2024-05-24 03:18:24.000000 nlpx-1.0.1/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)     3666 2024-05-24 04:05:18.000000 nlpx-1.0.1/nlpx/models/_trainer.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.1/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:05:24.086858 nlpx-1.0.1/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 04:05:23.000000 nlpx-1.0.1/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 04:05:24.094374 nlpx-1.0.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 04:05:18.000000 nlpx-1.0.1/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:22:21.243903 nlpx-1.0.2/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:22:21.243080 nlpx-1.0.2/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.2/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:22:21.226641 nlpx-1.0.2/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.2/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:22:21.242243 nlpx-1.0.2/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.2/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2639 2024-05-24 03:18:24.000000 nlpx-1.0.2/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)     3698 2024-05-24 04:22:17.000000 nlpx-1.0.2/nlpx/models/_trainer.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.2/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:22:21.238519 nlpx-1.0.2/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:22:21.000000 nlpx-1.0.2/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 04:22:21.000000 nlpx-1.0.2/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:22:21.000000 nlpx-1.0.2/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.2/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 04:22:21.000000 nlpx-1.0.2/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 04:22:21.244190 nlpx-1.0.2/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 04:22:17.000000 nlpx-1.0.2/setup.py
```

### Comparing `nlpx-1.0.1/PKG-INFO` & `nlpx-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.0.1/nlpx/models/_text_cnn.py` & `nlpx-1.0.2/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.1/nlpx/models/_trainer.py` & `nlpx-1.0.2/nlpx/models/_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 				scheduler.step()
 
 				losses += loss.item()
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
 			val_loss, val_acc = self.eval()
-			print('epoch-{}/{}  train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
-				epoch + 1, self.max_iter, losses / total, correct / total, val_loss, val_acc
+			print('epoch-{}/{}  train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}, lr: {:.4f}'.format(
+				epoch + 1, self.max_iter, losses / total, correct / total, val_loss, val_acc, scheduler.get_lr()
 			))
 			if epoch > 5 and val_acc > best_acc:
 				best_acc = val_acc
 				best_model = self.model
 
 			if val_acc >= best_acc:  # val_acc提升
 				cnt = 0
```

### Comparing `nlpx-1.0.1/nlpx/text_token.py` & `nlpx-1.0.2/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.1/nlpx.egg-info/PKG-INFO` & `nlpx-1.0.2/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.0.1/setup.py` & `nlpx-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.1',
+    version='1.0.2',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

