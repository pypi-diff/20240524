# Comparing `tmp/NodeGraphQt_QuiltiX_fork-0.6.0.tar.gz` & `tmp/nodegraphqt_quiltix_fork-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt_QuiltiX_fork-0.6.0.tar", last modified: Tue Aug  1 21:43:55 2023, max compression
+gzip compressed data, was "nodegraphqt_quiltix_fork-0.7.0.tar", last modified: Fri May 24 16:56:42 2024, max compression
```

## Comparing `NodeGraphQt_QuiltiX_fork-0.6.0.tar` & `nodegraphqt_quiltix_fork-0.7.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:55.074699 NodeGraphQt_QuiltiX_fork-0.6.0/
--rw-rw-rw-   0        0        0     1102 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/LICENSE.md
--rw-rw-rw-   0        0        0       49 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.808698 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/
--rw-rw-rw-   0        0        0     2469 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.832697 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/
--rw-rw-rw-   0        0        0        0 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/__init__.py
--rw-rw-rw-   0        0        0    12944 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/commands.py
--rw-rw-rw-   0        0        0     2816 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/factory.py
--rw-rw-rw-   0        0        0    95829 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/graph.py
--rw-rw-rw-   0        0        0     8107 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/menu.py
--rw-rw-rw-   0        0        0    14329 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/model.py
--rw-rw-rw-   0        0        0    14340 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/node.py
--rw-rw-rw-   0        0        0    12091 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/port.py
--rw-rw-rw-   0        0        0     7347 2023-04-19 19:16:50.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/constants.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.839700 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/
--rw-rw-rw-   0        0        0        0 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0    11832 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-rw-rw-   0        0        0     4621 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.866698 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/
--rw-rw-rw-   0        0        0        0 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-rw-rw-   0        0        0     4151 2023-04-19 19:16:50.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-rw-rw-   0        0        0     2455 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-rw-rw-   0        0        0     4995 2023-04-19 19:16:50.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-rw-rw-   0        0        0     6304 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-rw-rw-   0        0        0     2948 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-rw-rw-   0        0        0     2489 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-rw-rw-   0        0        0    20682 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-rw-rw-   0        0        0      761 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-rw-rw-   0        0        0     7267 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-rw-rw-   0        0        0      406 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/errors.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.880701 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/
--rw-rw-rw-   0        0        0        0 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/__init__.py
--rw-rw-rw-   0        0        0     4467 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/backdrop_node.py
--rw-rw-rw-   0        0        0    24217 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/base_node.py
--rw-rw-rw-   0        0        0     1251 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/base_node_circle.py
--rw-rw-rw-   0        0        0     5148 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/group_node.py
--rw-rw-rw-   0        0        0     3899 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/port_node.py
--rw-rw-rw-   0        0        0      239 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.920700 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/
--rw-rw-rw-   0        0        0        0 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/__init__.py
--rw-rw-rw-   0        0        0     7060 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_abstract.py
--rw-rw-rw-   0        0        0    10763 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_backdrop.py
--rw-rw-rw-   0        0        0    37593 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_base.py
--rw-rw-rw-   0        0        0    10186 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_circle.py
--rw-rw-rw-   0        0        0    12346 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_group.py
--rw-rw-rw-   0        0        0     4273 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-rw-rw-   0        0        0     3364 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_port_in.py
--rw-rw-rw-   0        0        0     3325 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_port_out.py
--rw-rw-rw-   0        0        0     3749 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_text_item.py
--rw-rw-rw-   0        0        0    17657 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/pipe.py
--rw-rw-rw-   0        0        0    10582 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/port.py
--rw-rw-rw-   0        0        0     2885 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/slicer.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.945702 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/
--rw-rw-rw-   0        0        0        0 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/__init__.py
--rw-rw-rw-   0        0        0     3709 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/actions.py
--rw-rw-rw-   0        0        0     1873 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/dialogs.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.994700 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/icons/
--rw-rw-rw-   0        0        0    17542 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/icons/node_base.png
--rw-rw-rw-   0        0        0     4572 2023-07-30 20:16:41.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/node_graph.py
--rw-rw-rw-   0        0        0    13125 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/node_widgets.py
--rw-rw-rw-   0        0        0     5681 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/scene.py
--rw-rw-rw-   0        0        0    11158 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/tab_search.py
--rw-rw-rw-   0        0        0    47477 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/viewer.py
--rw-rw-rw-   0        0        0     6506 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/viewer_nav.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:55.024702 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt_QuiltiX_fork.egg-info/
--rw-rw-rw-   0        0        0     1847 2023-08-01 21:43:54.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt_QuiltiX_fork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2847 2023-08-01 21:43:54.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt_QuiltiX_fork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 21:43:54.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt_QuiltiX_fork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-08-01 21:43:54.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt_QuiltiX_fork.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-08-01 21:43:54.000000 NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt_QuiltiX_fork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1847 2023-08-01 21:43:55.075699 NodeGraphQt_QuiltiX_fork-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1075 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:54.740699 NodeGraphQt_QuiltiX_fork-0.6.0/examples/
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:55.044700 NodeGraphQt_QuiltiX_fork-0.6.0/examples/hotkeys/
--rw-rw-rw-   0        0        0        0 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/examples/hotkeys/__init__.py
--rw-rw-rw-   0        0        0     5721 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/examples/hotkeys/hotkey_functions.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:43:55.071700 NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/
--rw-rw-rw-   0        0        0        0 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/__init__.py
--rw-rw-rw-   0        0        0     2032 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/basic_nodes.py
--rw-rw-rw-   0        0        0     3671 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/custom_ports_node.py
--rw-rw-rw-   0        0        0      507 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/group_node.py
--rw-rw-rw-   0        0        0     1822 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/widget_nodes.py
--rw-rw-rw-   0        0        0     1104 2023-08-01 21:43:55.078700 NodeGraphQt_QuiltiX_fork-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-03-29 14:41:32.000000 NodeGraphQt_QuiltiX_fork-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.685887 nodegraphqt_quiltix_fork-0.7.0/
+-rw-rw-rw-   0        0        0     1102 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/LICENSE.md
+-rw-rw-rw-   0        0        0       49 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.493400 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/
+-rw-rw-rw-   0        0        0     2469 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.513401 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/__init__.py
+-rw-rw-rw-   0        0        0    12946 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/commands.py
+-rw-rw-rw-   0        0        0     2816 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/factory.py
+-rw-rw-rw-   0        0        0    95884 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/graph.py
+-rw-rw-rw-   0        0        0     8109 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/menu.py
+-rw-rw-rw-   0        0        0    14329 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/model.py
+-rw-rw-rw-   0        0        0    14340 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/node.py
+-rw-rw-rw-   0        0        0    12091 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/port.py
+-rw-rw-rw-   0        0        0     7349 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.522402 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0    11834 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-rw-rw-   0        0        0     4623 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.549400 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-rw-rw-   0        0        0     4153 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-rw-rw-   0        0        0     2457 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-rw-rw-   0        0        0     5927 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-rw-rw-   0        0        0     6306 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-rw-rw-   0        0        0     2950 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-rw-rw-   0        0        0     2489 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-rw-rw-   0        0        0    20676 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-rw-rw-   0        0        0      763 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-rw-rw-   0        0        0     7269 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-rw-rw-   0        0        0      406 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.564405 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/__init__.py
+-rw-rw-rw-   0        0        0     4467 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/backdrop_node.py
+-rw-rw-rw-   0        0        0    24217 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/base_node.py
+-rw-rw-rw-   0        0        0     1251 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/base_node_circle.py
+-rw-rw-rw-   0        0        0     5148 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/group_node.py
+-rw-rw-rw-   0        0        0     3899 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/port_node.py
+-rw-rw-rw-   0        0        0      239 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/pkg_info.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.597401 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/__init__.py
+-rw-rw-rw-   0        0        0     7134 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_abstract.py
+-rw-rw-rw-   0        0        0    10765 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-rw-rw-   0        0        0    37633 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_base.py
+-rw-rw-rw-   0        0        0    10188 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_circle.py
+-rw-rw-rw-   0        0        0    12348 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_group.py
+-rw-rw-rw-   0        0        0     4275 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-rw-rw-   0        0        0     3366 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_port_in.py
+-rw-rw-rw-   0        0        0     3327 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_port_out.py
+-rw-rw-rw-   0        0        0     3751 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_text_item.py
+-rw-rw-rw-   0        0        0    17733 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/pipe.py
+-rw-rw-rw-   0        0        0    10694 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/port.py
+-rw-rw-rw-   0        0        0     2918 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/slicer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.626401 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3711 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/actions.py
+-rw-rw-rw-   0        0        0     1875 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/dialogs.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.629402 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/icons/
+-rw-rw-rw-   0        0        0    17542 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/icons/node_base.png
+-rw-rw-rw-   0        0        0     4574 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/node_graph.py
+-rw-rw-rw-   0        0        0    13127 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/node_widgets.py
+-rw-rw-rw-   0        0        0     5683 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/scene.py
+-rw-rw-rw-   0        0        0    11160 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/tab_search.py
+-rw-rw-rw-   0        0        0    47494 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/viewer.py
+-rw-rw-rw-   0        0        0     6576 2024-05-24 16:36:58.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/viewer_nav.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.682403 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt_QuiltiX_fork.egg-info/
+-rw-rw-rw-   0        0        0     1923 2024-05-24 16:56:42.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt_QuiltiX_fork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2608 2024-05-24 16:56:42.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt_QuiltiX_fork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 16:56:42.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt_QuiltiX_fork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-24 16:56:42.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt_QuiltiX_fork.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-24 16:56:42.000000 nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt_QuiltiX_fork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1923 2024-05-24 16:56:42.684404 nodegraphqt_quiltix_fork-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.471403 nodegraphqt_quiltix_fork-0.7.0/examples/
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.666404 nodegraphqt_quiltix_fork-0.7.0/examples/hotkeys/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/examples/hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     5721 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/examples/hotkeys/hotkey_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:56:42.679403 nodegraphqt_quiltix_fork-0.7.0/examples/nodes/
+-rw-rw-rw-   0        0        0        0 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/examples/nodes/__init__.py
+-rw-rw-rw-   0        0        0     2032 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/examples/nodes/basic_nodes.py
+-rw-rw-rw-   0        0        0     3671 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/examples/nodes/custom_ports_node.py
+-rw-rw-rw-   0        0        0      507 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/examples/nodes/group_node.py
+-rw-rw-rw-   0        0        0     1822 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/examples/nodes/widget_nodes.py
+-rw-rw-rw-   0        0        0     1101 2024-05-24 16:56:42.696402 nodegraphqt_quiltix_fork-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      123 2024-05-24 16:36:52.000000 nodegraphqt_quiltix_fork-0.7.0/setup.py
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/LICENSE.md` & `nodegraphqt_quiltix_fork-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/__init__.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/commands.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtWidgets
+from qtpy import QtWidgets
 
 from NodeGraphQt.constants import PortTypeEnum
 
 
 class PropertyChangedCmd(QtWidgets.QUndoCommand):
     """
     Node property changed command.
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/factory.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/graph.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 import copy
 import json
 import os
 import re
 
-from Qt import QtCore, QtWidgets
+from qtpy import QtCore, QtWidgets, QtGui
 
 from NodeGraphQt.base.commands import (NodeAddedCmd,
                                        NodeRemovedCmd,
                                        NodeMovedCmd,
                                        PortConnectedCmd)
 from NodeGraphQt.base.factory import NodeFactory
 from NodeGraphQt.base.menu import NodeGraphMenu, NodesMenu
@@ -145,15 +145,15 @@
             layout_direction = self._model.layout_direction
 
         self._node_factory = (
             kwargs.get('node_factory') or NodeFactory())
 
         self._undo_view = None
         self._undo_stack = (
-            kwargs.get('undo_stack') or QtWidgets.QUndoStack(self))
+            kwargs.get('undo_stack') or QtGui.QUndoStack(self))
 
         self._widget = None
 
         self._sub_graphs = {}
 
         self._viewer = (
             kwargs.get('viewer') or NodeViewer(undo_stack=self._undo_stack))
@@ -464,15 +464,15 @@
             NodeGraphWidget: node graph widget.
         """
         if self._widget is None:
             self._widget = NodeGraphWidget(graph=self)
             self._widget.addTab(self._viewer, 'Node Graph')
             # hide the close button on the first tab.
             tab_bar = self._widget.tabBar()
