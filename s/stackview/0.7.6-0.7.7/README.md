# Comparing `tmp/stackview-0.7.6.tar.gz` & `tmp/stackview-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackview-0.7.6.tar", last modified: Sat Mar 30 17:29:03 2024, max compression
+gzip compressed data, was "stackview-0.7.7.tar", last modified: Fri May 24 13:48:41 2024, max compression
```

## Comparing `stackview-0.7.6.tar` & `stackview-0.7.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 17:29:03.513773 stackview-0.7.6/
--rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.7.6/LICENSE
--rw-rw-rw-   0        0        0    11857 2024-03-30 17:29:03.512771 stackview-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0    11059 2024-03-30 17:15:46.000000 stackview-0.7.6/README.md
--rw-rw-rw-   0        0        0       42 2024-03-30 17:29:03.514776 stackview-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0     1114 2024-03-30 17:28:27.000000 stackview-0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:29:03.483694 stackview-0.7.6/stackview/
--rw-rw-rw-   0        0        0      613 2024-03-30 17:28:27.000000 stackview-0.7.6/stackview/__init__.py
--rw-rw-rw-   0        0        0     7993 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_annotate.py
--rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.7.6/stackview/_assist.py
--rw-rw-rw-   0        0        0     1429 2024-03-23 12:49:32.000000 stackview-0.7.6/stackview/_bia_bob_plugins.py
--rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.7.6/stackview/_colormaps.py
--rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.7.6/stackview/_context.py
--rw-rw-rw-   0        0        0     5584 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_crop.py
--rw-rw-rw-   0        0        0     5184 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_curtain.py
--rw-rw-rw-   0        0        0     4115 2023-11-17 12:56:59.000000 stackview-0.7.6/stackview/_image_widget.py
--rw-rw-rw-   0        0        0     4358 2024-03-30 17:15:46.000000 stackview-0.7.6/stackview/_imshow.py
--rw-rw-rw-   0        0        0     7964 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_interact.py
--rw-rw-rw-   0        0        0     2367 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_orthogonal.py
--rw-rw-rw-   0        0        0     3516 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_picker.py
--rw-rw-rw-   0        0        0     5252 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_side_by_side.py
--rw-rw-rw-   0        0        0     2280 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_slice.py
--rw-rw-rw-   0        0        0     2823 2024-03-23 13:51:50.000000 stackview-0.7.6/stackview/_slice_viewer.py
--rw-rw-rw-   0        0        0     8753 2023-10-19 19:42:08.000000 stackview-0.7.6/stackview/_static_view.py
--rw-rw-rw-   0        0        0     6551 2024-03-30 17:27:56.000000 stackview-0.7.6/stackview/_switch.py
--rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.7.6/stackview/_uint_field.py
--rw-rw-rw-   0        0        0     2567 2023-01-01 15:16:44.000000 stackview-0.7.6/stackview/_utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-30 17:29:03.511768 stackview-0.7.6/stackview.egg-info/
--rw-rw-rw-   0        0        0    11857 2024-03-30 17:29:03.000000 stackview-0.7.6/stackview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2024-03-30 17:29:03.000000 stackview-0.7.6/stackview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 17:29:03.000000 stackview-0.7.6/stackview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2024-03-30 17:29:03.000000 stackview-0.7.6/stackview.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-03-30 17:29:03.000000 stackview-0.7.6/stackview.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-30 17:29:03.000000 stackview-0.7.6/stackview.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 13:48:41.577460 stackview-0.7.7/
+-rw-rw-rw-   0        0        0     1549 2022-11-28 22:36:36.000000 stackview-0.7.7/LICENSE
+-rw-rw-rw-   0        0        0    12050 2024-05-24 13:48:41.577460 stackview-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11252 2024-03-30 17:31:52.000000 stackview-0.7.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 13:48:41.577460 stackview-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2024-05-24 13:45:46.000000 stackview-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:48:41.561833 stackview-0.7.7/stackview/
+-rw-rw-rw-   0        0        0      613 2024-05-24 13:45:46.000000 stackview-0.7.7/stackview/__init__.py
+-rw-rw-rw-   0        0        0     7993 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_annotate.py
+-rw-rw-rw-   0        0        0     5101 2023-03-26 19:33:45.000000 stackview-0.7.7/stackview/_assist.py
+-rw-rw-rw-   0        0        0     1429 2024-03-23 12:49:32.000000 stackview-0.7.7/stackview/_bia_bob_plugins.py
+-rw-rw-rw-   0        0        0     5467 2023-04-15 09:27:34.000000 stackview-0.7.7/stackview/_colormaps.py
+-rw-rw-rw-   0        0        0     2060 2023-01-01 15:16:44.000000 stackview-0.7.7/stackview/_context.py
+-rw-rw-rw-   0        0        0     5584 2024-05-24 13:35:04.000000 stackview-0.7.7/stackview/_crop.py
+-rw-rw-rw-   0        0        0     5184 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_curtain.py
+-rw-rw-rw-   0        0        0     4115 2023-11-17 12:56:59.000000 stackview-0.7.7/stackview/_image_widget.py
+-rw-rw-rw-   0        0        0     4457 2024-05-24 13:45:55.000000 stackview-0.7.7/stackview/_imshow.py
+-rw-rw-rw-   0        0        0     7964 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_interact.py
+-rw-rw-rw-   0        0        0     2367 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_orthogonal.py
+-rw-rw-rw-   0        0        0     3516 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_picker.py
+-rw-rw-rw-   0        0        0     5252 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_side_by_side.py
+-rw-rw-rw-   0        0        0     2280 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_slice.py
+-rw-rw-rw-   0        0        0     2823 2024-03-23 13:51:50.000000 stackview-0.7.7/stackview/_slice_viewer.py
+-rw-rw-rw-   0        0        0     8753 2023-10-19 19:42:08.000000 stackview-0.7.7/stackview/_static_view.py
+-rw-rw-rw-   0        0        0     6551 2024-03-30 17:27:56.000000 stackview-0.7.7/stackview/_switch.py
+-rw-rw-rw-   0        0        0     1066 2022-12-30 17:39:31.000000 stackview-0.7.7/stackview/_uint_field.py
+-rw-rw-rw-   0        0        0     2567 2023-01-01 15:16:44.000000 stackview-0.7.7/stackview/_utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:48:41.577460 stackview-0.7.7/stackview.egg-info/
+-rw-rw-rw-   0        0        0    12050 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 13:48:41.000000 stackview-0.7.7/stackview.egg-info/top_level.txt
```

### Comparing `stackview-0.7.6/LICENSE` & `stackview-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/PKG-INFO` & `stackview-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.7.6
+Version: 0.7.7
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@uni-leipzig.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -93,15 +93,18 @@
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/labels_demo.png)
 
 ### matplotlib-like imshow
 
 To visualize images with more flexibility, there is `imshow`, which works similar like matplotlib's imshow and yet adds more flexibily, e.g. when it comes to colormaps. It supports `pure...` colormaps introduced in [microfilm](https://github.com/guiwitz/microfilm).
 
 ```python
+stackview.imshow(image, axes=True, colorbar=True, colormap='pure_magenta')
+```
 
