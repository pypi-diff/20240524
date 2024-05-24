# Comparing `tmp/diso-0.1.2.tar.gz` & `tmp/diso-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diso-0.1.2.tar", last modified: Thu Apr 11 04:01:13 2024, max compression
+gzip compressed data, was "diso-0.1.3.tar", last modified: Thu May 23 20:39:59 2024, max compression
```

## Comparing `diso-0.1.2.tar` & `diso-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-04-11 04:01:13.896841 diso-0.1.2/
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)      185 2024-04-08 20:12:31.000000 diso-0.1.2/LICENSE
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)       13 2024-04-08 20:12:31.000000 diso-0.1.2/MANIFEST.in
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     1027 2024-04-11 04:01:13.896841 diso-0.1.2/PKG-INFO
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     5047 2024-04-08 20:12:31.000000 diso-0.1.2/README.md
-drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-04-11 04:01:13.896841 diso-0.1.2/diso/
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     6465 2024-04-11 03:43:32.000000 diso-0.1.2/diso/__init__.py
-drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-04-11 04:01:13.896841 diso-0.1.2/diso.egg-info/
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     1027 2024-04-11 04:01:13.000000 diso-0.1.2/diso.egg-info/PKG-INFO
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)      290 2024-04-11 04:01:13.000000 diso-0.1.2/diso.egg-info/SOURCES.txt
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        1 2024-04-11 04:01:13.000000 diso-0.1.2/diso.egg-info/dependency_links.txt
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        1 2024-04-09 18:45:17.000000 diso-0.1.2/diso.egg-info/not-zip-safe
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        8 2024-04-11 04:01:13.000000 diso-0.1.2/diso.egg-info/requires.txt
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        5 2024-04-11 04:01:13.000000 diso-0.1.2/diso.egg-info/top_level.txt
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)       38 2024-04-11 04:01:13.896841 diso-0.1.2/setup.cfg
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     2596 2024-04-11 04:00:46.000000 diso-0.1.2/setup.py
-drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-04-11 04:01:13.896841 diso-0.1.2/src/
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    49634 2024-04-08 20:12:31.000000 diso-0.1.2/src/cudualmc.cu
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     4597 2024-04-08 20:12:31.000000 diso-0.1.2/src/cudualmc.h
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    36173 2024-04-08 20:12:31.000000 diso-0.1.2/src/cumc.cu
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     4282 2024-04-08 20:12:31.000000 diso-0.1.2/src/cumc.h
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    15997 2024-04-08 20:12:31.000000 diso-0.1.2/src/pybind.cpp
+drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-05-23 20:39:59.670632 diso-0.1.3/
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)      185 2024-04-08 20:12:31.000000 diso-0.1.3/LICENSE
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)       13 2024-04-08 20:12:31.000000 diso-0.1.3/MANIFEST.in
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     1027 2024-05-23 20:39:59.670632 diso-0.1.3/PKG-INFO
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     5439 2024-05-23 20:39:19.000000 diso-0.1.3/README.md
+drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-05-23 20:39:59.670632 diso-0.1.3/diso/
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     6402 2024-05-23 20:35:15.000000 diso-0.1.3/diso/__init__.py
+drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-05-23 20:39:59.670632 diso-0.1.3/diso.egg-info/
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     1027 2024-05-23 20:39:59.000000 diso-0.1.3/diso.egg-info/PKG-INFO
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)      290 2024-05-23 20:39:59.000000 diso-0.1.3/diso.egg-info/SOURCES.txt
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        1 2024-05-23 20:39:59.000000 diso-0.1.3/diso.egg-info/dependency_links.txt
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        1 2024-05-15 19:11:31.000000 diso-0.1.3/diso.egg-info/not-zip-safe
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        8 2024-05-23 20:39:59.000000 diso-0.1.3/diso.egg-info/requires.txt
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        5 2024-05-23 20:39:59.000000 diso-0.1.3/diso.egg-info/top_level.txt
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)       38 2024-05-23 20:39:59.670632 diso-0.1.3/setup.cfg
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     2596 2024-05-23 20:39:34.000000 diso-0.1.3/setup.py
+drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-05-23 20:39:59.670632 diso-0.1.3/src/
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    49716 2024-05-23 20:35:15.000000 diso-0.1.3/src/cudualmc.cu
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     4621 2024-05-23 20:35:15.000000 diso-0.1.3/src/cudualmc.h
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    36252 2024-05-23 20:35:15.000000 diso-0.1.3/src/cumc.cu
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     4306 2024-05-23 20:35:15.000000 diso-0.1.3/src/cumc.h
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    15969 2024-05-23 20:35:15.000000 diso-0.1.3/src/pybind.cpp
```

### Comparing `diso-0.1.2/PKG-INFO` & `diso-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diso
-Version: 0.1.2
+Version: 0.1.3
 Summary: Differentiable Iso-Surface Extraction Package
 Author-email: xiwei@ucsd.edu
 License: CC BY-NC 4.0
 Keywords: differentiable iso-surface extraction
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `diso-0.1.2/README.md` & `diso-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # Differentiable Iso-Surface Extraction Package (DISO)
+[***News***] DISO now supports batch training and checkpointing! It is no longer necessary to allocate multiple iso-surface extractors.
+
 This repository consists of a variety of differentiable iso-surface extraction algorithms implemented in `cuda`.
 
 Currently, two algorithms are incorporated:
 * Differentiable **Marching Cubes** [1] (DiffMC)
 * Differentiable **Dual Marching Cubes** [2] (DiffDMC)
 
 The differentiable iso-surface algorithms have multiple applications in gradient-based optimization, such as shape, texture, materials reconstruction from images.
@@ -34,34 +36,36 @@
 from diso import DiffDMC
 
 diffmc = DiffMC(dtype=torch.float32).cuda() # or dtype=torch.float64
 diffdmc = DiffDMC(dtype=torch.float32).cuda() # or dtype=torch.float64
 ```
 Then use its `forward` function to generate a single mesh:
 ```
-verts, faces = diffmc(sdf, deform)  # or deform=None
-verts, faces = diffdmc(sdf, deform)  # or deform=None
+verts, faces = diffmc(sdf, deform, normalize=True)  # or deform=None
+verts, faces = diffdmc(sdf, deform, return_quads=False, normalize=True)  # or deform=None
 ```
 
 Input
