# Comparing `tmp/spectralnet-0.1.1.tar.gz` & `tmp/spectralnet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralnet-0.1.1.tar", last modified: Mon Feb 12 08:59:12 2024, max compression
+gzip compressed data, was "spectralnet-0.1.2.tar", last modified: Fri May 24 10:24:43 2024, max compression
```

## Comparing `spectralnet-0.1.1.tar` & `spectralnet-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-02-12 08:59:12.982580 spectralnet-0.1.1/
--rw-r--r--   0 amitai     (501) staff       (20)     1082 2024-02-11 05:36:48.000000 spectralnet-0.1.1/LICENSE.md
--rw-r--r--   0 amitai     (501) staff       (20)     2974 2024-02-12 08:59:12.982495 spectralnet-0.1.1/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)     2480 2024-02-11 05:36:48.000000 spectralnet-0.1.1/README.md
--rw-r--r--   0 amitai     (501) staff       (20)      342 2024-02-11 05:36:48.000000 spectralnet-0.1.1/pyproject.toml
--rw-r--r--   0 amitai     (501) staff       (20)      615 2024-02-12 08:59:12.982844 spectralnet-0.1.1/setup.cfg
--rw-r--r--   0 amitai     (501) staff       (20)       38 2024-02-11 05:36:48.000000 spectralnet-0.1.1/setup.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-02-12 08:59:12.975724 spectralnet-0.1.1/src/
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-02-12 08:59:12.978003 spectralnet-0.1.1/src/spectralnet/
--rw-r--r--   0 amitai     (501) staff       (20)      202 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)    11241 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_cluster.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-02-12 08:59:12.979528 spectralnet-0.1.1/src/spectralnet/_losses/
--rw-r--r--   0 amitai     (501) staff       (20)       89 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_losses/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1574 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_losses/_siamese_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)     1011 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_losses/_spectralnet_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)     2795 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_metrics.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-02-12 08:59:12.980754 spectralnet-0.1.1/src/spectralnet/_models/
--rw-r--r--   0 amitai     (501) staff       (20)      126 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_models/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1522 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_models/_ae_model.py
--rw-r--r--   0 amitai     (501) staff       (20)      835 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_models/_siamesenet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     2608 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_models/_spectralnet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)    13175 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_reduction.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-02-12 08:59:12.981879 spectralnet-0.1.1/src/spectralnet/_trainers/
--rw-r--r--   0 amitai     (501) staff       (20)      133 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_trainers/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     4017 2024-02-12 08:39:22.000000 spectralnet-0.1.1/src/spectralnet/_trainers/_ae_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     9574 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_trainers/_siamesenet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     7960 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_trainers/_spectralnet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)       52 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_trainers/_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)    12557 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/spectralnet/_utils.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-02-12 08:59:12.982221 spectralnet-0.1.1/src/spectralnet.egg-info/
--rw-r--r--   0 amitai     (501) staff       (20)     2974 2024-02-12 08:59:12.000000 spectralnet-0.1.1/src/spectralnet.egg-info/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)      874 2024-02-12 08:59:12.000000 spectralnet-0.1.1/src/spectralnet.egg-info/SOURCES.txt
--rw-r--r--   0 amitai     (501) staff       (20)        1 2024-02-12 08:59:12.000000 spectralnet-0.1.1/src/spectralnet.egg-info/dependency_links.txt
--rw-r--r--   0 amitai     (501) staff       (20)       18 2024-02-12 08:59:12.000000 spectralnet-0.1.1/src/spectralnet.egg-info/top_level.txt
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-02-12 08:59:12.982051 spectralnet-0.1.1/src/tests/
--rw-r--r--   0 amitai     (501) staff       (20)        0 2024-02-11 05:36:48.000000 spectralnet-0.1.1/src/tests/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-05-24 10:24:43.299630 spectralnet-0.1.2/
+-rw-r--r--   0 amitai     (501) staff       (20)     1082 2024-05-24 10:18:03.000000 spectralnet-0.1.2/LICENSE.md
+-rw-r--r--   0 amitai     (501) staff       (20)     3280 2024-05-24 10:24:43.299497 spectralnet-0.1.2/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)     2480 2024-05-24 10:18:03.000000 spectralnet-0.1.2/README.md
+-rw-r--r--   0 amitai     (501) staff       (20)      342 2024-05-24 10:18:03.000000 spectralnet-0.1.2/pyproject.toml
+-rw-r--r--   0 amitai     (501) staff       (20)      787 2024-05-24 10:24:43.299989 spectralnet-0.1.2/setup.cfg
+-rw-r--r--   0 amitai     (501) staff       (20)       38 2024-05-24 10:18:03.000000 spectralnet-0.1.2/setup.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-05-24 10:24:43.269123 spectralnet-0.1.2/src/
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-05-24 10:24:43.281630 spectralnet-0.1.2/src/spectralnet/
+-rw-r--r--   0 amitai     (501) staff       (20)      202 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)    11241 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_cluster.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-05-24 10:24:43.284045 spectralnet-0.1.2/src/spectralnet/_losses/
+-rw-r--r--   0 amitai     (501) staff       (20)       89 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_losses/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1574 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_losses/_siamese_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1011 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_losses/_spectralnet_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2795 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_metrics.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-05-24 10:24:43.284744 spectralnet-0.1.2/src/spectralnet/_models/
+-rw-r--r--   0 amitai     (501) staff       (20)      126 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_models/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1522 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_models/_ae_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)      835 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_models/_siamesenet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2608 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_models/_spectralnet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)    13175 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_reduction.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-05-24 10:24:43.290819 spectralnet-0.1.2/src/spectralnet/_trainers/
+-rw-r--r--   0 amitai     (501) staff       (20)      133 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_trainers/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     4017 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_trainers/_ae_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9574 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_trainers/_siamesenet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     7960 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_trainers/_spectralnet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)       52 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_trainers/_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)    12557 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/spectralnet/_utils.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-05-24 10:24:43.294543 spectralnet-0.1.2/src/spectralnet.egg-info/
+-rw-r--r--   0 amitai     (501) staff       (20)     3280 2024-05-24 10:24:43.000000 spectralnet-0.1.2/src/spectralnet.egg-info/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)      912 2024-05-24 10:24:43.000000 spectralnet-0.1.2/src/spectralnet.egg-info/SOURCES.txt
+-rw-r--r--   0 amitai     (501) staff       (20)        1 2024-05-24 10:24:43.000000 spectralnet-0.1.2/src/spectralnet.egg-info/dependency_links.txt
+-rw-r--r--   0 amitai     (501) staff       (20)      141 2024-05-24 10:24:43.000000 spectralnet-0.1.2/src/spectralnet.egg-info/requires.txt
+-rw-r--r--   0 amitai     (501) staff       (20)       18 2024-05-24 10:24:43.000000 spectralnet-0.1.2/src/spectralnet.egg-info/top_level.txt
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2024-05-24 10:24:43.291581 spectralnet-0.1.2/src/tests/
+-rw-r--r--   0 amitai     (501) staff       (20)        0 2024-05-24 10:18:03.000000 spectralnet-0.1.2/src/tests/__init__.py
```

### Comparing `spectralnet-0.1.1/LICENSE.md` & `spectralnet-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/PKG-INFO` & `spectralnet-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/shaham-lab/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/shaham-lab/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: setuptools
+Requires-Dist: wheel
+Requires-Dist: torch>=2.0.0
+Requires-Dist: torchvision>=0.15.1
+Requires-Dist: h5py>=3.8.0
+Requires-Dist: numpy>=1.24
+Requires-Dist: annoy>=1.17.1
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: munkres
+Requires-Dist: matplotlib
+Requires-Dist: scikit-learn>=1.2.2
 
 # SpectralNet
 
 <p align="center">
     <img src="https://github.com/shaham-lab/SpectralNet/blob/main/figures/twomoons.png">
 
 SpectralNet is a Python package that performs spectral clustering with deep neural networks.<br><br>
