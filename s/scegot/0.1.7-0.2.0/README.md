# Comparing `tmp/scegot-0.1.7.tar.gz` & `tmp/scegot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scegot-0.1.7.tar", max compression
+gzip compressed data, was "scegot-0.2.0.tar", max compression
```

## Comparing `scegot-0.1.7.tar` & `scegot-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-09-27 02:07:19.257352 scegot-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0      747 2023-10-04 09:24:38.888769 scegot-0.1.7/README.md
--rw-r--r--   0        0        0     1323 2024-03-12 04:42:58.765323 scegot-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       44 2024-03-12 04:42:58.878089 scegot-0.1.7/scegot/__init__.py
--rw-r--r--   0        0        0    77823 2024-03-04 01:35:59.113272 scegot-0.1.7/scegot/scegot.py
--rw-r--r--   0        0        0     2303 1970-01-01 00:00:00.000000 scegot-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-15 02:27:47.445697 scegot-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      747 2024-05-15 02:27:47.445762 scegot-0.2.0/README.md
+-rw-r--r--   0        0        0     1325 2024-05-24 08:11:52.687560 scegot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2024-05-24 08:11:52.688437 scegot-0.2.0/scegot/__init__.py
+-rw-r--r--   0        0        0    78539 2024-05-24 08:11:52.688893 scegot-0.2.0/scegot/scegot.py
+-rw-r--r--   0        0        0     2323 1970-01-01 00:00:00.000000 scegot-0.2.0/PKG-INFO
```

### Comparing `scegot-0.1.7/LICENSE.txt` & `scegot-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scegot-0.1.7/README.md` & `scegot-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scegot-0.1.7/pyproject.toml` & `scegot-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "scegot"
-version = "0.1.7"
+version = "0.2.0"
 description = "single cell trajectory inference framework based on Entropic Gaussian mixture Optimal Transport"
 authors = ["Toshiaki Yachimura <toshiaki.yachimura.a4@tohoku.ac.jp>"]
 readme = "README.md"
 packages = [{include = "scegot/*.py"}]
 license = "MIT"
 homepage = "https://yachimura-lab.github.io/scEGOT/"
 repository = "https://github.com/yachimura-lab/scEGOT"
 documentation = "https://yachimura-lab.github.io/scEGOT/tutorial.html"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.9"
 scipy = "^1.11.4"
 scikit-learn = "^1.3.2"
-matplotlib = "<3.8.0"
+matplotlib = "^3.8.0"
 umap-learn = "^0.5.5"
 seaborn = "^0.13.1"
 natsort = "^8.4.0"
 POT = "^0.9.3"
 networkx = "^3.2.1"
 plotly = "^5.18.0"
 pydotplus = "^2.0.2"
 graphviz = "^0.20.1"
-anndata = "0.8"
-kaleido = "0.2.1"
+anndata = "^0.8"
+kaleido = "^0.2.1"
 cellmap = "^1.0.7"
 tqdm = "^4.66.1"
 screcode = "^0.2.5"
 llvmlite = "^0.41.1"
 pandas = "^2.2.0"
 numpy = "^1.26.3"
 pyarrow = "^15.0.0"
```

### Comparing `scegot-0.1.7/scegot/scegot.py` & `scegot-0.2.0/scegot/scegot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import itertools
-import ot
 import warnings
-import numpy as np
-import pandas as pd
+from io import BytesIO
+
 import anndata
 import cellmap
-from scipy import interpolate
-import scipy.linalg as spl
-from scipy.stats import multivariate_normal, zscore
-from scipy.sparse import csc_matrix, linalg, lil_matrix, issparse
-from sklearn import linear_model
-from sklearn.utils import check_random_state
-from sklearn.mixture import GaussianMixture
-from sklearn.neighbors import kneighbors_graph
-from sklearn.decomposition import PCA
-import umap.umap_ as umap
-import matplotlib.pyplot as plt
 import matplotlib.animation as animation
-from matplotlib.colors import ListedColormap
-from matplotlib import patheffects
+import matplotlib.pyplot as plt
 import networkx as nx
+import numpy as np
+import ot
+import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
-from IPython.display import Image, HTML, display
+import pydotplus
+import scipy.linalg as spl
 import screcode
 import seaborn as sns
-import pydotplus
-from tqdm import tqdm
-from io import BytesIO
-from PIL import Image as PILImage
+import umap.umap_ as umap
 from adjustText import adjust_text
