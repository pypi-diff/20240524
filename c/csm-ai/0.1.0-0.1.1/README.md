# Comparing `tmp/csm_ai-0.1.0.tar.gz` & `tmp/csm_ai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csm_ai-0.1.0.tar", last modified: Tue May 21 14:54:59 2024, max compression
+gzip compressed data, was "csm_ai-0.1.1.tar", last modified: Fri May 24 17:57:58 2024, max compression
```

## Comparing `csm_ai-0.1.0.tar` & `csm_ai-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-21 14:54:59.506218 csm_ai-0.1.0/
--rw-r--r--   0 rfeinman   (501) staff       (20)    11357 2024-05-15 14:49:42.000000 csm_ai-0.1.0/LICENSE
--rw-r--r--   0 rfeinman   (501) staff       (20)     1532 2024-05-21 14:54:59.506037 csm_ai-0.1.0/PKG-INFO
--rw-r--r--   0 rfeinman   (501) staff       (20)     1093 2024-05-21 14:48:23.000000 csm_ai-0.1.0/README.md
--rw-r--r--   0 rfeinman   (501) staff       (20)       97 2024-05-13 17:46:38.000000 csm_ai-0.1.0/pyproject.toml
--rw-r--r--   0 rfeinman   (501) staff       (20)       38 2024-05-21 14:54:59.506259 csm_ai-0.1.0/setup.cfg
--rw-r--r--   0 rfeinman   (501) staff       (20)      964 2024-05-21 14:48:20.000000 csm_ai-0.1.0/setup.py
-drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-21 14:54:59.504050 csm_ai-0.1.0/src/
-drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-21 14:54:59.505149 csm_ai-0.1.0/src/csm/
--rw-r--r--   0 rfeinman   (501) staff       (20)       78 2024-05-20 19:48:44.000000 csm_ai-0.1.0/src/csm/__init__.py
--rw-r--r--   0 rfeinman   (501) staff       (20)    14901 2024-05-20 23:13:39.000000 csm_ai-0.1.0/src/csm/client.py
--rw-r--r--   0 rfeinman   (501) staff       (20)       21 2024-05-21 00:55:52.000000 csm_ai-0.1.0/src/csm/version.py
-drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-21 14:54:59.505867 csm_ai-0.1.0/src/csm_ai.egg-info/
--rw-r--r--   0 rfeinman   (501) staff       (20)     1532 2024-05-21 14:54:59.000000 csm_ai-0.1.0/src/csm_ai.egg-info/PKG-INFO
--rw-r--r--   0 rfeinman   (501) staff       (20)      267 2024-05-21 14:54:59.000000 csm_ai-0.1.0/src/csm_ai.egg-info/SOURCES.txt
--rw-r--r--   0 rfeinman   (501) staff       (20)        1 2024-05-21 14:54:59.000000 csm_ai-0.1.0/src/csm_ai.egg-info/dependency_links.txt
--rw-r--r--   0 rfeinman   (501) staff       (20)       16 2024-05-21 14:54:59.000000 csm_ai-0.1.0/src/csm_ai.egg-info/requires.txt
--rw-r--r--   0 rfeinman   (501) staff       (20)        4 2024-05-21 14:54:59.000000 csm_ai-0.1.0/src/csm_ai.egg-info/top_level.txt
+drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-24 17:57:58.806795 csm_ai-0.1.1/
+-rw-r--r--   0 rfeinman   (501) staff       (20)    11357 2024-05-15 14:49:42.000000 csm_ai-0.1.1/LICENSE
+-rw-r--r--   0 rfeinman   (501) staff       (20)     1532 2024-05-24 17:57:58.806557 csm_ai-0.1.1/PKG-INFO
+-rw-r--r--   0 rfeinman   (501) staff       (20)     1093 2024-05-24 17:40:36.000000 csm_ai-0.1.1/README.md
+-rw-r--r--   0 rfeinman   (501) staff       (20)       97 2024-05-13 17:46:38.000000 csm_ai-0.1.1/pyproject.toml
+-rw-r--r--   0 rfeinman   (501) staff       (20)       38 2024-05-24 17:57:58.806847 csm_ai-0.1.1/setup.cfg
+-rw-r--r--   0 rfeinman   (501) staff       (20)      964 2024-05-21 14:48:20.000000 csm_ai-0.1.1/setup.py
+drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-24 17:57:58.804324 csm_ai-0.1.1/src/
+drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-24 17:57:58.805452 csm_ai-0.1.1/src/csm/
+-rw-r--r--   0 rfeinman   (501) staff       (20)       78 2024-05-20 19:48:44.000000 csm_ai-0.1.1/src/csm/__init__.py
+-rw-r--r--   0 rfeinman   (501) staff       (20)    14899 2024-05-24 17:41:13.000000 csm_ai-0.1.1/src/csm/client.py
+-rw-r--r--   0 rfeinman   (501) staff       (20)       21 2024-05-24 17:55:04.000000 csm_ai-0.1.1/src/csm/version.py
+drwxr-xr-x   0 rfeinman   (501) staff       (20)        0 2024-05-24 17:57:58.806273 csm_ai-0.1.1/src/csm_ai.egg-info/
+-rw-r--r--   0 rfeinman   (501) staff       (20)     1532 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/PKG-INFO
+-rw-r--r--   0 rfeinman   (501) staff       (20)      267 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 rfeinman   (501) staff       (20)        1 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 rfeinman   (501) staff       (20)       16 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/requires.txt
+-rw-r--r--   0 rfeinman   (501) staff       (20)        4 2024-05-24 17:57:58.000000 csm_ai-0.1.1/src/csm_ai.egg-info/top_level.txt
```

### Comparing `csm_ai-0.1.0/LICENSE` & `csm_ai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csm_ai-0.1.0/PKG-INFO` & `csm_ai-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csm-ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: The official Python library for the CSM API
 Home-page: https://github.com/CommonSenseMachines/csm-ai
 Author: Common Sense Machines
 Author-email: support@csm.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -37,15 +37,15 @@
 
 Run an `image-to-3d` job:
 
 ```python
 # a) using a local image path
 image_path = "/path/to/image.png"
 
-mesh_path = csm_client.image_to_3d(image_path, mesh_format='glb', verbose=True)
+mesh_path = csm_client.image_to_3d(image_path, mesh_format='glb')
 
 # b) using an image URL
 image_url = "https://upload.wikimedia.org/wikipedia/en/a/a9/MarioNSMBUDeluxe.png"
 
 mesh_path = csm_client.image_to_3d(image_url, mesh_format='obj')
 ```
 