+![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow_pure_magenta.png)
 
 ... or drawing label images. 
 
 ```python
 import matplotlib.pyplot as plt
 fig, axs = plt.subplots(1, 3, figsize=(15,15))
```

### Comparing `stackview-0.7.6/README.md` & `stackview-0.7.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,18 @@
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/labels_demo.png)
 
 ### matplotlib-like imshow
 
 To visualize images with more flexibility, there is `imshow`, which works similar like matplotlib's imshow and yet adds more flexibily, e.g. when it comes to colormaps. It supports `pure...` colormaps introduced in [microfilm](https://github.com/guiwitz/microfilm).
 
 ```python
+stackview.imshow(image, axes=True, colorbar=True, colormap='pure_magenta')
+```
 
+![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow_pure_magenta.png)
 
 ... or drawing label images. 
 
 ```python
 import matplotlib.pyplot as plt
 fig, axs = plt.subplots(1, 3, figsize=(15,15))
```

### Comparing `stackview-0.7.6/setup.py` & `stackview-0.7.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stackview",
-    version="0.7.6",
+    version="0.7.7",
     author="Robert Haase",
     author_email="robert.haase@uni-leipzig.de",
     description="Interactive image stack viewing in jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/haesleinhuepf/stackview/",
     packages=setuptools.find_packages(),
