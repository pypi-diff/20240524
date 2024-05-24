# Comparing `tmp/xmipp_metadata-1.0.8.tar.gz` & `tmp/xmipp_metadata-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmipp_metadata-1.0.8.tar", last modified: Wed Apr 19 08:14:13 2023, max compression
+gzip compressed data, was "xmipp_metadata-1.1.0.tar", last modified: Fri May 24 15:20:28 2024, max compression
```

## Comparing `xmipp_metadata-1.0.8.tar` & `xmipp_metadata-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.299775 xmipp_metadata-1.0.8/xmipp_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_em.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3039 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_mrc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9178 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/metadata/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9142 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/metadata/xmipp_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/test_image_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.299775 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:20:28.762846 xmipp_metadata-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-24 15:20:28.762846 xmipp_metadata-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:20:28.762846 xmipp_metadata-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:20:28.758846 xmipp_metadata-1.1.0/xmipp_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:20:28.758846 xmipp_metadata-1.1.0/xmipp_metadata/image_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/image_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2612 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/image_handler/image_em.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21229 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/image_handler/image_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3085 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/image_handler/image_mrc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9223 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/image_handler/image_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:20:28.762846 xmipp_metadata-1.1.0/xmipp_metadata/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/metadata/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12040 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/metadata/xmipp_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:20:28.762846 xmipp_metadata-1.1.0/xmipp_metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/tests/test_image_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/tests/test_metadata_two_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-24 15:13:11.000000 xmipp_metadata-1.1.0/xmipp_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:20:28.758846 xmipp_metadata-1.1.0/xmipp_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-24 15:20:28.000000 xmipp_metadata-1.1.0/xmipp_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-24 15:20:28.000000 xmipp_metadata-1.1.0/xmipp_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:20:28.000000 xmipp_metadata-1.1.0/xmipp_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-24 15:20:28.000000 xmipp_metadata-1.1.0/xmipp_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 15:20:28.000000 xmipp_metadata-1.1.0/xmipp_metadata.egg-info/top_level.txt
```

### Comparing `xmipp_metadata-1.0.8/LICENSE` & `xmipp_metadata-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/README.rst` & `xmipp_metadata-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/setup.py` & `xmipp_metadata-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/__init__.py` & `xmipp_metadata-1.1.0/xmipp_metadata/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-__version__ = "1.0.8"
+__version__ = "1.1.0"
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/__init__.py` & `xmipp_metadata-1.1.0/xmipp_metadata/image_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_em.py` & `xmipp_metadata-1.1.0/xmipp_metadata/image_handler/image_em.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,28 @@
 
 
 class ImageEM(object):
     '''
     Class to read an EM file
     '''
 
+    DEBUG = False
+
     def __init__(self, filename=None):
         if filename:
             self.read(filename)
         else:
             self.header, self.data = None, None
 
     def __del__(self):
         '''
         Close the current file before deleting
         '''