```

### Comparing `spectralnet-0.1.1/README.md` & `spectralnet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/setup.cfg` & `spectralnet-0.1.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spectralnet
-version = 0.1.1
+version = 0.1.2
 author = Amitai
 description = Spectral Clustering Using Deep Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shaham-lab/SpectralNet.git
 project_urls = 
 	Bug Tracker = https://github.com/shaham-lab/SpectralNet/issues
@@ -14,14 +14,26 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.11
+install_requires = 
+	setuptools
+	wheel
+	torch>=2.0.0
+	torchvision>=0.15.1
+	h5py>=3.8.0
+	numpy>=1.24
+	annoy>=1.17.1
+	scipy>=1.10.1
+	munkres
+	matplotlib
+	scikit-learn>=1.2.2
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `spectralnet-0.1.1/src/spectralnet/_cluster.py` & `spectralnet-0.1.2/src/spectralnet/_cluster.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_losses/_siamese_loss.py` & `spectralnet-0.1.2/src/spectralnet/_losses/_siamese_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_losses/_spectralnet_loss.py` & `spectralnet-0.1.2/src/spectralnet/_losses/_spectralnet_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_metrics.py` & `spectralnet-0.1.2/src/spectralnet/_metrics.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_models/_ae_model.py` & `spectralnet-0.1.2/src/spectralnet/_models/_ae_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_models/_siamesenet_model.py` & `spectralnet-0.1.2/src/spectralnet/_models/_siamesenet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_models/_spectralnet_model.py` & `spectralnet-0.1.2/src/spectralnet/_models/_spectralnet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_reduction.py` & `spectralnet-0.1.2/src/spectralnet/_reduction.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_trainers/_ae_trainer.py` & `spectralnet-0.1.2/src/spectralnet/_trainers/_ae_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_trainers/_siamesenet_trainer.py` & `spectralnet-0.1.2/src/spectralnet/_trainers/_siamesenet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_trainers/_spectralnet_trainer.py` & `spectralnet-0.1.2/src/spectralnet/_trainers/_spectralnet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet/_utils.py` & `spectralnet-0.1.2/src/spectralnet/_utils.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.1.1/src/spectralnet.egg-info/PKG-INFO` & `spectralnet-0.1.2/src/spectralnet.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/shaham-lab/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/shaham-lab/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: setuptools
+Requires-Dist: wheel
+Requires-Dist: torch>=2.0.0
+Requires-Dist: torchvision>=0.15.1
+Requires-Dist: h5py>=3.8.0
+Requires-Dist: numpy>=1.24
+Requires-Dist: annoy>=1.17.1
+Requires-Dist: scipy>=1.10.1
+Requires-Dist: munkres
+Requires-Dist: matplotlib
+Requires-Dist: scikit-learn>=1.2.2
 
 # SpectralNet
 
 <p align="center">
     <img src="https://github.com/shaham-lab/SpectralNet/blob/main/figures/twomoons.png">
 
 SpectralNet is a Python package that performs spectral clustering with deep neural networks.<br><br>
```

### Comparing `spectralnet-0.1.1/src/spectralnet.egg-info/SOURCES.txt` & `spectralnet-0.1.2/src/spectralnet.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/spectralnet/_cluster.py
 src/spectralnet/_metrics.py
 src/spectralnet/_reduction.py
 src/spectralnet/_utils.py
 src/spectralnet.egg-info/PKG-INFO
 src/spectralnet.egg-info/SOURCES.txt
 src/spectralnet.egg-info/dependency_links.txt
+src/spectralnet.egg-info/requires.txt
 src/spectralnet.egg-info/top_level.txt
 src/spectralnet/_losses/__init__.py
 src/spectralnet/_losses/_siamese_loss.py
 src/spectralnet/_losses/_spectralnet_loss.py
 src/spectralnet/_models/__init__.py
 src/spectralnet/_models/_ae_model.py
 src/spectralnet/_models/_siamesenet_model.py
```