```

### Comparing `stackview-0.7.6/stackview/__init__.py` & `stackview-0.7.7/stackview/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.6"
+__version__ = "0.7.7"
 
 from ._static_view import jupyter_displayable_output, insight
 from ._utilities import merge_rgb
 from ._context import nop
 from ._crop import crop
 from ._slice_viewer import _SliceViewer
 from ._annotate import annotate
```

### Comparing `stackview-0.7.6/stackview/_annotate.py` & `stackview-0.7.7/stackview/_annotate.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_assist.py` & `stackview-0.7.7/stackview/_assist.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_bia_bob_plugins.py` & `stackview-0.7.7/stackview/_bia_bob_plugins.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_colormaps.py` & `stackview-0.7.7/stackview/_colormaps.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_context.py` & `stackview-0.7.7/stackview/_context.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_crop.py` & `stackview-0.7.7/stackview/_crop.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_curtain.py` & `stackview-0.7.7/stackview/_curtain.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_image_widget.py` & `stackview-0.7.7/stackview/_image_widget.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_imshow.py` & `stackview-0.7.7/stackview/_imshow.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,17 +59,20 @@
         warnings.warn("The parameter min_display_intensity is deprecated, use min_display_intensity instead.")
         min_display_intensity = vmin
 
     if vmax is not None:
         warnings.warn("The parameter max_display_intensity is deprecated, use max_display_intensity instead.")
         max_display_intensity = vmax
 
-    if len(image.shape) == 3:
+    if len(image.shape) == 3 and image.shape[-1] > 4:
         image = image.max(axis=0)
 
+    if 'cupy.ndarray' in str(type(image)):
+        image = image.get()
+
     image = np.asarray(image)
     if len(image.shape) == 1:
         image = image[np.newaxis]
 
     if labels is None:
         labels = is_label_image(image)
```

### Comparing `stackview-0.7.6/stackview/_interact.py` & `stackview-0.7.7/stackview/_interact.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_orthogonal.py` & `stackview-0.7.7/stackview/_orthogonal.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_picker.py` & `stackview-0.7.7/stackview/_picker.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_side_by_side.py` & `stackview-0.7.7/stackview/_side_by_side.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_slice.py` & `stackview-0.7.7/stackview/_slice.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_slice_viewer.py` & `stackview-0.7.7/stackview/_slice_viewer.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_static_view.py` & `stackview-0.7.7/stackview/_static_view.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_switch.py` & `stackview-0.7.7/stackview/_switch.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_uint_field.py` & `stackview-0.7.7/stackview/_uint_field.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview/_utilities.py` & `stackview-0.7.7/stackview/_utilities.py`

 * *Files identical despite different names*

### Comparing `stackview-0.7.6/stackview.egg-info/PKG-INFO` & `stackview-0.7.7/stackview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackview
-Version: 0.7.6
+Version: 0.7.7
 Summary: Interactive image stack viewing in jupyter notebooks
 Home-page: https://github.com/haesleinhuepf/stackview/
 Author: Robert Haase
 Author-email: robert.haase@uni-leipzig.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -93,15 +93,18 @@
 ![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/labels_demo.png)
 
 ### matplotlib-like imshow
 
 To visualize images with more flexibility, there is `imshow`, which works similar like matplotlib's imshow and yet adds more flexibily, e.g. when it comes to colormaps. It supports `pure...` colormaps introduced in [microfilm](https://github.com/guiwitz/microfilm).
 
 ```python
+stackview.imshow(image, axes=True, colorbar=True, colormap='pure_magenta')
+```
 
+![img.png](https://raw.githubusercontent.com/haesleinhuepf/stackview/main/docs/images/imshow_pure_magenta.png)
 
 ... or drawing label images. 
 
 ```python
 import matplotlib.pyplot as plt
 fig, axs = plt.subplots(1, 3, figsize=(15,15))
```

### Comparing `stackview-0.7.6/stackview.egg-info/SOURCES.txt` & `stackview-0.7.7/stackview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