-        print("File closed succesfully!")
+        if self.DEBUG:
+            print("File closed succesfully!")
 
     def __len__(self):
         return self.header["zdim"]
 
     def __iter__(self):
         '''
         Generator method to loop through all the images in the stack
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_handler.py` & `xmipp_metadata-1.1.0/xmipp_metadata/image_handler/image_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,39 +25,48 @@
 # **************************************************************************
 
 
 from pathlib import Path
 
 import numpy as np
 
+from joblib import Parallel, delayed
+from scipy.ndimage import shift
+
 from skimage.transform import rescale, resize, warp
 from skimage import filters
 from skimage.measure import label
+from skimage.morphology import opening, ball
 
 import morphsnakes as ms
 
 from scipy.ndimage.filters import gaussian_filter, median_filter
+from scipy.spatial import ConvexHull, Delaunay
 
 from .image_mrc import ImageMRC
 
 from .image_spider import ImageSpider
 
 from .image_em import ImageEM
 
+from xmipp_metadata.utils import fibonacci_hemisphere, compute_rotations, FourierInterpolator, \
+    compute_projection, RealInterpolator
+
 
 class ImageHandler(object):
     '''
     Class to open several CryoEM image formats. Currently supported files include:
         - MRC files (supported trough mrcfile package)
         - Xmipp Spider files (STK and VOL)
 
     Currently, only reading operations are supported
     '''
 
     BINARIES = None
+    DEBUG = False
 
     def __init__(self, binary_file=None):
         if binary_file:
             binary_file = str(binary_file)
             if ":mrcs" in binary_file:
                 binary_file = binary_file.replace(":mrcs", "")
             elif ":mrc" in binary_file:
@@ -92,15 +101,16 @@
             return len(self.BINARIES)
         else:
             return 0
 
     def __del__(self):
         if self.BINARIES is not None and isinstance(self.BINARIES, ImageSpider):
             self.BINARIES.close()
-        print("File closed succesfully!")
+        if self.DEBUG:
+            print("File closed succesfully!")
 
     def read(self, binary_file):
         '''
         Reading of a binary image file
             :param binary_file (string) --> Path to the binary file to be read
         '''
         if self.BINARIES:
@@ -120,15 +130,15 @@
                 or self.binary_file.suffix == ".xmp" or self.binary_file.suffix == ".spi":
             self.BINARIES = ImageSpider(self.binary_file)
         elif self.binary_file.suffix == ".em" or self.binary_file.suffix == ".ems":
             self.BINARIES = ImageEM(self.binary_file)
 
         return self
 
-    def write(self, data, filename=None, overwrite=False, sr=1.0):
+    def write(self, data, filename=None, overwrite=True, sr=1.0):
         if not overwrite and filename is None and len(self) != data.shape[0]:
             raise Exception("Cannot save file. Number of images "
                             "in new data is different. Please, set overwrite to True "
                             "if you are sure you want to do this.")
 
         filename = self.binary_file if filename is None else Path(filename)
         sr = 1.0 if sr == 0.0 else sr
@@ -137,15 +147,15 @@
             ImageMRC().write(data, filename, overwrite=overwrite, sr=sr)
         elif filename.suffix == ".stk" or filename.suffix == ".vol" \
                 or filename.suffix == ".xmp" or filename.suffix == ".spi":
             ImageSpider().write(data, filename, overwrite=overwrite, sr=sr)
         elif filename.suffix == ".em" or filename.suffix == ".ems":
             ImageEM().write(data, filename, overwrite=overwrite, sr=sr)
 
-    def convert(self, orig_file, dest_file, overwrite=False):
+    def convert(self, orig_file, dest_file, overwrite=True):
         self.read(orig_file)
         data = self.getData()
         self.write(data, dest_file, sr=self.getSamplingRate(), overwrite=overwrite)
 
     def getData(self):
         return self[:]
 
@@ -169,17 +179,18 @@
         else:
             return None
 
     def setSamplingRate(self, input_file, sr):
         self.read(input_file)
         self.write(np.squeeze(self.getData()), sr=sr, overwrite=True)
 
-    def scaleSplines(self, inputFn, outputFn, scaleFactor=None, finalDimension=None,
-                     isStack=False, overwrite=False):
-        self.read(inputFn)
+    def scaleSplines(self, inputFn=None, outputFn=None, scaleFactor=None, finalDimension=None,
+                     isStack=False, overwrite=True):
+        if isinstance(inputFn, str):
+            self.read(inputFn)
         data = np.squeeze(self.getData())
 
         if finalDimension is None:
             if isStack:
                 aux = []
                 for slice in data:
                     aux.append(rescale(slice, scaleFactor))
@@ -205,18 +216,22 @@
                     finalDimension = finalDimension * np.ones(len(data.shape))
                 data = resize(data, finalDimension)
 
         scaleFactor = finalDimension[0] / data.shape[0] if scaleFactor is None else scaleFactor
         new_sr = self.getSamplingRate() / scaleFactor
         new_sr = new_sr if new_sr > 0.0 else 1.0
 
-        self.write(data, outputFn, sr=new_sr, overwrite=overwrite)
+        if isinstance(outputFn, str):
+            self.write(data, outputFn, sr=new_sr, overwrite=overwrite)
+        else:
+            return data
 
-    def affineTransform(self, inputFn, outputFn, transformation, isStack=False, overwrite=False):
-        self.read(inputFn)
+    def affineTransform(self, transformation, inputFn=None, outputFn=None, isStack=False, overwrite=True):
+        if isinstance(inputFn, str):
+            self.read(inputFn)
         data = np.squeeze(self.getData())
 
         # Transformation dim
         tr_dim = data.ndim if isStack else data.ndim + 1
 
         # Make transformation homogeneous (if not already)
         if transformation.shape[0] != tr_dim:
@@ -269,46 +284,97 @@
                 aux.append(warp(slice, coords))
             data = np.asarray(aux)
         else:
             data = warp(data, coords)
 
         sr = self.getSamplingRate() if self.getSamplingRate() > 0.0 else 1.0
 
-        self.write(data, outputFn, sr=sr, overwrite=overwrite)
+        if isinstance(outputFn, str):
+            self.write(data, outputFn, sr=sr, overwrite=overwrite)
+        else:
+            return data
 
-    def createCircularMask(self, outputFile, boxSize=None, radius=None, center=None, is3D=True,
+    def createCircularMask(self, outputFile=None, boxSize=None, radius=None, center=None, is3D=True,
                            sr=1.0):
         if boxSize is None and radius is None:
             raise ValueError("At least boxSize or radius should be set.")
 
         boxSize = int(2 * radius) if boxSize is None else boxSize
         radius = 0.5 * boxSize if radius is None else radius
-        center = (radius, radius) if center is None else center
+
+        if boxSize is not None:
+            center = (0.5 * boxSize, 0.5 * boxSize)
+        elif radius is not None:
+            center = (radius, radius)
 
         # Create circular mask
         if is3D:
             Z, Y, X = np.ogrid[:boxSize, :boxSize, :boxSize]
             dist_from_center = np.sqrt((X - center[0]) ** 2 + (Y - center[1]) ** 2 + (Z - center[1]) ** 2)
         else:
             Y, X = np.ogrid[:boxSize, :boxSize]
             dist_from_center = np.sqrt((X - center[0]) ** 2 + (Y - center[1]) ** 2)
 
         mask = dist_from_center <= radius
 
-        self.write(mask, outputFile, overwrite=True, sr=sr)
+        if isinstance(outputFile, str):
+            self.write(mask, outputFile, overwrite=True, sr=sr)
+        else:
+            return mask
 
-    def addNoise(self, input_file, output_file, std=1.0, avg=0.0, overwrite=False):
-        self.read(input_file)
+    def addNoise(self, input_file=None, output_file=None, std=1.0, avg=0.0, overwrite=True):
+        if isinstance(input_file, str):
+            self.read(input_file)
         data = np.squeeze(self.getData())
         noise = np.random.normal(loc=avg, scale=std, size=data.shape)
         data_noise = data + noise
-        self.write(data_noise, output_file, overwrite=overwrite, sr=self.getSamplingRate())
+        if isinstance(output_file, str):
+            self.write(data_noise, output_file, overwrite=overwrite, sr=self.getSamplingRate())
+        else:
+            return output_file
+
+    def __fillHull(self, image):
+        """
+        Compute the convex hull of the given binary image and
+        return a mask of the filled hull.
+
+        Adapted from:
+        https://stackoverflow.com/a/46314485/162094
+        This version is slightly (~40%) faster for 3D volumes,
+        by being a little more stingy with RAM.
+        """
+        # (The variable names below assume 3D input,
+        # but this would still work in 4D, etc.)
+
+        assert (np.array(image.shape) <= np.iinfo(np.int16).max).all(), \
+            f"This function assumes your image is smaller than {2 ** 15} in each dimension"
+
+        points = np.argwhere(image).astype(np.int16)
+        hull = ConvexHull(points)
+        deln = Delaunay(points[hull.vertices])
+
+        # Instead of allocating a giant array for all indices in the volume,
+        # just iterate over the slices one at a time.
+        idx_2d = np.indices(image.shape[1:], np.int16)
+        idx_2d = np.moveaxis(idx_2d, 0, -1)
+
+        idx_3d = np.zeros((*image.shape[1:], image.ndim), np.int16)
+        idx_3d[:, :, 1:] = idx_2d
+
+        mask = np.zeros_like(image, dtype=bool)
+        for z in range(len(image)):
+            idx_3d[:, :, 0] = z
+            s = deln.find_simplex(idx_3d)
+            mask[z, (s != -1)] = 1
+
+        return mask
 
     def generateMask(self, iterations=150, smoothing=0, lambda1=1, lambda2=2, std=1, boxsize=128,
-                     smoothStairEdges=False, keep_largest=True):
+                     smoothStairEdges=False, keep_largest=True, dust_size=None, convex=True, applyThreshold=True,
+                     threshold="otsu"):
         '''Generate automatically a binary protein mask based on a combination of snakes and
         Otsu method.
             :param int iterations: Number of iterations for computing the snake mask.
             :param int smoothing: Number of times the smoothing operator is applied per iteration.
                                   Reasonable values are around 0-4. Larger values lead to smoother
                                   segmentations.
             :param int lambda1: Weight parameter for the outer region. If `lambda1` is larger than
