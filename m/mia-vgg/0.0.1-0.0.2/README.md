# Comparing `tmp/mia_vgg-0.0.1.tar.gz` & `tmp/mia_vgg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia_vgg-0.0.1.tar", last modified: Fri May 24 09:05:03 2024, max compression
+gzip compressed data, was "mia_vgg-0.0.2.tar", last modified: Fri May 24 10:48:28 2024, max compression
```

## Comparing `mia_vgg-0.0.1.tar` & `mia_vgg-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 09:05:03.322384 mia_vgg-0.0.1/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 09:05:03.322384 mia_vgg-0.0.1/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-24 09:04:49.000000 mia_vgg-0.0.1/pyproject.toml
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-24 09:05:03.322384 mia_vgg-0.0.1/setup.cfg
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 09:05:03.322384 mia_vgg-0.0.1/src/
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 09:05:03.322384 mia_vgg-0.0.1/src/mia_vgg/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.1/src/mia_vgg/__init__.py
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     1974 2024-05-24 09:03:46.000000 mia_vgg-0.0.1/src/mia_vgg/train_target.py
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 09:05:03.322384 mia_vgg-0.0.1/src/mia_vgg.egg-info/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 09:05:03.000000 mia_vgg-0.0.1/src/mia_vgg.egg-info/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-24 09:05:03.000000 mia_vgg-0.0.1/src/mia_vgg.egg-info/SOURCES.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-24 09:05:03.000000 mia_vgg-0.0.1/src/mia_vgg.egg-info/dependency_links.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-24 09:05:03.000000 mia_vgg-0.0.1/src/mia_vgg.egg-info/requires.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-24 09:05:03.000000 mia_vgg-0.0.1/src/mia_vgg.egg-info/top_level.txt
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:48:28.695256 mia_vgg-0.0.2/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 10:48:28.695256 mia_vgg-0.0.2/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-24 10:48:16.000000 mia_vgg-0.0.2/pyproject.toml
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-24 10:48:28.695256 mia_vgg-0.0.2/setup.cfg
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:48:28.695256 mia_vgg-0.0.2/src/
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:48:28.695256 mia_vgg-0.0.2/src/mia_vgg/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.2/src/mia_vgg/__init__.py
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2169 2024-05-24 10:47:30.000000 mia_vgg-0.0.2/src/mia_vgg/train_target.py
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:48:28.695256 mia_vgg-0.0.2/src/mia_vgg.egg-info/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 10:48:28.000000 mia_vgg-0.0.2/src/mia_vgg.egg-info/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-24 10:48:28.000000 mia_vgg-0.0.2/src/mia_vgg.egg-info/SOURCES.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-24 10:48:28.000000 mia_vgg-0.0.2/src/mia_vgg.egg-info/dependency_links.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-24 10:48:28.000000 mia_vgg-0.0.2/src/mia_vgg.egg-info/requires.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-24 10:48:28.000000 mia_vgg-0.0.2/src/mia_vgg.egg-info/top_level.txt
```

### Comparing `mia_vgg-0.0.1/PKG-INFO` & `mia_vgg-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.1
+Version: 0.0.2
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mia_vgg-0.0.1/pyproject.toml` & `mia_vgg-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mia_vgg"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jan Aalmoes", email="jan.aalmoes@protonmail.com" },
 ]
 description = "MIA on VGG dataset using pytorch"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mia_vgg-0.0.1/src/mia_vgg/train_target.py` & `mia_vgg-0.0.2/src/mia_vgg/train_target.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,35 +32,41 @@
 
     num_ftrs = model.classifier[len(model.classifier)-1].in_features
 
     model.classifier[len(model.classifier)-1] = nn.Linear(num_ftrs, 2)
 
     criterion = nn.CrossEntropyLoss()
     optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
+    device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+    model.to(device)
 
     epochs = 10
     for epoch in range(epochs):
         running_loss = 0
         for i,data in enumerate(trainloader):
             optimizer.zero_grad()
             x,y = data
+            x.to(device)
+            y.to(device)
             soft = model(x)
             loss = criterion(soft, y)
             loss.backward()
             optimizer.step()
 
             running_loss += loss.item()
             if i%1==0:
                 print(f"epoch : {epoch}, batch : {i}/{len(trainloader)} - loss: {running_loss/100:.3f}")
                 running_loss = 0
 
     with torch.no_grad():
         correct = 0
         for data in testloader:
             x,y = data
+            x.to(device)
+            y.yo(device)
             soft = model(x)
             _, yhat = torch.max(soft, 1)
             correct += (yhat == y).sum().item()
         print(correct/len(testloader))
         
 if __name__=="__main__":
     train()
```

### Comparing `mia_vgg-0.0.1/src/mia_vgg.egg-info/PKG-INFO` & `mia_vgg-0.0.2/src/mia_vgg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.1
+Version: 0.0.2
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

