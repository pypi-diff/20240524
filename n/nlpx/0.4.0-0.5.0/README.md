# Comparing `tmp/nlpx-0.4.0.tar.gz` & `tmp/nlpx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-0.4.0.tar", last modified: Thu May 23 12:32:15 2024, max compression
+gzip compressed data, was "nlpx-0.5.0.tar", last modified: Thu May 23 12:45:21 2024, max compression
```

## Comparing `nlpx-0.4.0.tar` & `nlpx-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 12:32:15.000938 nlpx-0.4.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 12:32:15.000068 nlpx-0.4.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.4.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 12:32:14.990915 nlpx-0.4.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.4.0/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 12:32:14.998820 nlpx-0.4.0/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-23 12:28:24.000000 nlpx-0.4.0/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2751 2024-05-23 12:31:28.000000 nlpx-0.4.0/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.4.0/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 12:32:14.996893 nlpx-0.4.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 12:32:14.000000 nlpx-0.4.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      243 2024-05-23 12:32:14.000000 nlpx-0.4.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 12:32:14.000000 nlpx-0.4.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 12:32:14.000000 nlpx-0.4.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-23 12:32:14.000000 nlpx-0.4.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-23 12:32:15.001234 nlpx-0.4.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-23 12:32:08.000000 nlpx-0.4.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 12:45:21.716466 nlpx-0.5.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 12:45:21.715053 nlpx-0.5.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.5.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 12:45:21.703269 nlpx-0.5.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.5.0/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 12:45:21.713931 nlpx-0.5.0/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-23 12:28:24.000000 nlpx-0.5.0/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2488 2024-05-23 12:43:26.000000 nlpx-0.5.0/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.5.0/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 12:45:21.710468 nlpx-0.5.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 12:45:21.000000 nlpx-0.5.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      243 2024-05-23 12:45:21.000000 nlpx-0.5.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 12:45:21.000000 nlpx-0.5.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 12:45:21.000000 nlpx-0.5.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-23 12:45:21.000000 nlpx-0.5.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-23 12:45:21.716846 nlpx-0.5.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1013 2024-05-23 12:45:16.000000 nlpx-0.5.0/setup.py
```

### Comparing `nlpx-0.4.0/PKG-INFO` & `nlpx-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.4.0
+Version: 0.5.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.4.0/nlpx/models/_text_cnn.py` & `nlpx-0.5.0/nlpx/models/_text_cnn.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,45 +30,41 @@
         self.convs = nn.ModuleList([
             nn.Sequential(
                 nn.Conv1d(in_channels=word_dim, out_channels=cnn_channels, kernel_size=kernel_size, bias=False),
                 nn.ReLU6(inplace=True),  # inplace为True，将会改变输入的数据 ，否则不会改变原输入，只会产生新的输出
                 nn.AdaptiveMaxPool1d(1)
             ) for kernel_size in kernel_sizes
         ])
-        self.num_hidden_layer = num_hidden_layer
+
         num_features = cnn_channels * len(kernel_sizes)
-        if num_hidden_layer:
-            self.hidden_layers = nn.ModuleList([
-                nn.Sequential(
-                    nn.Linear(in_features=num_features, out_features=num_features, bias=False),
-                    nn.LayerNorm(normalized_shape=num_features),
-                    nn.ReLU6(inplace=True)
-                ) for _ in range(num_hidden_layer)
-            ])
+        self.fc = nn.ModuleList([
+            nn.Sequential(
+                nn.Linear(in_features=num_features, out_features=num_features, bias=False),
+                nn.LayerNorm(normalized_shape=num_features),
+                nn.ReLU6(inplace=True)
+            ) for _ in range(num_hidden_layer)
+        ])
 
-        self.classifier = nn.Linear(in_features=num_features, out_features=out_features)
-        self.dropout = nn.Dropout(drop_out) if drop_out else None
+        if drop_out:
+            self.fc.append(nn.Dropout(drop_out))
+
+        self.fc.append(nn.Linear(in_features=num_features, out_features=out_features))
 
     def forward(self, inputs, labels=None):
         """
         :param inputs: [(batch, sentence, word_dim)]
         :param labels: [long]
         """
         input_embeddings = inputs.transpose(2, 1)
         out = torch.cat([conv(input_embeddings) for conv in self.convs], dim=1)
         out = out.transpose(2, 1)
 
-        if self.num_hidden_layer:
-            for hidden_layer in self.hidden_layers:
-                out = hidden_layer(out)
-
-        if self.dropout:
-            out = self.dropout(out)
+        for hidden_layer in self.fc:
+            out = hidden_layer(out)
 
-        out = self.classifier(out)
         logits = out.squeeze(1)
 
         if labels is None:
             return logits
         else:
             loss = F.cross_entropy(logits, labels)
             return loss, logits
```

### Comparing `nlpx-0.4.0/nlpx/text_token.py` & `nlpx-0.5.0/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.4.0/nlpx.egg-info/PKG-INFO` & `nlpx-0.5.0/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.4.0
+Version: 0.5.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.4.0/setup.py` & `nlpx-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.4.0',
+    version='0.5.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

