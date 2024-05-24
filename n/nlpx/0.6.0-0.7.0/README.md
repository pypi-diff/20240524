# Comparing `tmp/nlpx-0.6.0.tar.gz` & `tmp/nlpx-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-0.6.0.tar", last modified: Fri May 24 00:27:06 2024, max compression
+gzip compressed data, was "nlpx-0.7.0.tar", last modified: Fri May 24 01:40:33 2024, max compression
```

## Comparing `nlpx-0.6.0.tar` & `nlpx-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 00:27:06.725838 nlpx-0.6.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 00:27:06.725123 nlpx-0.6.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.6.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 00:27:06.714302 nlpx-0.6.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.6.0/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 00:27:06.724050 nlpx-0.6.0/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-23 12:28:24.000000 nlpx-0.6.0/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2560 2024-05-24 00:26:05.000000 nlpx-0.6.0/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.6.0/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 00:27:06.719804 nlpx-0.6.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 00:27:06.000000 nlpx-0.6.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      243 2024-05-24 00:27:06.000000 nlpx-0.6.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 00:27:06.000000 nlpx-0.6.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 00:26:43.000000 nlpx-0.6.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 00:27:06.000000 nlpx-0.6.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 00:27:06.726105 nlpx-0.6.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 00:26:54.000000 nlpx-0.6.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 01:40:33.734597 nlpx-0.7.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 01:40:33.734068 nlpx-0.7.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.7.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 01:40:33.719656 nlpx-0.7.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.7.0/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 01:40:33.733028 nlpx-0.7.0/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-23 12:28:24.000000 nlpx-0.7.0/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2638 2024-05-24 01:39:49.000000 nlpx-0.7.0/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.7.0/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-24 01:40:33.726037 nlpx-0.7.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-24 01:40:33.000000 nlpx-0.7.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      243 2024-05-24 01:40:33.000000 nlpx-0.7.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 01:40:33.000000 nlpx-0.7.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-24 00:26:43.000000 nlpx-0.7.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-24 01:40:33.000000 nlpx-0.7.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-24 01:40:33.734848 nlpx-0.7.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-24 01:40:31.000000 nlpx-0.7.0/setup.py
```

### Comparing `nlpx-0.6.0/PKG-INFO` & `nlpx-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.6.0
+Version: 0.7.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.6.0/nlpx/models/_text_cnn.py` & `nlpx-0.7.0/nlpx/models/_text_cnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,45 +28,48 @@
         >>> output = model(X)
         >>> loss, output = model(X, targets)
         """
         super().__init__()
         self.convs = nn.ModuleList([
             nn.Sequential(
                 nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
-                activation(inplace=True),  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
+                activation,  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
                 nn.AdaptiveMaxPool1d(1)
             ) for kernel_size in kernel_sizes
         ])
 
         num_features = cnn_channels * len(kernel_sizes)
-        self.fc = nn.ModuleList([
+        self.hidden_layers = nn.ModuleList([
             nn.Sequential(
                 nn.Linear(in_features=num_features, out_features=num_features, bias=False),
                 nn.LayerNorm(normalized_shape=num_features),
-                activation(inplace=True)
+                activation
             ) for _ in range(num_hidden_layer)
         ])
 
+        self.fc = nn.Linear(in_features=num_features, out_features=out_features)
         if drop_out:
-            self.fc.append(nn.Dropout(drop_out))
-
-        self.fc.append(nn.Linear(in_features=num_features, out_features=out_features))
+            self.fc = nn.Sequential(
+                nn.Dropout(drop_out),
+                self.fc
+            )
 
     def forward(self, inputs, labels=None):
         """
         :param inputs: [(batch, sentence, word_dim)]
         :param labels: [long]
         """
         input_embeddings = inputs.transpose(2, 1)
         out = torch.cat([conv(input_embeddings) for conv in self.convs], dim=1)
         out = out.transpose(2, 1)
 
-        for hidden_layer in self.fc:
+        for hidden_layer in self.hidden_layers:
             out = hidden_layer(out)
 
+        out = self.fc(out)
         logits = out.squeeze(1)
 
         if labels is None:
             return logits
         else:
             loss = F.cross_entropy(logits, labels)
             return loss, logits
```

### Comparing `nlpx-0.6.0/nlpx/text_token.py` & `nlpx-0.7.0/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.6.0/nlpx.egg-info/PKG-INFO` & `nlpx-0.7.0/nlpx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.6.0
+Version: 0.7.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.6.0/setup.py` & `nlpx-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.6.0',
+    version='0.7.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

