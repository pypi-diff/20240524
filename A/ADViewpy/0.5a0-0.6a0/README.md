# Comparing `tmp/ADViewpy-0.5a0.tar.gz` & `tmp/ADViewpy-0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ADViewpy-0.5a0.tar", last modified: Wed May 22 13:57:15 2024, max compression
+gzip compressed data, was "ADViewpy-0.6a0.tar", last modified: Fri May 24 05:51:58 2024, max compression
```

## Comparing `ADViewpy-0.5a0.tar` & `ADViewpy-0.6a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:57:15.590843 ADViewpy-0.5a0/
-drwxrwxrwx   0        0        0        0 2024-05-22 13:57:15.585029 ADViewpy-0.5a0/ADViewpy/
--rw-rw-rw-   0        0        0    46666 2024-05-22 13:41:29.000000 ADViewpy-0.5a0/ADViewpy/ADViewpy.py
--rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.5a0/ADViewpy/__init__.py
--rw-rw-rw-   0        0        0    19348 2024-05-22 13:41:29.000000 ADViewpy-0.5a0/ADViewpy/myCanvas.py
--rw-rw-rw-   0        0        0     3062 2024-05-21 03:27:21.000000 ADViewpy-0.5a0/ADViewpy/myUtils.py
--rw-rw-rw-   0        0        0    56158 2024-05-22 13:41:29.000000 ADViewpy-0.5a0/ADViewpy/pairwiseCanvas.py
--rw-rw-rw-   0        0        0    23499 2024-05-22 13:41:29.000000 ADViewpy-0.5a0/ADViewpy/rtCanvas.py
--rw-rw-rw-   0        0        0    65738 2024-05-22 13:41:29.000000 ADViewpy-0.5a0/ADViewpy/tcCanvas.py
--rw-rw-rw-   0        0        0    21925 2024-05-22 13:41:29.000000 ADViewpy-0.5a0/ADViewpy/treeDistributionView.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:57:15.589846 ADViewpy-0.5a0/ADViewpy.egg-info/
--rw-rw-rw-   0        0        0     6202 2024-05-22 13:57:15.000000 ADViewpy-0.5a0/ADViewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-05-22 13:57:15.000000 ADViewpy-0.5a0/ADViewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:57:15.000000 ADViewpy-0.5a0/ADViewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-22 13:57:15.000000 ADViewpy-0.5a0/ADViewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-22 13:57:15.000000 ADViewpy-0.5a0/ADViewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6202 2024-05-22 13:57:15.591847 ADViewpy-0.5a0/PKG-INFO
--rw-rw-rw-   0        0        0     5716 2024-05-21 03:16:52.000000 ADViewpy-0.5a0/README.md
--rw-rw-rw-   0        0        0      554 2024-05-22 13:57:10.000000 ADViewpy-0.5a0/pyproject.toml
--rw-rw-rw-   0        0        0       94 2024-05-22 13:57:15.592844 ADViewpy-0.5a0/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-22 13:57:10.000000 ADViewpy-0.5a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:51:58.302763 ADViewpy-0.6a0/
+drwxrwxrwx   0        0        0        0 2024-05-24 05:51:58.294997 ADViewpy-0.6a0/ADViewpy/
+-rw-rw-rw-   0        0        0    46666 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/ADViewpy.py
+-rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.6a0/ADViewpy/__init__.py
+-rw-rw-rw-   0        0        0    19348 2024-05-24 05:51:48.000000 ADViewpy-0.6a0/ADViewpy/myCanvas.py
+-rw-rw-rw-   0        0        0     3062 2024-05-21 03:27:21.000000 ADViewpy-0.6a0/ADViewpy/myUtils.py
+-rw-rw-rw-   0        0        0    56104 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/pairwiseCanvas.py
+-rw-rw-rw-   0        0        0    23713 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/rtCanvas.py
+-rw-rw-rw-   0        0        0    65738 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/tcCanvas.py
+-rw-rw-rw-   0        0        0    22310 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/treeDistributionView.py
+drwxrwxrwx   0        0        0        0 2024-05-24 05:51:58.301764 ADViewpy-0.6a0/ADViewpy.egg-info/
+-rw-rw-rw-   0        0        0     6202 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6202 2024-05-24 05:51:58.303763 ADViewpy-0.6a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5716 2024-05-21 03:16:52.000000 ADViewpy-0.6a0/README.md
+-rw-rw-rw-   0        0        0      554 2024-05-24 05:51:48.000000 ADViewpy-0.6a0/pyproject.toml
+-rw-rw-rw-   0        0        0       94 2024-05-24 05:51:58.303763 ADViewpy-0.6a0/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-24 05:51:48.000000 ADViewpy-0.6a0/setup.py
```

### Comparing `ADViewpy-0.5a0/ADViewpy/ADViewpy.py` & `ADViewpy-0.6a0/ADViewpy/ADViewpy.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.5a0/ADViewpy/myCanvas.py` & `ADViewpy-0.6a0/ADViewpy/myCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.5a0/ADViewpy/myUtils.py` & `ADViewpy-0.6a0/ADViewpy/myUtils.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.5a0/ADViewpy/pairwiseCanvas.py` & `ADViewpy-0.6a0/ADViewpy/pairwiseCanvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,15 +511,15 @@
                 similarity = "Similarity :  " + str(node.pairwise_similarity * 100) + "%"
             else:
                 similarity = "Similarity :  " + str(node.corr_similarity * 100) + "%"
 
         if len(similarity) * 10 > label_length:
             label_length = len(similarity) * 10
 
