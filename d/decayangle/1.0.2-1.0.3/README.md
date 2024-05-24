# Comparing `tmp/decayangle-1.0.2.tar.gz` & `tmp/decayangle-1.0.3.tar.gz`

## Comparing `decayangle-1.0.2.tar` & `decayangle-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 decayangle-1.0.2/.pylintrc
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 decayangle-1.0.2/docs/Makefile
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 decayangle-1.0.2/docs/conf.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 decayangle-1.0.2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 decayangle-1.0.2/docs/make.bat
--rw-r--r--   0        0        0    18517 2020-02-02 00:00:00.000000 decayangle-1.0.2/notebooks/decay_example.ipynb
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/backend.py
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/config.py
--rw-r--r--   0        0        0    31347 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/decay_topology.py
--rw-r--r--   0        0        0    17707 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/kinematics.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/lorentz.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 decayangle-1.0.2/src/decayangle/numerics_helpers.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_Nbody.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_config.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_decay.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_kinematics.py
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_lorentz.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_sorting.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 decayangle-1.0.2/tests/test_topology.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 decayangle-1.0.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 decayangle-1.0.2/LICENSE.md
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 decayangle-1.0.2/README.md
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 decayangle-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    12513 2020-02-02 00:00:00.000000 decayangle-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 decayangle-1.0.3/.pylintrc
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 decayangle-1.0.3/docs/Makefile
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 decayangle-1.0.3/docs/conf.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 decayangle-1.0.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 decayangle-1.0.3/docs/make.bat
+-rw-r--r--   0        0        0    18517 2020-02-02 00:00:00.000000 decayangle-1.0.3/notebooks/decay_example.ipynb
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 decayangle-1.0.3/src/decayangle/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.3/src/decayangle/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 decayangle-1.0.3/src/decayangle/backend.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 decayangle-1.0.3/src/decayangle/config.py
+-rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 decayangle-1.0.3/src/decayangle/decay_topology.py
+-rw-r--r--   0        0        0    19193 2020-02-02 00:00:00.000000 decayangle-1.0.3/src/decayangle/kinematics.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 decayangle-1.0.3/src/decayangle/lorentz.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 decayangle-1.0.3/src/decayangle/numerics_helpers.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 decayangle-1.0.3/tests/test_Nbody.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 decayangle-1.0.3/tests/test_config.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 decayangle-1.0.3/tests/test_decay.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 decayangle-1.0.3/tests/test_kinematics.py
+-rw-r--r--   0        0        0    17898 2020-02-02 00:00:00.000000 decayangle-1.0.3/tests/test_lorentz.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 decayangle-1.0.3/tests/test_sorting.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 decayangle-1.0.3/tests/test_topology.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 decayangle-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 decayangle-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0    12803 2020-02-02 00:00:00.000000 decayangle-1.0.3/README.md
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 decayangle-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    13924 2020-02-02 00:00:00.000000 decayangle-1.0.3/PKG-INFO
```

### Comparing `decayangle-1.0.2/.pylintrc` & `decayangle-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/docs/Makefile` & `decayangle-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/docs/conf.py` & `decayangle-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/docs/index.rst` & `decayangle-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/docs/make.bat` & `decayangle-1.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/notebooks/decay_example.ipynb` & `decayangle-1.0.3/notebooks/decay_example.ipynb`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/src/decayangle/decay_topology.py` & `decayangle-1.0.3/src/decayangle/decay_topology.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from __future__ import annotations
 from typing import List, Tuple, Union, Any, Dict, Optional, Generator, Callable
-from functools import cached_property
 from collections import namedtuple
 import numpy as np
 from jax import numpy as jnp
 import networkx as nx
 from decayangle.lorentz import LorentzTrafo
 from decayangle import kinematics as akm
 from decayangle.numerics_helpers import matrix_vector_product
@@ -39,15 +39,15 @@
     Attributes:
         value (Union[int, Tuple[int]]): the value of the node
         parent (Node): the parent node of the node
         daughters (Tuple[Node]): the daughters of the node
         ordering_function (function): function ordering the daughters and node values of the node
     """
     @staticmethod
-    def construct_topology(node: "Node", topology: Tuple[Union[int, tuple]]):
+    def construct_topology(node: Node, topology: Tuple[Union[int, tuple]]):
         """Construct a topology from a tuple of integers and tuples, in the form like the string representation of a topology
 
         i.e. ((1,2), 3)
         or ((1, (2, 3)), 4) for a four body decay
 
         Args:
             node (Node): the node to add the daughters to
@@ -59,15 +59,15 @@
         right = Node(tuple(flat(topology[1])))
         node.add_daughter(left)
         node.add_daughter(right)
         Node.construct_topology(left, topology[0])
         Node.construct_topology(right, topology[1])
 
     @classmethod
-    def get_node(cls, value: Union[int, Tuple[int], "Node"]) -> "Node":
+    def get_node(cls, value: Union[int, Tuple[int], Node]) -> Node:
         """Get a node from a value or return the value if a node is given
 
         Args:
             value (Union[int, Tuple[int], Node]): the value of the node
 
         Returns:
             Node: the node
@@ -118,15 +118,15 @@
         """
         return self.__sorting_fun
 
     @ordering_function.setter
     def ordering_function(self, value):
         """
         Set the sorting function for the node and all daughters
-        Sorting functions are epected to return the same data type as the input
+        Sorting functions are expected to return the same data type as the input
         They need to accept lists, tuples and integers as input
         """
 
         if not isinstance(value((1, 2, 3)), tuple):
             raise ValueError(
                 "Sorting function has to be a function returning the sorted value of the same datatype and accepting tupels and lists of integers"
             )
@@ -139,24 +139,24 @@
         self.__daughters = self.__sorted_daughters()
         
         if isinstance(self.value, tuple):
             self.value = self.ordering_function(self.value)
         for d in self.__daughters:
             d.ordering_function = value
 
-    def __sorted_daughters(self) -> Tuple["Node"]:
+    def __sorted_daughters(self) -> Tuple[Node]:
         """
         Sort the daughters of the node, by passing the values to the sorting function
         Then return the daughters in the order of the sorted values
         """
         daughter_values = [d.value for d in self.__daughters]
         sorted_values = self.ordering_function(daughter_values)
         return tuple(self.__daughters[daughter_values.index(v)] for v in sorted_values)
 
-    def add_daughter(self, daughter: "Node"):
+    def add_daughter(self, daughter: Node):
         """Add a daughter to the node. 
         The daughter has to be of type Node, since this function should only be called when constructing a topology.
         No checks are made to ensure that the daughter is not already a daughter of the node.
         Daughters are re-sorted after adding a new daughter.
         
         Args:
             daughter (Node): the daughter to add
@@ -165,23 +165,23 @@
             raise ValueError("Daughter has to be a Node")
 
         self.__daughters = self.__daughters + (daughter,)
         self.__daughters = self.__sorted_daughters()
         daughter.parent = self
 
     @property
-    def daughters(self) -> Tuple["Node"]:
+    def daughters(self) -> Tuple[Node]:
         """Get the daughters of the node
 
         Returns:
             List[Node]: the daughters of the node
         """
         return self.__daughters
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if len(self.daughters) == 0:
             return str(self.value)
         return (
             f"( {self.value} -> " + f"{', '.join([str(d) for d in self.daughters])} )"
         )
 
     @property
@@ -189,18 +189,18 @@
         """Check if the node is a final state node by checking if it has daughters
 
         Returns:
             bool: True if the node is a final state node, False otherwise
         """
         return len(self.daughters) == 0
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.__repr__()
 
-    def contains(self, contained_node: "Node") -> bool:
+    def contains(self, contained_node: Node) -> bool:
         """Check if a node is contained in the topology
 
         Args:
             contained_node (Node): the node to check for
 
         Returns:
             bool: True if the node is contained in the topology, False otherwise
@@ -212,15 +212,15 @@
         elif set(self.value) == set(contained_node.value):
             return True
         for d in self.daughters:
             if d.contains(contained_node):
                 return True
         return False
 
-    def preorder(self) -> List["Node"]:
+    def preorder(self) -> List[Node]:
         """Get the nodes in the tree in preorder. 
         This is a recursive function, which will return the nodes in the tree in the order of the preorder traversal.
         This means, root first, then daughters in the order they were added.
 
         Returns:
             list: the nodes in the tree in preorder
         """
@@ -254,36 +254,45 @@
 
         Returns:
             the mass of the particle, as set by the momenta dictionary
             This expects the momenta to be jax or numpy compatible
         """
         return akm.mass(self.momentum(momenta))
 
-    def transform(self, trafo: LorentzTrafo, momenta: dict) -> Dict[int, Union[np.array, jnp.array]]:
+    def transform(self, trafo: LorentzTrafo, momenta: Dict[str, Union[np.array, jnp.array]]) -> Dict[int, Union[np.array, jnp.array]]:
         """Transform the momenta of the final state particles
 
         Args:
             trafo (LorentzTrafo): transformation to apply
             momenta (dict): the momenta of the final state particles
 
         Returns:
             dict: the transformed momenta
         """
         return {
             k: matrix_vector_product(trafo.matrix_4x4, v) for k, v in momenta.items()
         }
 
-    def boost(self, target: Union["Node", int], momenta: dict) -> LorentzTrafo:
+    def boost(self, target: Union[Node, int], momenta: Dict[str, Union[np.array, jnp.array]], tol: Optional[float]=None) -> LorentzTrafo:
         """Get the boost from this node to a target node
         The momenta dictionary will define the initial configuration.
         It is expected, that the momenta are jax or numpy compatible and that the momenta are given in the rest frame of this node.
+
+        Args:
+            target (Union[Node, int]): the target node to boost to
+            momenta (dict): the momenta of the final state particles
+            tol (float, optional): tolerance for the gamma check. Defaults to the value in the config.
         """
+
+        if tol is None:
+            tol = cfg.gamma_tolerance
         if not cb.allclose(
             akm.gamma(self.momentum(momenta)),
             cb.ones_like(akm.gamma(self.momentum(momenta))),
+            rtol=tol
         ):
             gamma = akm.gamma(self.momentum(momenta))
             cfg.raise_if_safety_on( 
                 ValueError(
                     f"gamma = {gamma} For the time being only particles at rest are supported as start nodes for a boost. This will be fixed in the future."
                 )
             )
@@ -295,77 +304,89 @@
 
         if target not in self.daughters:
             raise ValueError(
                 f"Target node {target} is not a direct daughter of this node {self}"
             )
 
         # rotate so that the target momentum is aligned with the
-        rotation, _, _ = self.rotate_to(target, momenta)
+        rotation, _, _ = self.rotate_to(target, momenta, tol=tol)
         rotated_momenta = self.transform(rotation, momenta)
 
         # boost to the rest frame of the target
         xi = -akm.rapidity(target.momentum(rotated_momenta))
         boost = LorentzTrafo(zero, zero, xi, zero, zero, zero)
 
         return boost @ rotation
 
     def align_with_daughter(
-        self, momenta: Dict[int, Union[np.array, jnp.array]], nth_daughter: int = 0
+        self, momenta: Dict[int, Union[np.array, jnp.array]], nth_daughter: int = 0, tol: Optional[float]=None
     ) -> Dict[int, Union[np.array, jnp.array]]:
         """Align the momenta with the nth daughter. It is written in this way, to highlight, that one can only align with the direct daughters of a node.
         This requires the momenta to be in the rest frame of the node.
 
         Args:
             momenta (dict): the momenta of the final state particles
             nth_daughter (int, optional): the daughter to align with. Defaults to 0.
+            tol (float, optional): tolerance for the gamma check. Defaults to the value in the config.
 
         Returns:
             dict: the aligned momenta
         """
         if nth_daughter >= len(self.daughters):
             raise ValueError(
                 f"Node {self} does not have a daughter with index {nth_daughter}"
             )
-        rotation, _, _ = self.rotate_to(self.daughters[nth_daughter], momenta)
+        rotation, _, _ = self.rotate_to(self.daughters[nth_daughter], momenta, tol=tol)
         return self.transform(rotation, momenta)
 
-    def helicity_angles(self, momenta: dict) -> HelicityAngles:
+    def helicity_angles(self, momenta: Dict[str, Union[np.array, jnp.array]], tol: Optional[float]=None) -> HelicityAngles:
         """
         Get the helicity angles for the daughters of this node.
         The angles are with respect to the first daughter. 
         Here the ordering scheme can be important.
 
         Parameters:
             momenta: Dictionary of momenta for the final state particles
+            tol: Tolerance for the gamma check
 
         Returns:
             Helicity angles for the final state particles
 
         """
 
         # define the daughter for which the momentum should be aligned with the positive z after the rotation
         positive_z = self.daughters[0]
-        _, theta_rf, psi_rf = self.rotate_to(positive_z, momenta)
+        _, theta_rf, psi_rf = self.rotate_to(positive_z, momenta, tol=tol)
         return HelicityAngles(theta_rf, psi_rf)
 
     def rotate_to(
-        self, target: "Node", momenta: dict
-    ) -> Tuple[LorentzTrafo, float, float]:
+        self, target: Node, momenta: Dict[str, Union[np.array, jnp.array]],
+        tol: Optional[float]=None
+    ) -> Tuple[LorentzTrafo, Union[float, np.array, jnp.array], Union[float, np.array, jnp.array]]:
         """Get the rotation from this node to a target node
         The momenta dictionary will define the initial configuration.
         It is expected, that the momenta are jax or numpy compatible and that the momenta are given in the rest frame of this node.
 
+        Args:
+            target (Node): the target node to rotate to
+            momenta (dict): the momenta of the final state particles
+            tol (float, optional): tolerance for the gamma check. Defaults to the value in the config.
+
         Returns:
-            rotation: The rotation to align the target momentum with the z-axis
-            psi_rf: The angle of the target momentum in the rest frame of this node
-            theta_rf: The angle of the target momentum in the rest frame of this node
+            rotation (LorentzTrafo): the rotation to apply
+            theta_rf (Union[float, np.array, jnp.array]): the polar angle of the rotation
+            psi_rf (Union[float, np.array, jnp.array]): the azimuthal angle of the rotation
         """
+
+        if tol is None:
+            tol = cfg.gamma_tolerance
         if not cb.allclose(
             akm.gamma(self.momentum(momenta)),
             cb.ones_like(akm.gamma(self.momentum(momenta))),
+            rtol=tol
         ):
             gamma = akm.gamma(self.momentum(momenta))
             cfg.raise_if_safety_on(
                 ValueError(
                     f"gamma = {gamma} For the time being only particles at rest are supported as start nodes for a boost. This will be fixed in the future."
                 )
             ) 
@@ -459,37 +480,44 @@
 
         self.__sorting_fun = value
         self.__root.ordering_function = value
 
     def __repr__(self) -> str:
         return f"Topology: {self.root}"
 
-    def contains(self, contained_node: Union["Node", int]) -> bool:
+    def contains(self, contained_node: Union[Node, int]) -> bool:
         """Check if a node is contained in the topology
 
         Args:
             contained_node (Node): the node to check for
 
         Returns:
             bool: True if the node is contained in the topology, False otherwise
         """
         contained_node = Node.get_node(contained_node)
         contained_node.ordering_function = self.ordering_function
         return self.root.contains(contained_node)
 
-    def to_rest_frame(self, momenta: dict) -> Dict[int, Union[np.array, jnp.array]]:
+    def to_rest_frame(self, momenta: Dict[str, Union[np.array, jnp.array]], tol: Optional[float]=None) -> Dict[int, Union[np.array, jnp.array]]:
         """Transform the momenta to the rest frame of the root node
 
         Args:
             momenta (dict): the momenta of the final state particles
+            tol (float, optional): tolerance for the gamma check. Defaults to the value in the config. When the original gamma is close to 1, the momenta are assumed to be in the rest frame of the root node.
 
         Returns:
             dict: the momenta in the rest frame of the root node
         """
+        if tol is None:
+            tol = cfg.gamma_tolerance
+
         momentum = self.root.momentum(momenta)
+        gamma = akm.gamma(momentum)
+        if cb.allclose(gamma, cb.ones_like(gamma), rtol=tol):
+            return momenta
         return {k: akm.boost_to_rest(v, momentum) for k, v in momenta.items()}
 
     def __build_boost_tree(self) -> Tuple[nx.DiGraph, Dict[int, Node]]:
         boost_tree = nx.DiGraph()
         node_dict = {}
         for node in self.preorder():
             boost_tree.add_node(node.value)
@@ -504,20 +532,22 @@
         """nodes of the tree
 
         Returns:
             Dict[Union[tuple, int], Node]: A dict of the nodes with the node value as key
         """
         return {n.value: n for n in self.preorder()}
 
-    def helicity_angles(self, momenta: dict) -> Dict[Tuple[Union[tuple ,int], Union[tuple ,int]], HelicityAngles]:
+    def helicity_angles(self, momenta: Dict[str, Union[np.array, jnp.array]], tol:Optional[float]=None) -> Dict[Tuple[Union[tuple ,int], Union[tuple ,int]], HelicityAngles]:
         """
         Get a tree with the helicity angles for every internal node
 
         Parameters:
-            momenta: Dictionary of momenta for the final state particles
+            momenta(Dictionary): Dictionary of momenta for the final state particles
+            tol(float): Tolerance for the gamma check. Defaults to the value in the config.
+
 
         Returns:
             Helicity angles for the final state particles
 
         """
         helicity_angles = {}
 
@@ -531,81 +561,84 @@
                 isobar, spectator = node.daughters
                 helicity_angles[(isobar.value, spectator.value)] = node.helicity_angles(
                     momenta_in_node_frame
                 )
         return helicity_angles
 
     def boost(
-        self, target: Union["Node", int], momenta: dict, inverse: bool = False
+        self, target: Union[Node, int], momenta: Dict[str, Union[np.array, jnp.array]], inverse: bool = False, tol: Optional[float]=None
     ) -> LorentzTrafo:
         """
         Get the boost from the root node to a target node.
 
         Parameters:
             target: Node to boost to
             momenta: Dictionary of momenta for the final state particles
             inverse: If True, return the inverse of the boost
+            tol: Tolerance for the gamma check. Defaults to the value in the config.
 
         Returns:
             Boost from the root node to the target node
 
         """
         target = Node.get_node(target)
         boost_tree, node_dict = self.__build_boost_tree()
         path = nx.shortest_path(boost_tree, self.root.value, target.value)[1:]
-        trafo = self.root.boost(node_dict[path[0]], momenta)
+        trafo = self.root.boost(node_dict[path[0]], momenta, tol=tol)
         momenta = self.root.transform(trafo, momenta)
         trafos = [trafo]
         for i in range(1, len(path)):
-            boost = node_dict[path[i - 1]].boost(node_dict[path[i]], momenta)
+            boost = node_dict[path[i - 1]].boost(node_dict[path[i]], momenta, tol=tol)
             momenta = node_dict[path[i - 1]].transform(boost, momenta)
             trafo = boost @ trafo
             trafos.append(boost)
         if inverse:
             # this is more precise then the naive inverse
             inverse_trafo = trafos[0].inverse()
             for trafo in trafos[1:]:
                 inverse_trafo = inverse_trafo @ trafo.inverse()
             return inverse_trafo
         return trafo
 
     def rotate_between_topologies(
-        self, other: "Topology", target: Union["Node", int], momenta: dict
+        self, other: "Topology", target: Union[Node, int], momenta: Dict[str, Union[np.array, jnp.array]], tol: Optional[float]=None
     ) -> LorentzTrafo:
         """Get the relative Wigner angles between two topologies
 
         Parameters:
             other: Topology to compare to
             target: Node to compare to
             momenta: Dictionary of momenta for the final state particles
+            tol: Tolerance for the gamma check. Defaults to the value in the config.
 
         Returns:
             The rotation between the two rest frames for the target node, one arrives at by boosting from the mother rest frame to the target rest frame as described by the two topologies
         """
         target = Node.get_node(target)
         # invert self, since this final state is seen as the reference
-        boost1_inv = self.boost(target, momenta, inverse=True)
-        boost2 = other.boost(target, momenta)
+        boost1_inv = self.boost(target, momenta, inverse=True, tol=tol)
+        boost2 = other.boost(target, momenta, tol=tol)
         return (boost2 @ boost1_inv)
 
     def relative_wigner_angles(
-        self, other: "Topology", momenta: dict
+        self, other: "Topology", momenta: Dict[str, Union[np.array, jnp.array]], tol: Optional[float]=None
     ) -> Dict[int, Tuple[Union[jnp.ndarray, np.array], Union[jnp.ndarray, np.array]]]:
         """Get the relative Wigner angles between two topologies
 
         Parameters:
             other: Topology to compare to
             target: Node to compare to
             momenta: Dictionary of momenta for the final state particles
+            tol: Tolerance for the gamma check. Defaults to the value in the config.
 
         Returns:
             Dict of the relative Wigner angles with the final state node as key
         """
         return {
-            target.value: self.rotate_between_topologies(other, target, momenta).wigner_angles()
+            target.value: self.rotate_between_topologies(other, target, momenta, tol=tol).wigner_angles()
             for target in self.final_state_nodes
         }
 
     def align_with_daughter(
         self, momenta: Dict[int, Union[np.array, jnp.array]], node: Optional[Union[int, Node]]=None
     ) -> Dict[int, Union[np.array, jnp.array]]:
         """Align the momenta with the node passed as argument. If no node is passed, the first daughter is used.
```

