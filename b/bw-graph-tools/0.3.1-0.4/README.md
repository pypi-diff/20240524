# Comparing `tmp/bw_graph_tools-0.3.1.tar.gz` & `tmp/bw_graph_tools-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_graph_tools-0.3.1.tar", last modified: Sun May 12 02:21:12 2024, max compression
+gzip compressed data, was "bw_graph_tools-0.4.tar", last modified: Fri May 24 13:54:21 2024, max compression
```

## Comparing `bw_graph_tools-0.3.1.tar` & `bw_graph_tools-0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 02:21:12.876002 bw_graph_tools-0.3.1/
--rw-r--r--   0 cmutel     (501) staff       (20)     1456 2024-05-12 00:14:28.000000 bw_graph_tools-0.3.1/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2024-05-12 00:14:20.000000 bw_graph_tools-0.3.1/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     4881 2024-05-12 02:21:12.875817 bw_graph_tools-0.3.1/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     3201 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 02:21:12.872735 bw_graph_tools-0.3.1/bw_graph_tools/
--rw-r--r--   0 cmutel     (501) staff       (20)      603 2024-05-12 01:52:38.000000 bw_graph_tools-0.3.1/bw_graph_tools/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)      123 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/bw_graph_tools/errors.py
--rw-r--r--   0 cmutel     (501) staff       (20)    25946 2024-05-12 02:13:01.000000 bw_graph_tools-0.3.1/bw_graph_tools/graph_traversal.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2077 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/bw_graph_tools/graph_traversal_utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9280 2024-05-12 01:31:09.000000 bw_graph_tools-0.3.1/bw_graph_tools/matrix_tools.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7924 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/bw_graph_tools/shortest_path.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1295 2024-05-12 02:11:22.000000 bw_graph_tools-0.3.1/bw_graph_tools/testing.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 02:21:12.875157 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     4881 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      601 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      205 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       15 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/top_level.txt
--rw-r--r--   0 cmutel     (501) staff       (20)     2478 2024-05-12 02:00:32.000000 bw_graph_tools-0.3.1/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2024-05-12 02:21:12.876048 bw_graph_tools-0.3.1/setup.cfg
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 02:21:12.874764 bw_graph_tools-0.3.1/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)     7001 2024-05-12 01:36:14.000000 bw_graph_tools-0.3.1/tests/test_first_heuristic.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2494 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/tests/test_get_path_from_matrix.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1176 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/tests/test_matrix_utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4782 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/tests/test_second_heuristic.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3670 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/tests/test_third_heuristic.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 13:54:21.568507 bw_graph_tools-0.4/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1456 2024-05-12 00:14:28.000000 bw_graph_tools-0.4/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2024-05-12 00:14:20.000000 bw_graph_tools-0.4/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     4879 2024-05-24 13:54:21.568301 bw_graph_tools-0.4/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     3201 2024-05-11 23:47:54.000000 bw_graph_tools-0.4/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 13:54:21.565100 bw_graph_tools-0.4/bw_graph_tools/
+-rw-r--r--   0 cmutel     (501) staff       (20)      601 2024-05-24 13:51:37.000000 bw_graph_tools-0.4/bw_graph_tools/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      123 2024-05-11 23:47:54.000000 bw_graph_tools-0.4/bw_graph_tools/errors.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    27026 2024-05-24 13:08:36.000000 bw_graph_tools-0.4/bw_graph_tools/graph_traversal.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2035 2024-05-24 13:23:33.000000 bw_graph_tools-0.4/bw_graph_tools/graph_traversal_utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9311 2024-05-24 13:23:33.000000 bw_graph_tools-0.4/bw_graph_tools/matrix_tools.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8025 2024-05-24 13:23:33.000000 bw_graph_tools-0.4/bw_graph_tools/shortest_path.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1296 2024-05-24 13:23:32.000000 bw_graph_tools-0.4/bw_graph_tools/testing.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 13:54:21.567408 bw_graph_tools-0.4/bw_graph_tools.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4879 2024-05-24 13:54:21.000000 bw_graph_tools-0.4/bw_graph_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      601 2024-05-24 13:54:21.000000 bw_graph_tools-0.4/bw_graph_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-24 13:54:21.000000 bw_graph_tools-0.4/bw_graph_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      205 2024-05-24 13:54:21.000000 bw_graph_tools-0.4/bw_graph_tools.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       15 2024-05-24 13:54:21.000000 bw_graph_tools-0.4/bw_graph_tools.egg-info/top_level.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)     2478 2024-05-12 02:00:32.000000 bw_graph_tools-0.4/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)       38 2024-05-24 13:54:21.568544 bw_graph_tools-0.4/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-24 13:54:21.567183 bw_graph_tools-0.4/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)     7001 2024-05-12 01:36:14.000000 bw_graph_tools-0.4/tests/test_first_heuristic.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2553 2024-05-24 13:23:33.000000 bw_graph_tools-0.4/tests/test_get_path_from_matrix.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1176 2024-05-11 23:47:54.000000 bw_graph_tools-0.4/tests/test_matrix_utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4698 2024-05-24 13:23:33.000000 bw_graph_tools-0.4/tests/test_second_heuristic.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3600 2024-05-24 13:23:33.000000 bw_graph_tools-0.4/tests/test_third_heuristic.py
```

### Comparing `bw_graph_tools-0.3.1/LICENSE` & `bw_graph_tools-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3.1/PKG-INFO` & `bw_graph_tools-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_graph_tools
-Version: 0.3.1
+Version: 0.4
 Summary: Graph traversal class and utilities
 Author-email: Chris Mutel <cmutel@gmail.com>
 Maintainer-email: Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_graph_tools
 Project-URL: homepage, https://github.com/brightway-lca/bw_graph_tools
 Project-URL: tracker, https://github.com/brightway-lca/bw_graph_tools/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bw_graph_tools-0.3.1/README.md` & `bw_graph_tools-0.4/README.md`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3.1/bw_graph_tools/__init__.py` & `bw_graph_tools-0.4/bw_graph_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     "guess_production_exchanges",
     "NewNodeEachVisitGraphTraversal",
     "Node",
     "path_as_brightway_objects",
     "to_normalized_adjacency_matrix",
 )
 