-        label_x = self.left_tree_width + ((self.right_tree_width - self.left_tree_width - 50) / 2)
+        label_x = self.left_tree_width - 100
         label_y = node.pos_in_pairwise.y
         if node.pos_in_pairwise.y + 40 > self.height:
             label_y = self.height - 40
 
         if subtree_root:
             self.draw_rec(label_x-10 , label_y - 15, label_length + 10,65,BLACK,self.HOVER_NODE_LAYER)
         else:
```

### Comparing `ADViewpy-0.5a0/ADViewpy/rtCanvas.py` & `ADViewpy-0.6a0/ADViewpy/rtCanvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,27 +205,35 @@
                               layer_index=self.FILTER_NODE_LAYER)
 
     def check_attribute_in_range(self,node):
         exact_match_result = False
         support_value_result = False
 
         if self.support_value_interval:
-            if node.support >= self.support_value_interval[0] and node.support <= self.support_value_interval[1]:
+            if (node.label and int(node.label) >= self.support_value_interval[0] and int(node.label) <=
+                    self.support_value_interval[1]):
                 support_value_result = True
             else:
                 support_value_result = False
 
+        elif self.exact_match_interval:
+            support_value_result = True
+
         if self.exact_match_interval:
             exact_match_percentage = node.exact_match / len(self.adPy.tc) * 100
 
             if exact_match_percentage >= self.exact_match_interval[0] and exact_match_percentage <= self.exact_match_interval[1]:
                 exact_match_result = True
             else:
                 exact_match_result = False
 
+        elif self.support_value_interval:
+            exact_match_result = True
+
+
         return (exact_match_result and support_value_result)
 
     def insert_node_section_list(self,node):
         top_section_index = math.floor(node.mouse_range.topL.y / MIN_SECTION_HEIGHT)
         bottom_section_index = math.floor(node.mouse_range.botR.y / MIN_SECTION_HEIGHT)
 
         if not self.inner_section:
```

### Comparing `ADViewpy-0.5a0/ADViewpy/tcCanvas.py` & `ADViewpy-0.6a0/ADViewpy/tcCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.5a0/ADViewpy/treeDistributionView.py` & `ADViewpy-0.6a0/ADViewpy/treeDistributionView.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,21 +186,29 @@
         segment_allocatable_width = self.segment_bar_width - segment_count * MINIMUN_BUTTON_WIDTH
         color = LIGHT_GREY
 
         sorted_topology_list = sorted(self.subtree_chosen.topology_list.items(), key=lambda x: len(x[1][1]),
                                       reverse=True)
         self.segment_button_list = []
         for item in sorted_topology_list:
+            self.adPy.output.append(item[1][0])
             tree_list = item[1][1]
 
             new_button_style = widgets.ButtonStyle(button_color=color)
             color = lighten_color(color,amount=20)
 