@@ -55,9 +55,9 @@
 prompt = "3d asset of a character head, cartoon style, low poly, front view"
 
 mesh_path, image_path = csm_client.text_to_3d(prompt, mesh_format='glb')
 ```
 
 **Mesh formats:** Choose any of ['obj', 'glb', 'usdz'] for the `mesh_format` argument.
 
-**Verbose mode:** Run client functions with option `verbose=True` to see additional status messages and logs.
+**Verbose mode:** Run client functions with option `verbose=True` (the default) to see additional status messages and logs.
```

### Comparing `csm_ai-0.1.0/README.md` & `csm_ai-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 Run an `image-to-3d` job:
 
 ```python
 # a) using a local image path
 image_path = "/path/to/image.png"
 
-mesh_path = csm_client.image_to_3d(image_path, mesh_format='glb', verbose=True)
+mesh_path = csm_client.image_to_3d(image_path, mesh_format='glb')
 
 # b) using an image URL
 image_url = "https://upload.wikimedia.org/wikipedia/en/a/a9/MarioNSMBUDeluxe.png"
 
 mesh_path = csm_client.image_to_3d(image_url, mesh_format='obj')
 ```
 
@@ -41,9 +41,9 @@
 prompt = "3d asset of a character head, cartoon style, low poly, front view"
 
 mesh_path, image_path = csm_client.text_to_3d(prompt, mesh_format='glb')
 ```
 
 **Mesh formats:** Choose any of ['obj', 'glb', 'usdz'] for the `mesh_format` argument.
 
-**Verbose mode:** Run client functions with option `verbose=True` to see additional status messages and logs.
+**Verbose mode:** Run client functions with option `verbose=True` (the default) to see additional status messages and logs.
```

### Comparing `csm_ai-0.1.0/setup.py` & `csm_ai-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `csm_ai-0.1.0/src/csm/client.py` & `csm_ai-0.1.1/src/csm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             image,
             *,
             generate_spin_video=False,
             diffusion_time_steps=75,
             mesh_format='obj',
             output='./',
             timeout=200,
-            verbose=False,
+            verbose=True,
         ):
         r"""Generate a 3D mesh from an image.
 
         The input image can be provided as a URL, a local path, or a :class:`PIL.Image`.
 
         Parameters
         ----------
@@ -357,15 +357,15 @@
             style_id="",
             guidance=6,
             generate_spin_video=False,
             diffusion_time_steps=75,
             mesh_format='obj',
             output='./',
             timeout=200,
-            verbose=False,
+            verbose=True,
         ):
         r"""Generate a 3D mesh from a text prompt.
 
         Parameters
         ----------
         prompt : str
             The input text prompt.
```

### Comparing `csm_ai-0.1.0/src/csm_ai.egg-info/PKG-INFO` & `csm_ai-0.1.1/src/csm_ai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csm-ai
-Version: 0.1.0
+Version: 0.1.1
 Summary: The official Python library for the CSM API
 Home-page: https://github.com/CommonSenseMachines/csm-ai
 Author: Common Sense Machines
 Author-email: support@csm.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -37,15 +37,15 @@
 
 Run an `image-to-3d` job:
 
 ```python
 # a) using a local image path
 image_path = "/path/to/image.png"
 
-mesh_path = csm_client.image_to_3d(image_path, mesh_format='glb', verbose=True)
+mesh_path = csm_client.image_to_3d(image_path, mesh_format='glb')
 
 # b) using an image URL
 image_url = "https://upload.wikimedia.org/wikipedia/en/a/a9/MarioNSMBUDeluxe.png"
 
 mesh_path = csm_client.image_to_3d(image_url, mesh_format='obj')
 ```
 
@@ -55,9 +55,9 @@
 prompt = "3d asset of a character head, cartoon style, low poly, front view"
 
 mesh_path, image_path = csm_client.text_to_3d(prompt, mesh_format='glb')
 ```
 
 **Mesh formats:** Choose any of ['obj', 'glb', 'usdz'] for the `mesh_format` argument.
 
-**Verbose mode:** Run client functions with option `verbose=True` to see additional status messages and logs.
+**Verbose mode:** Run client functions with option `verbose=True` (the default) to see additional status messages and logs.
```