+from IPython.display import HTML, Image, display
+from matplotlib import patheffects
+from matplotlib.colors import ListedColormap
+from PIL import Image as PILImage
+from scipy import interpolate
+from scipy.sparse import csc_matrix, issparse, lil_matrix, linalg
+from scipy.stats import multivariate_normal, zscore
+from sklearn import linear_model
+from sklearn.decomposition import PCA
+from sklearn.mixture import GaussianMixture
+from sklearn.neighbors import kneighbors_graph
+from sklearn.utils import check_random_state
+from tqdm import tqdm
 
 sns.set_style("whitegrid")
 
 
 def is_notebook() -> bool:
     try:
         from IPython import get_ipython
@@ -396,15 +397,15 @@
             plt.scatter(X_item.values[:, 0], X_item.values[:, 1], s=1.0, alpha=0.8)
         else:
             plt.scatter(
                 X_item.values[:, 0],
                 X_item.values[:, 1],
                 c=gmm_label,
                 alpha=0.5,
-                cmap=plt.cm.get_cmap(cmap, gmm_n_components),
+                cmap=plt.get_cmap(cmap, gmm_n_components),
             )
             plt.colorbar(ticks=range(gmm_n_components), label="cluster")
             plt.clim(-0.5, gmm_n_components - 0.5)
 
         if figure_labels is not None:
             plt.xlabel(figure_labels[0])
             plt.ylabel(figure_labels[1])
