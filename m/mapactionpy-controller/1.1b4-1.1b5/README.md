# Comparing `tmp/mapactionpy_controller-1.1b4.tar.gz` & `tmp/mapactionpy_controller-1.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mapactionpy_controller-1.1b4.tar", last modified: Sat Feb 27 20:53:44 2021, max compression
+gzip compressed data, was "dist/mapactionpy_controller-1.1b5.tar", last modified: Sat Mar  6 13:04:15 2021, max compression
```

## Comparing `mapactionpy_controller-1.1b4.tar` & `mapactionpy_controller-1.1b5.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/
--rw-rw-r--   0 travis    (2000) travis    (2000)      213 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    13076 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    10826 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/VERSION
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3490 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/check_naming_convention.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7981 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4282 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/config_verify.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3862 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/crash_move_folder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      187 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/data_schemas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6124 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/data_search.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1928 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/data_source.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/event.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7120 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/01_geoextent.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      710 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/02_category.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     4399 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/03_theme.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/04_geometry.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      252 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/05_scale.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/06_source.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/07_permission.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)      116 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/99_DNCmetadata.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/a_map_frame.csv
--rw-rw-r--   0 travis    (2000) travis    (2000)     1012 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/cmf_description.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/cmf_description_flat_test.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      718 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/cmf_description_relative_paths_test.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1916 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/data_naming_convention.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/data_schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)      176 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/data_schemas/admin0_affected_area_py.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/data_schemas/admin1_reference.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/data_schemas/null-schema.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/data_schemas/stle_ste_pt.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    18931 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/dummy_layerProperties.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     5681 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/dummy_mapCookbook.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      733 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/event_description.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/example_single_layer_properties.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/example_single_map_recipe.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      916 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/layer_file_naming_convention.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      665 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/map_project_naming_convention.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      706 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/example/map_template_naming_convention.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     8804 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/jira_tasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5581 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/layer_properties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6287 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/main_stack.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4322 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/map_cookbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2229 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/map_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5562 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/map_doc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8682 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/map_recipe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1513 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/map_report.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/map_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4227 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/name_clause_validators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4004 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/name_convention.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14809 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/plugin_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6038 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/plugin_controller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1930 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/recipe_atlas.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7784 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/recipe_frame.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15427 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/recipe_layer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)      589 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/atlas-v0.2.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/cmf-v0.1.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     7755 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/cmf-v0.2.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/event-v0.2.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     3302 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/layer_properties-v0.1.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     6651 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/layer_properties-v0.2.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     3506 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/map-recipe-v0.1.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     8157 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/map-recipe-v0.2.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     9240 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/map-recipe-v0.3.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)     2169 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/map-template-v0.2.schema
--rw-rw-r--   0 travis    (2000) travis    (2000)      745 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/state_serialization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4080 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/steps.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      266 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/major-configuration-error.mustache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1859 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/misnamed-gis-file.mustache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/missing-gis-file.mustache
--rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/multiple-matching-files.mustache
--rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/schema-error.mustache
--rw-rw-r--   0 travis    (2000) travis    (2000)     9274 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/task_renderer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2031 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/temp-step-list.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26496 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/fixtures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_check_naming_convention.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4590 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2858 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_config_verify.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11360 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_data_search.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3353 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_event.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8539 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_jira_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5713 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_layer_properties.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4699 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_main_stack.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18993 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_map_cookbook.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5455 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_mapactionpy_controller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9724 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_name_convention.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4681 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_plugin_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4559 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_plugin_controller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8975 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_recipe_layer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2658 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_steps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5497 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_task_rendering.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      447 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_to_integrate_from_arcmap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4534 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/mapactionpy_controller/xml_exporter.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13076 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4763 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      148 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-02-27 20:53:44.000000 mapactionpy_controller-1.1b4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     4576 2021-02-27 20:51:30.000000 mapactionpy_controller-1.1b4/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      213 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13076 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10826 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/VERSION
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3490 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/check_naming_convention.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7981 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4282 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/config_verify.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3862 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/crash_move_folder.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      187 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/data_schemas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6124 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/data_search.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1928 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/data_source.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/event.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7120 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/01_geoextent.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      710 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/02_category.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4399 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/03_theme.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/04_geometry.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      252 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/05_scale.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/06_source.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/07_permission.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)      116 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/99_DNCmetadata.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/a_map_frame.csv
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1012 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/cmf_description.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/cmf_description_flat_test.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      718 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/cmf_description_relative_paths_test.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1916 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/data_naming_convention.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/data_schemas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      176 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/data_schemas/admin0_affected_area_py.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      177 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/data_schemas/admin1_reference.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/data_schemas/null-schema.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      177 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/data_schemas/stle_ste_pt.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18931 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/dummy_layerProperties.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5681 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/dummy_mapCookbook.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      733 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/event_description.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/example_single_layer_properties.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/example_single_map_recipe.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      916 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/layer_file_naming_convention.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      665 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/map_project_naming_convention.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      706 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/example/map_template_naming_convention.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8804 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/jira_tasks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5581 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/layer_properties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6351 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/main_stack.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4322 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/map_cookbook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2229 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/map_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5562 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/map_doc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8682 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/map_recipe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1513 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/map_report.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/map_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4227 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/name_clause_validators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4004 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/name_convention.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14809 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/plugin_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6038 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/plugin_controller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1930 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/recipe_atlas.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7784 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/recipe_frame.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15797 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/recipe_layer.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      589 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/atlas-v0.2.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3064 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/cmf-v0.1.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7755 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/cmf-v0.2.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/event-v0.2.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3302 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/layer_properties-v0.1.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6651 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/layer_properties-v0.2.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3506 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/map-recipe-v0.1.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8157 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/map-recipe-v0.2.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9240 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/map-recipe-v0.3.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2169 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/map-template-v0.2.schema
+-rw-rw-r--   0 travis    (2000) travis    (2000)      745 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/state_serialization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4080 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/steps.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      266 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/major-configuration-error.mustache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1859 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/misnamed-gis-file.mustache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/missing-gis-file.mustache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/multiple-matching-files.mustache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1277 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/schema-error.mustache
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9274 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/task_renderer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2031 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/temp-step-list.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      117 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26496 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/fixtures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1518 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_check_naming_convention.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4590 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2858 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_config_verify.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11360 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_data_search.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3353 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_event.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8539 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_jira_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5713 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_layer_properties.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4699 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_main_stack.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18993 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_map_cookbook.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5455 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_mapactionpy_controller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9724 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_name_convention.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4681 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_plugin_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4559 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_plugin_controller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9758 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_recipe_layer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2658 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_steps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5497 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_task_rendering.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      447 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_to_integrate_from_arcmap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4534 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/mapactionpy_controller/xml_exporter.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13076 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4763 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      148 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-06 13:04:15.000000 mapactionpy_controller-1.1b5/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4576 2021-03-06 13:01:56.000000 mapactionpy_controller-1.1b5/setup.py
```

### Comparing `mapactionpy_controller-1.1b4/PKG-INFO` & `mapactionpy_controller-1.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapactionpy_controller
-Version: 1.1b4
+Version: 1.1b5
 Summary: Controls the workflow of map and infographic production
 Home-page: http://github.com/mapaction/mapactionpy_controller
 Author: MapAction
 Author-email: github@mapaction.com
 License: GPL3
 Description: About
         =====