-* `sdf`: queries SDF values on the grid vertices (see the `test.py` for how to create the grid). The gradient will be back-propagated to the source that generates the SDF values. (**[N, N, N, 3]**)
+* `sdf`: queries SDF values on the grid vertices (see the `test/example.py` for how to create the grid). The gradient will be back-propagated to the source that generates the SDF values. (**[N, N, N, 3]**)
 * `deform (optional)`: (learnable) deformation values on the grid vertices, the range must be [-0.5, 0.5], default=None.  (**[N, N, N, 3]**)
+* `normalize`: whether to normalize the output vertices, default=True. If set to **True**, the vertices are normalized to [0, 1]. When **False**, the vertices remain unnormalized as [0, dim-1], 
+* `return_quads`: whether return quad meshes; only applicable for DiffDMC, default=False. If set to **True**, the function returns quad meshes (**[F, 4]**).
 
 Output
-* `verts`: mesh vertices within the range of [0, 1]. (**[V, 3]**)
-* `faces`: mesh face indices (starting from 0). (**[F, 3]**). Note `DiffMC` can return quads with `return_quads` set as True.
+* `verts`: mesh vertices within the range of [0, 1] or [0, dim-1]. (**[V, 3]**)
+* `faces`: mesh face indices (starting from 0). (**[F, 3]**).
 
 The gradient will be automatically computed when `backward` function is called.
 
 # Batch Training
-Each instance of `diffmc` or `diffdmc` can handle only a single shape because it saves intermediate results for the backward pass. If you wish to implement batch training, you can construct `batchsize` extractors as follows:
+You can loop over the batch size to conduct an iso-surface extraction on each object, then compute the loss for the backward pass.
 ```
-extractors = [DiffMC(dtype=torch.float32).cuda() for i in batchsize]
+extractor = DiffMC(dtype=torch.float32).cuda()  # or DiffDMC
 for bs in range(batchsize):
-    verts, faces = extractors[bs](sdf, deform)
+    verts, faces = extractor(sdf, deform)
     # compute and accumulate losses
 loss.backward()
 ```
 Note: It is suggested to create the extractors outside the `epoch` loop so that they can be reused by different iterations and avoid allocating memory every time.
 
 # Speed Comparison
 We compare our library with DMTet [3] and FlexiCubes [4] on two examples: a simple round cube and a random initialized signed distance function.