-__version__ = "0.3.1"
+__version__ = "0.4"
 
-from .graph_traversal_utils import get_path_from_matrix, path_as_brightway_objects
-from .matrix_tools import guess_production_exchanges, to_normalized_adjacency_matrix
 from .graph_traversal import (
     AssumedDiagonalGraphTraversal,
     Edge,
     Flow,
     NewNodeEachVisitGraphTraversal,
     Node,
 )
+from .graph_traversal_utils import get_path_from_matrix, path_as_brightway_objects
+from .matrix_tools import guess_production_exchanges, to_normalized_adjacency_matrix
```

### Comparing `bw_graph_tools-0.3.1/bw_graph_tools/graph_traversal.py` & `bw_graph_tools-0.4/bw_graph_tools/graph_traversal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import warnings
 from dataclasses import dataclass
 from functools import lru_cache
 from heapq import heappop, heappush
 from typing import Optional
 
-from bw2calc import LCA
-from scipy.sparse import spmatrix
 import matrix_utils as mu
 import numpy as np
+from bw2calc import LCA
+from scipy.sparse import spmatrix
 
 try:
     from bw2data import databases
 except ImportError:
     databases = {}
 
 
@@ -67,29 +67,38 @@
     reference_product_index : int
         The technosphere matrix row index of this activity's reference product
     reference_product_production_amount : float
         The *net* production amount of this activity's reference product
     supply_amount : float
         The amount of the *activity* (not reference product!) needed to supply the demand from the requesting supply chain edge.
     cumulative_score : float
-        Total LCIA score attributed to `supply_amount` of this activity. Includes direct emissions unless explicitly removed.
+        Total LCIA score attributed to `supply_amount` of this activity, including impacts from direct emissions.
     direct_emissions_score : float
         Total LCIA score attributed only to the direct characterized biosphere flows of `supply_amount` of this activity.