```

### Comparing `mapactionpy_controller-1.1b4/README.md` & `mapactionpy_controller-1.1b5/README.md`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/__init__.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/check_naming_convention.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/check_naming_convention.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/cli.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/cli.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/config_verify.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/config_verify.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/crash_move_folder.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/crash_move_folder.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/data_search.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/data_search.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/data_source.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/data_source.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/event.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/event.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/01_geoextent.csv` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/01_geoextent.csv`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/02_category.csv` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/02_category.csv`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/03_theme.csv` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/03_theme.csv`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/06_source.csv` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/06_source.csv`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/cmf_description.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/cmf_description.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/cmf_description_flat_test.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/cmf_description_flat_test.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/cmf_description_relative_paths_test.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/cmf_description_relative_paths_test.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/data_naming_convention.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/data_naming_convention.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/dummy_layerProperties.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/dummy_layerProperties.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/dummy_mapCookbook.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/dummy_mapCookbook.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/event_description.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/event_description.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/example_single_layer_properties.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/example_single_layer_properties.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/example_single_map_recipe.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/example_single_map_recipe.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/layer_file_naming_convention.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/layer_file_naming_convention.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/map_project_naming_convention.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/map_project_naming_convention.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/example/map_template_naming_convention.json` & `mapactionpy_controller-1.1b5/mapactionpy_controller/example/map_template_naming_convention.json`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/jira_tasks.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/jira_tasks.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/layer_properties.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/layer_properties.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/main_stack.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/main_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 Execution continous until there are no more Steps.
 
 Note: main_stack.py also includes humanfriendly.terminal which ought really to be part of the CLI.
 """
 import logging
 import traceback
 import six
+import sys
 from collections import deque
 
 import humanfriendly.terminal as hft
 import humanfriendly.terminal.spinners as spinners
 
 from mapactionpy_controller.steps import Step
 from mapactionpy_controller.task_renderer import TaskReferralBase
@@ -159,11 +160,10 @@
 
         return n_state
     except Exception as exp:
         pass_back = {
             'exp': exp,
             'stack_trace': traceback.format_exc()
         }
-
-        # print(pass_back)
-
+        # print error and then exit with a non-zero exit code
         parse_feedback(logging.ERROR, 'Unable to continue following the previous error', None, **pass_back)
+        sys.exit(1)
```

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/map_cookbook.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/map_cookbook.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/map_data.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/map_data.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/map_doc.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/map_doc.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/map_recipe.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/map_recipe.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/map_report.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/map_report.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/map_result.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/map_result.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/name_clause_validators.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/name_clause_validators.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/name_convention.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/name_convention.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/plugin_base.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/plugin_base.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/plugin_controller.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/plugin_controller.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/recipe_atlas.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/recipe_atlas.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/recipe_frame.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/recipe_frame.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/recipe_layer.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/recipe_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,32 +289,38 @@
         logging.debug('Attempting to validate jsonschema for gis data')
         if not self.data_source_path:
             error_msg = ('Cannot check data schema for layer ("{}") before the relevant data has been found.'
                          ' Please use `get_data_finder()` first.'.format(self.name))
             logging.debug(error_msg)
             raise ValueError(error_msg)
 
+        recipe = kwargs['state']
+
+        if not self.data_source_path.endswith('.shp'):
+            logging.info("Unable to check schema on for data sources which aren't shapefiles."
+                         " Skipping schema check on file: {}".format(self.data_source_path))
+            return recipe
+
         # Validate
         try:
-            recipe = kwargs['state']
+            # Check for self consistancy before proceeding
             self._check_lyr_is_in_recipe(recipe)
 
-            from jsonschema import validate
-            gdf = geopandas.read_file(self.data_source_path)
-
+            # Only load one row since we are only checking the schema
+            gdf = geopandas.read_file(self.data_source_path, rows=1)
             # Make columns needed for validation
             gdf['geometry_type'] = gdf['geometry'].apply(lambda x: x.geom_type)
             # print(gdf.crs)
             if isinstance(gdf.crs, dict):
                 gdf['crs'] = gdf.crs['init']
             else:
                 gdf['crs'] = gdf.crs
 
             instance_list = gdf.to_dict('list')
-            validate(instance=instance_list, schema=self.data_schema)
+            jsonschema.validate(instance=instance_list, schema=self.data_schema)
             logging.debug('Successfully validates jsonschema for gis data')
         # except jsonschema.ValidationError as jsve:
         except Exception as exp:
             error_msg = ('Failed whilst check data schema for layer ("{}") with exception: {}'.format(
                 self.name, exp))
             logging.debug(error_msg)
             self.error_messages.append('Data schema check failed')
```

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/atlas-v0.2.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/atlas-v0.2.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/cmf-v0.1.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/cmf-v0.1.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/cmf-v0.2.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/cmf-v0.2.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/event-v0.2.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/event-v0.2.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/layer_properties-v0.1.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/layer_properties-v0.1.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/layer_properties-v0.2.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/layer_properties-v0.2.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/map-recipe-v0.1.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/map-recipe-v0.1.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/map-recipe-v0.2.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/map-recipe-v0.2.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/map-recipe-v0.3.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/map-recipe-v0.3.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/schemas/map-template-v0.2.schema` & `mapactionpy_controller-1.1b5/mapactionpy_controller/schemas/map-template-v0.2.schema`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/state_serialization.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/state_serialization.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/steps.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/steps.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/misnamed-gis-file.mustache` & `mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/misnamed-gis-file.mustache`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/missing-gis-file.mustache` & `mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/missing-gis-file.mustache`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/multiple-matching-files.mustache` & `mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/multiple-matching-files.mustache`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/task-templates/schema-error.mustache` & `mapactionpy_controller-1.1b5/mapactionpy_controller/task-templates/schema-error.mustache`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/task_renderer.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/task_renderer.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/temp-step-list.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/temp-step-list.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/fixtures.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_check_naming_convention.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_check_naming_convention.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_cli.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_config_verify.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_config_verify.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_data_search.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_data_search.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_event.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_jira_client.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_jira_client.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_layer_properties.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_layer_properties.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_main_stack.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_main_stack.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_map_cookbook.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_map_cookbook.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_mapactionpy_controller.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_mapactionpy_controller.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_name_convention.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_name_convention.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_plugin_base.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_plugin_base.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_plugin_controller.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_plugin_controller.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_recipe_layer.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_recipe_layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -235,14 +235,31 @@
             test_lyr.data_schema = test_schema
             with self.assertRaises(ValueError) as arcm:
                 test_lyr.check_data_against_schema(state=test_recipe)
 
             ve = arcm.exception
             self.assertIsInstance(ve.args[0], recipe_layer.FixSchemaErrorTask)
 
+        # test a logger is call for case where a raster layer is tested. This unittest
+        # is only available for py3.4+, though the production code is required for py2.7
+        if six.PY3:
+            test_lyr.data_source_path = os.path.join(
+                self.parent_dir, 'tests', 'testfiles', 'test_shp_files',
+                'lbn_evel_dem_ras_s1_pp_cdr.tif')
+            test_lyr.data_schema = passing_schema
+
+            with self.assertLogs(level='INFO') as cm:
+                result = test_lyr.check_data_against_schema(state=test_recipe)
+
+            print('cm.output = {}'.format(cm.output))
+            self.assertRegexpMatches(
+                cm.output.pop(),
+                'Unable to check schema on for data sources which aren.t shapefiles'
+            )
+
     def test_calc_extent(self):
         test_recipe = MapRecipe(fixtures.recipe_with_layer_name_only, self.lyr_props)
 
         test_lyr = test_recipe.all_layers().pop()
         # Use a simple test shapefile
         test_lyr.data_source_path = os.path.join(
             self.parent_dir, 'tests', 'testfiles', 'test_shp_files',
```

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_steps.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_steps.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/tests/test_task_rendering.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/tests/test_task_rendering.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller/xml_exporter.py` & `mapactionpy_controller-1.1b5/mapactionpy_controller/xml_exporter.py`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/PKG-INFO` & `mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapactionpy-controller
-Version: 1.1b4
+Version: 1.1b5
 Summary: Controls the workflow of map and infographic production
 Home-page: http://github.com/mapaction/mapactionpy_controller
 Author: MapAction
 Author-email: github@mapaction.com
 License: GPL3
 Description: About
         =====
```

### Comparing `mapactionpy_controller-1.1b4/mapactionpy_controller.egg-info/SOURCES.txt` & `mapactionpy_controller-1.1b5/mapactionpy_controller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapactionpy_controller-1.1b4/setup.py` & `mapactionpy_controller-1.1b5/setup.py`

 * *Files identical despite different names*