@@ -324,14 +390,21 @@
                                 The output size of the mask generated will keep the original map dimensions, even
                                 if this parameter is used
             :param bool smoothStairEdges: Smooth the snake mask borders to avoid stair caise like borders.
                                           We recommend setting it to True if boxsized downsamples the original map.
             :param bool keep_largest: Keep the largest component only detected by the snakes mask. This will help the
                                       posterior Otsu thresholding step to find the appropriate threshold to segment the
                                       protein.
+            :param str threshold: Threshold method use to improve the snakes masking. Valid options are:
+                                  ["isodata", "li", "mean", "minimum", "otsu", "triangle", "yen"]
+            :param float dust_size: Removes any connected component whose size is smaller than or equal to this value
+            :param bool convex: Determines whether to create convex mask from the estimated morphSnake mask before
+                                further processing it
+            :param bool applyThreshold: Determines whether to apply a final thresholding step to generate a tight mask
+                                        to the input image/volume
         '''
         # Read the data
         data = np.squeeze(self.getData())
         data_ori = data.copy()
 
         # Filter to remove noise (optional step)
         if std is not None:
@@ -358,23 +431,72 @@
             acwe_ls1 = labels == np.argmax(np.bincount(labels.flat)[1:]) + 1
 
         # Upscale mask (if downscaling was applied)
         if boxsize is not None:
             finalDimension = ori_boxsize * np.ones(len(data.shape))
             acwe_ls1 = resize(acwe_ls1.astype(bool), finalDimension).astype(np.float32)
 
+        # Remove dust
+        if dust_size is not None:
+            acwe_ls1 = opening(acwe_ls1.astype(bool), ball(5))
+            labels = label(acwe_ls1)
+            assert (labels.max() != 0)  # assume at least 1 CC
+            keep_regions = (np.argwhere(np.bincount(labels.flat)[1:] > dust_size) + 1)
+            aux = np.zeros(acwe_ls1.shape)
+            for lid in keep_regions:
+                aux += labels == lid
+            acwe_ls1 = aux.astype(np.float32)
 
         if smoothStairEdges:
             acwe_ls1 = (median_filter(acwe_ls1, size=5) >= 0.001).astype(np.float32)
-
-        data_ori = data_ori * acwe_ls1
-        acwe_ls1 = (data_ori >= filters.threshold_otsu(data_ori)).astype(np.float32)
+        
+        if convex:
+            acwe_ls1 = self.__fillHull(acwe_ls1.astype(bool)).astype(float)
+
+        if applyThreshold:
+            data_ori = data_ori * acwe_ls1
+            threshold_fun = getattr(filters, "threshold_" + threshold)
+            acwe_ls1 = (data_ori >= threshold_fun(data_ori)).astype(np.float32)
 
         return acwe_ls1
 
+    def generateProjections(self, num_projections, degrees=True, volume=None, n_jobs=8, pad=0, useFourier=True):
+        """
+        Generate 2D projections of a 3D volume uniformly over the projection sphere.
+
+        Args:
+            volume (numpy.ndarray): 3D numpy array representing the volume.
+            num_projections (int): Number of projections to generate.
+
+        Returns:
+            projections (list of numpy.ndarray): List containing 2D projections.
+            euler_angles (numpy.ndarray): Array of shape (num_projections, 3) containing
+                                          Euler angles in ZYZ format for each projection.
+        """
+        # Read the data
+        if volume is None:
+            volume = np.squeeze(self.getData())
+
+        theta, phi = fibonacci_hemisphere(num_projections)
+        rots = np.stack([compute_rotations(t, p) for t, p in zip(theta, phi)], axis=0)
+
+        if useFourier:
+            interpolator = FourierInterpolator(volume, pad=pad)
+        else:
+            interpolator = RealInterpolator(volume)
+
+        results = np.array(Parallel(n_jobs=n_jobs)(delayed(compute_projection)(rot, interpolator) for rot in rots),
+                           dtype=object)
+        projections, euler_angles = np.stack(results[:, 0], axis=0), np.stack(results[:, 1], axis=0)
+
+        if degrees:
+            euler_angles = np.rad2deg(euler_angles)
+
+        return projections, euler_angles
+
 
     def close(self):
         '''
         Close the current binary file
         '''
         if isinstance(self.BINARIES, ImageSpider):
             self.BINARIES.close()
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_mrc.py` & `xmipp_metadata-1.1.0/xmipp_metadata/image_handler/image_mrc.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,28 @@
 
 
 class ImageMRC(object):
     '''
     Class to read an MRC file
     '''
 
+    DEBUG = False
+
     def __init__(self, filename=None):
         if filename:
             self.read(filename)
         else:
             self.mrc_handle, self.header = None, None
 
     def __del__(self):
         '''
         Close the current file before deleting
         '''
-        print("File closed succesfully!")
+        if self.DEBUG:
+            print("File closed succesfully!")
 
     def __len__(self):
         return self.mrc_handle.header["nz"]
 
     def __iter__(self):
         '''
         Generator method to loop through all the images in the stack
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_spider.py` & `xmipp_metadata-1.1.0/xmipp_metadata/image_handler/image_spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,31 @@
     '''
     Class to read an STK image file generated with XMIPP
     '''
 
     HEADER_OFFSET = 1024
     FLOAT32_BYTES = 4
     TYPE = None
