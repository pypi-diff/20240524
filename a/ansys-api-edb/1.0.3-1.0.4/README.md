# Comparing `tmp/ansys_api_edb-1.0.3.tar.gz` & `tmp/ansys_api_edb-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_api_edb-1.0.3.tar", last modified: Wed Apr 24 18:44:02 2024, max compression
+gzip compressed data, was "ansys_api_edb-1.0.4.tar", last modified: Fri May 24 11:47:41 2024, max compression
```

## Comparing `ansys_api_edb-1.0.3.tar` & `ansys_api_edb-1.0.4.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:44:02.186763 ansys_api_edb-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 18:44:02.186763 ansys_api_edb-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:44:02.166763 ansys_api_edb-1.0.3/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:44:02.166763 ansys_api_edb-1.0.3/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:44:02.166763 ansys_api_edb-1.0.3/ansys/api/edb/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:44:02.182763 ansys_api_edb-1.0.3/ansys/api/edb/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/arc_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/board_bend_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/bondwire.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/bondwire_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/bundle_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/cell.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/cell_instance.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/circle.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/component_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/component_group.proto
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/component_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/component_pin.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/component_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/connectable.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/database.proto
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/dataset_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/debye_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/definition_obj.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/die_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/dielectric_material_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/differential_pair.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/djordjecvic_sarkar_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/edb_defs.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/edb_messages.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/edge_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/extended_net.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/group.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/hfss_simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/hfss_simulation_setup.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/hierarchy_obj.proto
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/ic_component_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/inst_array.proto
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/io_component_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layer_collection.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layer_map.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layout.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_instance.proto
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_instance_context.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj_instance.proto
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj_instance_2d_geometry.proto
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj_instance_3d_geometry.proto
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj_instance_geometry.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/material_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/material_property_thermal_modifier.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/mcad_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/multipole_debye_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/net.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/netclass.proto
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/netlist_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/package_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/padstack_def.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/padstack_def_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/padstack_inst_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/padstack_instance.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/path.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/pin_group.proto
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/pin_group_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/pin_pair_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/point_3d_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/point_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/point_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/polygon.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/polygon_data.proto
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/port_post_processing_prop.proto
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/port_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/primitive.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/r_tree.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/raptor_x_simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/rectangle.proto
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/refs.proto
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/rlc.proto
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/rlc_component_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/simulation_setup.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/siwave_dcir_simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/siwave_simulation_settings.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/solder_ball_property.proto
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/sparameter_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/spice_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/stackup_layer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/structure3d.proto
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/term_inst.proto
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/term_inst_term.proto
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/text.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/transform.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/transform3d.proto
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/value.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/variable_server.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/via_group.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/via_layer.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/ansys/api/edb/v1/voltage_regulator.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:44:02.182763 ansys_api_edb-1.0.3/ansys_api_edb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 18:44:02.000000 ansys_api_edb-1.0.3/ansys_api_edb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-24 18:44:02.000000 ansys_api_edb-1.0.3/ansys_api_edb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:44:02.000000 ansys_api_edb-1.0.3/ansys_api_edb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 18:44:02.000000 ansys_api_edb-1.0.3/ansys_api_edb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 18:44:02.000000 ansys_api_edb-1.0.3/ansys_api_edb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 18:44:02.000000 ansys_api_edb-1.0.3/ansys_api_edb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:44:02.186763 ansys_api_edb-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-24 18:43:52.000000 ansys_api_edb-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:41.021328 ansys_api_edb-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-24 11:47:41.021328 ansys_api_edb-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:41.005328 ansys_api_edb-1.0.4/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:41.005328 ansys_api_edb-1.0.4/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:41.005328 ansys_api_edb-1.0.4/ansys/api/edb/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:41.021328 ansys_api_edb-1.0.4/ansys/api/edb/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/arc_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/board_bend_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/bondwire.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/bondwire_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/bundle_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/cell.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/cell_instance.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/circle.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/component_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/component_group.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/component_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/component_pin.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/component_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/connectable.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/database.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/dataset_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/debye_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/definition_obj.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/die_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/dielectric_material_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/differential_pair.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/djordjecvic_sarkar_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/edb_defs.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/edb_messages.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/edge_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/extended_net.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/group.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/hfss_simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/hfss_simulation_setup.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/hierarchy_obj.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/ic_component_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/inst_array.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/io_component_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layer_collection.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layer_map.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layout.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_instance.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_instance_context.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj_instance.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj_instance_2d_geometry.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj_instance_3d_geometry.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj_instance_geometry.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/material_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/material_property_thermal_modifier.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/mcad_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/multipole_debye_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/net.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/netclass.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/netlist_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/package_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/padstack_def.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/padstack_def_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/padstack_inst_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/padstack_instance.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/path.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/pin_group.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/pin_group_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/pin_pair_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/point_3d_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/point_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/point_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/polygon.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/polygon_data.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/port_post_processing_prop.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/port_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/primitive.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/r_tree.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/raptor_x_simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/rectangle.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/refs.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/rlc.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/rlc_component_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/simulation_setup.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/siwave_dcir_simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/siwave_simulation_settings.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/solder_ball_property.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/sparameter_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/spice_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/stackup_layer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/structure3d.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/term_inst.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/term_inst_term.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/text.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/transform.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/transform3d.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/value.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/variable_server.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/via_group.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/via_layer.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/ansys/api/edb/v1/voltage_regulator.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:41.021328 ansys_api_edb-1.0.4/ansys_api_edb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-24 11:47:40.000000 ansys_api_edb-1.0.4/ansys_api_edb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-24 11:47:41.000000 ansys_api_edb-1.0.4/ansys_api_edb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:47:40.000000 ansys_api_edb-1.0.4/ansys_api_edb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 11:47:40.000000 ansys_api_edb-1.0.4/ansys_api_edb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 11:47:40.000000 ansys_api_edb-1.0.4/ansys_api_edb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 11:47:40.000000 ansys_api_edb-1.0.4/ansys_api_edb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:47:41.021328 ansys_api_edb-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-24 11:47:33.000000 ansys_api_edb-1.0.4/setup.py
```

### Comparing `ansys_api_edb-1.0.3/LICENCE` & `ansys_api_edb-1.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/PKG-INFO` & `ansys_api_edb-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-edb
-Version: 1.0.3
-Summary: Autogenerated Python gRPC interface package for ansys-api-edb, built on 18:44:02 on 24 April 2024
+Version: 1.0.4
+Summary: Autogenerated Python gRPC interface package for ansys-api-edb, built on 11:47:40 on 24 May 2024
 Home-page: https://github.com/ansys/ansys-api-edb
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-edb/#readme
```

### Comparing `ansys_api_edb-1.0.3/README.md` & `ansys_api_edb-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/arc_data.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/arc_data.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/board_bend_def.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/board_bend_def.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/bondwire.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/bondwire.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/bondwire_def.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/bondwire_def.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/cell.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/cell.proto`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
   rpc SetProductProperty (SetProductPropertyMessage) returns (google.protobuf.Empty) {}
 
   // Delete a simulation setup by name
   rpc DeleteSimulationSetup (StringPropertyMessage) returns (google.protobuf.Empty) {}
 
   // Get simulation setups
   rpc GetSimulationSetups (EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamSimulationSetups (EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Generate auto HFSS regions
   rpc GenerateAutoHFSSRegions (EDBObjMessage) returns (google.protobuf.Empty) {}
 
   // Generate via smart box
   rpc GenerateViaSmartBox (StringPropertyMessage) returns (PolygonDataListMessage) {}
 }
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/cell_instance.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/cell_instance.proto`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   rpc FindByName(ObjectNameInLayoutMessage) returns (EDBObjMessage) {}
 
   // Get the reference layout
   rpc GetReferenceLayout(EDBObjMessage) returns (EDBObjMessage) {}
 
   // Terminal Instances
   rpc GetTermInsts(EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamTermInsts(EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Get if component is 3dplaced
   rpc GetIs3DPlacement(EDBObjMessage) returns (google.protobuf.BoolValue) {}
 
   // Set if component is 3dplaced
   rpc Set3DPlacement(BoolPropertyMessage) returns (google.protobuf.Empty) {}
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/circle.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/circle.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/component_def.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/component_def.proto`

 * *Files 11% similar despite different names*

```diff
@@ -26,17 +26,25 @@
   rpc SetFootprintCell(EDBObjPairMessage) returns (google.protobuf.Empty) {}
 
   // Get the footprint name of the component def
   rpc GetFootprintCell(EDBObjMessage) returns (EDBObjMessage) {}
 
   // Get the component models owned by this component def
   rpc GetComponentModels(EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamComponentModels(EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Get the component pins owned by this component def.
   rpc GetComponentPins(EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamComponentPins(EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
+
+  // Add component model to this component def
+  rpc AddComponentModel(EDBObjPairMessage) returns (google.protobuf.Empty) {}
+
+  // Remove component from this component def
+  rpc RemoveComponentModel(EDBObjPairMessage) returns (google.protobuf.Empty) {}
 }
 
 
 message ComponentDefCreateMessage {
   EDBObjMessage db = 1;
   string comp_name = 2;
   EDBObjMessage fp = 3;
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/component_group.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/component_group.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/component_model.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/component_model.proto`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 // Component Definition Service
 service ComponentModelService {
   // Set reference file
   rpc SetReferenceFile(StringPropertyMessage) returns (google.protobuf.Empty) {}
 
   // Get reference file
   rpc GetReferenceFile(EDBObjMessage) returns (google.protobuf.StringValue) {}
+
+  // Find component model by name
+  rpc FindByName(StringPropertyMessage) returns (EDBObjMessage) {}
+
+  // Find component model by id
+  rpc FindById(IntPropertyMessage) returns (EDBObjMessage) {}
 }
 
 service NPortComponentModelService {
   // Create nport component model
   rpc Create(google.protobuf.StringValue) returns (EDBObjMessage) {}
 }
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/component_pin.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/component_pin.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/component_property.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/component_property.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/connectable.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/connectable.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/database.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/database.proto`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
   rpc Close (EDBObjMessage) returns (google.protobuf.Empty) {} 
 
   // Determines whether the database is read only
   rpc IsReadOnly(EDBObjMessage) returns (google.protobuf.BoolValue) {}
 
   // Gets the top circuits in a database
   rpc GetTopCircuits (EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamTopCircuits (EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Gets the id of a database
   rpc GetId (EDBObjMessage) returns (google.protobuf.Int64Value) {} 
 
   // Finds a database with the provided id
   rpc FindById (google.protobuf.Int64Value) returns (EDBObjMessage) {}
   
@@ -65,19 +66,22 @@
   rpc SetSourceVersion(EDBObjNameMessage) returns (google.protobuf.Empty) {}
 
   // copy cells
   rpc CopyCells (CopyCellsMessage) returns (EDBObjCollectionMessage) {}
 
   // Get defs
   rpc GetDefinitionObjs (GetDefinitionObjsMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamDefinitionObjs (GetDefinitionObjsMessage) returns (stream EDBObjCollectionMessage) {}
   
   // get cells
   rpc TopCircuitCells (EDBObjMessage) returns (EDBObjCollectionMessage) {}
   rpc GetCircuits (EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamCircuits (EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
   rpc GetFootprints (EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamFootprints (EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
   
 }
 
 // Message for Open
 message OpenDatabaseMessage {
   string edb_path = 1;
   bool read_only = 2;
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/dataset_def.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/dataset_def.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/debye_model.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/debye_model.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/die_property.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/die_property.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/differential_pair.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/differential_pair.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/djordjecvic_sarkar_model.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/djordjecvic_sarkar_model.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/edb_defs.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/edb_defs.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/edb_messages.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/edb_messages.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/edge_term.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/edge_term.proto`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   rpc GetParameters (EDBObjMessage) returns (EdgeParamsMessage) {}
 }
 
 service EdgeTerminalService {
   rpc Create (EdgeTermCreationMessage) returns (EDBObjMessage) {}
 
   rpc GetEdges (EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamEdges (EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   rpc SetEdges (EdgeTermSetEdgesMessage) returns (google.protobuf.Empty) {}
 }
 
 message EdgeTypeMessage {
   EdgeType t = 1;
 }
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/extended_net.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/extended_net.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/group.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/group.proto`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   rpc RemoveMember(GroupModifyMemberMessage) returns (google.protobuf.Empty) {}
 
   // Ungroup this group
   rpc Ungroup(BoolPropertyMessage) returns (google.protobuf.Empty) {}
 
   // Get iterable for group members
   rpc GetMembers(EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamMembers(EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Get the type of the group
   rpc GetGroupType(EDBObjMessage) returns (GroupTypeMessage) {}
 }
 
 message GroupModifyMemberMessage {
   EDBObjMessage target = 1;
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/hfss_simulation_settings.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/hfss_simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/hfss_simulation_setup.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/hfss_simulation_setup.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/hierarchy_obj.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/hierarchy_obj.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/ic_component_property.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/ic_component_property.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/inst_array.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/inst_array.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/io_component_property.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/io_component_property.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layer.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layer.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layer_collection.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layer_collection.proto`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,15 @@
   rpc FindByName (FindLayerByNameMessage) returns (EDBObjMessage) {}
   
   // Get top bottom stackup layers of specific type
   rpc GetTopBottomStackupLayers (GetTopBottomStackupLayersMessage) returns (TopBottomStackupLayersMessage) {}
 
   // Get a list of layers in the LayerCollection filtered by the given layer filter
   rpc GetLayers (GetLayersMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamLayers (GetLayersMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Get the layer's product property corresponding to the given product and attribute ids
   rpc GetProductProperty (GetProductPropertyMessage) returns (google.protobuf.StringValue) {}
 
   // Set the layer's product property corresponding to the given product and attribute ids
   rpc SetProductProperty (SetProductPropertyMessage) returns (google.protobuf.Empty) {}
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layer_map.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layer_map.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layout.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layout.proto`

 * *Files 8% similar despite different names*

```diff
@@ -21,35 +21,38 @@
   rpc GetLayerCollection (EDBObjMessage) returns (EDBObjMessage) {}
 
   // Sets the layer collection of the layout
   rpc SetLayerCollection (SetLayerCollectionMessage) returns (google.protobuf.Empty) {}
 
   // Gets the layout objects that belong to the layout
   rpc GetItems (LayoutGetItemsMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamItems (LayoutGetItemsMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Get expanded extent from nets
   rpc GetExpandedExtentFromNets (LayoutExpandedExtentMessage) returns (PolygonDataMessage) {}
 
   // Convert primitives to via
   rpc ConvertPrimitivesToVias(LayoutConvertP2VMessage) returns (google.protobuf.Empty) {}
 
   // Gets if the port reference terminals are connected
   rpc ArePortReferenceTerminalsConnected (EDBObjMessage) returns (LayoutPortRefTerminalsConnectedMessage) {}
 
   // Gets list of zone primitives
   rpc GetZonePrimitives (EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamZonePrimitives (EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Set fixed zone primitives
   rpc SetFixedZonePrimitives (PointerPropertyMessage) returns (google.protobuf.Empty) {}
 
   // Get fixed zone primitive
   rpc GetFixedZonePrimitive (EDBObjMessage) returns (EDBObjMessage) {}
 
   // Get board bend definitions
   rpc GetBoardBendDefs (EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamBoardBendDefs (EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Synchronize bend manager
   rpc SynchronizeBendManager (EDBObjMessage) returns (google.protobuf.Empty) {}
 
   // Get the layout instance of the layout
   rpc GetLayoutInstance(EDBObjMessage) returns (EDBObjMessage) {}
 }
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_instance.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_instance.proto`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
   rpc Refresh(EDBObjMessage) returns (google.protobuf.Empty) {}
 
   rpc QueryLayoutObjInstances(LayoutObjInstancesQueryMessage) returns (LayoutObjInstancesQueryResultsMessage) {}
 
   rpc GetLayoutObjInstanceInContext(GetLayoutObjInstanceInContextMessage) returns (EDBObjMessage) {}
 
   rpc GetConnectedObjects(GetConnectedObjectsMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamConnectedObjects(GetConnectedObjectsMessage) returns (stream EDBObjCollectionMessage) {}
 }
 
 message LayoutObjInstancesQueryMessage {
   EDBObjMessage layout_inst = 1;
   oneof spatial_filter {
     PointMessage point_filter = 2;
     PolygonDataMessage region_filter = 3;
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_instance_context.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_instance_context.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj.proto`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,14 @@
   NET_CLASS = 9;
   CELL = 10;
   DIFFERENTIAL_PAIR = 11;
   PIN_GROUP = 12;
   VOLTAGE_REGULATOR = 13;
   EXTENDED_NET = 14;
   LAYOUT_OBJ_TYPE_COUNT = 15;
-  INST_ARRAY = 16;
   INVALID_LAYOUT_OBJ = -1;
 }
 
 // LayoutObj service definition
 service LayoutObjService {
   // Gets the layout of the layout object
   rpc GetLayout (LayoutObjTargetMessage) returns (EDBObjMessage) {}
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj_instance.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj_instance.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj_instance_2d_geometry.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj_instance_2d_geometry.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj_instance_3d_geometry.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj_instance_3d_geometry.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/layout_obj_instance_geometry.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/layout_obj_instance_geometry.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/material_def.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/material_def.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/material_property_thermal_modifier.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/material_property_thermal_modifier.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/mcad_model.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/mcad_model.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/multipole_debye_model.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/multipole_debye_model.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/net.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/net.proto`

 * *Files 13% similar despite different names*

```diff
@@ -21,13 +21,14 @@
 
   // is_power_ground accessors
   rpc GetIsPowerGround (EDBObjMessage) returns (google.protobuf.BoolValue) {}
   rpc SetIsPowerGround (BoolPropertyMessage) returns (google.protobuf.Empty) {}
 
   // layout objects getter
   rpc GetLayoutObjects (NetGetLayoutObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamLayoutObjects (NetGetLayoutObjMessage) returns (stream EDBObjCollectionMessage) {}
 }
 
 message NetGetLayoutObjMessage {
   EDBObjMessage net = 1;
   LayoutObjType obj_type = 2;
 }
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/netclass.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/netclass.proto`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
   rpc GetDescription(EDBObjMessage) returns (google.protobuf.StringValue) {}
 
   rpc SetDescription(StringPropertyMessage) returns (google.protobuf.Empty) {}
 
   rpc IsPowerGround(EDBObjMessage) returns (google.protobuf.BoolValue) {}
   
   rpc GetNets(EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamNets(EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
   
   rpc AddNet(NetClassEditMessage) returns (google.protobuf.Empty) {}
 
   rpc RemoveNet(NetClassEditMessage) returns (google.protobuf.Empty) {}
 
   rpc ContainsNet(NetClassEditMessage) returns (google.protobuf.BoolValue) {}    
 }
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/package_def.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/package_def.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/padstack_def.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/padstack_def.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/padstack_def_data.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/padstack_def_data.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/padstack_inst_term.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/padstack_inst_term.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/padstack_instance.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/padstack_instance.proto`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,16 @@
   // Get Terminal of PadstackInst
   rpc GetPadstackInstanceTerminal(EDBObjMessage) returns (EDBObjMessage) {}
   
   // Check if PadstackInst is in pin group
   rpc IsInPinGroup(PadstackInstIsInPinGroupMessage) returns (google.protobuf.BoolValue) {}
   
   // Get pin groups of PadstackInst
-  rpc GetPinGroups(EDBObjMessage) returns (EDBObjCollectionMessage ) {}
+  rpc GetPinGroups(EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamPinGroups(EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
 }
 
 message PadstackInstCreateMessage{
   EDBObjMessage layout = 1;
   EDBObjMessage net = 2;
   string name = 3;
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/path.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/path.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/pin_group.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/pin_group.proto`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
   rpc GetName (EDBObjMessage) returns (google.protobuf.StringValue) {}
 
   rpc AddPins (PinGroupPinsModifyMessage) returns (google.protobuf.Empty) {}
 
   rpc RemovePins (PinGroupPinsModifyMessage) returns (google.protobuf.Empty) {}
 
   rpc GetPins (EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamPins (EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 }
 
 message PinGroupCreationMessage {
   EDBObjMessage layout = 1;
   string name = 2;
   repeated EDBObjMessage pins = 3;
 }
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/pin_group_term.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/pin_group_term.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/pin_pair_model.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/pin_pair_model.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/point_3d_data.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/point_3d_data.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/point_data.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/point_data.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/point_term.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/point_term.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/polygon.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/polygon.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/polygon_data.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/polygon_data.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/port_property.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/port_property.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/primitive.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/primitive.proto`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
   rpc IsVoid (EDBObjMessage) returns (google.protobuf.BoolValue) {}
 
   // Get HasVoids
   rpc HasVoids(EDBObjMessage) returns (google.protobuf.BoolValue) {}
 
   // Gets an iterator of the voids in the Primitive
   rpc Voids(EDBObjMessage) returns (EDBObjCollectionMessage) {}
+  rpc StreamVoids(EDBObjMessage) returns (stream EDBObjCollectionMessage) {}
 
   // Get Owner
   rpc GetOwner(EDBObjMessage) returns (EDBObjMessage) {}
   
   // Get isParametrized
   rpc IsParameterized(EDBObjMessage) returns (google.protobuf.BoolValue) {}
```

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/r_tree.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/r_tree.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/raptor_x_simulation_settings.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/raptor_x_simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/rectangle.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/rectangle.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/refs.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/refs.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/rlc_component_property.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/rlc_component_property.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/simulation_settings.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/simulation_setup.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/simulation_setup.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/siwave_dcir_simulation_settings.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/siwave_dcir_simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/siwave_simulation_settings.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/siwave_simulation_settings.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/solder_ball_property.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/solder_ball_property.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/sparameter_model.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/sparameter_model.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/spice_model.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/spice_model.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/stackup_layer.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/stackup_layer.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/structure3d.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/structure3d.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/term.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/term.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/term_inst.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/term_inst.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/term_inst_term.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/term_inst_term.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/text.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/text.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/transform.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/transform.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/transform3d.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/transform3d.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/variable_server.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/variable_server.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/via_group.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/via_group.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/via_layer.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/via_layer.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys/api/edb/v1/voltage_regulator.proto` & `ansys_api_edb-1.0.4/ansys/api/edb/v1/voltage_regulator.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/ansys_api_edb.egg-info/PKG-INFO` & `ansys_api_edb-1.0.4/ansys_api_edb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-edb
-Version: 1.0.3
-Summary: Autogenerated Python gRPC interface package for ansys-api-edb, built on 18:44:02 on 24 April 2024
+Version: 1.0.4
+Summary: Autogenerated Python gRPC interface package for ansys-api-edb, built on 11:47:40 on 24 May 2024
 Home-page: https://github.com/ansys/ansys-api-edb
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-edb/#readme
```

### Comparing `ansys_api_edb-1.0.3/ansys_api_edb.egg-info/SOURCES.txt` & `ansys_api_edb-1.0.4/ansys_api_edb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys_api_edb-1.0.3/setup.py` & `ansys_api_edb-1.0.4/setup.py`

 * *Files identical despite different names*