```

### Comparing `diso-0.1.2/diso/__init__.py` & `diso-0.1.3/diso/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,54 +3,53 @@
 import torch.nn.functional as F
 from torch.autograd import Function
 
 from . import _C
 
 
 class DiffMC(nn.Module):
-    def __init__(self, dtype=torch.float32, device="cuda:0"):
+    def __init__(self, dtype=torch.float32):
         super().__init__()
         self.dtype = dtype
         if dtype == torch.float32:
             mc = _C.CUMCFloat()
         elif dtype == torch.float64:
             mc = _C.CUMCDouble()
-        torch.cuda.set_device(device)
 
         class DMCFunction(Function):
             @staticmethod
             def forward(ctx, grid, deform, isovalue):
                 if deform is None:
                     verts, tris = mc.forward(grid, isovalue)
                 else:
                     verts, tris = mc.forward(grid, deform, isovalue)
-                ctx.grid = grid
-                ctx.deform = deform
                 ctx.isovalue = isovalue
+                ctx.save_for_backward(grid, deform)
                 return verts, tris
 
             @staticmethod
             def backward(ctx, adj_verts, adj_faces):
-                adj_grid = torch.zeros_like(ctx.grid)
-                if ctx.deform is None:
+                grid, deform = ctx.saved_tensors
+                DMCFunction.forward(ctx, grid, deform, ctx.isovalue)
+                adj_grid = torch.zeros_like(grid)
+                if deform is None:
                     mc.backward(
-                        ctx.grid, ctx.isovalue, adj_verts, adj_grid
+                        grid, ctx.isovalue, adj_verts, adj_grid
                     )
                     return adj_grid, None, None, None, None
                 else:
-                    adj_deform = torch.zeros_like(ctx.deform)
+                    adj_deform = torch.zeros_like(deform)
                     mc.backward(
-                        ctx.grid, ctx.deform, ctx.isovalue, adj_verts, adj_grid, adj_deform
+                        grid, deform, ctx.isovalue, adj_verts, adj_grid, adj_deform
                     )
                     return adj_grid, adj_deform, None, None, None
 
         self.func = DMCFunction
 
-    def forward(self, grid, deform=None, isovalue=0.0, device="cuda:0", normalize=True):
-        torch.cuda.set_device(device)
+    def forward(self, grid, deform=None, isovalue=0.0, normalize=True):
         if grid.min() >= 0 or grid.max() <= 0:
             return torch.zeros((0, 3), dtype=self.dtype, device=grid.device), torch.zeros((0, 3), dtype=torch.int32, device=grid.device)
         dimX, dimY, dimZ = grid.shape
         grid = F.pad(grid, (1, 1, 1, 1, 1, 1), "constant", 1)
         if deform is not None:
             deform = F.pad(deform, (0, 0, 1, 1, 1, 1, 1, 1), "constant", 0)
         verts, tris = self.func.apply(grid, deform, isovalue)
@@ -58,54 +57,53 @@
         if normalize:
             verts = verts / (
                 torch.tensor([dimX, dimY, dimZ], dtype=verts.dtype, device=verts.device) - 1
             )
         return verts, tris.long()
 
 class DiffDMC(nn.Module):
-    def __init__(self, dtype=torch.float32, device="cuda:0"):
+    def __init__(self, dtype=torch.float32):
         super().__init__()
         self.dtype = dtype
         if dtype == torch.float32:
             dmc = _C.CUDMCFloat()
         elif dtype == torch.float64:
             dmc = _C.CUDMCDouble()
-        torch.cuda.set_device(device)
 
         class DDMCFunction(Function):
             @staticmethod
             def forward(ctx, grid, deform, isovalue):
                 if deform is None:
                     verts, quads = dmc.forward(grid, isovalue)
                 else:
                     verts, quads = dmc.forward(grid, deform, isovalue)
-                ctx.grid = grid
-                ctx.deform = deform
                 ctx.isovalue = isovalue
+                ctx.save_for_backward(grid, deform)
                 return verts, quads
 
             @staticmethod
             def backward(ctx, adj_verts, adj_faces):