-            for btn_flag in [tab_bar.RightSide, tab_bar.LeftSide]:
+            for btn_flag in [QtWidgets.QTabBar.ButtonPosition.RightSide, QtWidgets.QTabBar.ButtonPosition.LeftSide]:
                 tab_btn = tab_bar.tabButton(0, btn_flag)
                 if tab_btn:
                     tab_btn.deleteLater()
                     tab_bar.setTabButton(0, btn_flag, None)
             self._widget.tabCloseRequested.connect(
                 self._on_close_sub_graph_tab
             )
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/menu.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 import re
 from distutils.version import LooseVersion
 
-from Qt import QtGui, QtCore
+from qtpy import QtGui, QtCore
 
 from NodeGraphQt.errors import NodeMenuError
 from NodeGraphQt.widgets.actions import BaseMenu, GraphAction, NodeAction
 
 
 class NodeGraphMenu(object):
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/model.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/node.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/base/port.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/constants.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 import os
 
-from Qt import QtWidgets
+from qtpy import QtWidgets
 from enum import Enum
 
 from .pkg_info import __version__ as _v
 
 __doc__ = """
 | The :py:mod:`NodeGraphQt.constants` namespace contains variables and enums 
  used throughout the NodeGraphQt library.
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/nodes_palette.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 from collections import defaultdict
 
-from Qt import QtWidgets, QtCore, QtGui
+from qtpy import QtWidgets, QtCore, QtGui
 
 from NodeGraphQt.constants import URN_SCHEME
 
 
 class NodesGridDelagate(QtWidgets.QStyledItemDelegate):
 
     def paint(self, painter, option, index):
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/nodes_tree.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-from Qt import QtWidgets, QtCore, QtGui
+from qtpy import QtWidgets, QtCore, QtGui
 
 from NodeGraphQt.constants import URN_SCHEME
 
 TYPE_NODE = QtWidgets.QTreeWidgetItem.UserType + 1
 TYPE_CATEGORY = QtWidgets.QTreeWidgetItem.UserType + 2
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtWidgets, QtCore, QtGui
+from qtpy import QtWidgets, QtCore, QtGui
 
 from .custom_widget_vectors import PropVector3, PropVector4
 from .prop_widgets_abstract import BaseProperty
 
 
 class PropColorPickerRGB(BaseProperty):
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtWidgets, QtCore
+from qtpy import QtWidgets, QtCore
 
 from NodeGraphQt.widgets.dialogs import FileDialog
 from .prop_widgets_abstract import BaseProperty
 
 
 class PropFilePath(BaseProperty):
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtWidgets, QtCore
+from qtpy import QtWidgets, QtCore
 
 from .prop_widgets_abstract import BaseProperty
 
 
 class PropSlider(BaseProperty):
     """
     Displays a node property as a "Slider" widget in the PropertiesBin