### Comparing `decayangle-1.0.2/src/decayangle/kinematics.py` & `decayangle-1.0.3/src/decayangle/kinematics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Union
+from typing import Tuple, Union, Optional
 from functools import partial
 from jax import numpy as jnp
 import numpy as np
 from decayangle.config import config as cfg
 from decayangle.numerics_helpers import save_arccos
 
 cb = cfg.backend
@@ -50,26 +50,27 @@
     """
     sigma_z = cb.array([[1, 0], [0, -1]])
     eye = cb.eye(2)
     return cb.cosh(xi / 2) * eye + cb.sinh(xi / 2) * sigma_z
 
 
 def rotate_to_z_axis(v: Union[jnp.array, np.array]) -> Union[jnp.array, np.array]:
-    """Given a vector, rotate it to the z-axis
+    """Given a vector, calculate the angles to rotate it to the z-axis
+    This is done by rotating into the x-z plane (rotation around z axis by -psi_rf) and then into the z-axis (rotation around y axis by -theta_rf)
 
     Args:
         v (Union[jnp.array, np.array]): the 4 vector to be rotated
 
     Returns:
         Union[jnp.array, np.array]: the rotation angles around first z and then y axis
     """
     v = cb.array(v)
-    psi_rf = -cb.arctan2(y_component(v), x_component(v))
+    psi_rf = cb.arctan2(y_component(v), x_component(v))
     theta_rf = cb.arccos(z_component(v) / p(v))