@@ -714,15 +715,18 @@
             node_info["cluster_gmm"] = list(
                 itertools.chain.from_iterable(self.gmm_label_converter)
             )
 
         node_sortby_weight = (
             node_info.reset_index()
             .groupby("node_days")
-            .apply(lambda x: x.sort_values("node_weights", ascending=False), include_groups=False)
+            .apply(
+                lambda x: x.sort_values("node_weights", ascending=False),
+                include_groups=False,
+            )
         )
         node_sortby_weight = node_sortby_weight.reset_index()
         node_info = pd.DataFrame(
             node_sortby_weight.values, columns=node_sortby_weight.columns
         )
         node_info["cluster_weight"] = list(
             itertools.chain.from_iterable(
@@ -963,15 +967,15 @@
             pos = {}
             for node in G.nodes():
                 if order is None:
                     pos[node] = (G.nodes[node]["day"], -G.nodes[node]["cluster_gmm"])
                 else:
                     pos[node] = (G.nodes[node]["day"], -G.nodes[node]["cluster_weight"])
         fig, ax = plt.subplots(figsize=(12, 10))
-        
+
         # draw edge border
         nx.draw(
             G,
             pos,
             node_size=[node["weight"] * 4500 for node in G.nodes.values()],
             node_color="white",
             edge_color="black",
@@ -989,15 +993,15 @@
             edge_color="white",
             arrows=True,
             arrowsize=30,
             linewidths=2,
             ax=ax,
             width=5.0,
         )
-        
+
         # draw edges
         node_cmap = (
             plt.cm.tab10(np.arange(10))
             if len(self.X_raw) <= 10
             else plt.cm.tab20(np.arange(20))
         )
         nx.draw(
@@ -1028,15 +1032,15 @@
                 ha="center",
                 va="center",
             )
             text_.set_path_effects(
                 [patheffects.withStroke(linewidth=3, foreground="w")]
             )
             texts.append(text_)
-            
+
         if layout == "normal":
             adjust_text(texts)
 
         plt.show()
 
         if save:
             fig.savefig(save_path, dpi=200, bbox_inches="tight")
@@ -1257,14 +1261,23 @@
 
         if save:
             fig.write_image(save_path)
 
     def plot_pathway_single_gene_2d(
         self, gene_name, mode="pca", col=None, save=False, save_path=None
     ):
+        warnings.warn(
+            "scegot.plot_pathway_single_gene_2d() will be depricated. Use scegot.plot_gene_expression_2d() instead.",
+            FutureWarning,
+        )
+        self.plot_gene_expression_2d(gene_name, mode, col, save, save_path)
+
+    def plot_gene_expression_2d(
+        self, gene_name, mode="pca", col=None, save=False, save_path=None
+    ):
         if mode not in ["pca", "umap"]:
             raise ValueError("The parameter 'mode' should be 'pca' or 'umap'.")
 
         if save and save_path is None:
             save_path = "./pathway_single_gene_2d.png"
 
         X_concated = pd.concat(self.X_pca if mode == "pca" else self.X_umap)
@@ -1286,14 +1299,21 @@
 
         if save:
             fig.write_image(save_path)
 
     def plot_pathway_single_gene_3d(
         self, gene_name, col=None, save=False, save_path=None
     ):
+        warnings.warn(
+            "scegot.plot_pathway_single_gene_3d() will be depricated. Use scegot.plot_gene_expression_3d() instead.",
+            FutureWarning,
+        )
+        self.plot_gene_expression_3d(gene_name, col, save, save_path)
+
+    def plot_gene_expression_3d(self, gene_name, col=None, save=False, save_path=None):
         if save and save_path is None:
             save_path = "./pathway_single_gene_3d.html"
 
         X_concated = pd.concat(self.X_pca)
         if col:
             x_col, y_col, z_col = col
         else:
@@ -1464,19 +1484,19 @@
         plt.xlabel(x_col_name)
         plt.ylabel(y_col_name)
         plt.xlim(x_range)
         plt.ylim(y_range)
         plt.legend(loc=0)
         plt.title("true and interpolation distributions")
 
-        plt.show()
-
         if save:
             plt.savefig(save_path)
 
+        plt.show()
+
     def animate_gene_expression(
         self,
         target_gene_name,
         mode="pca",
         interpolate_interval=11,
         n_samples=5000,
         x_range=None,
@@ -1660,17 +1680,17 @@
                 velocity = (
                     self.umap_model.transform(velocity + self.X_pca[i].values)
                     - self.X_umap[i]
                 )
 
             velocity = pd.DataFrame(
                 velocity,
-                columns=self.X_pca[0].columns
-                if mode == "pca"
-                else self.X_umap[0].columns,
+                columns=(
+                    self.X_pca[0].columns if mode == "pca" else self.X_umap[0].columns
+                ),
             )
             velocities = pd.concat([velocities, velocity])
 
         return velocities
 
     def plot_cell_velocity(
         self,
@@ -1694,16 +1714,15 @@
         x_coordinate = X_concated.iloc[:, 0]
         y_coordinate = X_concated.iloc[:, 1]
 
         x_velocity = velocities.iloc[:, 0]
         y_velocity = velocities.iloc[:, 1]
 
         speed = [
-            np.sqrt(x_vel**2 + y_vel**2)
-            for x_vel, y_vel in zip(x_velocity, y_velocity)
+            np.sqrt(x_vel**2 + y_vel**2) for x_vel, y_vel in zip(x_velocity, y_velocity)
         ]
 
         plt.figure(figsize=(10, 8))
         plt.quiver(
             x_coordinate,
             y_coordinate,
             x_velocity / speed,
@@ -1803,15 +1822,15 @@
             density=3.0,
         )
         if color_points in ["gmm", "day"]:
             scatter = plt.scatter(
                 pd.concat(X).iloc[:, 0],
                 pd.concat(X).iloc[:, 1],
                 c=colors,
-                cmap=plt.cm.get_cmap(cmap, len(set(colors))),
+                cmap=plt.get_cmap(cmap, len(set(colors))),
                 s=20,
                 alpha=0.5,
             )
             if color_points == "gmm" and cluster_names is not None:
                 handles = scatter.legend_elements(num=list(range(len(cluster_names))))[
                     0
                 ]
```

### Comparing `scegot-0.1.7/PKG-INFO` & `scegot-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: scegot
-Version: 0.1.7
+Version: 0.2.0
 Summary: single cell trajectory inference framework based on Entropic Gaussian mixture Optimal Transport
 Home-page: https://yachimura-lab.github.io/scEGOT/
 License: MIT
 Author: Toshiaki Yachimura
 Author-email: toshiaki.yachimura.a4@tohoku.ac.jp
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: POT (>=0.9.3,<0.10.0)
-Requires-Dist: anndata (==0.8)
+Requires-Dist: anndata (>=0.8,<0.9)
 Requires-Dist: cellmap (>=1.0.7,<2.0.0)
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
-Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: kaleido (>=0.2.1,<0.3.0)
 Requires-Dist: llvmlite (>=0.41.1,<0.42.0)
-Requires-Dist: matplotlib (<3.8.0)
+Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
 Requires-Dist: natsort (>=8.4.0,<9.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydotplus (>=2.0.2,<3.0.0)
```