+    direct_emissions_score_outside_specific_flows : float
+        The score attributable to *direct emissions* of this node which isn't broken out into separate `Flow` objects.
+    remaining_cumulative_score_outside_specific_flows : float
+        The *cumulative* score of this node, including direct emissions, which isn't broken out into separate `Flow` objects.
+    terminal : bool
+        Boolean flag indicating whether graph traversal was cutoff at this node
 
     """
 
     unique_id: int
     activity_datapackage_id: int
     activity_index: int
     reference_product_datapackage_id: int
     reference_product_index: int
     reference_product_production_amount: float
     supply_amount: float
     cumulative_score: float
     direct_emissions_score: float
+    direct_emissions_score_outside_specific_flows: float = 0.0
+    remaining_cumulative_score_outside_specific_flows: float = 0.0
+    terminal: bool = False
 
     def __lt__(self, other):
         # Needed for sorting
         return self.cumulative_score < other.cumulative_score
 
 
 @dataclass
@@ -237,15 +246,15 @@
             Add separate `Flow` nodes for important individual biosphere
             emissions
         static_activity_indices : set
             A set of activity matrix indices which we don't want the graph to
             traverse
         functional_unit_unique_id : int
             An integer id we can use for the functional unit virtual activity.
-            Shouldn't overlap any other activity ids. Don't change unless you 
+            Shouldn't overlap any other activity ids. Don't change unless you
             really know what you are doing.
 
         Returns
         -------
         dict
             Dictionary with keys `nodes`, `edges`, `flows`, `calculation_counter`
 
@@ -254,16 +263,15 @@
         if total_score == 0:
             raise ValueError("Zero total LCA score makes traversal impossible")
 
         cutoff_score = abs(total_score * cutoff)
         biosphere_cutoff_score = abs(total_score * biosphere_cutoff)
         technosphere_matrix = lca_object.technosphere_matrix
         production_exchange_mapping = {
-            x: y
-            for x, y in zip(*cls.get_production_exchanges(lca_object.technosphere_mm))
+            x: y for x, y in zip(*cls.get_production_exchanges(lca_object.technosphere_mm))
         }
         heap, edges, flows = [], [], []
         calculation_count = Counter()
         characterized_biosphere = cls.get_characterized_biosphere(lca_object)
         caching_solver = CachingSolver(lca_object)
 
         nodes = {
@@ -279,17 +287,15 @@
                 direct_emissions_score=0.0,
             )
         }
 
         cls.traverse_edges(
             consumer_index=functional_unit_unique_id,
             consumer_unique_id=functional_unit_unique_id,
-            product_indices=[
-                lca_object.dicts.product[key] for key in lca_object.demand
-            ],
+            product_indices=[lca_object.dicts.product[key] for key in lca_object.demand],
             product_amounts=lca_object.demand.values(),
             lca=lca_object,
             calculation_count=calculation_count,
             characterized_biosphere=characterized_biosphere,
             matrix=technosphere_matrix,
             edges=edges,
             flows=flows,
@@ -320,14 +326,19 @@
             skip_coproducts=skip_coproducts,
             separate_biosphere_flows=separate_biosphere_flows,
             biosphere_cutoff_score=biosphere_cutoff_score,
         )
 
         flows.sort(reverse=True)
 
+        non_terminal_nodes = {edge.consumer_unique_id for edge in edges}
+        for node_id_key in nodes:
+            if node_id_key not in non_terminal_nodes:
+                nodes[node_id_key].terminal = True
+
         return {
             "nodes": nodes,
             "edges": edges,
             "flows": flows,
             "calculation_count": calculation_count.value,
         }
 
@@ -458,56 +469,59 @@
             producer_index = production_exchange_mapping[product_index]
 
             if producer_index in static_activity_indices:
                 continue
 
             supply = caching_solver(product_index, product_amount)
             cumulative_score = float((characterized_biosphere * supply).sum())
-            reference_product_net_production_amount = matrix[
-                product_index, producer_index
-            ]
+            reference_product_net_production_amount = matrix[product_index, producer_index]
             scale = product_amount / reference_product_net_production_amount
 
             if abs(cumulative_score) < cutoff_score:
                 continue
 
             producing_node = Node(
                 unique_id=next(calculation_count),
                 activity_datapackage_id=lca.dicts.activity.reversed[producer_index],
                 activity_index=producer_index,
-                reference_product_datapackage_id=lca.dicts.product.reversed[
-                    product_index
-                ],
+                reference_product_datapackage_id=lca.dicts.product.reversed[product_index],
                 reference_product_index=product_index,
                 reference_product_production_amount=reference_product_net_production_amount,
                 supply_amount=scale,
                 cumulative_score=cumulative_score,
-                direct_emissions_score=(
-                    scale * characterized_biosphere[:, producer_index]
-                ).sum(),
+                direct_emissions_score=(scale * characterized_biosphere[:, producer_index]).sum(),
             )
             edges.append(
                 Edge(
                     consumer_index=consumer_index,
                     consumer_unique_id=consumer_unique_id,
                     producer_index=producer_index,
                     producer_unique_id=producing_node.unique_id,
                     product_index=product_index,
                     amount=product_amount,
                 )
             )
 
             if separate_biosphere_flows:
-                cls.add_biosphere_flows(
+                flow_score = cls.add_biosphere_flows(
                     flows=flows,
                     matrix=(scale * characterized_biosphere[:, producer_index]).tocoo(),
                     lca=lca,
                     node=producing_node,
                     biosphere_cutoff_score=biosphere_cutoff_score,
                 )
+            else:
+                flow_score = 0
+
+            producing_node.direct_emissions_score_outside_specific_flows = (
+                producing_node.direct_emissions_score - flow_score
+            )
+            producing_node.remaining_cumulative_score_outside_specific_flows = (
+                producing_node.cumulative_score - flow_score
+            )
 
             heappush(heap, (abs(1 / cumulative_score), producing_node))
             nodes[producing_node.unique_id] = producing_node
 
     @classmethod
     def get_characterized_biosphere(cls, lca: LCA) -> spmatrix:
         """