-    return psi_rf, -theta_rf
+    return -psi_rf, -theta_rf
 
 
 @partial(cb.vectorize, signature="()->(2,2)")
 def rotation_matrix_2_2_x(theta: float) -> Union[jnp.array, np.array]:
     """Build a 2x2 rotation matrix around the x-axis
 
     Args:
@@ -271,43 +272,50 @@
         @ boost_matrix_4_4_z(xi)
         @ rotation_matrix_4_4_z(phi_rf)
         @ rotation_matrix_4_4_y(theta_rf)
         @ rotation_matrix_4_4_z(psi_rf)
     )
 
 
-def decode_rotation_4x4(rotation_matrix: jnp.array) -> Tuple[float, float, float]:
+def decode_rotation_4x4(rotation_matrix: Union[jnp.array, np.array]) -> Tuple[float, float, float]:
     r"""decode a 4x4 rotation matrix into the 3 rotation angles
 
     Args:
-        matrix (_type_): _description_
+        matrix (jax.numpy.ndarray): the 4x4 rotation matrix
+    
+    Returns:
+        Tuple[float, float, float]: the 3 rotation angles (phi, theta, psi)
     """
     phi = cb.arctan2(rotation_matrix[..., 1, 2], rotation_matrix[..., 0, 2])
     theta = save_arccos(rotation_matrix[..., 2, 2])
     psi = cb.arctan2(rotation_matrix[..., 2, 1], -rotation_matrix[..., 2, 0])
     return phi, theta, psi
 
 
-def decode_4_4(matrix, tol=1e-14):
+def decode_4_4(matrix, tol:Optional[float]=None) -> Tuple[Union[float, np.array, jnp.array]]:
     r"""decode a 4x4 matrix into the 6 kinematic parameters
 
     Args:
         matrix (jax.numpy.ndarray): the 4x4 matrix
