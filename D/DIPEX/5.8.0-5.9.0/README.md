# Comparing `tmp/dipex-5.8.0.tar.gz` & `tmp/dipex-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dipex-5.8.0.tar", max compression
+gzip compressed data, was "dipex-5.9.0.tar", max compression
```

## Comparing `dipex-5.8.0.tar` & `dipex-5.9.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0        0 2023-10-06 08:31:34.882324 dipex-5.8.0/exporters/sql_export/__init__.py
--rw-r--r--   0        0        0    40011 2023-10-06 08:31:34.705312 dipex-5.8.0/exporters/sql_export/gql_lora_cache_async.py
--rw-r--r--   0        0        0     2111 2023-10-06 08:31:34.706313 dipex-5.8.0/exporters/sql_export/lc_for_jobs_db.py
--rw-r--r--   0        0        0     1584 2023-10-06 08:31:34.706313 dipex-5.8.0/exporters/sql_export/log.py
--rw-r--r--   0        0        0     2742 2023-10-06 08:31:34.706313 dipex-5.8.0/exporters/sql_export/lora_cache.py
--rw-r--r--   0        0        0     1396 2023-10-06 08:31:34.706313 dipex-5.8.0/exporters/sql_export/main.py
--rw-r--r--   0        0        0    54838 2023-10-06 08:31:34.706313 dipex-5.8.0/exporters/sql_export/old_lora_cache.py
--rw-r--r--   0        0        0    29560 2023-10-06 08:31:34.710313 dipex-5.8.0/exporters/sql_export/sql_export.py
--rw-r--r--   0        0        0     9642 2023-10-06 08:31:34.711313 dipex-5.8.0/exporters/sql_export/sql_table_defs.py
--rw-r--r--   0        0        0     5385 2023-10-06 08:31:34.711313 dipex-5.8.0/exporters/sql_export/sql_url.py
--rw-r--r--   0        0        0     5543 2023-10-06 08:31:34.731314 dipex-5.8.0/exporters/sql_export/trigger.py
--rw-r--r--   0        0        0     5075 2023-10-06 08:31:34.734314 dipex-5.8.0/exporters/utils/priority_by_class.py
--rw-r--r--   0        0        0        0 2023-10-06 08:31:34.883324 dipex-5.8.0/integrations/__init__.py
--rw-r--r--   0        0        0     3369 2023-10-06 08:31:34.735314 dipex-5.8.0/integrations/aarhus/config.py
--rw-r--r--   0        0        0     5126 2023-10-06 08:31:34.735314 dipex-5.8.0/integrations/aarhus/dar_helper.py
--rw-r--r--   0        0        0     3163 2023-10-06 08:31:34.736314 dipex-5.8.0/integrations/aarhus/initial.py
--rw-r--r--   0        0        0     3234 2023-10-06 08:31:34.736314 dipex-5.8.0/integrations/aarhus/initial_classes.py
--rw-r--r--   0        0        0     9582 2023-10-06 08:31:34.736314 dipex-5.8.0/integrations/aarhus/los_files.py
--rw-r--r--   0        0        0     3705 2023-10-06 08:31:34.736314 dipex-5.8.0/integrations/aarhus/los_import.py
--rw-r--r--   0        0        0     5086 2023-10-06 08:31:34.736314 dipex-5.8.0/integrations/aarhus/los_leder.py
--rw-r--r--   0        0        0    18392 2023-10-06 08:31:34.737314 dipex-5.8.0/integrations/aarhus/los_org.py
--rw-r--r--   0        0        0     9228 2023-10-06 08:31:34.737314 dipex-5.8.0/integrations/aarhus/los_pers.py
--rw-r--r--   0        0        0    21785 2023-10-06 08:31:34.737314 dipex-5.8.0/integrations/aarhus/los_stam.py
--rw-r--r--   0        0        0     4085 2023-10-06 08:31:34.737314 dipex-5.8.0/integrations/aarhus/payloads.py
--rw-r--r--   0        0        0        0 2023-10-06 08:31:34.892325 dipex-5.8.0/integrations/aarhus/tests/__init__.py
--rw-r--r--   0        0        0     1262 2023-10-06 08:31:34.738314 dipex-5.8.0/integrations/aarhus/tests/conftest.py
--rw-r--r--   0        0        0     3250 2023-10-06 08:31:34.738314 dipex-5.8.0/integrations/aarhus/tests/helpers.py
--rw-r--r--   0        0        0     2101 2023-10-06 08:31:34.738314 dipex-5.8.0/integrations/aarhus/tests/strategies.py
--rw-r--r--   0        0        0     1447 2023-10-06 08:31:34.738314 dipex-5.8.0/integrations/aarhus/tests/test_config.py
--rw-r--r--   0        0        0     1009 2023-10-06 08:31:34.738314 dipex-5.8.0/integrations/aarhus/tests/test_initial.py
--rw-r--r--   0        0        0     3178 2023-10-06 08:31:34.739315 dipex-5.8.0/integrations/aarhus/tests/test_los_files.py
--rw-r--r--   0        0        0     1200 2023-10-06 08:31:34.739315 dipex-5.8.0/integrations/aarhus/tests/test_los_import.py
--rw-r--r--   0        0        0    10703 2023-10-06 08:31:34.739315 dipex-5.8.0/integrations/aarhus/tests/test_los_leder.py
--rw-r--r--   0        0        0    11047 2023-10-06 08:31:34.739315 dipex-5.8.0/integrations/aarhus/tests/test_los_org.py
--rw-r--r--   0        0        0     6773 2023-10-06 08:31:34.740315 dipex-5.8.0/integrations/aarhus/tests/test_los_pers.py
--rw-r--r--   0        0        0    12108 2023-10-06 08:31:34.740315 dipex-5.8.0/integrations/aarhus/tests/test_los_stam.py
--rw-r--r--   0        0        0     1045 2023-10-06 08:31:34.740315 dipex-5.8.0/integrations/aarhus/tests/test_payloads.py
--rw-r--r--   0        0        0     7336 2023-10-06 08:31:34.740315 dipex-5.8.0/integrations/aarhus/tests/test_util.py
--rw-r--r--   0        0        0     6857 2023-10-06 08:31:34.740315 dipex-5.8.0/integrations/aarhus/util.py
--rw-r--r--   0        0        0     1073 2023-10-06 08:31:34.740315 dipex-5.8.0/integrations/aarhus/uuids.py
--rw-r--r--   0        0        0        0 2023-10-06 08:31:34.896325 dipex-5.8.0/integrations/ad_integration/__init__.py
--rw-r--r--   0        0        0    15777 2023-10-06 08:31:34.741315 dipex-5.8.0/integrations/ad_integration/ad_common.py
--rw-r--r--   0        0        0      852 2023-10-06 08:31:34.741315 dipex-5.8.0/integrations/ad_integration/ad_exceptions.py
--rw-r--r--   0        0        0    31045 2023-10-06 08:31:34.741315 dipex-5.8.0/integrations/ad_integration/ad_fix_enddate.py
--rw-r--r--   0        0        0     3960 2023-10-06 08:31:34.742315 dipex-5.8.0/integrations/ad_integration/ad_jinja_filters.py
--rwxr-xr-x   0        0        0    20093 2023-10-06 08:31:34.742315 dipex-5.8.0/integrations/ad_integration/ad_life_cycle.py
--rw-r--r--   0        0        0     2392 2023-10-06 08:31:34.742315 dipex-5.8.0/integrations/ad_integration/ad_logger.py
--rw-r--r--   0        0        0     7203 2023-10-06 08:31:34.742315 dipex-5.8.0/integrations/ad_integration/ad_reader.py
--rw-r--r--   0        0        0    34412 2023-10-06 08:31:34.743315 dipex-5.8.0/integrations/ad_integration/ad_sync.py
--rw-r--r--   0        0        0    15426 2023-10-06 08:31:34.743315 dipex-5.8.0/integrations/ad_integration/ad_template_engine.py
--rw-r--r--   0        0        0      384 2023-10-06 08:31:34.743315 dipex-5.8.0/integrations/ad_integration/ad_templates.py
--rw-r--r--   0        0        0    54693 2023-10-06 08:31:34.743315 dipex-5.8.0/integrations/ad_integration/ad_writer.py
--rw-r--r--   0        0        0    11131 2023-10-06 08:31:34.744315 dipex-5.8.0/integrations/ad_integration/import_ad_group_into_mo.py
--rw-r--r--   0        0        0     8896 2023-10-06 08:31:34.744315 dipex-5.8.0/integrations/ad_integration/mo_to_ad_sync.py
--rw-r--r--   0        0        0     2522 2023-10-06 08:31:34.744315 dipex-5.8.0/integrations/ad_integration/payloads.py
--rw-r--r--   0        0        0     9206 2023-10-06 08:31:34.744315 dipex-5.8.0/integrations/ad_integration/read_ad_conf_settings.py
--rw-r--r--   0        0        0     7898 2023-10-06 08:31:34.744315 dipex-5.8.0/integrations/ad_integration/sync_mo_uuid_to_ad.py
--rw-r--r--   0        0        0     7518 2023-10-06 08:31:34.745315 dipex-5.8.0/integrations/ad_integration/test_connectivity.py
--rw-r--r--   0        0        0        0 2023-10-06 08:31:34.896325 dipex-5.8.0/integrations/ad_integration/tests/__init__.py
--rw-r--r--   0        0        0    17787 2023-10-06 08:31:34.745315 dipex-5.8.0/integrations/ad_integration/tests/mocks.py
--rw-r--r--   0        0        0      434 2023-10-06 08:31:34.745315 dipex-5.8.0/integrations/ad_integration/tests/name_simulator.py
--rw-r--r--   0        0        0     3238 2023-10-06 08:31:34.745315 dipex-5.8.0/integrations/ad_integration/tests/test_ad_common.py
--rw-r--r--   0        0        0    27949 2023-10-06 08:31:34.745315 dipex-5.8.0/integrations/ad_integration/tests/test_ad_fix_enddate.py
--rw-r--r--   0        0        0     4992 2023-10-06 08:31:34.746315 dipex-5.8.0/integrations/ad_integration/tests/test_ad_jinja_filters.py
--rw-r--r--   0        0        0    21210 2023-10-06 08:31:34.746315 dipex-5.8.0/integrations/ad_integration/tests/test_ad_life_cycle.py
--rw-r--r--   0        0        0      580 2023-10-06 08:31:34.746315 dipex-5.8.0/integrations/ad_integration/tests/test_ad_logger.py
--rw-r--r--   0        0        0     3989 2023-10-06 08:31:34.746315 dipex-5.8.0/integrations/ad_integration/tests/test_ad_reader.py
--rw-r--r--   0        0        0    43922 2023-10-06 08:31:34.746315 dipex-5.8.0/integrations/ad_integration/tests/test_ad_sync.py
--rw-r--r--   0        0        0    71554 2023-10-06 08:31:34.747315 dipex-5.8.0/integrations/ad_integration/tests/test_ad_writer.py
--rw-r--r--   0        0        0     2259 2023-10-06 08:31:34.747315 dipex-5.8.0/integrations/ad_integration/tests/test_dot_mapping.py
--rw-r--r--   0        0        0     1205 2023-10-06 08:31:34.747315 dipex-5.8.0/integrations/ad_integration/tests/test_first_included.py
--rw-r--r--   0        0        0     5180 2023-10-06 08:31:34.747315 dipex-5.8.0/integrations/ad_integration/tests/test_import_ad_group_into_mo.py
--rw-r--r--   0        0        0     4116 2023-10-06 08:31:34.747315 dipex-5.8.0/integrations/ad_integration/tests/test_location_element.py
--rw-r--r--   0        0        0    11237 2023-10-06 08:31:34.748315 dipex-5.8.0/integrations/ad_integration/tests/test_mo_data_source.py
--rw-r--r--   0        0        0     5873 2023-10-06 08:31:34.748315 dipex-5.8.0/integrations/ad_integration/tests/test_mo_to_ad_sync.py
--rw-r--r--   0        0        0     1471 2023-10-06 08:31:34.748315 dipex-5.8.0/integrations/ad_integration/tests/test_morestsource.py
--rw-r--r--   0        0        0     5408 2023-10-06 08:31:34.748315 dipex-5.8.0/integrations/ad_integration/tests/test_read_ad_conf_settings.py
--rw-r--r--   0        0        0     1896 2023-10-06 08:31:34.748315 dipex-5.8.0/integrations/ad_integration/tests/test_recursive_dict_update.py
--rw-r--r--   0        0        0     5579 2023-10-06 08:31:34.748315 dipex-5.8.0/integrations/ad_integration/tests/test_sync_mo_uuid_to_ad.py
--rw-r--r--   0        0        0    23437 2023-10-06 08:31:34.749315 dipex-5.8.0/integrations/ad_integration/tests/test_usernames.py
--rw-r--r--   0        0        0    18469 2023-10-06 08:31:34.749315 dipex-5.8.0/integrations/ad_integration/tests/test_utils.py
--rw-r--r--   0        0        0    13493 2023-10-06 08:31:34.749315 dipex-5.8.0/integrations/ad_integration/user_names.py
--rw-r--r--   0        0        0     4306 2023-10-06 08:31:34.749315 dipex-5.8.0/integrations/ad_integration/username_rules/method_2.py
--rw-r--r--   0        0        0     4558 2023-10-06 08:31:34.749315 dipex-5.8.0/integrations/ad_integration/utils.py
--rw-r--r--   0        0        0        0 2023-10-06 08:31:34.897325 dipex-5.8.0/integrations/calculate_primary/__init__.py
--rw-r--r--   0        0        0     3121 2023-10-06 08:31:34.750315 dipex-5.8.0/integrations/calculate_primary/calculate_primary.py
--rw-r--r--   0        0        0    19033 2023-10-06 08:31:34.750315 dipex-5.8.0/integrations/calculate_primary/common.py
--rw-r--r--   0        0        0     2597 2023-10-06 08:31:34.750315 dipex-5.8.0/integrations/calculate_primary/default.py
--rw-r--r--   0        0        0     4045 2023-10-06 08:31:34.750315 dipex-5.8.0/integrations/calculate_primary/opus.py
--rw-r--r--   0        0        0     3651 2023-10-06 08:31:34.750315 dipex-5.8.0/integrations/calculate_primary/sd.py
--rw-r--r--   0        0        0        0 2023-10-06 08:31:34.897325 dipex-5.8.0/integrations/calculate_primary/tests/__init__.py
--rw-r--r--   0        0        0    19238 2023-10-06 08:31:34.751315 dipex-5.8.0/integrations/calculate_primary/tests/test_primary.py
--rw-r--r--   0        0        0      896 2023-10-06 08:31:34.751315 dipex-5.8.0/integrations/cpr_mapper.py
--rw-r--r--   0        0        0     1010 2023-10-06 08:31:34.751315 dipex-5.8.0/integrations/dawa_helper.py
--rw-r--r--   0        0        0       99 2023-10-06 08:31:34.751315 dipex-5.8.0/integrations/kle/__init__.py
--rw-r--r--   0        0        0    13325 2023-10-06 08:31:34.752315 dipex-5.8.0/integrations/kle/kle_import.py
--rw-r--r--   0        0        0     4584 2023-10-06 08:31:34.752315 dipex-5.8.0/integrations/kle/kle_import_export.py
--rw-r--r--   0        0        0     9061 2023-10-06 08:31:34.752315 dipex-5.8.0/integrations/kle/kle_xlsx.py
--rw-r--r--   0        0        0     2261 2023-10-06 08:31:34.752315 dipex-5.8.0/integrations/kle/payloads.py
--rw-r--r--   0        0        0     4550 2023-10-06 08:31:34.752315 dipex-5.8.0/integrations/opus/clear_and_import_opus.py
--rw-r--r--   0        0        0    40237 2023-10-06 08:31:34.753316 dipex-5.8.0/integrations/opus/opus_diff_import.py
--rw-r--r--   0        0        0      353 2023-10-06 08:31:34.753316 dipex-5.8.0/integrations/opus/opus_exceptions.py
--rw-r--r--   0        0        0     4348 2023-10-06 08:31:34.753316 dipex-5.8.0/integrations/opus/opus_file_reader.py
--rw-r--r--   0        0        0    14167 2023-10-06 08:31:34.753316 dipex-5.8.0/integrations/opus/opus_helpers.py
--rw-r--r--   0        0        0     2958 2023-10-06 08:31:34.754315 dipex-5.8.0/integrations/opus/opus_reimport_one.py
--rw-r--r--   0        0        0     4515 2023-10-06 08:31:34.754315 dipex-5.8.0/integrations/opus/org_tree_print/main.py
--rw-r--r--   0        0        0     5449 2023-10-06 08:31:34.754315 dipex-5.8.0/integrations/opus/payloads.py
--rw-r--r--   0        0        0    18762 2023-10-06 08:31:34.755316 dipex-5.8.0/integrations/opus/tests/test_opus_diff_import.py
--rw-r--r--   0        0        0     1406 2023-10-06 08:31:34.755316 dipex-5.8.0/integrations/opus/tests/test_opus_file_reader.py
--rw-r--r--   0        0        0     3966 2023-10-06 08:31:34.755316 dipex-5.8.0/integrations/opus/tests/test_opus_helpers.py
--rw-r--r--   0        0        0     4562 2023-10-06 08:31:34.756316 dipex-5.8.0/integrations/rundb/db_overview.py
--rw-r--r--   0        0        0     1228 2023-10-06 08:31:34.756316 dipex-5.8.0/integrations/rundb/tests/test_db_overview.py
--rw-r--r--   0        0        0     2576 2023-10-06 08:31:38.602565 dipex-5.8.0/pyproject.toml
--rw-r--r--   0        0        0     3893 1970-01-01 00:00:00.000000 dipex-5.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-10-06 08:45:26.899334 dipex-5.9.0/exporters/sql_export/__init__.py
+-rw-r--r--   0        0        0    40011 2023-10-06 08:45:26.773326 dipex-5.9.0/exporters/sql_export/gql_lora_cache_async.py
+-rw-r--r--   0        0        0     2111 2023-10-06 08:45:26.773326 dipex-5.9.0/exporters/sql_export/lc_for_jobs_db.py
+-rw-r--r--   0        0        0     1584 2023-10-06 08:45:26.773326 dipex-5.9.0/exporters/sql_export/log.py
+-rw-r--r--   0        0        0     2742 2023-10-06 08:45:26.773326 dipex-5.9.0/exporters/sql_export/lora_cache.py
+-rw-r--r--   0        0        0     1396 2023-10-06 08:45:26.773326 dipex-5.9.0/exporters/sql_export/main.py
+-rw-r--r--   0        0        0    54838 2023-10-06 08:45:26.774326 dipex-5.9.0/exporters/sql_export/old_lora_cache.py
+-rw-r--r--   0        0        0    29560 2023-10-06 08:45:26.778326 dipex-5.9.0/exporters/sql_export/sql_export.py
+-rw-r--r--   0        0        0     9642 2023-10-06 08:45:26.778326 dipex-5.9.0/exporters/sql_export/sql_table_defs.py
+-rw-r--r--   0        0        0     5385 2023-10-06 08:45:26.778326 dipex-5.9.0/exporters/sql_export/sql_url.py
+-rw-r--r--   0        0        0     5543 2023-10-06 08:45:26.780326 dipex-5.9.0/exporters/sql_export/trigger.py
+-rw-r--r--   0        0        0     5075 2023-10-06 08:45:26.783327 dipex-5.9.0/exporters/utils/priority_by_class.py
+-rw-r--r--   0        0        0        0 2023-10-06 08:45:26.899334 dipex-5.9.0/integrations/__init__.py
+-rw-r--r--   0        0        0     3369 2023-10-06 08:45:26.784327 dipex-5.9.0/integrations/aarhus/config.py
+-rw-r--r--   0        0        0     5126 2023-10-06 08:45:26.784327 dipex-5.9.0/integrations/aarhus/dar_helper.py
+-rw-r--r--   0        0        0     3163 2023-10-06 08:45:26.784327 dipex-5.9.0/integrations/aarhus/initial.py
+-rw-r--r--   0        0        0     3234 2023-10-06 08:45:26.785327 dipex-5.9.0/integrations/aarhus/initial_classes.py
+-rw-r--r--   0        0        0     9582 2023-10-06 08:45:26.785327 dipex-5.9.0/integrations/aarhus/los_files.py
+-rw-r--r--   0        0        0     3705 2023-10-06 08:45:26.785327 dipex-5.9.0/integrations/aarhus/los_import.py
+-rw-r--r--   0        0        0     5086 2023-10-06 08:45:26.785327 dipex-5.9.0/integrations/aarhus/los_leder.py
+-rw-r--r--   0        0        0    18392 2023-10-06 08:45:26.785327 dipex-5.9.0/integrations/aarhus/los_org.py
+-rw-r--r--   0        0        0     9228 2023-10-06 08:45:26.786327 dipex-5.9.0/integrations/aarhus/los_pers.py
+-rw-r--r--   0        0        0    21785 2023-10-06 08:45:26.786327 dipex-5.9.0/integrations/aarhus/los_stam.py
+-rw-r--r--   0        0        0     4085 2023-10-06 08:45:26.786327 dipex-5.9.0/integrations/aarhus/payloads.py
+-rw-r--r--   0        0        0        0 2023-10-06 08:45:26.899334 dipex-5.9.0/integrations/aarhus/tests/__init__.py
+-rw-r--r--   0        0        0     1262 2023-10-06 08:45:26.786327 dipex-5.9.0/integrations/aarhus/tests/conftest.py
+-rw-r--r--   0        0        0     3250 2023-10-06 08:45:26.787327 dipex-5.9.0/integrations/aarhus/tests/helpers.py
+-rw-r--r--   0        0        0     2101 2023-10-06 08:45:26.787327 dipex-5.9.0/integrations/aarhus/tests/strategies.py
+-rw-r--r--   0        0        0     1447 2023-10-06 08:45:26.787327 dipex-5.9.0/integrations/aarhus/tests/test_config.py
+-rw-r--r--   0        0        0     1009 2023-10-06 08:45:26.787327 dipex-5.9.0/integrations/aarhus/tests/test_initial.py
+-rw-r--r--   0        0        0     3178 2023-10-06 08:45:26.787327 dipex-5.9.0/integrations/aarhus/tests/test_los_files.py
+-rw-r--r--   0        0        0     1200 2023-10-06 08:45:26.787327 dipex-5.9.0/integrations/aarhus/tests/test_los_import.py
+-rw-r--r--   0        0        0    10703 2023-10-06 08:45:26.788327 dipex-5.9.0/integrations/aarhus/tests/test_los_leder.py
+-rw-r--r--   0        0        0    11047 2023-10-06 08:45:26.788327 dipex-5.9.0/integrations/aarhus/tests/test_los_org.py
+-rw-r--r--   0        0        0     6773 2023-10-06 08:45:26.788327 dipex-5.9.0/integrations/aarhus/tests/test_los_pers.py
+-rw-r--r--   0        0        0    12108 2023-10-06 08:45:26.788327 dipex-5.9.0/integrations/aarhus/tests/test_los_stam.py
+-rw-r--r--   0        0        0     1045 2023-10-06 08:45:26.788327 dipex-5.9.0/integrations/aarhus/tests/test_payloads.py
+-rw-r--r--   0        0        0     7336 2023-10-06 08:45:26.789327 dipex-5.9.0/integrations/aarhus/tests/test_util.py
+-rw-r--r--   0        0        0     6857 2023-10-06 08:45:26.789327 dipex-5.9.0/integrations/aarhus/util.py
+-rw-r--r--   0        0        0     1073 2023-10-06 08:45:26.789327 dipex-5.9.0/integrations/aarhus/uuids.py
+-rw-r--r--   0        0        0        0 2023-10-06 08:45:26.899334 dipex-5.9.0/integrations/ad_integration/__init__.py
+-rw-r--r--   0        0        0    15777 2023-10-06 08:45:26.789327 dipex-5.9.0/integrations/ad_integration/ad_common.py
+-rw-r--r--   0        0        0      852 2023-10-06 08:45:26.790327 dipex-5.9.0/integrations/ad_integration/ad_exceptions.py
+-rw-r--r--   0        0        0    31045 2023-10-06 08:45:26.790327 dipex-5.9.0/integrations/ad_integration/ad_fix_enddate.py
+-rw-r--r--   0        0        0     3960 2023-10-06 08:45:26.790327 dipex-5.9.0/integrations/ad_integration/ad_jinja_filters.py
+-rwxr-xr-x   0        0        0    20093 2023-10-06 08:45:26.791327 dipex-5.9.0/integrations/ad_integration/ad_life_cycle.py
+-rw-r--r--   0        0        0     2392 2023-10-06 08:45:26.791327 dipex-5.9.0/integrations/ad_integration/ad_logger.py
+-rw-r--r--   0        0        0     7203 2023-10-06 08:45:26.791327 dipex-5.9.0/integrations/ad_integration/ad_reader.py
+-rw-r--r--   0        0        0    34412 2023-10-06 08:45:26.791327 dipex-5.9.0/integrations/ad_integration/ad_sync.py
+-rw-r--r--   0        0        0    15426 2023-10-06 08:45:26.792327 dipex-5.9.0/integrations/ad_integration/ad_template_engine.py
+-rw-r--r--   0        0        0      384 2023-10-06 08:45:26.792327 dipex-5.9.0/integrations/ad_integration/ad_templates.py
+-rw-r--r--   0        0        0    54693 2023-10-06 08:45:26.792327 dipex-5.9.0/integrations/ad_integration/ad_writer.py
+-rw-r--r--   0        0        0    11131 2023-10-06 08:45:26.793327 dipex-5.9.0/integrations/ad_integration/import_ad_group_into_mo.py
+-rw-r--r--   0        0        0     8896 2023-10-06 08:45:26.793327 dipex-5.9.0/integrations/ad_integration/mo_to_ad_sync.py
+-rw-r--r--   0        0        0     2522 2023-10-06 08:45:26.793327 dipex-5.9.0/integrations/ad_integration/payloads.py
+-rw-r--r--   0        0        0     9206 2023-10-06 08:45:26.793327 dipex-5.9.0/integrations/ad_integration/read_ad_conf_settings.py
+-rw-r--r--   0        0        0     7898 2023-10-06 08:45:26.793327 dipex-5.9.0/integrations/ad_integration/sync_mo_uuid_to_ad.py
+-rw-r--r--   0        0        0     7518 2023-10-06 08:45:26.794327 dipex-5.9.0/integrations/ad_integration/test_connectivity.py
+-rw-r--r--   0        0        0        0 2023-10-06 08:45:26.900334 dipex-5.9.0/integrations/ad_integration/tests/__init__.py
+-rw-r--r--   0        0        0    17787 2023-10-06 08:45:26.794327 dipex-5.9.0/integrations/ad_integration/tests/mocks.py
+-rw-r--r--   0        0        0      434 2023-10-06 08:45:26.794327 dipex-5.9.0/integrations/ad_integration/tests/name_simulator.py
+-rw-r--r--   0        0        0     3238 2023-10-06 08:45:26.794327 dipex-5.9.0/integrations/ad_integration/tests/test_ad_common.py
+-rw-r--r--   0        0        0    27949 2023-10-06 08:45:26.795328 dipex-5.9.0/integrations/ad_integration/tests/test_ad_fix_enddate.py
+-rw-r--r--   0        0        0     4992 2023-10-06 08:45:26.795328 dipex-5.9.0/integrations/ad_integration/tests/test_ad_jinja_filters.py
+-rw-r--r--   0        0        0    21210 2023-10-06 08:45:26.795328 dipex-5.9.0/integrations/ad_integration/tests/test_ad_life_cycle.py
+-rw-r--r--   0        0        0      580 2023-10-06 08:45:26.795328 dipex-5.9.0/integrations/ad_integration/tests/test_ad_logger.py
+-rw-r--r--   0        0        0     3989 2023-10-06 08:45:26.796327 dipex-5.9.0/integrations/ad_integration/tests/test_ad_reader.py
+-rw-r--r--   0        0        0    43922 2023-10-06 08:45:26.796327 dipex-5.9.0/integrations/ad_integration/tests/test_ad_sync.py
+-rw-r--r--   0        0        0    71554 2023-10-06 08:45:26.797328 dipex-5.9.0/integrations/ad_integration/tests/test_ad_writer.py
+-rw-r--r--   0        0        0     2259 2023-10-06 08:45:26.797328 dipex-5.9.0/integrations/ad_integration/tests/test_dot_mapping.py
+-rw-r--r--   0        0        0     1205 2023-10-06 08:45:26.797328 dipex-5.9.0/integrations/ad_integration/tests/test_first_included.py
+-rw-r--r--   0        0        0     5180 2023-10-06 08:45:26.797328 dipex-5.9.0/integrations/ad_integration/tests/test_import_ad_group_into_mo.py
+-rw-r--r--   0        0        0     4116 2023-10-06 08:45:26.797328 dipex-5.9.0/integrations/ad_integration/tests/test_location_element.py
+-rw-r--r--   0        0        0    11237 2023-10-06 08:45:26.798328 dipex-5.9.0/integrations/ad_integration/tests/test_mo_data_source.py
+-rw-r--r--   0        0        0     5873 2023-10-06 08:45:26.798328 dipex-5.9.0/integrations/ad_integration/tests/test_mo_to_ad_sync.py
+-rw-r--r--   0        0        0     1471 2023-10-06 08:45:26.798328 dipex-5.9.0/integrations/ad_integration/tests/test_morestsource.py
+-rw-r--r--   0        0        0     5408 2023-10-06 08:45:26.798328 dipex-5.9.0/integrations/ad_integration/tests/test_read_ad_conf_settings.py
+-rw-r--r--   0        0        0     1896 2023-10-06 08:45:26.798328 dipex-5.9.0/integrations/ad_integration/tests/test_recursive_dict_update.py
+-rw-r--r--   0        0        0     5579 2023-10-06 08:45:26.798328 dipex-5.9.0/integrations/ad_integration/tests/test_sync_mo_uuid_to_ad.py
+-rw-r--r--   0        0        0    23437 2023-10-06 08:45:26.799328 dipex-5.9.0/integrations/ad_integration/tests/test_usernames.py
+-rw-r--r--   0        0        0    18469 2023-10-06 08:45:26.799328 dipex-5.9.0/integrations/ad_integration/tests/test_utils.py
+-rw-r--r--   0        0        0    13493 2023-10-06 08:45:26.799328 dipex-5.9.0/integrations/ad_integration/user_names.py
+-rw-r--r--   0        0        0     4306 2023-10-06 08:45:26.800328 dipex-5.9.0/integrations/ad_integration/username_rules/method_2.py
+-rw-r--r--   0        0        0     4558 2023-10-06 08:45:26.800328 dipex-5.9.0/integrations/ad_integration/utils.py
+-rw-r--r--   0        0        0        0 2023-10-06 08:45:26.900334 dipex-5.9.0/integrations/calculate_primary/__init__.py
+-rw-r--r--   0        0        0     3121 2023-10-06 08:45:26.800328 dipex-5.9.0/integrations/calculate_primary/calculate_primary.py
+-rw-r--r--   0        0        0    19033 2023-10-06 08:45:26.800328 dipex-5.9.0/integrations/calculate_primary/common.py
+-rw-r--r--   0        0        0     2597 2023-10-06 08:45:26.801328 dipex-5.9.0/integrations/calculate_primary/default.py
+-rw-r--r--   0        0        0     4045 2023-10-06 08:45:26.801328 dipex-5.9.0/integrations/calculate_primary/opus.py
+-rw-r--r--   0        0        0     3651 2023-10-06 08:45:26.801328 dipex-5.9.0/integrations/calculate_primary/sd.py
+-rw-r--r--   0        0        0        0 2023-10-06 08:45:26.900334 dipex-5.9.0/integrations/calculate_primary/tests/__init__.py
+-rw-r--r--   0        0        0    19238 2023-10-06 08:45:26.801328 dipex-5.9.0/integrations/calculate_primary/tests/test_primary.py
+-rw-r--r--   0        0        0      896 2023-10-06 08:45:26.802328 dipex-5.9.0/integrations/cpr_mapper.py
+-rw-r--r--   0        0        0     1010 2023-10-06 08:45:26.802328 dipex-5.9.0/integrations/dawa_helper.py
+-rw-r--r--   0        0        0       99 2023-10-06 08:45:26.802328 dipex-5.9.0/integrations/kle/__init__.py
+-rw-r--r--   0        0        0    13325 2023-10-06 08:45:26.802328 dipex-5.9.0/integrations/kle/kle_import.py
+-rw-r--r--   0        0        0     4584 2023-10-06 08:45:26.802328 dipex-5.9.0/integrations/kle/kle_import_export.py
+-rw-r--r--   0        0        0     9061 2023-10-06 08:45:26.802328 dipex-5.9.0/integrations/kle/kle_xlsx.py
+-rw-r--r--   0        0        0     2261 2023-10-06 08:45:26.803328 dipex-5.9.0/integrations/kle/payloads.py
+-rw-r--r--   0        0        0     4550 2023-10-06 08:45:26.803328 dipex-5.9.0/integrations/opus/clear_and_import_opus.py
+-rw-r--r--   0        0        0    40237 2023-10-06 08:45:26.803328 dipex-5.9.0/integrations/opus/opus_diff_import.py
+-rw-r--r--   0        0        0      353 2023-10-06 08:45:26.803328 dipex-5.9.0/integrations/opus/opus_exceptions.py
+-rw-r--r--   0        0        0     4348 2023-10-06 08:45:26.804328 dipex-5.9.0/integrations/opus/opus_file_reader.py
+-rw-r--r--   0        0        0    14167 2023-10-06 08:45:26.804328 dipex-5.9.0/integrations/opus/opus_helpers.py
+-rw-r--r--   0        0        0     2958 2023-10-06 08:45:26.804328 dipex-5.9.0/integrations/opus/opus_reimport_one.py
+-rw-r--r--   0        0        0     4515 2023-10-06 08:45:26.804328 dipex-5.9.0/integrations/opus/org_tree_print/main.py
+-rw-r--r--   0        0        0     5449 2023-10-06 08:45:26.805328 dipex-5.9.0/integrations/opus/payloads.py
+-rw-r--r--   0        0        0    18762 2023-10-06 08:45:26.805328 dipex-5.9.0/integrations/opus/tests/test_opus_diff_import.py
+-rw-r--r--   0        0        0     1406 2023-10-06 08:45:26.806328 dipex-5.9.0/integrations/opus/tests/test_opus_file_reader.py
+-rw-r--r--   0        0        0     3966 2023-10-06 08:45:26.806328 dipex-5.9.0/integrations/opus/tests/test_opus_helpers.py
+-rw-r--r--   0        0        0     4562 2023-10-06 08:45:26.806328 dipex-5.9.0/integrations/rundb/db_overview.py
+-rw-r--r--   0        0        0     1228 2023-10-06 08:45:26.807328 dipex-5.9.0/integrations/rundb/tests/test_db_overview.py
+-rw-r--r--   0        0        0     2576 2023-10-06 08:45:29.893529 dipex-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3893 1970-01-01 00:00:00.000000 dipex-5.9.0/PKG-INFO
```

### Comparing `dipex-5.8.0/exporters/sql_export/gql_lora_cache_async.py` & `dipex-5.9.0/exporters/sql_export/gql_lora_cache_async.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/lc_for_jobs_db.py` & `dipex-5.9.0/exporters/sql_export/lc_for_jobs_db.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/log.py` & `dipex-5.9.0/exporters/sql_export/log.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/lora_cache.py` & `dipex-5.9.0/exporters/sql_export/lora_cache.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/main.py` & `dipex-5.9.0/exporters/sql_export/main.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/old_lora_cache.py` & `dipex-5.9.0/exporters/sql_export/old_lora_cache.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/sql_export.py` & `dipex-5.9.0/exporters/sql_export/sql_export.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/sql_table_defs.py` & `dipex-5.9.0/exporters/sql_export/sql_table_defs.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/sql_url.py` & `dipex-5.9.0/exporters/sql_export/sql_url.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/sql_export/trigger.py` & `dipex-5.9.0/exporters/sql_export/trigger.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/exporters/utils/priority_by_class.py` & `dipex-5.9.0/exporters/utils/priority_by_class.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/config.py` & `dipex-5.9.0/integrations/aarhus/config.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/dar_helper.py` & `dipex-5.9.0/integrations/aarhus/dar_helper.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/initial.py` & `dipex-5.9.0/integrations/aarhus/initial.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/initial_classes.py` & `dipex-5.9.0/integrations/aarhus/initial_classes.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/los_files.py` & `dipex-5.9.0/integrations/aarhus/los_files.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/los_import.py` & `dipex-5.9.0/integrations/aarhus/los_import.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/los_leder.py` & `dipex-5.9.0/integrations/aarhus/los_leder.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/los_org.py` & `dipex-5.9.0/integrations/aarhus/los_org.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/los_pers.py` & `dipex-5.9.0/integrations/aarhus/los_pers.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/los_stam.py` & `dipex-5.9.0/integrations/aarhus/los_stam.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/payloads.py` & `dipex-5.9.0/integrations/aarhus/payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/conftest.py` & `dipex-5.9.0/integrations/aarhus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/helpers.py` & `dipex-5.9.0/integrations/aarhus/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/strategies.py` & `dipex-5.9.0/integrations/aarhus/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_config.py` & `dipex-5.9.0/integrations/aarhus/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_initial.py` & `dipex-5.9.0/integrations/aarhus/tests/test_initial.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_los_files.py` & `dipex-5.9.0/integrations/aarhus/tests/test_los_files.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_los_import.py` & `dipex-5.9.0/integrations/aarhus/tests/test_los_import.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_los_leder.py` & `dipex-5.9.0/integrations/aarhus/tests/test_los_leder.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_los_org.py` & `dipex-5.9.0/integrations/aarhus/tests/test_los_org.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_los_pers.py` & `dipex-5.9.0/integrations/aarhus/tests/test_los_pers.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_los_stam.py` & `dipex-5.9.0/integrations/aarhus/tests/test_los_stam.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_payloads.py` & `dipex-5.9.0/integrations/aarhus/tests/test_payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/tests/test_util.py` & `dipex-5.9.0/integrations/aarhus/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/util.py` & `dipex-5.9.0/integrations/aarhus/util.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/aarhus/uuids.py` & `dipex-5.9.0/integrations/aarhus/uuids.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_common.py` & `dipex-5.9.0/integrations/ad_integration/ad_common.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_exceptions.py` & `dipex-5.9.0/integrations/ad_integration/ad_exceptions.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_fix_enddate.py` & `dipex-5.9.0/integrations/ad_integration/ad_fix_enddate.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_jinja_filters.py` & `dipex-5.9.0/integrations/ad_integration/ad_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_life_cycle.py` & `dipex-5.9.0/integrations/ad_integration/ad_life_cycle.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_logger.py` & `dipex-5.9.0/integrations/ad_integration/ad_logger.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_reader.py` & `dipex-5.9.0/integrations/ad_integration/ad_reader.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_sync.py` & `dipex-5.9.0/integrations/ad_integration/ad_sync.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_template_engine.py` & `dipex-5.9.0/integrations/ad_integration/ad_template_engine.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/ad_writer.py` & `dipex-5.9.0/integrations/ad_integration/ad_writer.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/import_ad_group_into_mo.py` & `dipex-5.9.0/integrations/ad_integration/import_ad_group_into_mo.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/mo_to_ad_sync.py` & `dipex-5.9.0/integrations/ad_integration/mo_to_ad_sync.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/payloads.py` & `dipex-5.9.0/integrations/ad_integration/payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/read_ad_conf_settings.py` & `dipex-5.9.0/integrations/ad_integration/read_ad_conf_settings.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/sync_mo_uuid_to_ad.py` & `dipex-5.9.0/integrations/ad_integration/sync_mo_uuid_to_ad.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/test_connectivity.py` & `dipex-5.9.0/integrations/ad_integration/test_connectivity.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/mocks.py` & `dipex-5.9.0/integrations/ad_integration/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_ad_common.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_ad_common.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_ad_fix_enddate.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_ad_fix_enddate.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_ad_jinja_filters.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_ad_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_ad_life_cycle.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_ad_life_cycle.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_ad_logger.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_ad_logger.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_ad_reader.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_ad_reader.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_ad_sync.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_ad_sync.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_ad_writer.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_ad_writer.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_dot_mapping.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_dot_mapping.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_first_included.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_first_included.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_import_ad_group_into_mo.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_import_ad_group_into_mo.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_location_element.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_location_element.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_mo_data_source.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_mo_data_source.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_mo_to_ad_sync.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_mo_to_ad_sync.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_morestsource.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_morestsource.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_read_ad_conf_settings.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_read_ad_conf_settings.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_recursive_dict_update.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_recursive_dict_update.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_sync_mo_uuid_to_ad.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_sync_mo_uuid_to_ad.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_usernames.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_usernames.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/tests/test_utils.py` & `dipex-5.9.0/integrations/ad_integration/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/user_names.py` & `dipex-5.9.0/integrations/ad_integration/user_names.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/username_rules/method_2.py` & `dipex-5.9.0/integrations/ad_integration/username_rules/method_2.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/ad_integration/utils.py` & `dipex-5.9.0/integrations/ad_integration/utils.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/calculate_primary/calculate_primary.py` & `dipex-5.9.0/integrations/calculate_primary/calculate_primary.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/calculate_primary/common.py` & `dipex-5.9.0/integrations/calculate_primary/common.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/calculate_primary/default.py` & `dipex-5.9.0/integrations/calculate_primary/default.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/calculate_primary/opus.py` & `dipex-5.9.0/integrations/calculate_primary/opus.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/calculate_primary/sd.py` & `dipex-5.9.0/integrations/calculate_primary/sd.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/calculate_primary/tests/test_primary.py` & `dipex-5.9.0/integrations/calculate_primary/tests/test_primary.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/cpr_mapper.py` & `dipex-5.9.0/integrations/cpr_mapper.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/dawa_helper.py` & `dipex-5.9.0/integrations/dawa_helper.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/kle/kle_import.py` & `dipex-5.9.0/integrations/kle/kle_import.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/kle/kle_import_export.py` & `dipex-5.9.0/integrations/kle/kle_import_export.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/kle/kle_xlsx.py` & `dipex-5.9.0/integrations/kle/kle_xlsx.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/kle/payloads.py` & `dipex-5.9.0/integrations/kle/payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/clear_and_import_opus.py` & `dipex-5.9.0/integrations/opus/clear_and_import_opus.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/opus_diff_import.py` & `dipex-5.9.0/integrations/opus/opus_diff_import.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/opus_file_reader.py` & `dipex-5.9.0/integrations/opus/opus_file_reader.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/opus_helpers.py` & `dipex-5.9.0/integrations/opus/opus_helpers.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/opus_reimport_one.py` & `dipex-5.9.0/integrations/opus/opus_reimport_one.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/org_tree_print/main.py` & `dipex-5.9.0/integrations/opus/org_tree_print/main.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/payloads.py` & `dipex-5.9.0/integrations/opus/payloads.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/tests/test_opus_diff_import.py` & `dipex-5.9.0/integrations/opus/tests/test_opus_diff_import.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/tests/test_opus_file_reader.py` & `dipex-5.9.0/integrations/opus/tests/test_opus_file_reader.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/opus/tests/test_opus_helpers.py` & `dipex-5.9.0/integrations/opus/tests/test_opus_helpers.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/rundb/db_overview.py` & `dipex-5.9.0/integrations/rundb/db_overview.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/integrations/rundb/tests/test_db_overview.py` & `dipex-5.9.0/integrations/rundb/tests/test_db_overview.py`

 * *Files identical despite different names*

### Comparing `dipex-5.8.0/pyproject.toml` & `dipex-5.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DIPEX"
-version = "5.8.0"
+version = "5.9.0"
 authors = ["Magenta ApS <info@magenta.dk>"]
 description = "OS2mo-data-import-and-export"
 license = "MPL-2.0"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/os2mo-data-import-and-export"
 keywords = ["DIPEX", "OS2mo-data-import-and-export"]
 packages = [
```

### Comparing `dipex-5.8.0/PKG-INFO` & `dipex-5.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DIPEX
-Version: 5.8.0
+Version: 5.9.0
 Summary: OS2mo-data-import-and-export
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: DIPEX,OS2mo-data-import-and-export
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
```

