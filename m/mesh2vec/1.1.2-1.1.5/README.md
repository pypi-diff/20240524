# Comparing `tmp/mesh2vec-1.1.2-py3-none-any.whl.zip` & `tmp/mesh2vec-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 23496 bytes, number of entries: 11
+Zip file size: 23989 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh2vec/__init__.py
--rw-r--r--  2.0 unx     7170 b- defN 80-Jan-01 00:00 mesh2vec/helpers.py
--rw-r--r--  2.0 unx    20114 b- defN 80-Jan-01 00:00 mesh2vec/mesh2vec_base.py
--rw-r--r--  2.0 unx    34326 b- defN 80-Jan-01 00:00 mesh2vec/mesh2vec_cae.py
--rw-r--r--  2.0 unx     4612 b- defN 80-Jan-01 00:00 mesh2vec/mesh2vec_exceptions.py
--rw-r--r--  2.0 unx    12133 b- defN 80-Jan-01 00:00 mesh2vec/mesh_features.py
+-rw-r--r--  2.0 unx     7172 b- defN 80-Jan-01 00:00 mesh2vec/helpers.py
+-rw-r--r--  2.0 unx    20115 b- defN 80-Jan-01 00:00 mesh2vec/mesh2vec_base.py
+-rw-r--r--  2.0 unx    34477 b- defN 80-Jan-01 00:00 mesh2vec/mesh2vec_cae.py
+-rw-r--r--  2.0 unx     4613 b- defN 80-Jan-01 00:00 mesh2vec/mesh2vec_exceptions.py
+-rw-r--r--  2.0 unx    14032 b- defN 80-Jan-01 00:00 mesh2vec/mesh_features.py
 -rw-r--r--  2.0 unx     2054 b- defN 80-Jan-01 00:00 mesh2vec/templates/ansa.py
--rw-r--r--  2.0 unx     1065 b- defN 80-Jan-01 00:00 mesh2vec-1.1.2.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 mesh2vec-1.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3857 b- defN 16-Jan-01 00:00 mesh2vec-1.1.2.dist-info/METADATA
-?rw-r--r--  2.0 unx      867 b- defN 16-Jan-01 00:00 mesh2vec-1.1.2.dist-info/RECORD
-11 files, 86286 bytes uncompressed, 22046 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx     1065 b- defN 80-Jan-01 00:00 mesh2vec-1.1.5.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 mesh2vec-1.1.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     3857 b- defN 16-Jan-01 00:00 mesh2vec-1.1.5.dist-info/METADATA
+?rw-r--r--  2.0 unx      867 b- defN 16-Jan-01 00:00 mesh2vec-1.1.5.dist-info/RECORD
+11 files, 88340 bytes uncompressed, 22539 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: mesh2vec/mesh_features.py
 Comment: 
 
 Filename: mesh2vec/templates/ansa.py
 Comment: 
 
-Filename: mesh2vec-1.1.2.dist-info/LICENSE
+Filename: mesh2vec-1.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: mesh2vec-1.1.2.dist-info/WHEEL
+Filename: mesh2vec-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: mesh2vec-1.1.2.dist-info/METADATA
+Filename: mesh2vec-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: mesh2vec-1.1.2.dist-info/RECORD
+Filename: mesh2vec-1.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mesh2vec/helpers.py

```diff
@@ -1,15 +1,17 @@
 """helper functions"""
+
 from typing import OrderedDict, List, Dict
 from collections import deque
 from abc import ABC, abstractmethod
 
 import numpy as np
 from scipy.sparse import csr_array, coo_array, eye
 
+
 # pylint: disable=invalid-name
 class AbstractAdjacencyStrategy(ABC):
     # pylint: disable=too-few-public-methods
     """
     Abstract class for adjacency finding strategies
     """
```

## mesh2vec/mesh2vec_base.py

```diff
@@ -1,8 +1,9 @@
 """Mesh2VecBase"""
+
 import collections
 from pathlib import Path
 from typing import List, Optional, Callable, OrderedDict, Dict, Union, Iterable
 
 import networkx
 import numpy as np
 import pandas as pd
```

## mesh2vec/mesh2vec_cae.py