@@ -28,14 +28,15 @@
         self._spinbox.setButtonSymbols(QtWidgets.QAbstractSpinBox.NoButtons)
         layout = QtWidgets.QHBoxLayout(self)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.addWidget(self._spinbox)
         layout.addWidget(self._slider)
         # store the original press event.
         self._slider_mouse_press_event = self._slider.mousePressEvent
+        self._slider_mouse_release_event = self._slider.mouseReleaseEvent
         self._slider.mousePressEvent = self._on_slider_mouse_press
         self._slider.mouseReleaseEvent = self._on_slider_mouse_release
 
         if self._disable_scroll:
             self._slider.wheelEvent = lambda _: None
             self._spinbox.wheelEvent = lambda _: None
 
@@ -47,33 +48,39 @@
         self._block = True
         self._slider_mouse_press_event(event)
 
     def _on_slider_mouse_release(self, event):
         if not self._realtime_update:
             self.value_changed.emit(self.toolTip(), self.get_value())
         self._block = False
+        self._slider_mouse_release_event(event)
 
     def _on_slider_changed(self, value):
+        self._spinbox.blockSignals(True)
         self._spinbox.setValue(value)
+        self._spinbox.blockSignals(False)
         if self._realtime_update:
             self.value_changed.emit(self.toolTip(), self.get_value())
 
     def _on_spnbox_changed(self, value):
         if value != self._slider.value():
+            self._slider.blockSignals(True)
             self._slider.setValue(value)
+            self._slider.blockSignals(False)
             if not self._block:
                 self.value_changed.emit(self.toolTip(), self.get_value())
 
     def get_value(self):
         return self._spinbox.value()
 
     def set_value(self, value):
         if value != self.get_value():
             self._block = True
             self._spinbox.setValue(value)
+            self._slider.setValue(value)
             self.value_changed.emit(self.toolTip(), value)
             self._block = False
 
     def set_min(self, value=0):
         self._spinbox.setMinimum(value)
         self._slider.setMinimum(value)
 
@@ -118,15 +125,31 @@
     def __init__(self, parent=None, decimals=2, disable_scroll=True, realtime_update=False):
         # Do not initialize Propslider, just its parents
         super(PropSlider, self).__init__(parent)
         self._block = False
         self._realtime_update = realtime_update
         self._disable_scroll = disable_scroll
         self._slider = QDoubleSlider(decimals=decimals)
-        self._spinbox = QtWidgets.QDoubleSpinBox()
+        self._spinbox = PropDoubleSpinBox()
         self._init()
         self._init_signal_connections()
 
     def _init_signal_connections(self):
         self._spinbox.valueChanged.connect(self._on_spnbox_changed)
         # Connect to double_value_changed instead valueChanged
         self._slider.double_value_changed.connect(self._on_slider_changed)
+
+
+class PropDoubleSpinBox(QtWidgets.QDoubleSpinBox):
+    def __init__(self):
+        super(PropDoubleSpinBox, self).__init__()
+        self.setKeyboardTracking(False)
+
+    def valueFromText(self, text):
+        dp = self.locale().decimalPoint()
+        new_text = text.replace(",", dp).replace(".", dp)
+        return super(PropDoubleSpinBox, self).valueFromText(new_text)
+
+    def validate(self, text, pos):
+        dp = self.locale().decimalPoint()
+        new_text = text.replace(",", dp).replace(".", dp)
+        return super(PropDoubleSpinBox, self).validate(new_text, pos)
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtWidgets, QtCore, QtGui
+from qtpy import QtWidgets, QtCore, QtGui
 
 
 class _NumberValueMenu(QtWidgets.QMenu):
 
     mouseMove = QtCore.Signal(object)
     mouseRelease = QtCore.Signal(object)
     stepChange = QtCore.Signal()
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtWidgets
+from qtpy import QtWidgets
 
 from .custom_widget_value_edit import _NumberValueEdit
 from .prop_widgets_abstract import BaseProperty
 
 
 class _PropVector(BaseProperty):
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 from collections import defaultdict
 