-                adj_grid = torch.zeros_like(ctx.grid)
-                if ctx.deform is None:
+                grid, deform = ctx.saved_tensors
+                DDMCFunction.forward(ctx, grid, deform, ctx.isovalue)
+                adj_grid = torch.zeros_like(grid)
+                if deform is None:
                     dmc.backward(
-                        ctx.grid, ctx.isovalue, adj_verts, adj_grid
+                        grid, ctx.isovalue, adj_verts, adj_grid
                     )
                     return adj_grid, None, None, None, None
                 else:
-                    adj_deform = torch.zeros_like(ctx.deform)
+                    adj_deform = torch.zeros_like(deform)
                     dmc.backward(
-                        ctx.grid, ctx.deform, ctx.isovalue, adj_verts, adj_grid, adj_deform
+                        grid, deform, ctx.isovalue, adj_verts, adj_grid, adj_deform
                     )
                     return adj_grid, adj_deform, None, None, None
 
         self.func = DDMCFunction
 
-    def forward(self, grid, deform=None, isovalue=0.0, return_quads=False, device="cuda:0", normalize=True):
-        torch.cuda.set_device(device)
+    def forward(self, grid, deform=None, isovalue=0.0, return_quads=False, normalize=True):
         if grid.min() >= 0 or grid.max() <= 0:
             return torch.zeros((0, 3), dtype=self.dtype, device=grid.device), torch.zeros((0, 4), dtype=torch.int32, device=grid.device)
         dimX, dimY, dimZ = grid.shape
         grid = F.pad(grid, (1, 1, 1, 1, 1, 1), "constant", 1)
         if deform is not None:
             deform = F.pad(deform, (0, 0, 1, 1, 1, 1, 1, 1), "constant", 0)
         verts, quads = self.func.apply(grid, deform, isovalue)
```

### Comparing `diso-0.1.2/diso.egg-info/PKG-INFO` & `diso-0.1.3/diso.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diso
-Version: 0.1.2
+Version: 0.1.3
 Summary: Differentiable Iso-Surface Extraction Package
 Author-email: xiwei@ucsd.edu
 License: CC BY-NC 4.0
 Keywords: differentiable iso-surface extraction
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `diso-0.1.2/setup.py` & `diso-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             extra_compile_args=extra_compile_args,
         )
     ]
     return ext_modules
 
 setup(
     name="diso",
-    version="0.1.2",
+    version="0.1.3",
     author_email="xiwei@ucsd.edu",
     keywords="differentiable iso-surface extraction",
     description="Differentiable Iso-Surface Extraction Package",
     classifiers=[
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Intended Audience :: Developers",
```

### Comparing `diso-0.1.2/src/cudualmc.cu` & `diso-0.1.3/src/cudualmc.cu`

 * *Files 0% similar despite different names*

```diff
@@ -1053,17 +1053,18 @@
           get_quad_index(dmc, dmc.first_cell_used[dmc.gA(x + dx, y + dy, z + dz)], eid);
     }
     dmc.quads[quad_index] = q;
   }
 
   template <typename Scalar, typename IndexType>
   void CUDualMC<Scalar, IndexType>::forward(Scalar const *d_data, Vertex<Scalar> const *d_deform, IndexType dimX, IndexType dimY,
-                                            IndexType dimZ, Scalar iso)
+                                            IndexType dimZ, Scalar iso, int device)
   {
-
+    cudaSetDevice(device);
+    
     resize(dimX, dimY, dimZ);
 
     size_t temp_storage_bytes = 0;
 
     ensure_cell_storage_size(n_cells);
 
     // find and index used cells
@@ -1125,16 +1126,17 @@
 
     create_quads_kernel<<<(n_quads + BLOCK_SIZE - 1) / BLOCK_SIZE, BLOCK_SIZE>>>(*this);
   }
 
   template <typename Scalar, typename IndexType>
   void CUDualMC<Scalar, IndexType>::backward(Scalar const *d_data, Vertex<Scalar> const *d_deform, IndexType dimX, IndexType dimY,
                                              IndexType dimZ, Scalar iso, Scalar *adj_d_data, Vertex<Scalar> *adj_d_deform,
-                                             Vertex<Scalar> const *adj_verts)
+                                             Vertex<Scalar> const *adj_verts, int device)
   {
+    cudaSetDevice(device);
     adj_create_dmc_verts_kernel<<<(n_used_cells + BLOCK_SIZE - 1) / BLOCK_SIZE, BLOCK_SIZE>>>(
         *this, d_data, d_deform, iso, adj_d_data, adj_d_deform, adj_verts);      
   }
 
   template struct Vertex<float>;
   template struct Vertex<double>;
   template struct Quad<int>;
```