```diff
@@ -1,8 +1,9 @@
 """Mesh2VecCae"""
+
 import json
 import os
 import subprocess
 from collections import defaultdict
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import List, DefaultDict, Optional, Callable, Union, Tuple, Dict, Any
@@ -250,36 +251,40 @@
             selected_elements_part_indexes
         ]
         element_info["file_path"] = str(d3plot)
 
         return Mesh2VecCae(distance, mesh, element_info, calc_strategy=calc_strategy)
 
     @staticmethod
-    def from_keyfile_shell(distance: int, keyfile: Path, calc_strategy="bfs") -> "Mesh2VecCae":
+    def from_keyfile_shell(
+        distance: int, keyfile: Path, partid="", calc_strategy="bfs"
+    ) -> "Mesh2VecCae":
         """
         Read the given keyfile and use the shell elements to generate a hypergraph, using mesh
         nodes as hyperedges, and adjacent elements as hypervertices.
 
         Args:
             distance: the maximum distance for neighborhood generation and feature aggregation
             keyfile: path to keyfile
+            partid: part id to use for hypergraph generation
+                (default empty string, use all shell parts)
             calc_strategy: choose the algorithm to calculate adjacencies
 
                 * "dfs": depth first search (defaultl fast)
                 * "bfs": breadth first search (low memory consumption)
                 * "matmul": matrix multiplication (deprecated, for compatibility only)
 
         Example:
             >>> from pathlib import Path
             >>> from mesh2vec.mesh2vec_cae import Mesh2VecCae
             >>> m2v = Mesh2VecCae.from_keyfile_shell(4, Path("data/hat/Hatprofile.k"))
             >>> len(m2v._hyper_edges)
             6666
         """
-        mesh = CaeShellMesh.from_keyfile(keyfile)
+        mesh = CaeShellMesh.from_keyfile(keyfile, partid)
         element_info = pd.DataFrame({"element_id": mesh.element_ids})
         element_info["file_path"] = str(keyfile)
         return Mesh2VecCae(distance, mesh, element_info, calc_strategy=calc_strategy)
 
     def get_elements_info(self) -> pd.DataFrame:
         """
         Return a Pandas dataframe containing a row for each element in the hypergraph
@@ -343,15 +348,15 @@
         """
         # pylint: disable=too-many-locals
         okay_ansa = ["aspect", "warpage", "normal", "area", "skew"]
         okay_inplace = ["num_border", "is_tria", "midpoint"]
 
         for feature in features:
             if not feature in okay_ansa + okay_inplace:
-                if not allow_additional_ansa_features:
+                if allow_additional_ansa_features:
                     okay_ansa.append(feature)
                 else:
                     raise ValueError(
                         f"Feature {feature} is unknown and allow_additional_ansa_features "
                         f"is False. All features must be in {okay_ansa+okay_inplace}"
                     )
```

## mesh2vec/mesh2vec_exceptions.py

```diff
@@ -1,8 +1,9 @@
 """Exceptions for mesh2vec"""
+
 from typing import Any, Dict, List
 from loguru import logger
 import numpy as np
 
 
 class InvalidDistanceArgumentException(Exception):
     """Exception raised when an invalid distance was provided"""
```

## mesh2vec/mesh_features.py