@@ -526,17 +540,15 @@
         scipy.sparse.spmatrix
             Unmapped matrix of biosphere flows by activities.
 
         """
         return lca.characterization_matrix * lca.biosphere_matrix
 
     @classmethod
-    def get_production_exchanges(
-        cls, mapped_matrix: mu.MappedMatrix
-    ) -> (np.array, np.array):
+    def get_production_exchanges(cls, mapped_matrix: mu.MappedMatrix) -> (np.array, np.array):
         """
         Get matrix row and column indices of productions exchanges by trying a
         series of heuristics. See documentation for
         ``guess_production_exchanges``.
 
         Broken out as a separate method because subclasses could change this logic.
 
@@ -560,15 +572,15 @@
     def add_biosphere_flows(
         cls,
         flows: list[Flow],
         matrix: spmatrix,
         lca: LCA,
         node: Node,
         biosphere_cutoff_score: float,
-    ) -> None:
+    ) -> float:
         """
         Add individual biosphere flows as `Flow` instances to `flow` if their score is above `biosphere_cutoff_score`.
 
         Parameters
         ----------
         flows : list
             List of existing `Flow` instances
@@ -579,34 +591,35 @@
         node : `Node`
             Node whose direct biosphere flows we are examining
         biosphere_cutoff_score : float
             Score below which individual characterized biosphere flows are ignored
 
         Returns
         -------
-        `None`
-            Modifies `flows` by adding new `Flow` instances
+        The total LCIA score broken out to separate `Flow` instances
 
         """
+        added_score = 0.0
         for index, score in zip(matrix.row, matrix.data):
             if abs(score) > biosphere_cutoff_score:
+                added_score += score
                 flows.append(
                     Flow(
                         flow_datapackage_id=lca.dicts.biosphere.reversed[index],
                         flow_index=index,
                         activity_unique_id=node.unique_id,
                         activity_id=node.activity_datapackage_id,
                         activity_index=node.activity_index,
                         amount=(
-                            lca.biosphere_matrix[index, node.activity_index]
-                            * node.supply_amount
+                            lca.biosphere_matrix[index, node.activity_index] * node.supply_amount
                         ),
                         score=score,
                     )
                 )