### Comparing `diso-0.1.2/src/cudualmc.h` & `diso-0.1.3/src/cudualmc.h`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,14 @@
     __host__ void ensure_cell_storage_size(size_t cell_count);
     __host__ void ensure_used_cell_storage_size(size_t cell_count);
     __host__ void ensure_quad_storage_size(size_t quad_count);
     __host__ void ensure_vert_storage_size(size_t vert_count);
     __host__ void ensure_edge_storage_size(size_t edge_count);
 
     __host__ void forward(Scalar const *d_data, Vertex<Scalar> const *d_deform, IndexType dimX, IndexType dimY, IndexType dimZ,
-                          Scalar iso);
+                          Scalar iso, int device);
     __host__ void backward(Scalar const *d_data, Vertex<Scalar> const *d_deform, IndexType dimX, IndexType dimY,
                            IndexType dimZ, Scalar iso, Scalar *adj_d_data, Vertex<Scalar> *adj_d_deform,
-                           Vertex<Scalar> const *adj_verts);
+                           Vertex<Scalar> const *adj_verts, int device);
   };
 
 } // namespace cudualmc
```

### Comparing `diso-0.1.2/src/cumc.cu` & `diso-0.1.3/src/cumc.cu`

 * *Files 0% similar despite different names*

```diff
@@ -646,16 +646,17 @@
     //   mc.tris[firstOut + j] = {id_i, id_j, id_k};
     //   j++;
     // }
   }
 
   template <typename Scalar, typename IndexType>
   void CuMC<Scalar, IndexType>::forward(Scalar const *d_data, Vertex<Scalar> const *d_deform, IndexType dimX, IndexType dimY,
-                                        IndexType dimZ, Scalar iso)
+                                        IndexType dimZ, Scalar iso, int device)
   {
+    cudaSetDevice(device);
 
     resize(dimX, dimY, dimZ);
 
     size_t temp_storage_bytes = 0;
 
     ensure_cell_storage_size(n_cells);
 
@@ -729,16 +730,18 @@
     n_tris/=3;
 
   }
 
   template <typename Scalar, typename IndexType>
   void CuMC<Scalar, IndexType>::backward(Scalar const *d_data, Vertex<Scalar> const *d_deform, IndexType dimX, IndexType dimY,
                                          IndexType dimZ, Scalar iso, Scalar *adj_d_data, Vertex<Scalar> *adj_d_deform,
-                                         Vertex<Scalar> const *adj_verts)
+                                         Vertex<Scalar> const *adj_verts, int device)
   {
+    cudaSetDevice(device);
+
     adj_create_cell_mc_verts_kernel<<<(n_used_cells + BLOCK_SIZE - 1) / BLOCK_SIZE, BLOCK_SIZE>>>(
         *this, d_data, d_deform, iso, adj_d_data, adj_d_deform, adj_verts);
   }
 
   template struct Vertex<float>;
   template struct Vertex<double>;
   template struct Triangle<int>;
```

### Comparing `diso-0.1.2/src/cumc.h` & `diso-0.1.3/src/cumc.h`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,14 @@
     __host__ void ensure_cell_storage_size(size_t cell_count);
     __host__ void ensure_used_cell_storage_size(size_t cell_count);
     __host__ void ensure_vert_type_storage_size(size_t vert_count);
     __host__ void ensure_tri_storage_size(size_t tri_count);
     __host__ void ensure_vert_storage_size(size_t vert_count);
 
     __host__ void forward(Scalar const *d_data, Vertex<Scalar> const *d_deform, IndexType dimX, IndexType dimY, IndexType dimZ,
-                          Scalar iso);
+                          Scalar iso, int device);
     __host__ void backward(Scalar const *d_data, Vertex<Scalar> const *d_deform, IndexType dimX, IndexType dimY,
                            IndexType dimZ, Scalar iso, Scalar *adj_d_data, Vertex<Scalar> *adj_d_deform,
-                           Vertex<Scalar> const *adj_verts);
+                           Vertex<Scalar> const *adj_verts, int device);
   };
 
 } // namespace cumc
```

