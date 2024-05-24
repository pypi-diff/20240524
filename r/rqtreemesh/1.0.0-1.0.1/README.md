# Comparing `tmp/rqtreemesh-1.0.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/rqtreemesh-1.0.1-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 68285 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   129536 b- defN 24-Mar-17 16:10 _rqtreemesh.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     5768 b- defN 24-Mar-17 16:03 rqtreemesh/__init__.py
--rw-rw-rw-  2.0 fat     1233 b- defN 24-Mar-17 16:10 rqtreemesh-1.0.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4969 b- defN 24-Mar-17 16:10 rqtreemesh-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 24-Mar-17 16:10 rqtreemesh-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-Mar-17 16:10 rqtreemesh-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      581 b- defN 24-Mar-17 16:10 rqtreemesh-1.0.0.dist-info/RECORD
-7 files, 142217 bytes uncompressed, 67257 bytes compressed:  52.7%
+Zip file size: 70590 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat   133120 b- defN 24-May-24 13:26 _rqtreemesh.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     6667 b- defN 24-May-24 13:19 rqtreemesh/__init__.py
+-rw-rw-rw-  2.0 fat     1233 b- defN 24-May-24 13:26 rqtreemesh-1.0.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     5530 b- defN 24-May-24 13:26 rqtreemesh-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 24-May-24 13:26 rqtreemesh-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 24-May-24 13:26 rqtreemesh-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      581 b- defN 24-May-24 13:26 rqtreemesh-1.0.1.dist-info/RECORD
+7 files, 147261 bytes uncompressed, 69562 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: _rqtreemesh.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: rqtreemesh/__init__.py
 Comment: 
 
-Filename: rqtreemesh-1.0.0.dist-info/LICENSE.txt
+Filename: rqtreemesh-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: rqtreemesh-1.0.0.dist-info/METADATA
+Filename: rqtreemesh-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: rqtreemesh-1.0.0.dist-info/WHEEL
+Filename: rqtreemesh-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: rqtreemesh-1.0.0.dist-info/top_level.txt
+Filename: rqtreemesh-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rqtreemesh-1.0.0.dist-info/RECORD
+Filename: rqtreemesh-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rqtreemesh/__init__.py

```diff
@@ -137,7 +137,33 @@
                               str((1 - 2 * flip_zy) * vert[2 - flip_zy]),
                               "\n"]))
         f.write("\n")
         for triangle in triangles:
             f.write(" ".join(["f", str(int(triangle[0] + 1)),
                               str(int(triangle[1] + 1)),
                               str(int(triangle[2] + 1)), "\n"]))
+
+def write_stl(path: str, verts: np.ndarray, triangles: np.ndarray):
+    """
+    Export a generated mesh to a .stl file.
+
+    Parameters:
+    ----------
+    path: str
+        Output file path.
+    verts : np.ndarray
+        A numpy array where each row contains the x, y and z coordinates of a
+        vertex.
+    triangles : np.ndarray
+        A connectivity matrix as a numpy array, i.e each row contains a
+        triangle as three (zero-indexed) indices into verts.
+    """
+    verts = np.float32(verts)
+    if not issubclass(triangles.dtype.type, np.integer):
+        triangles = np.uint64(triangles)
+    with open(path, "wb") as f:
+        f.write(bytearray(80))
+        f.write(np.uint32(len(triangles)).tobytes())
+        for triangle in triangles:
+            f.write(bytearray(12))
+            f.write(verts[triangle].tobytes())
+            f.write(bytearray(2))
```

## Comparing `rqtreemesh-1.0.0.dist-info/LICENSE.txt` & `rqtreemesh-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `rqtreemesh-1.0.0.dist-info/METADATA` & `rqtreemesh-1.0.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqtreemesh
-Version: 1.0.0
+Version: 1.0.1
 Summary: An implementation of restricted quadtree triangulation (RQT), for converting raster heightmaps to 3D meshes.
 Home-page: https://github.com/philipschall/rqtreemesh
 Author: Philip Schall
 Author-email: philip.schall@live.com
 License: Unlicense
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -39,14 +39,18 @@
 
 Implemented in C++ with a pybind11 wrapper for Python.
 
 ## Quick Start
 
 `git clone --recursive` this repo and run `pip install .` on it.
 
+Alternatively:
+
+`pip install rqtreemesh`.
+
 This package requires `Numpy` and `Pillow`.
 
 ### Usage
 Functionality is provided by the `Heightmap` class. 
 ```python
 from rqtreemesh import Heightmap
 ```
@@ -80,14 +84,16 @@
 **Parameters**
 
  ```python
  path: str
  ```
  > Path to input raster heightmap in geoTIFF format with dimesnsions a power of two. E.g. 1024 x 2048. Maximum size is 32768 x 32768. The geolocation and spatial resolution of the heightmap will be obtained from the appropriate tags in the geoTIFF.
 ***
+Note that **rqtreemesh** was developed for converting Digital Elevation Models (DEMs) . For other heightmaps, such as where all values are between $0$ and $1$, scaling the `Heightmap.array` or `Heightmap.pixel_dim` may be necessary to obtain the desired result. Also take care when converting a DEM with planar units not equal to its elevation units (e.g. Geographic/WGS84 projection).
+***
 To generate a mesh, use the `generate_mesh` method.
 ```python
 heightmap = Heightmap...
 (vertices, triangles) = heightmap.generate_mesh(max_error: float, show_progress: bool = False) -> Tuple[np.ndarray, np.ndarray]
 ```
 **Parameters**
 ```python
@@ -102,32 +108,33 @@
 
 **Returns**
 ```python
 (vertices, triangles): Tuple[np.ndarray, np.ndarray]
 ```
 >A tuple containing the output mesh. `vertices` is an array where each row contains the x, y and z coordinates of a vertex. `triangles` is a connectivity matrix, i.e. an array where each row contains a triangle as three (zero-indexed) indices into the first element.
 ***
-To provide easy compatibility with most 3D software, a simple exporter to the Wavefront Object (.obj) format is also provided:
+To provide easy compatibility with most 3D software, basic exporters to the Wavefront Object (.obj) and Stereolithography (.stl) formats are provided:
 ```python
-from rqtreemesh import write_obj
+from rqtreemesh import write_obj, write_stl
 write_obj(path: str, verts: np.ndarray, triangles: np.ndarray, flip_zy: bool = False)
+write_stl(path: str, verts: np.ndarray, triangles: np.ndarray)
 ```
 **Parameters**
 ```python
 path: str
 ```
 >The output file path.
 ```python
 verts: np.ndarray, triangles: np.ndarray
 ```
 > A coordinate array and connectivity matrix, such as the output of `generate_mesh`.
 ```python
 flip_zy: bool = True
 ```
->Interchange the z and y axes of the exported mesh. Default value: False.
+>Interchange the z and y axes of the exported mesh (only for .obj export). Default value: False.
 ***
 <center>
 	<figure>
 	  <img src="https://github.com/philipschall/rqtreemesh/blob/main/images/ex.gif?raw=true">
 	  <figcaption><i>Triangulation of a 2 meter per pixel resolution heightmap of East Pawnee Butte, Colorado. A maximum error of 0 meters results in a mesh consisting of 32768 triangles (left). A maximum error of 0.5 meters produces 8156 triangles (middle), and a  maximum error of 1 meter produces 4074 triangles (right). </i></figcaption>
 	</figure>
 </center>
```