+    DEBUG = False
 
     def __init__(self, filename=None):
         if filename:
             self.stk_handler = open(filename, "rb")
             self.header_info = self.read_header()
             self.IMG_BYTES = self.FLOAT32_BYTES * self.header_info["n_columns"] ** 2
         else:
             self.stk_handler, self.header_info, self.IMG_BYTES = None, None, None
 
     def __del__(self):
         '''
         Close the current file before deleting
         '''
         self.close()
-        print("File closed succesfully!")
+        if self.DEBUG:
+            print("File closed succesfully!")
 
     def __len__(self):
         if self.TYPE == "stack":
             return self.header_info["n_images"]
         elif self.TYPE == "volume":
             return self.header_info["n_slices"]
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/metadata/__init__.py` & `xmipp_metadata-1.1.0/xmipp_metadata/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/tests/test_image_handler.py` & `xmipp_metadata-1.1.0/xmipp_metadata/tests/test_image_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,27 +24,35 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 
 import os
 import shutil
+
+import matplotlib.pyplot as plt
 from scipy.spatial.transform import Rotation as R
 import numpy as np
 import time
 
 from xmipp_metadata.image_handler import ImageHandler
+from xmipp_metadata.metadata import XmippMetaData
 
 
 # Change dir to correct path
 package_path = os.path.abspath(os.path.dirname(__file__))
 data_test_path = os.path.join(package_path, "data")
 os.chdir(data_test_path)
 
 
