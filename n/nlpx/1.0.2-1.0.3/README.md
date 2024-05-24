# Comparing `tmp/nlpx-1.0.2.tar.gz` & `tmp/nlpx-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.0.2.tar", last modified: Fri May 24 04:22:21 2024, max compression
+gzip compressed data, was "nlpx-1.0.3.tar", last modified: Fri May 24 04:23:56 2024, max compression
```

## Comparing `nlpx-1.0.2.tar` & `nlpx-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:22:21.243903 nlpx-1.0.2/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:22:21.243080 nlpx-1.0.2/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.2/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:22:21.226641 nlpx-1.0.2/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.2/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:22:21.242243 nlpx-1.0.2/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.2/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2639 2024-05-24 03:18:24.000000 nlpx-1.0.2/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)     3698 2024-05-24 04:22:17.000000 nlpx-1.0.2/nlpx/models/_trainer.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.2/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:22:21.238519 nlpx-1.0.2/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:22:21.000000 nlpx-1.0.2/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 04:22:21.000000 nlpx-1.0.2/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:22:21.000000 nlpx-1.0.2/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.2/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 04:22:21.000000 nlpx-1.0.2/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 04:22:21.244190 nlpx-1.0.2/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 04:22:17.000000 nlpx-1.0.2/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:23:56.321544 nlpx-1.0.3/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:23:56.320828 nlpx-1.0.3/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.0.3/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:23:56.312083 nlpx-1.0.3/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.0.3/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:23:56.319763 nlpx-1.0.3/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       76 2024-05-24 03:33:06.000000 nlpx-1.0.3/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2638 2024-05-24 04:23:40.000000 nlpx-1.0.3/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)     3698 2024-05-24 04:22:17.000000 nlpx-1.0.3/nlpx/models/_trainer.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.0.3/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 04:23:56.317150 nlpx-1.0.3/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 04:23:56.000000 nlpx-1.0.3/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      267 2024-05-24 04:23:56.000000 nlpx-1.0.3/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:23:56.000000 nlpx-1.0.3/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 04:05:23.000000 nlpx-1.0.3/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 04:23:56.000000 nlpx-1.0.3/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 04:23:56.321862 nlpx-1.0.3/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 04:23:53.000000 nlpx-1.0.3/setup.py
```

### Comparing `nlpx-1.0.2/PKG-INFO` & `nlpx-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.0.2/nlpx/models/_text_cnn.py` & `nlpx-1.0.3/nlpx/models/_text_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from torch import nn
 from torch.nn import functional as F
 
 
 class TextCNN(nn.Module):
 
     def __init__(self, word_dim: int, kernel_sizes=(2, 3, 4), cnn_channels=64, out_features=2,
-                 activation=nn.ReLU6(inplace=True), num_hidden_layer=0, drop_out=0):
+                 activation=nn.ReLU(inplace=True), num_hidden_layer=0, drop_out=0):
         """ TextCNN model
         Parameters
         ----------
         word_dim: int, dim of word, in_channels of cnn
         cnn_channels: int, out_channels of cnn
         kernel_sizes: size of each cnn kernel
         out_features: dim of output
```

### Comparing `nlpx-1.0.2/nlpx/models/_trainer.py` & `nlpx-1.0.3/nlpx/models/_trainer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.2/nlpx/text_token.py` & `nlpx-1.0.3/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.0.2/nlpx.egg-info/PKG-INFO` & `nlpx-1.0.3/nlpx.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.0.2/setup.py` & `nlpx-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.2',
+    version='1.0.3',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