```diff
@@ -1,8 +1,9 @@
 """calculation of mesh based features"""
+
 from typing import Tuple, List, Any, Optional
 
 import numpy as np
 import numpy.typing
 import pandas as pd
 import trimesh
 from lasso.dyna import D3plot, ArrayType
@@ -30,25 +31,29 @@
     return tri_faces, tri_features
 
 
 def _quad_to_tris(element_node_idxs: np.ndarray) -> Tuple[List[bool], np.ndarray]:
     if len(element_node_idxs.shape) == 3:  # points
         is_quads = [any(element[3] != element[2]) for element in element_node_idxs]
         tri_faces_nested = [
-            [element[:3].tolist(), element[[0, 2, 3]].tolist()]
-            if is_quad
-            else [element[:3].tolist()]
+            (
+                [element[:3].tolist(), element[[0, 2, 3]].tolist()]
+                if is_quad
+                else [element[:3].tolist()]
+            )
             for is_quad, element in zip(is_quads, element_node_idxs)
         ]
     else:
         is_quads = [element[3] != element[2] for element in element_node_idxs]
         tri_faces_nested = [
-            [element[:3].tolist(), element[[0, 2, 3]].tolist()]
-            if is_quad
-            else [element[:3].tolist()]
+            (
+                [element[:3].tolist(), element[[0, 2, 3]].tolist()]
+                if is_quad
+                else [element[:3].tolist()]
+            )
             for is_quad, element in zip(is_quads, element_node_idxs)
         ]
     tri_faces = np.array([tri_face for tri_faces in tri_faces_nested for tri_face in tri_faces])
     return is_quads, tri_faces
 
 
 def quads_to_tris_df(
@@ -121,18 +126,20 @@
 ) -> numpy.typing.NDArray[np.string_]:
     """replace overlapping values in array by adding nodes ids to element id"""
     if len(array) == len(np.unique(array)):
         return array
     cumcounts = pd.DataFrame(array, columns=["ids"]).groupby("ids").cumcount().values
     return np.array(
         [
-            old_id
-            if postfix == 0
-            else f"{old_id}_{point_uid[e[0]]}_{point_uid[e[1]]}_"
-            f"{point_uid[e[2]]}_{point_uid[e[3]]}"
+            (
+                old_id
+                if postfix == 0
+                else f"{old_id}_{point_uid[e[0]]}_{point_uid[e[1]]}_"
+                f"{point_uid[e[2]]}_{point_uid[e[3]]}"
+            )
             for old_id, e, postfix in zip(array, element_node_idxs, cumcounts)
         ]
     )
 
 
 class CaeShellMesh:
     """dataclass for points and elements"""
@@ -233,60 +240,88 @@
         ]
         elem_node_idxs = np.array(
             [[pnt_idx[element[f"N{i}"]] for i in range(1, 5)] for element in elements]
         )  # duplicate ids allowed?
         return CaeShellMesh(point_coordinates, pnt_ids, elem_ids, elem_node_idxs)
 
     @staticmethod
-    def from_keyfile(keyfile: str) -> "CaeShellMesh":
+    def from_keyfile(keyfile: str, partid: str = "") -> "CaeShellMesh":
         """
         create CaeShellMesh from keyfile
-            Example:
+
+        Args:
+            keyfile: path to LSDYNA keyfile in fixed column format
+            partid: part id to use for hypergraph generation
+
+        Example:
         >>> from mesh2vec.mesh_features import CaeShellMesh
         >>> mesh = CaeShellMesh.from_keyfile("data/hat/Hatprofile.k")
         >>> print(mesh.point_coordinates.shape)
         (6400, 3)
         """
 
+        # pylint: disable=too-many-branches, too-many-nested-blocks
         def parse_contents(file_contents):
             lines = file_contents.split("\n")
             current_section = ""
 
             point_coordinates = []
             pnt_ids = []
 
             elem_ids = []
             elem_node_ids = []
-
+            thickcard_options_set = set(["THICKNESS", "BETA", "MCID"])
             for line in lines:
                 if line.startswith("*"):
                     current_section = line.split()[0].upper()
+                    current_section_options = set(current_section.split("_")[1:])
+                    current_section_lines_per_entry = 1
+                    current_section_lineno = 0
                     continue
-                if line.startswith("$#"):  # comment
+                if line.startswith("$"):  # comment
                     continue
-
                 if current_section == "*NODE":
-                    data = line.split()
-                    if data:
-                        point_coordinates.append([float(data[1]), float(data[2]), float(data[3])])
-                        pnt_ids.append(data[0])
-
-                elif "*ELEMENT_SHELL" in current_section:
-                    data = line.split()
-                    if data:
-                        # check for floats - floats are a hint of options like THICKNESS
-                        if (
-                            not data[2].isdigit()
-                            or not data[3].isdigit()
-                            or not data[4].isdigit()
-                            or not data[5].isdigit()
-                        ):
-                            continue
-                        elem_node_ids.append([data[2], data[3], data[4], data[5]])
-                        elem_ids.append(data[0])
+                    try:
+                        point_coordinates.append(
+                            [float(line[8 + i * 16 : 8 + (i + 1) * 16]) for i in range(3)]
+                        )
+                        pnt_ids.append(line[:8].strip())
+                    except [ValueError, IndexError]:
+                        pass
+                elif current_section.startswith("*ELEMENT_SHELL"):
+
+                    if current_section_lineno % current_section_lines_per_entry == 0:
+                        if partid == "" or partid == line[8:16].strip():
+                            node_ids = [
+                                line[16 + i * 8 : 16 + (i + 1) * 8].strip() for i in range(8)
+                            ]
+                            node_ids = [
+                                node_id
+                                for node_id in node_ids
+                                if len(node_id) > 0 and node_id != "0"
+                            ]
+                            # pylint: disable=fixme
+                            # TODO: Check for unhandled options, e.g. COMPOSITE, DOF
+                            if current_section_lineno == 0:
+                                if len(current_section_options & thickcard_options_set) > 0:
+                                    current_section_lines_per_entry += 1  # skip thickness card
+                                    if len(node_ids) > 4:
+                                        current_section_lines_per_entry += (
+                                            1  # skip additional thickness card for mid-side nodes
+                                        )
+                                if "OFFSET" in current_section_options:
+                                    current_section_lines_per_entry += 1  # skip offset card
+                            elem_node_ids.append(
+                                [node_id for node_id in node_ids if len(node_id) > 0]
+                            )
+                            if node_ids[0] == 1.0:
+                                print("HERE")
+                            elem_ids.append(line[:8].strip())
+                    current_section_lineno += 1
+
             pnt_idx = {pnt_id: i for i, pnt_id in enumerate(pnt_ids)}
 
             elem_node_idx = np.array(
                 [[pnt_idx[elem_node_id[i]] for i in range(4)] for elem_node_id in elem_node_ids]
             )
 
             return point_coordinates, pnt_ids, elem_ids, elem_node_idx
```