+# Create outputs dir
+if not os.path.isdir("test_outputs"):
+    os.mkdir("test_outputs")
+
+
 # Clean output tests dir
 for filename in os.listdir("test_outputs"):
     file_path = os.path.join("test_outputs", filename)
     try:
         if os.path.isfile(file_path) or os.path.islink(file_path):
             os.unlink(file_path)
         elif os.path.isdir(file_path):
@@ -67,15 +75,15 @@
 
 # Write image (MRC)
 ih.write(img, filename=os.path.join("test_outputs", "test.mrc"), sr=4.0)
 
 
 # Raise error due to wrong overwrite
 try:
-    ih.write(img)
+    ih.write(img, overwrite=False)
 except Exception as e:
     print("Error raised correctly!")
 
 
 # Write image stack (STK)
 img = ih[0:10]
 ih.write(img, filename=os.path.join("test_outputs", "test_stack.stk"), sr=4.0)
@@ -177,24 +185,24 @@
 
 
 # Warp stack (STK) (Rot 90º)
 angle = 0.5 * np.pi
 transform = np.eye(3)
 transform[:-1, :-1] = np.asarray([[np.cos(angle), -np.sin(angle)],
                                   [np.sin(angle), np.cos(angle)]])
-ImageHandler().affineTransform("scaled_particles.stk",
-                               os.path.join("test_outputs", "test_stack_tr.stk",),
+ImageHandler().affineTransform(inputFn="scaled_particles.stk",
+                               outputFn=os.path.join("test_outputs", "test_stack_tr.stk",),
                                transformation=transform, isStack=True)
 
 
 # Warp stack (VOL) (Rot 90º)
 transform = np.eye(4)
 transform[:-1, :-1] = R.from_euler("zyz", [0.0, 0.0, angle]).as_matrix()
-ImageHandler().affineTransform("AK.vol",
-                               os.path.join("test_outputs", "test_tr.vol"),
+ImageHandler().affineTransform(inputFn="AK.vol",
+                               outputFn=os.path.join("test_outputs", "test_tr.vol"),
                                transformation=transform, isStack=False)
 
 
 # Set sampling rate (VOL)
 ImageHandler().setSamplingRate(os.path.join("test_outputs", "test_tr.vol"), sr=8.0)
 
 
@@ -203,11 +211,43 @@
                         os.path.join("test_outputs", "test_tr.vol"),
                         avg=0.0, std=0.2, overwrite=True)
 
 
 # Generate mask (VOL)
 ih = ImageHandler(os.path.join("test_outputs", "test_tr.vol"))
 start_time = time.time()
-mask = ih.generateMask(iterations=50, boxsize=64, smoothStairEdges=False)
+mask = ih.generateMask(iterations=50, boxsize=64, smoothStairEdges=False, dust_size=50)
+end_time = time.time()
+print(end_time - start_time)
+ih.write(mask, os.path.join("test_outputs", "test_generated_mask.vol"), sr=ih.getSamplingRate())
+ih.write(ih.getData() * mask, os.path.join("test_outputs", "test_generated_masked.vol"), sr=ih.getSamplingRate())
+
+
+# Generate projections (Fourier)
+ih = ImageHandler(os.path.join("AK.vol"))
+volume = ih.scaleSplines(finalDimension=64)
+print("Generating Fourier projections...")
+start_time = time.time()
+projections, angles = ih.generateProjections(500, degrees=True, pad=0, useFourier=True, volume=volume,
+                                             n_jobs=20)
+end_time = time.time()
+print(end_time - start_time)
+ImageHandler().write(projections, os.path.join("test_outputs", "projections_fourier.stk"))
+ImageHandler().write(volume, os.path.join("test_outputs", "volume_to_poject_fourier.mrc"))
+md = XmippMetaData(os.path.join("test_outputs", "projections_fourier.stk"), angles=angles)
+md.setMetaDataColumns(np.ones(len(md)), "subtomo_labels")
+md.write(os.path.join("test_outputs", "projections_fourier.xmd"), updateImagePaths=True)
+
+# # Generate projections (Real)
+ih = ImageHandler(os.path.join("AK.vol"))
+volume = ih.scaleSplines(finalDimension=64)
+print("Generating real projections...")
+start_time = time.time()
+projections, angles = ih.generateProjections(500, degrees=True, pad=0, useFourier=False, volume=volume,
+                                             n_jobs=20)
 end_time = time.time()
 print(end_time - start_time)
-ih.write(mask, os.path.join("test_outputs", "test_generated_mask.vol"), sr=2.0)
+ImageHandler().write(projections, os.path.join("test_outputs", "projections_real.stk"))
+ImageHandler().write(volume, os.path.join("test_outputs", "volume_to_poject_real.mrc"))
+md = XmippMetaData(os.path.join("test_outputs", "projections_real.stk"), angles=angles)
+md.setMetaDataColumns(np.ones(len(md)), "subtomo_labels")
+md.write(os.path.join("test_outputs", "projections_real.xmd"), updateImagePaths=True)
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata/tests/test_metadata.py` & `xmipp_metadata-1.1.0/xmipp_metadata/tests/test_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,7 +60,12 @@
 
 # Write metadata (do not update paths)
 metadata.write(filename=os.path.join("test_outputs", "test_same_paths.xmd"))
 
 
 # Write metadata (update paths)
 metadata.write(filename=os.path.join("test_outputs", "test_new_paths.xmd"), updateImagePaths=True)
+
+
+# Merge metadata (duplicate entries)
+metadata.concatenateMetadata(metadata)
+metadata.write(filename=os.path.join("test_outputs", "test_merged_duplicated.xmd"))
```

### Comparing `xmipp_metadata-1.0.8/xmipp_metadata.egg-info/SOURCES.txt` & `xmipp_metadata-1.1.0/xmipp_metadata.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 xmipp_metadata/image_handler/image_handler.py
 xmipp_metadata/image_handler/image_mrc.py
 xmipp_metadata/image_handler/image_spider.py
 xmipp_metadata/metadata/__init__.py
 xmipp_metadata/metadata/xmipp_metadata.py
 xmipp_metadata/tests/__init__.py
 xmipp_metadata/tests/test_image_handler.py
-xmipp_metadata/tests/test_metadata.py
+xmipp_metadata/tests/test_metadata.py
+xmipp_metadata/tests/test_metadata_two_sets.py
```