### Comparing `diso-0.1.2/src/pybind.cpp` & `diso-0.1.3/src/pybind.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -69,25 +69,25 @@
         indexType = torch::kLong;
       }
 
       IndexType dimX = grid.size(0);
       IndexType dimY = grid.size(1);
       IndexType dimZ = grid.size(2);
 
-      mc.forward(grid.data_ptr<Scalar>(), reinterpret_cast<Vertex<Scalar> *>(deform.data_ptr<Scalar>()), dimX, dimY, dimZ, iso);
+      mc.forward(grid.data_ptr<Scalar>(), reinterpret_cast<Vertex<Scalar> *>(deform.data_ptr<Scalar>()), dimX, dimY, dimZ, iso, grid.device().index());
 
       auto verts =
           torch::from_blob(
               mc.verts, torch::IntArrayRef{mc.n_verts, 3},
-              torch::TensorOptions().device(torch::kCUDA).dtype(scalarType))
+              grid.options().dtype(scalarType))
               .clone();
       auto tris =
           torch::from_blob(
               mc.tris, torch::IntArrayRef{mc.n_tris, 3},
-              torch::TensorOptions().device(torch::kCUDA).dtype(indexType))
+              grid.options().dtype(indexType))
               .clone();
 
       return {verts, tris};
     }
 
     std::tuple<torch::Tensor, torch::Tensor> forward(torch::Tensor grid,
                                                      Scalar iso)
@@ -116,25 +116,25 @@
         indexType = torch::kLong;
       }
 
       IndexType dimX = grid.size(0);
       IndexType dimY = grid.size(1);
       IndexType dimZ = grid.size(2);
 
-      mc.forward(grid.data_ptr<Scalar>(), NULL, dimX, dimY, dimZ, iso);
+      mc.forward(grid.data_ptr<Scalar>(), NULL, dimX, dimY, dimZ, iso, grid.device().index());
 
       auto verts =
           torch::from_blob(
               mc.verts, torch::IntArrayRef{mc.n_verts, 3},
-              torch::TensorOptions().device(torch::kCUDA).dtype(scalarType))
+              grid.options().dtype(scalarType))
               .clone();
       auto tris =
           torch::from_blob(
               mc.tris, torch::IntArrayRef{mc.n_tris, 3},
-              torch::TensorOptions().device(torch::kCUDA).dtype(indexType))
+              grid.options().dtype(indexType))
               .clone();
 
       return {verts, tris};
     }
 
     void backward(torch::Tensor grid, torch::Tensor deform, Scalar iso, torch::Tensor adj_verts,
                   torch::Tensor adj_grid, torch::Tensor adj_deform)
@@ -162,15 +162,15 @@
       IndexType dimX = grid.size(0);
       IndexType dimY = grid.size(1);
       IndexType dimZ = grid.size(2);
 
       mc.backward(
           grid.data_ptr<Scalar>(), reinterpret_cast<Vertex<Scalar> *>(deform.data_ptr<Scalar>()), dimX, dimY, dimZ, iso,
           adj_grid.data_ptr<Scalar>(), reinterpret_cast<Vertex<Scalar> *>(adj_deform.data_ptr<Scalar>()),
-          reinterpret_cast<Vertex<Scalar> *>(adj_verts.data_ptr<Scalar>()));
+          reinterpret_cast<Vertex<Scalar> *>(adj_verts.data_ptr<Scalar>()), grid.device().index());
     }
 
     void backward(torch::Tensor grid, Scalar iso, torch::Tensor adj_verts,
                   torch::Tensor adj_grid)
     {
       CHECK_INPUT(adj_verts);
       CHECK_INPUT(adj_grid);
@@ -192,15 +192,16 @@
       IndexType dimX = grid.size(0);
       IndexType dimY = grid.size(1);
       IndexType dimZ = grid.size(2);
 
       mc.backward(
           grid.data_ptr<Scalar>(), NULL, dimX, dimY, dimZ, iso,
           adj_grid.data_ptr<Scalar>(), NULL,
-          reinterpret_cast<Vertex<Scalar> *>(adj_verts.data_ptr<Scalar>()));
+          reinterpret_cast<Vertex<Scalar> *>(adj_verts.data_ptr<Scalar>()),
+          grid.device().index());
     }
   };
 
 } // namespace cumc
 
 namespace cudualmc
 {
@@ -261,25 +262,25 @@
         indexType = torch::kLong;
       }
 
       IndexType dimX = grid.size(0);
       IndexType dimY = grid.size(1);
       IndexType dimZ = grid.size(2);
 