## Comparing `mesh2vec-1.1.2.dist-info/LICENSE` & `mesh2vec-1.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mesh2vec-1.1.2.dist-info/METADATA` & `mesh2vec-1.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesh2vec
-Version: 1.1.2
+Version: 1.1.5
 Summary: mesh2vec
 Author: Renumics GmbH
 Author-email: info@renumics.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,15 +23,15 @@
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pillow (>=10.0.1,<11.0.0)
 Requires-Dist: plotly (>=5.11.0,<6.0.0)
 Requires-Dist: py (>=1.11.0,<2.0.0)
 Requires-Dist: pyglet (>=1.5.26,<2.0.0)
 Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: trimesh (>=3.14.1,<4.0.0)
-Requires-Dist: werkzeug (>=2.2.3,<3.0.0)
+Requires-Dist: werkzeug (>=3.0.3,<4.0.0)
 Description-Content-Type: text/markdown
 
 Mesh2Vec
 ========
 
 Quickstart
 -----------
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: mesh2vec Version: 1.1.2 Summary: mesh2vec Author:
+Metadata-Version: 2.1 Name: mesh2vec Version: 1.1.5 Summary: mesh2vec Author:
 Renumics GmbH Author-email: info@renumics.com Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: cleo (>=2.0.1,<3.0.0) Requires-Dist:
 igraph (>=0.11.3,<0.12.0) Requires-Dist: ipython (>=8.10.0,<9.0.0) Requires-
 Dist: joblib (>=1.2.0,<2.0.0) Requires-Dist: jupyter-server (>=2.11.2,<3.0.0)
 Requires-Dist: lasso-python (>=1.5.2.post1,<2.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: networkx (>=2.8.6,<3.0.0) Requires-Dist:
 notebook (>=6.5.2,<7.0.0) Requires-Dist: numba (>=0.58.1,<0.59.0) Requires-
 Dist: pandas (>=1.4.4,<2.0.0) Requires-Dist: pillow (>=10.0.1,<11.0.0)
 Requires-Dist: plotly (>=5.11.0,<6.0.0) Requires-Dist: py (>=1.11.0,<2.0.0)
 Requires-Dist: pyglet (>=1.5.26,<2.0.0) Requires-Dist: scipy (>=1.9.1,<2.0.0)
 Requires-Dist: trimesh (>=3.14.1,<4.0.0) Requires-Dist: werkzeug
-(>=2.2.3,<3.0.0) Description-Content-Type: text/markdown Mesh2Vec ========
+(>=3.0.3,<4.0.0) Description-Content-Type: text/markdown Mesh2Vec ========
 Quickstart -----------
                             ************ mmeesshh22vveecc ************
        Turn CAE mesh data into aggregated element feature vectors for ML
       _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_r_e_n_u_m_i_c_s_/_m_e_s_h_2_v_e_c_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_m_e_s_h_2_v_e_c_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_w_h_e_e_l_/
                                    _m_e_s_h_2_v_e_c_]
                         ******** _LL_aa_tt_ee_ss_tt_ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ********
```