-            button_width = MINIMUN_BUTTON_WIDTH + (len(tree_list)/total_grid * segment_allocatable_width)
-            new_button = widgets.Button(description=str(len(tree_list)), style=new_button_style,
+            button_width = MINIMUN_BUTTON_WIDTH + (len(tree_list)/total_grid * segment_allocatable_width)\
+
+            nodes_list = item[0].split(',')
+            if set(nodes_list) == self.subtree_chosen.leaf_set:
+                des_str = str(len(tree_list)) + "(R)"
+            else:
+                des_str = str(len(tree_list))
+
+            new_button = widgets.Button(description=des_str, style=new_button_style,
                                   layout=widgets.Layout(width=f'{button_width}px', height=f'{self.subtree_button_height}px',justify_content='flex-start'))
             new_button.style.font_weight = 'normal'
             new_button.style.font_family = self.FONT_FAMILY
             new_button.style.font_size = self.FONT_SIZE
             new_button.metadata = {'nodes_str' : item[0],'nodes_list': item[1][0],'tree_list': tree_list}
             new_button.on_click(self.on_segment_button_click)
 
@@ -263,14 +271,20 @@
     def draw_canvas_vgridbox(self):
     #     grid = widgets.GridBox([canvas1, canvas2, canvas3], layout=widgets.Layout(grid_template_columns="1fr", grid_gap='0px'))
         pass
 
     def draw_nodes_canvas(self):
         nodes_list = self.segment_button_clicked.metadata.get('nodes_str').split(',')
 
+        self.adPy.output.append(nodes_list)
+        self.adPy.output.append(self.subtree_chosen.leaf_set)
+
+        if set(nodes_list) == self.subtree_chosen.leaf_set:
+            self.agree_rt = True
+
         tmp_canvas = Canvas(width=self.DEFAULT_CANVAS_WIDTH, height=len(nodes_list) * RT_Y_INTERVAL + 30)
         tmp_canvas.fill_style = BLACK
         tmp_canvas.font = f'18px {self.FONT_FAMILY}'
 
         pointer_x = 10
         pointer_y = 20
         tmp_canvas.fill_text("Nodes in Subtree: ", pointer_x, pointer_y)
@@ -362,15 +376,15 @@
 
         for topology in topology_set:
             ad_canvas = Canvas(width = DEFAULT_AD_WIDTH + 10 ,height = ad_height + 10)
             ad_canvas.tree_count = topology_list.count(topology)
 
             self.tc_canvas_tmp.draw_cluster_number_bar(topology.sample_ad_tree, topology_list.count(topology),
                                                        canvas=ad_canvas,agree_rt=topology.agree_rt)
-            self.agree_rt = topology.agree_rt
+
             self.tc_canvas_tmp.draw_ad_tree(topology.sample_ad_tree, ad_canvas,cluster=True)
             ad_canvas.stroke_style = BLACK
             ad_canvas.stroke_rect(topology.sample_ad_tree.topL.x, topology.sample_ad_tree.topL.y,
                                   topology.sample_ad_tree.width, topology.sample_ad_tree.height)
             self.cluster_list.append(ad_canvas)
 
 
@@ -401,15 +415,14 @@
     def draw_canvas_frame(self,canvas):
         canvas.stroke_style = GREY
         canvas.stroke_rect(0, 0, canvas.width, canvas.height)
         canvas.stroke_rect(2, 2, canvas.width - 4, canvas.height - 4)
     def draw_rt_subtree_block_canvas(self):
         # 先在reference tree画黑点，然后再crop出来
         rt_canvas = self.adPy.rt_canvas
-        rt_canvas.clear_subtree_compare_canvas()
         nodes = self.segment_button_clicked.metadata.get('nodes_list')
         rt_canvas.draw_subtree_compare_nodes(nodes)
 
         self.rt_subtree_canvas_tmp = Canvas(width = rt_canvas.width,height = rt_canvas.height,sync_image_data=True)
         subtree_layer = rt_canvas.sorted_layer_list.index(self.subtree_chosen.label)
 
         self.rt_subtree_canvas_tmp.draw_image(rt_canvas[subtree_layer], 0, 0)
```

### Comparing `ADViewpy-0.5a0/ADViewpy.egg-info/PKG-INFO` & `ADViewpy-0.6a0/ADViewpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADViewpy
-Version: 0.5a0
+Version: 0.6a0
 Summary: ADViewpy is Python Library to visually compare phylogenetic trees
 Author: Ng Weng Shan
 Author-email: ngwengshan025@hotmail.com
 Project-URL: Homepage, https://github.com/Coralnws/ADViewpy-alpha.git
 Keywords: python,phylogenetic tree,aggregrated dendrogram,tree comparison
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ADViewpy-0.5a0/PKG-INFO` & `ADViewpy-0.6a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADViewpy
-Version: 0.5a0
+Version: 0.6a0
 Summary: ADViewpy is Python Library to visually compare phylogenetic trees
 Author: Ng Weng Shan
 Author-email: ngwengshan025@hotmail.com
 Project-URL: Homepage, https://github.com/Coralnws/ADViewpy-alpha.git
 Keywords: python,phylogenetic tree,aggregrated dendrogram,tree comparison
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ADViewpy-0.5a0/README.md` & `ADViewpy-0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.5a0/pyproject.toml` & `ADViewpy-0.6a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ADViewpy"
-version = '0.5.alpha'
+version = '0.6.alpha'
 description = "ADViewpy is Python Library to visually compare phylogenetic trees"
 readme = "README.md"
 #dependencies=[
 #        'dendropy',
 #        'ipycanvas',
 #        'ipywidgets',
 #        'scikit-learn',
```

### Comparing `ADViewpy-0.5a0/setup.py` & `ADViewpy-0.6a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.5.alpha'
+VERSION = '0.6.alpha'
 DESCRIPTION = ('ADViewpy is Python Library to visually compare phylogenetic trees')
 LONG_DESCRIPTION = 'ADViewpy is Python Library to visually compare phylogenetic trees, utilizing Aggregated Dendrogram for phylogenetic tree visualization. '
 
 
 setup(
     name="ADViewpy",
     version=VERSION,
```