-      dmc.forward(grid.data_ptr<Scalar>(), reinterpret_cast<Vertex<Scalar> *>(deform.data_ptr<Scalar>()), dimX, dimY, dimZ, iso);
+      dmc.forward(grid.data_ptr<Scalar>(), reinterpret_cast<Vertex<Scalar> *>(deform.data_ptr<Scalar>()), dimX, dimY, dimZ, iso, grid.device().index());
 
       auto verts =
           torch::from_blob(
               dmc.verts, torch::IntArrayRef{dmc.n_verts, 3},
-              torch::TensorOptions().device(torch::kCUDA).dtype(scalarType))
+              grid.options().dtype(scalarType))
               .clone();
       auto quads =
           torch::from_blob(
               dmc.quads, torch::IntArrayRef{dmc.n_quads, 4},
-              torch::TensorOptions().device(torch::kCUDA).dtype(indexType))
+              grid.options().dtype(indexType))
               .clone();
 
       return {verts, quads};
     }
 
     std::tuple<torch::Tensor, torch::Tensor> forward(torch::Tensor grid,
                                                      Scalar iso)
@@ -308,25 +309,25 @@
         indexType = torch::kLong;
       }
 
       IndexType dimX = grid.size(0);
       IndexType dimY = grid.size(1);
       IndexType dimZ = grid.size(2);
 
-      dmc.forward(grid.data_ptr<Scalar>(), NULL, dimX, dimY, dimZ, iso);
+      dmc.forward(grid.data_ptr<Scalar>(), NULL, dimX, dimY, dimZ, iso, grid.device().index());
 
       auto verts =
           torch::from_blob(
               dmc.verts, torch::IntArrayRef{dmc.n_verts, 3},
-              torch::TensorOptions().device(torch::kCUDA).dtype(scalarType))
+              grid.options().dtype(scalarType))
               .clone();
       auto quads =
           torch::from_blob(
               dmc.quads, torch::IntArrayRef{dmc.n_quads, 4},
-              torch::TensorOptions().device(torch::kCUDA).dtype(indexType))
+              grid.options().dtype(indexType))
               .clone();
 
       return {verts, quads};
     }
 
     void backward(torch::Tensor grid, torch::Tensor deform, Scalar iso, torch::Tensor adj_verts,
                   torch::Tensor adj_grid, torch::Tensor adj_deform)
@@ -354,15 +355,15 @@
       IndexType dimX = grid.size(0);
       IndexType dimY = grid.size(1);
       IndexType dimZ = grid.size(2);
 
       dmc.backward(
           grid.data_ptr<Scalar>(), reinterpret_cast<Vertex<Scalar> *>(deform.data_ptr<Scalar>()), dimX, dimY, dimZ, iso,
           adj_grid.data_ptr<Scalar>(), reinterpret_cast<Vertex<Scalar> *>(adj_deform.data_ptr<Scalar>()),
-          reinterpret_cast<Vertex<Scalar> *>(adj_verts.data_ptr<Scalar>()));
+          reinterpret_cast<Vertex<Scalar> *>(adj_verts.data_ptr<Scalar>()), grid.device().index());
     }
 
     void backward(torch::Tensor grid, Scalar iso, torch::Tensor adj_verts,
                   torch::Tensor adj_grid)
     {
       CHECK_INPUT(adj_verts);
       CHECK_INPUT(adj_grid);
@@ -384,15 +385,16 @@
       IndexType dimX = grid.size(0);
       IndexType dimY = grid.size(1);
       IndexType dimZ = grid.size(2);
 
       dmc.backward(
           grid.data_ptr<Scalar>(), NULL, dimX, dimY, dimZ, iso,
           adj_grid.data_ptr<Scalar>(), NULL,
-          reinterpret_cast<Vertex<Scalar> *>(adj_verts.data_ptr<Scalar>()));
+          reinterpret_cast<Vertex<Scalar> *>(adj_verts.data_ptr<Scalar>()),
+          grid.device().index());
     }
   };
 
 } // namespace cudualmc
 
 template <class C>
 void register_mc_class(pybind11::module m, std::string name)
```