+        return added_score
 
     @classmethod
     def get_demand_vector_for_activity(
         cls,
         node: Node,
         skip_coproducts: bool,
         matrix: spmatrix,
@@ -645,17 +658,15 @@
             rows.append(x)
             vals.append(y)
         return rows, vals
 
 
 class AssumedDiagonalGraphTraversal(NewNodeEachVisitGraphTraversal):
     @classmethod
-    def get_production_exchanges(
-        cls, mapped_matrix: mu.MappedMatrix
-    ) -> (np.ndarray, np.ndarray):
+    def get_production_exchanges(cls, mapped_matrix: mu.MappedMatrix) -> (np.ndarray, np.ndarray):
         """
         Assume production exchanges are always on the diagonal instead of
         examining matrix structure and input data.
 
         Parameters
         ----------
         mapped_matrix : matrix_utils.MappedMatrix
```

### Comparing `bw_graph_tools-0.3.1/bw_graph_tools/graph_traversal_utils.py` & `bw_graph_tools-0.4/bw_graph_tools/graph_traversal_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,11 @@
         unweighted=False,
     )
 
     return [
         (
             bd.get_node(id=lca.dicts.product.reversed[x]),
             bd.get_node(id=lca.dicts.activity.reversed[y]),
-            -1
-            * lca.technosphere_matrix[
-                y, x
-            ],  # Flip x and y because y is input to activity x
+            -1 * lca.technosphere_matrix[y, x],  # Flip x and y because y is input to activity x
         )
         for x, y in zip(path[:-1], path[1:])
     ]
```

### Comparing `bw_graph_tools-0.3.1/bw_graph_tools/matrix_tools.py` & `bw_graph_tools-0.4/bw_graph_tools/matrix_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,25 @@
         # normalized to [0, X] range.
         ident_mask = indices["row"] == indices["col"]
 
         # In theory these values should be on the diagonal, as the input row and col
         # values are the same. However, we don't have a strong guarantee that this is
         # true. So to eliminate duplicate values we combine to a (X, 2) array, and get
         # unique rows.
-        # Note that `unique` also does sorting, see 
+        # Note that `unique` also does sorting, see
         # https://stackoverflow.com/questions/16970982/find-unique-rows-in-numpy-array
-        combined = np.unique(np.vstack((
-            group.row_mapper.map_array(indices["row"][ident_mask]),
-            group.col_mapper.map_array(indices["col"][ident_mask])
-        )), axis=1)
+        combined = np.unique(
+            np.vstack(
+                (
+                    group.row_mapper.map_array(indices["row"][ident_mask]),
+                    group.col_mapper.map_array(indices["col"][ident_mask]),
+                )
+            ),
+            axis=1,
+        )
         row_mapped = combined[0, :]
         col_mapped = combined[1, :]
 
         if (row_mapped == -1).sum() or (col_mapped == -1).sum():
             ERROR = """
 Found unmapped values in technosphere matrix generator, but that should be impossible.
 
@@ -123,17 +128,15 @@
             )
             h2_col_indices = h2_col_indices[h2_col_counts == 1]
 
             # Remove elements found by first heuristic
             existing_mask = np.in1d(h2_col_indices, col_existing)
 
             # Need mask with correct shape for both row and col indices
-            mask = np.in1d(
-                group.col_masked[~group.flip], h2_col_indices[~existing_mask]
-            )
+            mask = np.in1d(group.col_masked[~group.flip], h2_col_indices[~existing_mask])
 
             not_flipped.append(
                 (
                     group.row_masked[~group.flip][mask],
                     group.col_masked[~group.flip][mask],
                 )
             )
@@ -191,33 +194,29 @@
         raise ValueError("Empty matrix")
 
     row_indices, col_indices = gpe_first_heuristic(mm)
 
     # Every column must have an activity with some reference product or the system
     # is not solvable. Therefore we can look across all columns. We will do
     # all the work in matrix indices.
-    missing = np.setdiff1d(
-        np.arange(mm.matrix.shape[0]), col_indices, assume_unique=True
-    )
+    missing = np.setdiff1d(np.arange(mm.matrix.shape[0]), col_indices, assume_unique=True)
 
     # Short circuit other steps if possible; assumption is that this step will
     # be taken for most matrices
     if not missing.size:
         return (row_indices, col_indices)
 
     row_indices, col_indices = gpe_second_heuristic(mm, row_indices, col_indices)
     row_indices, col_indices = gpe_third_heuristic(mm, row_indices, col_indices)
 
     # No idea how this could happen, but better raise an error than pass bad data
     if row_indices.shape != col_indices.shape:
         raise ValueError("Guessed row indices do not match guessed column indices.")
 
-    missing = np.setdiff1d(
-        np.arange(mm.matrix.shape[0]), col_indices, assume_unique=True
-    )
+    missing = np.setdiff1d(np.arange(mm.matrix.shape[0]), col_indices, assume_unique=True)
     if missing.size:
         raise UnclearProductionExchange(
             "Can't find production exchanges for columns: {}".format(list(missing))
         )
 
     return (row_indices, col_indices)
```

### Comparing `bw_graph_tools-0.3.1/bw_graph_tools/shortest_path.py` & `bw_graph_tools-0.4/bw_graph_tools/shortest_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,24 +32,31 @@
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
 OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
+
 from functools import partial
 from multiprocessing import Pool
-from typing import Optional, Union, Iterable
+from typing import Iterable, Optional, Union
 
 import numpy as np
 from scipy import sparse
 
 
