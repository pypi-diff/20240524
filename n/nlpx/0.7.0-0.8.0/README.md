# Comparing `tmp/nlpx-0.7.0.tar.gz` & `tmp/nlpx-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-0.7.0.tar", last modified: Fri May 24 01:40:33 2024, max compression
+gzip compressed data, was "nlpx-0.8.0.tar", last modified: Fri May 24 03:18:32 2024, max compression
```

## Comparing `nlpx-0.7.0.tar` & `nlpx-0.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 01:40:33.734597 nlpx-0.7.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 01:40:33.734068 nlpx-0.7.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.7.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 01:40:33.719656 nlpx-0.7.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.7.0/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 01:40:33.733028 nlpx-0.7.0/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-23 12:28:24.000000 nlpx-0.7.0/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2638 2024-05-24 01:39:49.000000 nlpx-0.7.0/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.7.0/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 01:40:33.726037 nlpx-0.7.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 01:40:33.000000 nlpx-0.7.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      243 2024-05-24 01:40:33.000000 nlpx-0.7.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 01:40:33.000000 nlpx-0.7.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 00:26:43.000000 nlpx-0.7.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 01:40:33.000000 nlpx-0.7.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 01:40:33.734848 nlpx-0.7.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 01:40:31.000000 nlpx-0.7.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:18:32.921223 nlpx-0.8.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 03:18:32.920579 nlpx-0.8.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.8.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:18:32.909251 nlpx-0.8.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.8.0/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:18:32.918135 nlpx-0.8.0/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-23 12:28:24.000000 nlpx-0.8.0/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2639 2024-05-24 03:18:24.000000 nlpx-0.8.0/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.8.0/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 03:18:32.915513 nlpx-0.8.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 03:18:32.000000 nlpx-0.8.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      243 2024-05-24 03:18:32.000000 nlpx-0.8.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 03:18:32.000000 nlpx-0.8.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 00:26:43.000000 nlpx-0.8.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 03:18:32.000000 nlpx-0.8.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 03:18:32.921502 nlpx-0.8.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 03:18:24.000000 nlpx-0.8.0/setup.py
```

### Comparing `nlpx-0.7.0/PKG-INFO` & `nlpx-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.7.0
+Version: 0.8.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.7.0/nlpx/models/_text_cnn.py` & `nlpx-0.8.0/nlpx/models/_text_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from torch import nn
 from torch.nn import functional as F
 
 
 class TextCNN(nn.Module):
 
     def __init__(self, word_dim: int, kernel_sizes=(2, 3, 4), cnn_channels=64, out_features=2,
-                 activation=nn.ReLU(inplace=True), num_hidden_layer=0, drop_out=0):
+                 activation=nn.ReLU6(inplace=True), num_hidden_layer=0, drop_out=0):
         """ TextCNN model
         Parameters
         ----------
         word_dim: int, dim of word, in_channels of cnn
         cnn_channels: int, out_channels of cnn
         kernel_sizes: size of each cnn kernel
         out_features: dim of output
```

### Comparing `nlpx-0.7.0/nlpx/text_token.py` & `nlpx-0.8.0/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.7.0/nlpx.egg-info/PKG-INFO` & `nlpx-0.8.0/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.7.0
+Version: 0.8.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.7.0/setup.py` & `nlpx-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.7.0',
+    version='0.8.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