-from Qt import QtWidgets, QtCore, QtGui, QtCompat
+from qtpy import QtWidgets, QtCore, QtGui
 
 from .node_property_factory import NodePropertyWidgetFactory
 from .prop_widgets_base import PropLineEdit
 
 
 class _PropertiesDelegate(QtWidgets.QStyledItemDelegate):
 
@@ -50,17 +50,17 @@
         super(_PropertiesList, self).__init__(parent)
         self.setItemDelegate(_PropertiesDelegate())
         self.setColumnCount(1)
         self.setShowGrid(False)
         self.verticalHeader().hide()
         self.horizontalHeader().hide()
 
-        QtCompat.QHeaderView.setSectionResizeMode(
+        QtWidgets.QHeaderView.setSectionResizeMode(
             self.verticalHeader(), QtWidgets.QHeaderView.ResizeToContents)
-        QtCompat.QHeaderView.setSectionResizeMode(
+        QtWidgets.QHeaderView.setSectionResizeMode(
             self.horizontalHeader(), 0, QtWidgets.QHeaderView.Stretch)
         self.setVerticalScrollMode(QtWidgets.QAbstractItemView.ScrollPerPixel)
 
     def wheelEvent(self, event):
         """
         Args:
             event (QtGui.QWheelEvent):
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtWidgets, QtCore
+from qtpy import QtWidgets, QtCore
 
 
 class BaseProperty(QtWidgets.QWidget):
     """
     Base class for a custom node property widget to be displayed in the
     PropertiesBin widget.
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtWidgets, QtCore
+from qtpy import QtWidgets, QtCore
 
 
 class PropLabel(QtWidgets.QLabel):
     """
     Displays a node property as a "QLabel" widget in the PropertiesBin widget.
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/backdrop_node.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/base_node.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/base_node_circle.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/group_node.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/nodes/port_node.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_abstract.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtCore, QtWidgets
+from qtpy import QtCore, QtWidgets
 
 from NodeGraphQt.constants import (
     Z_VAL_NODE,
     ITEM_CACHE_MODE,
     LayoutDirectionEnum,
     NodeEnum
 )
@@ -12,15 +12,15 @@
 class AbstractNodeItem(QtWidgets.QGraphicsItem):
     """
     The base class of all node qgraphics item.
     """
 
     def __init__(self, name='node', parent=None):
         super(AbstractNodeItem, self).__init__(parent)
-        self.setFlags(self.ItemIsSelectable | self.ItemIsMovable)
+        self.setFlags(QtWidgets.QGraphicsItem.GraphicsItemFlag.ItemIsSelectable | QtWidgets.QGraphicsItem.GraphicsItemFlag.ItemIsMovable)
         self.setCacheMode(ITEM_CACHE_MODE)
         self.setZValue(Z_VAL_NODE)
         self._properties = {
             'id': None,
             'name': name.strip(),
             'color': (13, 18, 23, 255),
             'border_color': (46, 57, 66, 255),
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_backdrop.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtGui, QtCore, QtWidgets
+from qtpy import QtGui, QtCore, QtWidgets
 
 from NodeGraphQt.constants import Z_VAL_PIPE, NodeEnum
 from NodeGraphQt.qgraphics.node_abstract import AbstractNodeItem
 from NodeGraphQt.qgraphics.pipe import PipeItem
 from NodeGraphQt.qgraphics.port import PortItem
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_base.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 from collections import OrderedDict
 
-from Qt import QtGui, QtCore, QtWidgets
+from qtpy import QtGui, QtCore, QtWidgets
 
 from NodeGraphQt.constants import (
     ITEM_CACHE_MODE,
     ICON_NODE_BASE,
     LayoutDirectionEnum,
     NodeEnum,
     PortEnum,
@@ -274,15 +274,15 @@
         """
         Re-implemented to update pipes on selection changed.
 
         Args:
             change:
             value:
         """
-        if change == self.ItemSelectedChange and self.scene():
+        if change == QtWidgets.QGraphicsItem.GraphicsItemChange.ItemSelectedChange and self.scene():
             self.reset_pipes()
             if value:
                 self.highlight_pipes()
             self.setZValue(Z_VAL_NODE)
             if not self.selected:
                 self.setZValue(Z_VAL_NODE + 1)
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_circle.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_circle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 from NodeGraphQt.constants import NodeEnum
 from NodeGraphQt.qgraphics.node_base import NodeItem
 
 
 class CircleNodeItem(NodeItem):
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_group.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 from NodeGraphQt.constants import NodeEnum, PortEnum
 from NodeGraphQt.qgraphics.node_base import NodeItem
 
 
 class GroupNodeItem(NodeItem):
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtGui, QtCore, QtWidgets
+from qtpy import QtGui, QtCore, QtWidgets
 
 from NodeGraphQt.constants import Z_VAL_NODE_WIDGET
 
 
 class XDisabledItem(QtWidgets.QGraphicsItem):
     """
     Node disabled overlay item.
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_port_in.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 from NodeGraphQt.constants import NodeEnum
 from NodeGraphQt.qgraphics.node_base import NodeItem
 
 
 class PortInputNodeItem(NodeItem):
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_port_out.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 from NodeGraphQt.constants import NodeEnum
 from NodeGraphQt.qgraphics.node_base import NodeItem
 
 
 class PortOutputNodeItem(NodeItem):
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/node_text_item.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Qt import QtWidgets, QtCore, QtGui
+from qtpy import QtWidgets, QtCore, QtGui
 
 
 class NodeTextItem(QtWidgets.QGraphicsTextItem):
     """
     NodeTextItem class used to display and edit the name of a NodeItem.
     """
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/pipe.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 import math
 
-from Qt import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 from NodeGraphQt.constants import (
     LayoutDirectionEnum,
     PipeEnum,
     PipeLayoutEnum,
     PortTypeEnum,
     ITEM_CACHE_MODE,
@@ -109,15 +109,15 @@
 
         pen = QtGui.QPen(color, pen_width, pen_style)
         pen.setCapStyle(QtCore.Qt.RoundCap)
         pen.setJoinStyle(QtCore.Qt.MiterJoin)
 
         painter.save()
         painter.setPen(pen)
-        painter.setRenderHint(painter.Antialiasing, True)
+        painter.setRenderHint(QtGui.QPainter.RenderHint.Antialiasing, True)
         painter.drawPath(self.path())
 
         # draw arrow
         if self.input_port and self.output_port:
             cen_x = self.path().pointAtPercent(0.5).x()
             cen_y = self.path().pointAtPercent(0.5).y()
             loc_pt = self.path().pointAtPercent(0.49)
@@ -358,15 +358,15 @@
         if self.input_port and self.input_port.node.disabled:
             return True
         if self.output_port and self.output_port.node.disabled:
             return True
         return False
 
     def itemChange(self, change, value):
-        if change == self.ItemSelectedChange and self.scene():
+        if change == QtWidgets.QGraphicsItem.GraphicsItemChange.ItemSelectedChange and self.scene():
             self.reset()
             if value:
                 self.highlight()
         return super(PipeItem, self).itemChange(change, value)
 
     @property
     def input_port(self):
@@ -438,15 +438,15 @@
 
         pen = QtGui.QPen(color, pen_width)
         pen.setStyle(pen_style)
         pen.setCapStyle(QtCore.Qt.RoundCap)
 
         painter.save()
         painter.setPen(pen)
-        painter.setRenderHint(painter.Antialiasing, True)
+        painter.setRenderHint(QtGui.QPainter.RenderHint.Antialiasing, True)
         painter.drawPath(self.path())
 
         cen_x = self.path().pointAtPercent(0.5).x()
         cen_y = self.path().pointAtPercent(0.5).y()
         loc_pt = self.path().pointAtPercent(0.9)
         tgt_pt = self.path().pointAtPercent(1.0)
         start_pt = self.path().pointAtPercent(0.0)
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/port.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/port.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtGui, QtCore, QtWidgets
+from qtpy import QtGui, QtCore, QtWidgets
 
 from NodeGraphQt.constants import (
     PortTypeEnum, PortEnum,
     Z_VAL_PORT,
     ITEM_CACHE_MODE)
 
 
@@ -12,16 +12,16 @@
     Base Port Item.
     """
 
     def __init__(self, parent=None):
         super(PortItem, self).__init__(parent)
         self.setAcceptHoverEvents(True)
         self.setCacheMode(ITEM_CACHE_MODE)
-        self.setFlag(self.ItemIsSelectable, False)
-        self.setFlag(self.ItemSendsScenePositionChanges, True)
+        self.setFlag(QtWidgets.QGraphicsItem.GraphicsItemFlag.ItemIsSelectable, False)
+        self.setFlag(QtWidgets.QGraphicsItem.GraphicsItemFlag.ItemSendsScenePositionChanges, True)
         self.setZValue(Z_VAL_PORT)
         self._pipes = []
         self._width = PortEnum.SIZE.value
         self._height = PortEnum.SIZE.value
         self._hovered = False
         self._name = 'port'
         self._display_name = True
@@ -110,15 +110,15 @@
             rect = QtCore.QRectF(port_rect.center().x() - w / 2,
                                  port_rect.center().y() - h / 2,
                                  w, h)
             painter.drawEllipse(rect)
         painter.restore()
 
     def itemChange(self, change, value):
-        if change == self.ItemScenePositionHasChanged:
+        if change == QtWidgets.QGraphicsItem.GraphicsItemChange.ItemScenePositionHasChanged:
             self.redraw_connected_pipes()
         return super(PortItem, self).itemChange(change, value)
 
     def mousePressEvent(self, event):
         super(PortItem, self).mousePressEvent(event)
         
     def mouseReleaseEvent(self, event):
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/qgraphics/slicer.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/qgraphics/slicer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python
 import math
 
-from Qt import QtCore, QtGui, QtWidgets
+from qtpy import QtCore, QtGui, QtWidgets
 
 from NodeGraphQt.constants import Z_VAL_NODE_WIDGET, PipeSlicerEnum
 
 
 class SlicerPipeItem(QtWidgets.QGraphicsPathItem):
     """
     Base item used for drawing the pipe connection slicer.
@@ -29,15 +29,15 @@
         p1 = self.path().pointAtPercent(0)
         p2 = self.path().pointAtPercent(1)
         size = 6.0
         offset = size / 2
         arrow_size = 4.0
 
         painter.save()
-        painter.setRenderHint(painter.Antialiasing, True)
+        painter.setRenderHint(QtGui.QPainter.RenderHint.Antialiasing.Antialiasing, True)
 
         font = painter.font()
         font.setPointSize(12)
         painter.setFont(font)
         text = 'slice'
         text_x = painter.fontMetrics().width(text) / 2
         text_y = painter.fontMetrics().height() / 1.5
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/actions.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtCore, QtWidgets
+from qtpy import QtCore, QtWidgets
 
 from NodeGraphQt.constants import ViewerEnum
 
 
 class BaseMenu(QtWidgets.QMenu):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/dialogs.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/dialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from Qt import QtWidgets
+from qtpy import QtWidgets
 
 _current_user_directory = os.path.expanduser('~')
 
 
 def set_dir(file):
     global _current_user_directory
     if os.path.isdir(file):
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/icons/node_base.png` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/node_graph.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/node_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Qt import QtWidgets, QtGui
+from qtpy import QtWidgets, QtGui
 
 from NodeGraphQt.constants import (
     NodeEnum, ViewerEnum, ViewerNavEnum
 )
 
 from NodeGraphQt.widgets.viewer_nav import NodeNavigationWidget
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/node_widgets.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/node_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtCore, QtWidgets
+from qtpy import QtCore, QtWidgets
 
 from NodeGraphQt.constants import ViewerEnum, Z_VAL_NODE_WIDGET
 from NodeGraphQt.errors import NodeWidgetError
 
 
 class _NodeGroupBox(QtWidgets.QGroupBox):
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/scene.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from Qt import QtGui, QtCore, QtWidgets
+from qtpy import QtGui, QtCore, QtWidgets
 
 from NodeGraphQt.constants import ViewerEnum
 
 
 class NodeScene(QtWidgets.QGraphicsScene):
 
     def __init__(self, parent=None):
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/tab_search.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/tab_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 import re
 from collections import OrderedDict
 
-from Qt import QtCore, QtWidgets, QtGui
+from qtpy import QtCore, QtWidgets, QtGui
 
 from NodeGraphQt.constants import ViewerEnum, ViewerNavEnum
 
 
 class TabSearchCompleter(QtWidgets.QCompleter):
     """
     QCompleter adapted from:
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/viewer.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 import math
 from distutils.version import LooseVersion
 
-from Qt import QtGui, QtCore, QtWidgets
+from qtpy import QtGui, QtCore, QtWidgets
 
 from NodeGraphQt.base.menu import BaseMenu
 from NodeGraphQt.constants import (
     LayoutDirectionEnum, PortTypeEnum, PipeLayoutEnum
 )
 from NodeGraphQt.qgraphics.node_abstract import AbstractNodeItem
 from NodeGraphQt.qgraphics.node_backdrop import BackdropNodeItem
@@ -569,15 +569,15 @@
         try:
             delta = event.delta()
         except AttributeError:
             # For PyQt5
             delta = event.angleDelta().y()
             if delta == 0:
                 delta = event.angleDelta().x()
-        self._set_viewer_zoom(delta, pos=event.pos())
+        self._set_viewer_zoom(delta, pos=event.position().toPoint())
 
     def dropEvent(self, event):
         pos = self.mapToScene(event.pos())
         event.setDropAction(QtCore.Qt.CopyAction)
         self.data_dropped.emit(
             event.mimeData(), QtCore.QPoint(pos.x(), pos.y()))
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt/widgets/viewer_nav.py` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt/widgets/viewer_nav.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Qt import QtWidgets, QtCore, QtGui
+from qtpy import QtWidgets, QtCore, QtGui
 
 from NodeGraphQt.constants import NodeEnum, ViewerNavEnum
 
 
 class NodeNavigationDelagate(QtWidgets.QStyledItemDelegate):
 
     def paint(self, painter, option, index):
@@ -91,18 +91,18 @@
 
 class NodeNavigationWidget(QtWidgets.QListView):
 
     navigation_changed = QtCore.Signal(str, list)
 
     def __init__(self, parent=None):
         super(NodeNavigationWidget, self).__init__(parent)
-        self.setSelectionMode(self.SingleSelection)
-        self.setResizeMode(self.Adjust)
-        self.setViewMode(self.ListMode)
-        self.setFlow(self.LeftToRight)
+        self.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
+        self.setResizeMode(QtWidgets.QListView.Adjust)
+        self.setViewMode(QtWidgets.QListView.ListMode)
+        self.setFlow(QtWidgets.QListView.LeftToRight)
         self.setDragEnabled(False)
         self.setMinimumHeight(20)
         self.setMaximumHeight(36)
         self.setSpacing(0)
 
         # self.viewport().setAutoFillBackground(False)
         self.setStyleSheet(
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt_QuiltiX_fork.egg-info/PKG-INFO` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt_QuiltiX_fork.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
-Name: NodeGraphQt-QuiltiX-fork
-Version: 0.6.0
-Summary: Node graph framework for PySide2/PyQt5 that can be
-Home-page: https://github.com/manuelkoester/NodeGraphQt/tree/develop
+Name: NodeGraphQt_QuiltiX_fork
+Version: 0.7.0
+Summary: [Fork] Node graph framework for PySide6 that can be
+Home-page: https://github.com/manuelkoester/NodeGraphQt/tree/qtpy
 Author: Johnny Chan, Manuel Koester, Richard Frangenberg
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: PySide2
 License-File: LICENSE.md
+Requires-Dist: qtpy>=2.3.0
+Provides-Extra: pyside6
+Requires-Dist: PySide6<6.7.0; extra == "pyside6"
 
 ## NodeGraphQt
 
 NodeGraphQt is a node graph UI framework for PySide2 that can be implemented and re-purposed into 
 applications.
 
 <img src="/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: NodeGraphQt-QuiltiX-fork Version: 0.6.0 Summary:
-Node graph framework for PySide2/PyQt5 that can be Home-page: https://
-github.com/manuelkoester/NodeGraphQt/tree/develop Author: Johnny Chan, Manuel
+Metadata-Version: 2.1 Name: NodeGraphQt_QuiltiX_fork Version: 0.7.0 Summary:
+[Fork] Node graph framework for PySide6 that can be Home-page: https://
+github.com/manuelkoester/NodeGraphQt/tree/qtpy Author: Johnny Chan, Manuel
 Koester, Richard Frangenberg License: MIT License Project-URL: Documentation,
 https://jchanvfx.github.io/NodeGraphQt/api/html/index.html Project-URL: Source,
 https://github.com/jchanvfx/NodeGraphQt/ Project-URL: Tracker, https://
 github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.6 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: PySide2 License-File: LICENSE.md ##
+Programming Language :: Python :: 3.9 Requires-Python: >=3.9 Description-
+Content-Type: text/markdown License-File: LICENSE.md Requires-Dist: qtpy>=2.3.0
+Provides-Extra: pyside6 Requires-Dist: PySide6<6.7.0; extra == "pyside6" ##
 NodeGraphQt NodeGraphQt is a node graph UI framework for PySide2 that can be
 implemented and re-purposed into applications. [/docs/_images/
 screenshot.png]#### Documentation _h_t_t_p_s_:_/_/_j_c_h_a_n_v_f_x_._g_i_t_h_u_b_._i_o_/_N_o_d_e_G_r_a_p_h_Q_t See
 the [basic_example.py](/examples/basic_example.py) python script from this
 repo. More examples can be found in the API documentation:
 https://jchanvfx.github.io/NodeGraphQt/api/html/examples/
 ex_overview.html#simple-example #### Vertical Layout [/docs/_images/
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/NodeGraphQt_QuiltiX_fork.egg-info/SOURCES.txt` & `nodegraphqt_quiltix_fork-0.7.0/NodeGraphQt_QuiltiX_fork.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -58,19 +58,14 @@
 NodeGraphQt/widgets/viewer_nav.py
 NodeGraphQt/widgets/icons/node_base.png
 NodeGraphQt_QuiltiX_fork.egg-info/PKG-INFO
 NodeGraphQt_QuiltiX_fork.egg-info/SOURCES.txt
 NodeGraphQt_QuiltiX_fork.egg-info/dependency_links.txt
 NodeGraphQt_QuiltiX_fork.egg-info/requires.txt
 NodeGraphQt_QuiltiX_fork.egg-info/top_level.txt
-NodeGraphQt_quiltix_fork.egg-info/PKG-INFO
-NodeGraphQt_quiltix_fork.egg-info/SOURCES.txt
-NodeGraphQt_quiltix_fork.egg-info/dependency_links.txt
-NodeGraphQt_quiltix_fork.egg-info/requires.txt
-NodeGraphQt_quiltix_fork.egg-info/top_level.txt
 examples/hotkeys/__init__.py
 examples/hotkeys/hotkey_functions.py
 examples/nodes/__init__.py
 examples/nodes/basic_nodes.py
 examples/nodes/custom_ports_node.py
 examples/nodes/group_node.py
 examples/nodes/widget_nodes.py
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/PKG-INFO` & `nodegraphqt_quiltix_fork-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt_QuiltiX_fork
-Version: 0.6.0
-Summary: Node graph framework for PySide2/PyQt5 that can be
-Home-page: https://github.com/manuelkoester/NodeGraphQt/tree/develop
+Version: 0.7.0
+Summary: [Fork] Node graph framework for PySide6 that can be
+Home-page: https://github.com/manuelkoester/NodeGraphQt/tree/qtpy
 Author: Johnny Chan, Manuel Koester, Richard Frangenberg
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: PySide2
 License-File: LICENSE.md
+Requires-Dist: qtpy>=2.3.0
+Provides-Extra: pyside6
+Requires-Dist: PySide6<6.7.0; extra == "pyside6"
 
 ## NodeGraphQt
 
 NodeGraphQt is a node graph UI framework for PySide2 that can be implemented and re-purposed into 
 applications.
 
 <img src="/docs/_images/screenshot.png" width="100%" title="NodeGraphQt">
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: NodeGraphQt_QuiltiX_fork Version: 0.6.0 Summary:
-Node graph framework for PySide2/PyQt5 that can be Home-page: https://
-github.com/manuelkoester/NodeGraphQt/tree/develop Author: Johnny Chan, Manuel
+Metadata-Version: 2.1 Name: NodeGraphQt_QuiltiX_fork Version: 0.7.0 Summary:
+[Fork] Node graph framework for PySide6 that can be Home-page: https://
+github.com/manuelkoester/NodeGraphQt/tree/qtpy Author: Johnny Chan, Manuel
 Koester, Richard Frangenberg License: MIT License Project-URL: Documentation,
 https://jchanvfx.github.io/NodeGraphQt/api/html/index.html Project-URL: Source,
 https://github.com/jchanvfx/NodeGraphQt/ Project-URL: Tracker, https://
 github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.6 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: PySide2 License-File: LICENSE.md ##
+Programming Language :: Python :: 3.9 Requires-Python: >=3.9 Description-
+Content-Type: text/markdown License-File: LICENSE.md Requires-Dist: qtpy>=2.3.0
+Provides-Extra: pyside6 Requires-Dist: PySide6<6.7.0; extra == "pyside6" ##
 NodeGraphQt NodeGraphQt is a node graph UI framework for PySide2 that can be
 implemented and re-purposed into applications. [/docs/_images/
 screenshot.png]#### Documentation _h_t_t_p_s_:_/_/_j_c_h_a_n_v_f_x_._g_i_t_h_u_b_._i_o_/_N_o_d_e_G_r_a_p_h_Q_t See
 the [basic_example.py](/examples/basic_example.py) python script from this
 repo. More examples can be found in the API documentation:
 https://jchanvfx.github.io/NodeGraphQt/api/html/examples/
 ex_overview.html#simple-example #### Vertical Layout [/docs/_images/
```

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/README.md` & `nodegraphqt_quiltix_fork-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/examples/hotkeys/hotkey_functions.py` & `nodegraphqt_quiltix_fork-0.7.0/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/basic_nodes.py` & `nodegraphqt_quiltix_fork-0.7.0/examples/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/custom_ports_node.py` & `nodegraphqt_quiltix_fork-0.7.0/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/examples/nodes/widget_nodes.py` & `nodegraphqt_quiltix_fork-0.7.0/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt_QuiltiX_fork-0.6.0/setup.cfg` & `nodegraphqt_quiltix_fork-0.7.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 6f64 6547 7261 7068 5174 5f51   = NodeGraphQt_Q
 00000020: 7569 6c74 6958 5f66 6f72 6b0d 0a76 6572  uiltiX_fork..ver
-00000030: 7369 6f6e 203d 2030 2e36 2e30 0d0a 6175  sion = 0.6.0..au
+00000030: 7369 6f6e 203d 2030 2e37 2e30 0d0a 6175  sion = 0.7.0..au
 00000040: 7468 6f72 203d 204a 6f68 6e6e 7920 4368  thor = Johnny Ch
 00000050: 616e 2c20 4d61 6e75 656c 204b 6f65 7374  an, Manuel Koest
 00000060: 6572 2c20 5269 6368 6172 6420 4672 616e  er, Richard Fran
 00000070: 6765 6e62 6572 670d 0a6c 6963 656e 7365  genberg..license
 00000080: 203d 204d 4954 204c 6963 656e 7365 0d0a   = MIT License..
 00000090: 6c69 6365 6e73 655f 6669 6c65 203d 204c  license_file = L
 000000a0: 4943 454e 5345 2e6d 640d 0a6c 6f6e 675f  ICENSE.md..long_
 000000b0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 000000c0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 000000d0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 000000e0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
 000000f0: 6578 742f 6d61 726b 646f 776e 0d0a 6465  ext/markdown..de
-00000100: 7363 7269 7074 696f 6e20 3d20 4e6f 6465  scription = Node
-00000110: 2067 7261 7068 2066 7261 6d65 776f 726b   graph framework
-00000120: 2066 6f72 2050 7953 6964 6532 2f50 7951   for PySide2/PyQ
-00000130: 7435 2074 6861 7420 6361 6e20 6265 0d0a  t5 that can be..
-00000140: 0969 6d70 6c65 6d65 6e74 6564 2061 6e64  .implemented and
-00000150: 2072 652d 7075 7270 6f73 6564 2069 6e74   re-purposed int
-00000160: 6f20 6170 706c 6963 6174 696f 6e73 2e0d  o applications..
-00000170: 0a63 6c61 7373 6966 6965 7273 203d 204f  .classifiers = O
-00000180: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000190: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-000001a0: 740d 0a09 4c69 6365 6e73 6520 3a3a 204f  t...License :: O
-000001b0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-000001c0: 4954 204c 6963 656e 7365 0d0a 0950 726f  IT License...Pro
-000001d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000001e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000001f0: 2e36 0d0a 7572 6c20 3d20 6874 7470 733a  .6..url = https:
-00000200: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 616e  //github.com/man
-00000210: 7565 6c6b 6f65 7374 6572 2f4e 6f64 6547  uelkoester/NodeG
-00000220: 7261 7068 5174 2f74 7265 652f 6465 7665  raphQt/tree/deve
-00000230: 6c6f 700d 0a70 726f 6a65 6374 5f75 726c  lop..project_url
-00000240: 7320 3d20 0d0a 0944 6f63 756d 656e 7461  s = ...Documenta
-00000250: 7469 6f6e 203d 2068 7474 7073 3a2f 2f6a  tion = https://j
-00000260: 6368 616e 7666 782e 6769 7468 7562 2e69  chanvfx.github.i
-00000270: 6f2f 4e6f 6465 4772 6170 6851 742f 6170  o/NodeGraphQt/ap
-00000280: 692f 6874 6d6c 2f69 6e64 6578 2e68 746d  i/html/index.htm
-00000290: 6c0d 0a09 536f 7572 6365 203d 2068 7474  l...Source = htt
-000002a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000002b0: 6a63 6861 6e76 6678 2f4e 6f64 6547 7261  jchanvfx/NodeGra
-000002c0: 7068 5174 2f0d 0a09 5472 6163 6b65 7220  phQt/...Tracker 
-000002d0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-000002e0: 2e63 6f6d 2f6a 6368 616e 7666 782f 4e6f  .com/jchanvfx/No
-000002f0: 6465 4772 6170 6851 742f 6973 7375 6573  deGraphQt/issues
-00000300: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
-00000310: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000320: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-00000330: 5f64 6174 6120 3d20 5472 7565 0d0a 7079  _data = True..py
-00000340: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000350: 3e3d 332e 360d 0a69 6e73 7461 6c6c 5f72  >=3.6..install_r
-00000360: 6571 7569 7265 7320 3d20 0d0a 0951 742e  equires = ...Qt.
-00000370: 7079 3e3d 312e 322e 300d 0a0d 0a5b 6f70  py>=1.2.0....[op
-00000380: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
-00000390: 7569 7265 5d0d 0a50 7953 6964 6532 203d  uire]..PySide2 =
-000003a0: 2050 7953 6964 6532 3e3d 352e 3135 0d0a   PySide2>=5.15..
-000003b0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000003c0: 6765 732e 6669 6e64 5d0d 0a65 7863 6c75  ges.find]..exclu
-000003d0: 6465 203d 2065 7861 6d70 6c65 730d 0a0d  de = examples...
-000003e0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000003f0: 655f 6461 7461 5d0d 0a4e 6f64 6547 7261  e_data]..NodeGra
-00000400: 7068 5174 203d 2077 6964 6765 7473 2f69  phQt = widgets/i
-00000410: 636f 6e73 2f6e 6f64 655f 6261 7365 2e70  cons/node_base.p
-00000420: 6e67 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ng....[egg_info]
-00000430: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-00000440: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000100: 7363 7269 7074 696f 6e20 3d20 5b46 6f72  scription = [For
+00000110: 6b5d 204e 6f64 6520 6772 6170 6820 6672  k] Node graph fr
+00000120: 616d 6577 6f72 6b20 666f 7220 5079 5369  amework for PySi
+00000130: 6465 3620 7468 6174 2063 616e 2062 650d  de6 that can be.
+00000140: 0a09 696d 706c 656d 656e 7465 6420 616e  ..implemented an
+00000150: 6420 7265 2d70 7572 706f 7365 6420 696e  d re-purposed in
+00000160: 746f 2061 7070 6c69 6361 7469 6f6e 732e  to applications.
+00000170: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+00000180: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000190: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001a0: 6e74 0d0a 094c 6963 656e 7365 203a 3a20  nt...License :: 
+000001b0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+000001c0: 4d49 5420 4c69 6365 6e73 650d 0a09 5072  MIT License...Pr
+000001d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001f0: 332e 390d 0a75 726c 203d 2068 7474 7073  3.9..url = https
+00000200: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d61  ://github.com/ma
+00000210: 6e75 656c 6b6f 6573 7465 722f 4e6f 6465  nuelkoester/Node
+00000220: 4772 6170 6851 742f 7472 6565 2f71 7470  GraphQt/tree/qtp
+00000230: 790d 0a70 726f 6a65 6374 5f75 726c 7320  y..project_urls 
+00000240: 3d20 0d0a 0944 6f63 756d 656e 7461 7469  = ...Documentati
+00000250: 6f6e 203d 2068 7474 7073 3a2f 2f6a 6368  on = https://jch
+00000260: 616e 7666 782e 6769 7468 7562 2e69 6f2f  anvfx.github.io/
+00000270: 4e6f 6465 4772 6170 6851 742f 6170 692f  NodeGraphQt/api/
+00000280: 6874 6d6c 2f69 6e64 6578 2e68 746d 6c0d  html/index.html.
+00000290: 0a09 536f 7572 6365 203d 2068 7474 7073  ..Source = https
+000002a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a63  ://github.com/jc
+000002b0: 6861 6e76 6678 2f4e 6f64 6547 7261 7068  hanvfx/NodeGraph
+000002c0: 5174 2f0d 0a09 5472 6163 6b65 7220 3d20  Qt/...Tracker = 
+000002d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000002e0: 6f6d 2f6a 6368 616e 7666 782f 4e6f 6465  om/jchanvfx/Node
+000002f0: 4772 6170 6851 742f 6973 7375 6573 0d0a  GraphQt/issues..
+00000300: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
+00000310: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
+00000320: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000330: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
+00000340: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000350: 332e 390d 0a69 6e73 7461 6c6c 5f72 6571  3.9..install_req
+00000360: 7569 7265 7320 3d20 0d0a 0971 7470 793e  uires = ...qtpy>
+00000370: 3d32 2e33 2e30 0d0a 0d0a 5b6f 7074 696f  =2.3.0....[optio
+00000380: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
+00000390: 655d 0d0a 5079 5369 6465 3620 3d20 5079  e]..PySide6 = Py
+000003a0: 5369 6465 363c 362e 372e 300d 0a0d 0a5b  Side6<6.7.0....[
+000003b0: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+000003c0: 2e66 696e 645d 0d0a 6578 636c 7564 6520  .find]..exclude 
+000003d0: 3d20 6578 616d 706c 6573 0d0a 0d0a 5b6f  = examples....[o
+000003e0: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
+000003f0: 6174 615d 0d0a 4e6f 6465 4772 6170 6851  ata]..NodeGraphQ
+00000400: 7420 3d20 7769 6467 6574 732f 6963 6f6e  t = widgets/icon
+00000410: 732f 6e6f 6465 5f62 6173 652e 706e 670d  s/node_base.png.
+00000420: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000430: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000440: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