-def get_distances(adjacency: sparse.csr_matrix, sources: Optional[Union[int, Iterable]] = None, method: str = 'D',
-                  return_predecessors: bool = False, unweighted: bool = False, n_jobs: Optional[int] = None):
+def get_distances(
+    adjacency: sparse.csr_matrix,
+    sources: Optional[Union[int, Iterable]] = None,
+    method: str = "D",
+    return_predecessors: bool = False,
+    unweighted: bool = False,
+    n_jobs: Optional[int] = None,
+):
     """Compute distances between nodes.
 
     * Graphs
     * Digraphs
 
 
     Based on SciPy (scipy.sparse.csgraph.shortest_path)
@@ -84,51 +91,69 @@
         Returned only if ``return_predecessors == True``. The matrix of predecessors, which can be used to reconstruct
         the shortest paths. Row ``i`` of the predecessor matrix contains information on the shortest paths from the
         ``i``-th source: each entry ``predecessors[i, j]`` gives the index of the previous node in the path from
         the ``i``-th source to node ``j`` (-1 if no path exists from the ``i``-th source to node ``j``).
 
     """
     n_jobs, directed = 1, True
-    if method == 'FW' and n_jobs != 1:
-        raise ValueError('The Floyd-Warshall algorithm cannot be used with parallel computations.')
+    if method == "FW" and n_jobs != 1:
+        raise ValueError("The Floyd-Warshall algorithm cannot be used with parallel computations.")
     if sources is None:
         sources = np.arange(adjacency.shape[0])
     elif np.issubdtype(type(sources), np.integer):
         sources = np.array([sources])
     n = len(sources)
-    local_function = partial(sparse.csgraph.shortest_path,
-                             adjacency, method, directed, return_predecessors, unweighted, False)
+    local_function = partial(
+        sparse.csgraph.shortest_path,
+        adjacency,
+        method,
+        directed,
+        return_predecessors,
+        unweighted,
+        False,
+    )
     if n_jobs == 1 or n == 1:
         try:
-            res = sparse.csgraph.shortest_path(adjacency, method, directed, return_predecessors,
-                                               unweighted, False, sources)
+            res = sparse.csgraph.shortest_path(
+                adjacency, method, directed, return_predecessors, unweighted, False, sources
+            )
         except sparse.csgraph.NegativeCycleError:
-            raise ValueError("The shortest path computation could not be completed because a negative cycle is present.")
+            raise ValueError(
+                "The shortest path computation could not be completed because a negative cycle is present."
+            )
     else:
         try:
             with Pool(n_jobs) as pool:
                 res = np.array(pool.map(local_function, sources))
         except sparse.csgraph.NegativeCycleError:
             pool.terminate()
-            raise ValueError("The shortest path computation could not be completed because a negative cycle is present.")
+            raise ValueError(
+                "The shortest path computation could not be completed because a negative cycle is present."
+            )
     if return_predecessors:
         res[1][res[1] < 0] = -1
         if n == 1:
             return res[0].ravel(), res[1].astype(int).ravel()
         else:
             return res[0], res[1].astype(int)
     else:
         if n == 1:
             return res.ravel()
         else:
             return res
 
 