+        tol (float, optional): the tolerance for the gamma factor. When not given the default value from the config ('gamma_tolerance') will be used.
     """
+    if tol is None:
+        tol = cfg.gamma_tolerance
+
     m = 1.0
     v_0 = cb.array([0, 0, 0, m])
 
     v = matrix @ v_0
     w = time_component(v)
     abs_mom = p(v)
     gma = w / m
 
     # gamma can be smaller than 1 due to numerical errors
     # for large deviations we will raise an exception
-    gma = cb.where((abs(gma) < 1) & (abs(gma - 1) < 1e-14), 1, gma)
+    gma = cb.where((abs(gma) < 1) & (abs(gma - 1) < tol), 1, gma)
     if cb.any(gma < 1):
         cfg.raise_if_safety_on(
              ValueError(
                 f"gamma is {gma}, which is less than 1. This is not a valid Lorentz transformation"
             )
         )
 
@@ -363,21 +371,20 @@
         psi_rf (float): the recovered psi_rf angle from the 4x4 matrix
 
     Returns:
         tuple: the adjusted rotation angles
     """
     new_2x2 = build_2_2(phi, theta, xi, phi_rf, theta_rf, psi_rf)
 
-    # TODO: is this amount of numerical tolerance maybe a little too much?
-    two_pi_shifted = cb.all(
-        cb.all(cb.isclose(m_original_2x2, -new_2x2, atol=3e-2), axis=-1), axis=-1
+    not_two_pi_shifted = cb.all(
+        cb.all(cb.isclose(m_original_2x2, new_2x2, rtol=cfg.shift_precision), axis=-1), axis=-1
     )
 
-    not_two_pi_shifted = cb.all(
-        cb.all(cb.isclose(m_original_2x2, new_2x2, atol=3e-2), axis=-1), axis=-1
+    two_pi_shifted = cb.all(
+        cb.all(cb.isclose(m_original_2x2, -new_2x2, rtol=cfg.shift_precision), axis=-1), axis=-1
     )
     if cb.any(not_two_pi_shifted & two_pi_shifted):
         cfg.raise_if_safety_on(
              ValueError(
                 f"The 2x2 matrix does not match the reconstruced parameters!"
                 f"This can happen due to numerical errors."
                 f"The original matrix is {m_original_2x2} and the reconstructed matrix is {new_2x2}"
@@ -551,90 +558,104 @@
     Args:
         p (jax.numpy.ndarray): momentum 4-vector
     """
     b = beta(momentum)
     return 0.5 * cb.log((b + 1) / (1 - b))
 
 
-def norm(vec):
+def norm(vec: Union[jnp.array, np.array]):
     """
     Calculate norm of 3-vector
 
-    :param vec: Input 3-vector
-    :returns: Scalar norm
+    Args:
+        vec (Union[jnp.array, np.array]): 3-vector
+    Returns:
+        Union[jnp.array, np.array]: norm of the 3-vector
 
     """
     return cb.sqrt(cb.sum(vec * vec, -1))
 
 
-def p(vector):
+def p(vector: Union[jnp.array, np.array]):
     """
     Calculate absolute value of the 4-momentum
 
-    :param vector: Input 4-momentum vector
-    :returns: Absolute momentum (scalar)
+    Args:
+        vector (Union[jnp.array, np.array]): 4-momentum vector
+    Returns:
+        Union[jnp.array, np.array]: absolute value of the 4-momentum
 
     """
     return norm(spatial_components(vector))
 
 
-def scalar_product(vec1, vec2):
+def scalar_product(vec1: Union[jnp.array, np.array], vec2: Union[jnp.array, np.array]) -> Union[jnp.array, np.array]:
     """
     Calculate scalar product of two 3-vectors
 
-    :param vec1: First 3-vector
-    :param vec2: Secont 3-vector
-    :returns: Scalar product
+    Args:
+        vec1 (Union[jnp.array, np.array]): first 3-vector
+        vec2 (Union[jnp.array, np.array]): second 3-vector
+
+    Returns:
+        Union[jnp.array, np.array]: scalar product of the two vectors
 
     """
     return cb.sum(vec1 * vec2, -1)
 
 
-def scalar(x):
+def scalar(x: Union[jnp.array, np.array]) -> Union[jnp.array, np.array]:
     """
     Create a scalar (array with only one component in last index) which can be used
     to e.g. scale a vector.
 
-    :param x: Initial value
-    :returns: Scalar value
+    Args:
+        x (Union[jnp.array, np.array]): input array
+    Returns:
+        Union[jnp.array, np.array]: scalar array
 
     """
     return cb.stack([x], axis=-1)
 
 
-def lorentz_boost(vector, boostvector):
+def lorentz_boost(vector: Union[jnp.array, np.array], boostvector: Union[jnp.array, np.array]) -> Union[jnp.array, np.array]:
     """
     Perform Lorentz boost of the 4-vector vector using boost vector boostvector.
     We do not use the matrices here, to make things a little easier
 
-    :param vector: 4-vector to be boosted
-    :param boostvector: boost vector.
-                        Can be either 3-vector or 4-vector
-                        (only spatial components are used)
-    :returns: Boosted 4-vector
+    Args:
+        vector (Union[jnp.array, np.array]): 4-vector to be boosted
+        boostvector (Union[jnp.array, np.array]): Boost momentum 4-vector in the same frame as vector
+                        (should have nonzero mass!)
+    Returns:
+        Union[jnp.array, np.array]: 4-vector boosted to the boostvector frame
 
     """
     boost = spatial_components(boostvector)
     b2 = scalar_product(boost, boost)
     gma = 1.0 / cb.sqrt(1.0 - b2)
     gma2 = (gma - 1.0) / b2
+    gma2 = cb.where(cb.isclose(b2, 0), 0 , gma2)
     ve = time_component(vector)
     vp = spatial_components(vector)
     bp = scalar_product(vp, boost)
     vp2 = vp + scalar(gma2 * bp + gma * ve) * boost
     ve2 = gma * (ve + bp)
+    
     return lorentz_vector(vp2, ve2)
 
 
-def boost_to_rest(vector, boostvector):
+def boost_to_rest(vector: Union[jnp.array, np.array], boostvector: Union[jnp.array, np.array]) -> Union[jnp.array, np.array]:
     """
     Perform Lorentz boost to the rest frame of the
     4-vector boostvector.
 
-    :param vector: 4-vector to be boosted
-    :param boostvector: Boost momentum 4-vector in the same frame as vector
+    Args:
+        vector (Union[jnp.array, np.array]): 4-vector to be boosted
+        boostvector (Union[jnp.array, np.array]): Boost momentum 4-vector in the same frame as vector
                         (should have nonzero mass!)
-    :returns: 4-vector boosed to boostvector rest frame
+    Returns:
+        Union[jnp.array, np.array]: 4-vector boosted to the rest frame of boostvector
 
     """
     boost = -spatial_components(boostvector) / scalar(time_component(boostvector))
     return lorentz_boost(vector, boost)
```

### Comparing `decayangle-1.0.2/src/decayangle/lorentz.py` & `decayangle-1.0.3/src/decayangle/lorentz.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Union
+from typing import Tuple, Union, Optional
 from collections import namedtuple
 import numpy as np
 import jax.numpy as jnp
 from decayangle.kinematics import (
     build_4_4,
     build_2_2,
     decode_4_4,
@@ -45,24 +45,25 @@
         if isinstance(other, LorentzTrafo):
             return LorentzTrafo(
                 matrix_2x2=self.matrix_2x2 @ other.matrix_2x2,
                 matrix_4x4=self.matrix_4x4 @ other.matrix_4x4,
             )
         raise ValueError("Only LorentzTrafo can be multiplied with LorentzTrafo")
 
-    def decode(self, two_pi_aware=True) -> Tuple[Union[np.array, jnp.array]]:
+    def decode(self, two_pi_aware=True, tol:Optional[float]=None) -> Tuple[Union[np.array, jnp.array]]:
         """Decode the parameters of the Lorentz transformation
 
         Args:
             two_pi_aware (bool, optional): If true the check for a roation of 2 pi will be made. Defaults to True.
+            tol (Optional[float], optional): The tolerance for the check of a 2 pi rotation. If None the default tolerance of the config will be used. Defaults to None.
 
         Returns:
             Tuple[Union[np.array, jnp.array]]: The parameters of the Lorentz transformation
         """
-        params = decode_4_4(self.matrix_4x4)
+        params = decode_4_4(self.matrix_4x4, tol=tol)
         if two_pi_aware:
             params = adjust_for_2pi_rotation(self.matrix_2x2, *params)
         return params
 
     def __repr__(self):
         return (
             "LorentzTrafo"
```

### Comparing `decayangle-1.0.2/src/decayangle/numerics_helpers.py` & `decayangle-1.0.3/src/decayangle/numerics_helpers.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/tests/test_Nbody.py` & `decayangle-1.0.3/tests/test_Nbody.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/tests/test_decay.py` & `decayangle-1.0.3/tests/test_decay.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/tests/test_kinematics.py` & `decayangle-1.0.3/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/tests/test_sorting.py` & `decayangle-1.0.3/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/tests/test_topology.py` & `decayangle-1.0.3/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/LICENSE.md` & `decayangle-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.2/README.md` & `decayangle-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 from decayangle.decay_topology import Topology
 from decayangle.config import config as cfg
 cfg.sorting = "off"
 
 root = 0
 topologies = [
     Topology(root, decay_topology=((1, 2), 3)),
-    Topology(root, decay_topology=((1, 3), 2)), 
+    Topology(root, decay_topology=((3, 1), 2)), 
     Topology(root, decay_topology=((2, 3), 1)) 
 ]
 ```
 
 A list of topologies can be fused into a `TopologyCollection` like
 
 ```python
@@ -182,15 +182,15 @@
 Intermediate node is written as tuples of the particles they consist of.
 Each intermediate state is represented by a `Node` object, which holds the information on the daughters of said state as well as its value (the aforementioned tuple). 
 
 A particular scheme is used to order daughters, and determine node names.
 Helicity angle are always calculated with respect to the first daughter.
 
 The ordering scheme can be customized at `TopologyCollection` level.
-The schemes is specified by a function, which is <expected to take in integers or tuples and return an integer used to sort the daughters, and integers in the node name. 
+The schemes is specified by a function, which is to take in a list or tuple of node values (tuples of integers or integers) and return the sorted version of it.
 
 ```python
 tg = TopologyCollection(0, [1,2,3])
 tg.ordering_function = lambda x: x
 ```
 The code above will just leave the object as it comes. Thus applying no sorting.
 
@@ -214,16 +214,31 @@
 
 ```python
 from decayangle.config import config as cfg
 cfg.numerical_safety_checks = False
 ```
 Now `nan` and `inf` will be handeled only by `numpy` internally.
 
-## Related projects
+## Further configuration options
+- The required precision for comparisons of $\gamma$. This controlls, which deviation of $\gamma$ from 1 is accepted before an exception is thrown. Thie default value should usually not be touched. In special cases, this may be useful though, if the decay topology is very complicated.
+
+```{python}
+from decayangle.config import config as cfg
+cfg.gamma_tolerance = 1e-8 # the absolute tolerance of gamma around 1
+# this is checked at numerous places in the code
+```
+
+- The required precision for a shift of $2 \pi$. This is checked to determine if the $2 \pi$ rotation needs to be applied. I.e. if the SU(2) matrix, which is build from the decoded angles is in the range of +- `cfg.shift_precision` of the matrix, which is produced during the consecutive boosts, then no $2 \pi$ shift is applied. If the negative of the SU(2) matrix, which is build from the decoded angles is in the range of +- `cfg.shift_precision` of the matrix, which is produced during the consecutive boosts, then a $2 \pi$ shift is applied. If both are true, then an error is thrown. Thus in rare cases the precision may have to be adjusted or the `cfg.numerical_safety_checks` config option has to be turned off. The exception is in place to warn the user of cases, where an ambiguity due to numerical imprecision may happen.
 
+```{python}
+from decayangle.config import config as cfg
+cfg.shift_precision = 1e-6
+```
+
+## Related projects
 Amplitude analyses dealing with non-zero spin of final-state particles have to implement wigner rotations in some way.
 However, there are a few projects addressing these rotations explicitly using analytic expressions in [DPD paper](https://inspirehep.net/literature/1758460), derived for three-body decays:
 - [ThreeBodyDecays.jl](https://github.com/mmikhasenko/ThreeBodyDecays.jl), 
 - [SymbolicThreeBodyDecays.jl](https://github.com/mmikhasenko/SymbolicThreeBodyDecays.jl),
 - [ComPWA/ampform-dpd](https://github.com/ComPWA/ampform-dpd).
 Consistency of the `decayangle` framework with these appoaches is validated in the tests.
```

### Comparing `decayangle-1.0.2/pyproject.toml` & `decayangle-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/decayangle"]
 
 [project]
 name = "decayangle"
 description = 'A tool for wigner rotations in n-body decays'
-version = '1.0.2'
+version = '1.0.3'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Kai Habermann", email = "kai.habermann@gmx.net" },
   { name = "Mikhail Mikhasenko", email = "mikhail.mikhasenko@cern.ch"},
```

### Comparing `decayangle-1.0.2/PKG-INFO` & `decayangle-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: decayangle
-Version: 1.0.2
+Version: 1.0.3
 Summary: A tool for wigner rotations in n-body decays
 Project-URL: Documentation, https://kaihabermann.github.io/decayangle/
 Project-URL: Issues, https://github.com/KaiHabermann/decayangle/issues
 Project-URL: Source, https://github.com/KaiHabermann/decayangle
 Author-email: Kai Habermann <kai.habermann@gmx.net>, Mikhail Mikhasenko <mikhail.mikhasenko@cern.ch>
 License-Expression: MIT
 License-File: LICENSE.md
@@ -157,15 +157,15 @@
 from decayangle.decay_topology import Topology
 from decayangle.config import config as cfg
 cfg.sorting = "off"
 
 root = 0
 topologies = [
     Topology(root, decay_topology=((1, 2), 3)),
-    Topology(root, decay_topology=((1, 3), 2)), 
+    Topology(root, decay_topology=((3, 1), 2)), 
     Topology(root, decay_topology=((2, 3), 1)) 
 ]
 ```
 
 A list of topologies can be fused into a `TopologyCollection` like
 
 ```python
@@ -209,15 +209,15 @@
 Intermediate node is written as tuples of the particles they consist of.
 Each intermediate state is represented by a `Node` object, which holds the information on the daughters of said state as well as its value (the aforementioned tuple). 
 
 A particular scheme is used to order daughters, and determine node names.
 Helicity angle are always calculated with respect to the first daughter.
 
 The ordering scheme can be customized at `TopologyCollection` level.
-The schemes is specified by a function, which is <expected to take in integers or tuples and return an integer used to sort the daughters, and integers in the node name. 
+The schemes is specified by a function, which is to take in a list or tuple of node values (tuples of integers or integers) and return the sorted version of it.
 
 ```python
 tg = TopologyCollection(0, [1,2,3])
 tg.ordering_function = lambda x: x
 ```
 The code above will just leave the object as it comes. Thus applying no sorting.
 
@@ -241,16 +241,31 @@
 
 ```python
 from decayangle.config import config as cfg
 cfg.numerical_safety_checks = False
 ```
 Now `nan` and `inf` will be handeled only by `numpy` internally.
 
-## Related projects
+## Further configuration options
+- The required precision for comparisons of $\gamma$. This controlls, which deviation of $\gamma$ from 1 is accepted before an exception is thrown. Thie default value should usually not be touched. In special cases, this may be useful though, if the decay topology is very complicated.
+
+```{python}
+from decayangle.config import config as cfg
+cfg.gamma_tolerance = 1e-8 # the absolute tolerance of gamma around 1
+# this is checked at numerous places in the code
+```
 
+- The required precision for a shift of $2 \pi$. This is checked to determine if the $2 \pi$ rotation needs to be applied. I.e. if the SU(2) matrix, which is build from the decoded angles is in the range of +- `cfg.shift_precision` of the matrix, which is produced during the consecutive boosts, then no $2 \pi$ shift is applied. If the negative of the SU(2) matrix, which is build from the decoded angles is in the range of +- `cfg.shift_precision` of the matrix, which is produced during the consecutive boosts, then a $2 \pi$ shift is applied. If both are true, then an error is thrown. Thus in rare cases the precision may have to be adjusted or the `cfg.numerical_safety_checks` config option has to be turned off. The exception is in place to warn the user of cases, where an ambiguity due to numerical imprecision may happen.
+
+```{python}
+from decayangle.config import config as cfg
+cfg.shift_precision = 1e-6
+```
+
+## Related projects
 Amplitude analyses dealing with non-zero spin of final-state particles have to implement wigner rotations in some way.
 However, there are a few projects addressing these rotations explicitly using analytic expressions in [DPD paper](https://inspirehep.net/literature/1758460), derived for three-body decays:
 - [ThreeBodyDecays.jl](https://github.com/mmikhasenko/ThreeBodyDecays.jl), 
 - [SymbolicThreeBodyDecays.jl](https://github.com/mmikhasenko/SymbolicThreeBodyDecays.jl),
 - [ComPWA/ampform-dpd](https://github.com/ComPWA/ampform-dpd).
 Consistency of the `decayangle` framework with these appoaches is validated in the tests.
```

