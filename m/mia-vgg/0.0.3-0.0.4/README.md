# Comparing `tmp/mia_vgg-0.0.3.tar.gz` & `tmp/mia_vgg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia_vgg-0.0.3.tar", last modified: Fri May 24 10:52:30 2024, max compression
+gzip compressed data, was "mia_vgg-0.0.4.tar", last modified: Fri May 24 10:55:57 2024, max compression
```

## Comparing `mia_vgg-0.0.3.tar` & `mia_vgg-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:52:30.585238 mia_vgg-0.0.3/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 10:52:30.585238 mia_vgg-0.0.3/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-24 10:52:22.000000 mia_vgg-0.0.3/pyproject.toml
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-24 10:52:30.585238 mia_vgg-0.0.3/setup.cfg
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:52:30.585238 mia_vgg-0.0.3/src/
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:52:30.585238 mia_vgg-0.0.3/src/mia_vgg/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.3/src/mia_vgg/__init__.py
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2185 2024-05-24 10:52:06.000000 mia_vgg-0.0.3/src/mia_vgg/train_target.py
-drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:52:30.585238 mia_vgg-0.0.3/src/mia_vgg.egg-info/
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 10:52:30.000000 mia_vgg-0.0.3/src/mia_vgg.egg-info/PKG-INFO
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-24 10:52:30.000000 mia_vgg-0.0.3/src/mia_vgg.egg-info/SOURCES.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-24 10:52:30.000000 mia_vgg-0.0.3/src/mia_vgg.egg-info/dependency_links.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-24 10:52:30.000000 mia_vgg-0.0.3/src/mia_vgg.egg-info/requires.txt
--rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-24 10:52:30.000000 mia_vgg-0.0.3/src/mia_vgg.egg-info/top_level.txt
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:55:57.601889 mia_vgg-0.0.4/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 10:55:57.601889 mia_vgg-0.0.4/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      541 2024-05-24 10:55:51.000000 mia_vgg-0.0.4/pyproject.toml
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       38 2024-05-24 10:55:57.601889 mia_vgg-0.0.4/setup.cfg
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:55:57.601889 mia_vgg-0.0.4/src/
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:55:57.601889 mia_vgg-0.0.4/src/mia_vgg/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-22 12:56:18.000000 mia_vgg-0.0.4/src/mia_vgg/__init__.py
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)     2184 2024-05-24 10:55:44.000000 mia_vgg-0.0.4/src/mia_vgg/train_target.py
+drwxr-xr-x   0 jaalmoes  (1000) jaalmoes  (1000)        0 2024-05-24 10:55:57.601889 mia_vgg-0.0.4/src/mia_vgg.egg-info/
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      558 2024-05-24 10:55:57.000000 mia_vgg-0.0.4/src/mia_vgg.egg-info/PKG-INFO
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)      240 2024-05-24 10:55:57.000000 mia_vgg-0.0.4/src/mia_vgg.egg-info/SOURCES.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        1 2024-05-24 10:55:57.000000 mia_vgg-0.0.4/src/mia_vgg.egg-info/dependency_links.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)       29 2024-05-24 10:55:57.000000 mia_vgg-0.0.4/src/mia_vgg.egg-info/requires.txt
+-rw-r--r--   0 jaalmoes  (1000) jaalmoes  (1000)        8 2024-05-24 10:55:57.000000 mia_vgg-0.0.4/src/mia_vgg.egg-info/top_level.txt
```

### Comparing `mia_vgg-0.0.3/PKG-INFO` & `mia_vgg-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.3
+Version: 0.0.4
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mia_vgg-0.0.3/pyproject.toml` & `mia_vgg-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mia_vgg"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jan Aalmoes", email="jan.aalmoes@protonmail.com" },
 ]
 description = "MIA on VGG dataset using pytorch"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mia_vgg-0.0.3/src/mia_vgg/train_target.py` & `mia_vgg-0.0.4/src/mia_vgg/train_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """Train VGG16."""
     transform = v2.Compose([PILToTensor(),
                            v2.ToDtype(torch.float32, scale=True)])
     celeba = datasets.CelebA(root="data", download=True, target_transform=trgtsf, transform=transform)
     x = celeba[0][0]
 
     train, test = random_split(celeba, [0.8,0.2])
-    trainloader = DataLoader(train, batch_size=300)
+    trainloader = DataLoader(train, batch_size=32)
     testloader = DataLoader(test)
 
     weights = models.VGG16_Weights
     model = models.vgg16(weights=weights)
 
     num_ftrs = model.classifier[len(model.classifier)-1].in_features
```

### Comparing `mia_vgg-0.0.3/src/mia_vgg.egg-info/PKG-INFO` & `mia_vgg-0.0.4/src/mia_vgg.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_vgg
-Version: 0.0.3
+Version: 0.0.4
 Summary: MIA on VGG dataset using pytorch
 Author-email: Jan Aalmoes <jan.aalmoes@protonmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

