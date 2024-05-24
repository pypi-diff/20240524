# Comparing `tmp/mia_vgg-0.0.5.tar.gz` & `tmp/mia_vgg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia_vgg-0.0.5.tar", last modified: Fri May 24 11:01:00 2024, max compression
+gzip compressed data, was "mia_vgg-0.0.6.tar", last modified: Fri May 24 11:09:11 2024, max compression
```

## Comparing `mia_vgg-0.0.5.tar` & `mia_vgg-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:01:00.208533 mia_vgg-0.0.5/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 11:01:00.208533 mia_vgg-0.0.5/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-24 11:00:52.000000 mia_vgg-0.0.5/pyproject.toml
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-24 11:01:00.208533 mia_vgg-0.0.5/setup.cfg
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:01:00.208533 mia_vgg-0.0.5/src/
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:01:00.208533 mia_vgg-0.0.5/src/mia_vgg/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.5/src/mia_vgg/__init__.py
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2185 2024-05-24 11:00:44.000000 mia_vgg-0.0.5/src/mia_vgg/train_target.py
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:01:00.208533 mia_vgg-0.0.5/src/mia_vgg.egg-info/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 11:01:00.000000 mia_vgg-0.0.5/src/mia_vgg.egg-info/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-24 11:01:00.000000 mia_vgg-0.0.5/src/mia_vgg.egg-info/SOURCES.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-24 11:01:00.000000 mia_vgg-0.0.5/src/mia_vgg.egg-info/dependency_links.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-24 11:01:00.000000 mia_vgg-0.0.5/src/mia_vgg.egg-info/requires.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-24 11:01:00.000000 mia_vgg-0.0.5/src/mia_vgg.egg-info/top_level.txt
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:09:11.731830 mia_vgg-0.0.6/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 11:09:11.731830 mia_vgg-0.0.6/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-24 11:09:02.000000 mia_vgg-0.0.6/pyproject.toml
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-24 11:09:11.731830 mia_vgg-0.0.6/setup.cfg
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:09:11.731830 mia_vgg-0.0.6/src/
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:09:11.731830 mia_vgg-0.0.6/src/mia_vgg/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.6/src/mia_vgg/__init__.py
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2228 2024-05-24 11:08:52.000000 mia_vgg-0.0.6/src/mia_vgg/train_target.py
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 11:09:11.731830 mia_vgg-0.0.6/src/mia_vgg.egg-info/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 11:09:11.000000 mia_vgg-0.0.6/src/mia_vgg.egg-info/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-24 11:09:11.000000 mia_vgg-0.0.6/src/mia_vgg.egg-info/SOURCES.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-24 11:09:11.000000 mia_vgg-0.0.6/src/mia_vgg.egg-info/dependency_links.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-24 11:09:11.000000 mia_vgg-0.0.6/src/mia_vgg.egg-info/requires.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-24 11:09:11.000000 mia_vgg-0.0.6/src/mia_vgg.egg-info/top_level.txt
```

### Comparing `mia_vgg-0.0.5/PKG-INFO` & `mia_vgg-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.5
+Version: 0.0.6
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mia_vgg-0.0.5/pyproject.toml` & `mia_vgg-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mia_vgg"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Jan Aalmoes", email="jan.aalmoes@protonmail.com" },
 ]
 description = "MIA on VGG dataset using pytorch"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mia_vgg-0.0.5/src/mia_vgg/train_target.py` & `mia_vgg-0.0.6/src/mia_vgg/train_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,30 +20,30 @@
     """Train VGG16."""
     transform = v2.Compose([PILToTensor(),
                            v2.ToDtype(torch.float32, scale=True)])
     celeba = datasets.CelebA(root="data", download=True, target_transform=trgtsf, transform=transform)
     x = celeba[0][0]
 
     train, test = random_split(celeba, [0.8,0.2])
-    trainloader = DataLoader(train, batch_size=100)
+    trainloader = DataLoader(train, batch_size=101)
     testloader = DataLoader(test)
 
     weights = models.VGG16_Weights
     model = models.vgg16(weights=weights)
 
     num_ftrs = model.classifier[len(model.classifier)-1].in_features
 
     model.classifier[len(model.classifier)-1] = nn.Linear(num_ftrs, 2)
 
     criterion = nn.CrossEntropyLoss()
     optimizer = optim.SGD(model.parameters(), lr=0.001, momentum=0.9)
     device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
     model.to(device)
 
-    epochs = 10
+    epochs = 1
     for epoch in range(epochs):
         running_loss = 0
         for i,data in enumerate(trainloader):
             optimizer.zero_grad()
             x,y = data
             x = x.to(device)
             y = y.to(device)
@@ -53,14 +53,17 @@
             optimizer.step()
 
             running_loss += loss.item()
             if i%1==0:
                 print(f"epoch : {epoch}, batch : {i}/{len(trainloader)} - loss: {running_loss/100:.3f}")
                 running_loss = 0
 
+            if i>10:
+                break
+
     with torch.no_grad():
         correct = 0
         for data in testloader:
             x,y = data
             x = x.to(device)
             y = y.yo(device)
             soft = model(x)
```

### Comparing `mia_vgg-0.0.5/src/mia_vgg.egg-info/PKG-INFO` & `mia_vgg-0.0.6/src/mia_vgg.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.5
+Version: 0.0.6
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