-def get_shortest_path(adjacency: sparse.csr_matrix, sources: Union[int, Iterable], targets: Union[int, Iterable],
-                      method: str = 'D', unweighted: bool = False, n_jobs: Optional[int] = None):
+def get_shortest_path(
+    adjacency: sparse.csr_matrix,
+    sources: Union[int, Iterable],
+    targets: Union[int, Iterable],
+    method: str = "D",
+    unweighted: bool = False,
+    n_jobs: Optional[int] = None,
+):
     """Compute the shortest paths in the graph.
 
     Parameters
     ----------
     adjacency :
         The adjacency matrix of the graph
     sources : int or iterable
@@ -177,15 +202,16 @@
         source = sources[0]
     elif len(targets) == 1:
         source2target = False
         source = targets[0]
         targets = sources
     else:
         raise ValueError(
-            'This request is ambiguous. Either use one source and multiple targets or multiple sources and one target.')
+            "This request is ambiguous. Either use one source and multiple targets or multiple sources and one target."
+        )
 
     if source2target:
         dists, preds = get_distances(adjacency, source, method, True, unweighted, n_jobs)
     else:
         dists, preds = get_distances(adjacency.T, source, method, True, unweighted, n_jobs)
 
     paths = []
```

### Comparing `bw_graph_tools-0.3.1/bw_graph_tools/testing.py` & `bw_graph_tools-0.4/bw_graph_tools/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from numbers import Number
 from typing import Union
+
 import numpy as np
 
-from . import Node, Edge, Flow
+from . import Edge, Flow, Node
 
 
 def equal_dict(a: Union[Node, Edge, Flow], b: dict, fields: list[str]):
     for field in fields:
         if field in b:
             if isinstance(b[field], Number):
                 assert np.allclose(getattr(a, field), b[field])
```

### Comparing `bw_graph_tools-0.3.1/bw_graph_tools.egg-info/PKG-INFO` & `bw_graph_tools-0.4/bw_graph_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_graph_tools
-Version: 0.3.1
+Version: 0.4
 Summary: Graph traversal class and utilities
 Author-email: Chris Mutel <cmutel@gmail.com>
 Maintainer-email: Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_graph_tools
 Project-URL: homepage, https://github.com/brightway-lca/bw_graph_tools
 Project-URL: tracker, https://github.com/brightway-lca/bw_graph_tools/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bw_graph_tools-0.3.1/bw_graph_tools.egg-info/SOURCES.txt` & `bw_graph_tools-0.4/bw_graph_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3.1/pyproject.toml` & `bw_graph_tools-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3.1/tests/test_first_heuristic.py` & `bw_graph_tools-0.4/tests/test_first_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3.1/tests/test_get_path_from_matrix.py` & `bw_graph_tools-0.4/tests/test_get_path_from_matrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,17 +26,19 @@
         matrix="test",
         data_array=data,
         indices_array=edges,
         flip_array=flip,
     )
     mm = mu.MappedMatrix(packages=[dp], matrix="test")
     mapper = mm.col_mapper.to_dict()
-    assert get_path_from_matrix(
-        matrix=mm.matrix, source=mapper[A], target=mapper[C]
-    ) == [mapper[A], mapper[B], mapper[C]]
+    assert get_path_from_matrix(matrix=mm.matrix, source=mapper[A], target=mapper[C]) == [
+        mapper[A],
+        mapper[B],
+        mapper[C],
+    ]
 
 
 def test_take_longer_path_direct_edge_available():
     A = 101
     B = 102
     C = 103
     edges = np.array(
@@ -57,17 +59,19 @@
         matrix="test",
         data_array=data,
         indices_array=edges,
         flip_array=flip,
     )
     mm = mu.MappedMatrix(packages=[dp], matrix="test")
     mapper = mm.col_mapper.to_dict()
-    assert get_path_from_matrix(
-        matrix=mm.matrix, source=mapper[A], target=mapper[C]
-    ) == [mapper[A], mapper[B], mapper[C]]
+    assert get_path_from_matrix(matrix=mm.matrix, source=mapper[A], target=mapper[C]) == [
+        mapper[A],
+        mapper[B],
+        mapper[C],
+    ]
 
 
 def test_take_longer_path_no_direct_edge():
     A = 101
     B = 102
     C = 103
     D = 104
@@ -91,10 +95,13 @@
         matrix="test",
         data_array=data,
         indices_array=edges,
         flip_array=flip,
     )
     mm = mu.MappedMatrix(packages=[dp], matrix="test")
     mapper = mm.col_mapper.to_dict()
-    assert get_path_from_matrix(
-        matrix=mm.matrix, source=mapper[A], target=mapper[D]
-    ) == [mapper[A], mapper[B], mapper[C], mapper[D]]
+    assert get_path_from_matrix(matrix=mm.matrix, source=mapper[A], target=mapper[D]) == [
+        mapper[A],
+        mapper[B],
+        mapper[C],
+        mapper[D],
+    ]
```

### Comparing `bw_graph_tools-0.3.1/tests/test_matrix_utils.py` & `bw_graph_tools-0.4/tests/test_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3.1/tests/test_second_heuristic.py` & `bw_graph_tools-0.4/tests/test_second_heuristic.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,15 @@
         data_array=data,
         flip_array=flip,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_second_heuristic(
-        mm=mm, row_existing=np.array([]), col_existing=np.array([])
-    )
+    row, col = gpe_second_heuristic(mm=mm, row_existing=np.array([]), col_existing=np.array([]))
     assert np.array_equal(np.array([1]), row)
     assert np.array_equal(np.array([1]), col)
 
 
 def test_second_heuristic_off_diagonal():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2, 3, 4])
@@ -56,17 +54,15 @@
         data_array=data,
         flip_array=flip,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_second_heuristic(
-        mm=mm, row_existing=np.array([]), col_existing=np.array([])
-    )
+    row, col = gpe_second_heuristic(mm=mm, row_existing=np.array([]), col_existing=np.array([]))
     assert np.array_equal(np.array([0, 1]), row)
     assert np.array_equal(np.array([1, 0]), col)
 
 
 def test_second_heuristic_exclude_multiple_flips():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2, 3, 4])
@@ -87,17 +83,15 @@
         data_array=data,
         flip_array=flip,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_second_heuristic(
-        mm=mm, row_existing=np.array([]), col_existing=np.array([])
-    )
+    row, col = gpe_second_heuristic(mm=mm, row_existing=np.array([]), col_existing=np.array([]))
     assert np.array_equal(np.array([1]), row)
     assert np.array_equal(np.array([1]), col)
 
 
 def test_second_heuristic_overlap_existing():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2, 3, 4])
@@ -118,17 +112,15 @@
         data_array=data,
         flip_array=flip,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_second_heuristic(
-        mm=mm, row_existing=np.array([0]), col_existing=np.array([0])
-    )
+    row, col = gpe_second_heuristic(mm=mm, row_existing=np.array([0]), col_existing=np.array([0]))
     assert np.array_equal(np.array([0, 1]), row)
     assert np.array_equal(np.array([0, 1]), col)
 
 
 def test_second_heuristic_complement_existing():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2, 3, 4])
@@ -149,17 +141,15 @@
         data_array=data,
         flip_array=flip,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_second_heuristic(
-        mm=mm, row_existing=np.array([10]), col_existing=np.array([10])
-    )
+    row, col = gpe_second_heuristic(mm=mm, row_existing=np.array([10]), col_existing=np.array([10]))
     assert np.array_equal(np.array([10, 1, 0]), row)
     assert np.array_equal(np.array([10, 1, 0]), col)
 
 
 def test_second_heuristic_no_flip():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2, 3, 4])
@@ -178,12 +168,10 @@
         name="foo",
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_second_heuristic(
-        mm=mm, row_existing=np.array([0]), col_existing=np.array([0])
-    )
+    row, col = gpe_second_heuristic(mm=mm, row_existing=np.array([0]), col_existing=np.array([0]))
     assert np.array_equal(np.array([0]), row)
     assert np.array_equal(np.array([0]), col)
```

### Comparing `bw_graph_tools-0.3.1/tests/test_third_heuristic.py` & `bw_graph_tools-0.4/tests/test_third_heuristic.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
         name="foo",
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_third_heuristic(
-        mm=mm, row_existing=np.array([]), col_existing=np.array([])
-    )
+    row, col = gpe_third_heuristic(mm=mm, row_existing=np.array([]), col_existing=np.array([]))
     assert np.array_equal(np.array([1]), row)
     assert np.array_equal(np.array([1]), col)
 
 
 def test_third_heuristic_off_diagonal():
     dp1 = bwp.create_datapackage()
     data = np.array([-1, 2, -3, 4])
@@ -52,17 +50,15 @@
         name="foo",
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_third_heuristic(
-        mm=mm, row_existing=np.array([]), col_existing=np.array([])
-    )
+    row, col = gpe_third_heuristic(mm=mm, row_existing=np.array([]), col_existing=np.array([]))
     assert np.array_equal(np.array([0, 1]), row)
     assert np.array_equal(np.array([1, 0]), col)
 
 
 def test_third_heuristic_multiple_positive_per_column():
     dp1 = bwp.create_datapackage()
     data = np.array([1, -2, 3, 4])
@@ -81,17 +77,15 @@
         name="foo",
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_third_heuristic(
-        mm=mm, row_existing=np.array([]), col_existing=np.array([])
-    )
+    row, col = gpe_third_heuristic(mm=mm, row_existing=np.array([]), col_existing=np.array([]))
     assert np.array_equal(np.array([1]), row)
     assert np.array_equal(np.array([1]), col)
 
 
 def test_third_heuristic_overlap_existing():
     dp1 = bwp.create_datapackage()
     data = np.array([1, -2, 3, -4])
@@ -110,17 +104,15 @@
         name="foo",
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_third_heuristic(
-        mm=mm, row_existing=np.array([0]), col_existing=np.array([0])
-    )
+    row, col = gpe_third_heuristic(mm=mm, row_existing=np.array([0]), col_existing=np.array([0]))
     assert np.array_equal(np.array([0, 1]), row)
     assert np.array_equal(np.array([0, 1]), col)
 
 
 def test_third_heuristic_complement_existing():
     dp1 = bwp.create_datapackage()
     data = np.array([1, -2, 3, -4])
@@ -139,12 +131,10 @@
         name="foo",
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
-    row, col = gpe_third_heuristic(
-        mm=mm, row_existing=np.array([10]), col_existing=np.array([10])
-    )
+    row, col = gpe_third_heuristic(mm=mm, row_existing=np.array([10]), col_existing=np.array([10]))
     assert np.array_equal(np.array([10, 0, 1]), row)
     assert np.array_equal(np.array([10, 0, 1]), col)
```

