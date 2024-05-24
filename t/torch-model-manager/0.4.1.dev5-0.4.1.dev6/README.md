# Comparing `tmp/torch_model_manager-0.4.1.dev5.tar.gz` & `tmp/torch_model_manager-0.4.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.1.dev5.tar", last modified: Thu May 23 14:19:08 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.1.dev6.tar", last modified: Fri May 24 08:01:37 2024, max compression
```

## Comparing `torch_model_manager-0.4.1.dev5.tar` & `torch_model_manager-0.4.1.dev6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 14:19:08.084504 torch_model_manager-0.4.1.dev5/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-23 14:19:08.084504 torch_model_manager-0.4.1.dev5/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev5/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-23 14:19:08.084504 torch_model_manager-0.4.1.dev5/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2243 2024-05-23 14:19:06.000000 torch_model_manager-0.4.1.dev5/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 14:19:08.080504 torch_model_manager-0.4.1.dev5/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 14:19:08.080504 torch_model_manager-0.4.1.dev5/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev5/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev5/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 14:19:08.080504 torch_model_manager-0.4.1.dev5/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev5/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev5/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 14:19:08.084504 torch_model_manager-0.4.1.dev5/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.1.dev5/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-0.4.1.dev5/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.1.dev5/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    20851 2024-05-23 14:18:54.000000 torch_model_manager-0.4.1.dev5/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev5/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev5/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 14:19:08.084504 torch_model_manager-0.4.1.dev5/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-23 14:19:08.000000 torch_model_manager-0.4.1.dev5/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-23 14:19:08.000000 torch_model_manager-0.4.1.dev5/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-23 14:19:08.000000 torch_model_manager-0.4.1.dev5/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      241 2024-05-23 14:19:08.000000 torch_model_manager-0.4.1.dev5/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-23 14:19:08.000000 torch_model_manager-0.4.1.dev5/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 14:19:08.084504 torch_model_manager-0.4.1.dev5/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev5/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.1.dev5/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 08:01:37.158006 torch_model_manager-0.4.1.dev6/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-24 08:01:37.158006 torch_model_manager-0.4.1.dev6/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev6/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-24 08:01:37.158006 torch_model_manager-0.4.1.dev6/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2243 2024-05-24 08:01:35.000000 torch_model_manager-0.4.1.dev6/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 08:01:37.150006 torch_model_manager-0.4.1.dev6/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 08:01:37.154006 torch_model_manager-0.4.1.dev6/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev6/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev6/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 08:01:37.154006 torch_model_manager-0.4.1.dev6/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev6/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev6/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 08:01:37.154006 torch_model_manager-0.4.1.dev6/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.1.dev6/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-0.4.1.dev6/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.1.dev6/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    21181 2024-05-24 08:00:18.000000 torch_model_manager-0.4.1.dev6/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev6/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev6/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 08:01:37.154006 torch_model_manager-0.4.1.dev6/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9225 2024-05-24 08:01:37.000000 torch_model_manager-0.4.1.dev6/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-24 08:01:37.000000 torch_model_manager-0.4.1.dev6/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-24 08:01:37.000000 torch_model_manager-0.4.1.dev6/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      241 2024-05-24 08:01:37.000000 torch_model_manager-0.4.1.dev6/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-24 08:01:37.000000 torch_model_manager-0.4.1.dev6/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-24 08:01:37.154006 torch_model_manager-0.4.1.dev6/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev6/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.1.dev6/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.1.dev5/PKG-INFO` & `torch_model_manager-0.4.1.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.1.dev5
+Version: 0.4.1.dev6
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.1.dev5/README.md` & `torch_model_manager-0.4.1.dev6/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev5/setup.py` & `torch_model_manager-0.4.1.dev6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.1.dev5',
+    version='0.4.1.dev6',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.1.dev5/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.1.dev6/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev5/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.1.dev6/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev5/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.1.dev6/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev5/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.1.dev6/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev5/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.1.dev6/torch_model_manager/segmentation_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from groundingdino.util.inference import Model
 from utils import helpers
 from segment_anything import sam_model_registry, SamPredictor
 from scipy.stats import hmean
 import pandas as pd
 from tqdm import tqdm
 from PIL import Image
-
+import matplotlib.pyplot as plt
+from torchvision import transforms
 from sklearn.preprocessing import LabelEncoder
 
 DEVICE = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
 # class SegmentationManager:
 #     def __init__(self, sam_type='vit_h', checkpoint_path=None, return_prompts=False, device=DEVICE):
 #         self.device = device
@@ -358,16 +359,23 @@
 
             # Apply the grounding SAM pipeline
             detections, annotated_image = self.grounding_sam(image_path, 
                                                              classes, 
                                                              box_threshold=box_threshold, 
                                                              text_threshold=text_threshold, 
                                                              nms_threshold=nms_threshold)
+
             if run is not None and output_namespaces["annotated_images"] is not None:
-                run.log_tensors(tensors=[torch.Tensor(annotated_image)], paths=[os.path.join(output_namespaces["annotated_images"], image_name)], on_series=False)
+                # Define a transform to convert the image to tensor
+                transform = transforms.ToTensor()
+
+                # Convert the image to PyTorch tensor
+                rgb_image = transform(annotated_image)
+                rgb_image = rgb_image[[2, 1, 0], :, :]
+                run.log_tensors(tensors=[rgb_image], paths=[os.path.join(output_namespaces["annotated_images"], image_name)], on_series=False)
             if run is not None and output_namespaces["detections"] is not None:
                 run.log_files(data = detections, namespace=os.path.join(output_namespaces["detections"], image_name), extension="pkl", wait=True)
             # Calculate the harmonic mean of confidences
             confidences = detections.confidence
             class_ids = [classes[id] for id in detections.class_id]
             harmonic_means = self.aggregator(class_ids, confidences, agg=agg)
             annotation_matrix.loc[image_name, harmonic_means[:, 0]] = harmonic_means[:, 1]
```

### Comparing `torch_model_manager-0.4.1.dev5/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.1.dev6/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev5/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.1.dev6/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev5/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.1.dev6/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.1.dev5
+Version: 0.4.1.dev6
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.1.dev5/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.1.dev6/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev5/utils/helpers.py` & `torch_model_manager-0.4.1.dev6/utils/helpers.py`

 * *Files identical despite different names*

