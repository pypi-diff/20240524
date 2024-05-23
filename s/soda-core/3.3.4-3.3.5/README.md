# Comparing `tmp/soda_core-3.3.4.tar.gz` & `tmp/soda_core-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core-3.3.4.tar", last modified: Tue May  7 23:39:59 2024, max compression
+gzip compressed data, was "soda_core-3.3.5.tar", last modified: Thu May 23 22:50:28 2024, max compression
```

## Comparing `soda_core-3.3.4.tar` & `soda_core-3.3.5.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.483956 soda_core-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 23:39:42.000000 soda_core-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 23:39:59.483956 soda_core-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:39:59.483956 soda_core-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-07 23:39:42.000000 soda_core-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.463956 soda_core-3.3.4/soda/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.467956 soda_core-3.3.4/soda/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    23383 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.467956 soda_core-3.3.4/soda/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/cloud/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/cloud/dbt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/cloud/historic_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/cloud/soda_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.467956 soda_core-3.3.4/soda/common/
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/attributes_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/exception_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/json_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/random_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/string_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/undefined_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/common/yaml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.467956 soda_core-3.3.4/soda/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/configuration/configuration_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.463956 soda_core-3.3.4/soda/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.467956 soda_core-3.3.4/soda/core/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/core/api/data_source_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.471956 soda_core-3.3.4/soda/execution/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.471956 soda_core-3.3.4/soda/execution/check/
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/anomaly_detection_metric_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/anomaly_metric_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/automated_monitoring_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/change_over_time_metric_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    23233 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/discover_tables_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/distribution_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/freshness_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/group_by_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/group_evolution_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/metric_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6021 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/profile_columns_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/reference_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/row_count_comparison_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/sample_tables_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/schema_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/user_defined_failed_rows_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check/user_defined_failed_rows_expression_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check_outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/check_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    56258 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/data_source_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/data_source_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/derived_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.475956 soda_core-3.3.4/soda/execution/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/column_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/group_by_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/group_evolution_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/numeric_query_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/query_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/reference_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/schema_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/user_defined_failed_rows_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/metric/user_defined_numeric_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/partition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.475956 soda_core-3.3.4/soda/execution/query/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/aggregation_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/duplicates_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/group_by_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/group_evolution_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/reference_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/sample_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/schema_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/user_defined_failed_rows_expression_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/user_defined_failed_rows_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/query/user_defined_numeric_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/schema_comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/table.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/execution/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.475956 soda_core-3.3.4/soda/model/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/model/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.475956 soda_core-3.3.4/soda/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/profiling/discover_table_result_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/profiling/discover_tables_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/profiling/discover_tables_result_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/profiling/numeric_column_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/profiling/profile_columns_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/profiling/sample_tables_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/profiling/text_column_profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.479956 soda_core-3.3.4/soda/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/db_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/default_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/http_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/log_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/sample_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/sample_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sampler/soda_cloud_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    45305 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.483956 soda_core-3.3.4/soda/sodacl/
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/anomaly_detection_metric_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/anomaly_metric_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.483956 soda_core-3.3.4/soda/sodacl/antlr/
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/antlr/SodaCLAntlrLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/antlr/SodaCLAntlrListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   122618 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/antlr/SodaCLAntlrParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/antlr/SodaCLAntlrVisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/change_over_time_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/change_over_time_metric_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/column_checks_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/column_configurations_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/columnset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/data_source_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/data_source_scan_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/distribution_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/file_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/for_each_column_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/for_each_dataset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/format_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/freshness_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/group_by_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/group_evolution_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/metric_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/metric_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/missing_and_valid_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/name_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/partition_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/reference_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/row_count_comparison_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/schema_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/sodacl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    93135 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/sodacl_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/table_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/tableset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/threshold_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/user_defined_failed_rows_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.483956 soda_core-3.3.4/soda/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/telemetry/memory_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/telemetry/soda_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/telemetry/soda_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-07 23:39:42.000000 soda_core-3.3.4/soda/telemetry/soda_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:59.483956 soda_core-3.3.4/soda_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-07 23:39:59.000000 soda_core-3.3.4/soda_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-07 23:39:59.000000 soda_core-3.3.4/soda_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:39:59.000000 soda_core-3.3.4/soda_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 23:39:59.000000 soda_core-3.3.4/soda_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-07 23:39:59.000000 soda_core-3.3.4/soda_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:39:59.000000 soda_core-3.3.4/soda_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.721960 soda_core-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:50:11.000000 soda_core-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 22:50:28.721960 soda_core-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:28.721960 soda_core-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-23 22:50:11.000000 soda_core-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.701960 soda_core-3.3.5/soda/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.701960 soda_core-3.3.5/soda/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    23383 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.701960 soda_core-3.3.5/soda/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/cloud/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/cloud/dbt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/cloud/historic_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/cloud/soda_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.705960 soda_core-3.3.5/soda/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/attributes_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/exception_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/json_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/random_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/string_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/undefined_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/common/yaml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.705960 soda_core-3.3.5/soda/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/configuration/configuration_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.697960 soda_core-3.3.5/soda/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.705960 soda_core-3.3.5/soda/core/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/core/api/data_source_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.705960 soda_core-3.3.5/soda/execution/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.709960 soda_core-3.3.5/soda/execution/check/
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/anomaly_detection_metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/anomaly_metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/automated_monitoring_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/change_over_time_metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23233 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/discover_tables_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/distribution_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/freshness_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/group_by_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/group_evolution_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6021 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/profile_columns_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/reference_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/row_count_comparison_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/sample_tables_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/schema_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/user_defined_failed_rows_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check/user_defined_failed_rows_expression_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56258 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/data_source_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/data_source_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/derived_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.709960 soda_core-3.3.5/soda/execution/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/column_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/group_by_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/group_evolution_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/numeric_query_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/query_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/reference_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/schema_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/user_defined_failed_rows_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/metric/user_defined_numeric_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.709960 soda_core-3.3.5/soda/execution/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/aggregation_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/duplicates_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/group_by_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/group_evolution_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/reference_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/sample_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/user_defined_failed_rows_expression_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/user_defined_failed_rows_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/query/user_defined_numeric_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/schema_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/execution/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.713960 soda_core-3.3.5/soda/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/model/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.713960 soda_core-3.3.5/soda/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/profiling/discover_table_result_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/profiling/discover_tables_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/profiling/discover_tables_result_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/profiling/numeric_column_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/profiling/profile_columns_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/profiling/sample_tables_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/profiling/text_column_profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.713960 soda_core-3.3.5/soda/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/db_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/default_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/http_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/log_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/sample_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/sample_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sampler/soda_cloud_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45305 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.717960 soda_core-3.3.5/soda/sodacl/
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/anomaly_detection_metric_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/anomaly_metric_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.717960 soda_core-3.3.5/soda/sodacl/antlr/
+-rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/antlr/SodaCLAntlrLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/antlr/SodaCLAntlrListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122618 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/antlr/SodaCLAntlrParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/antlr/SodaCLAntlrVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/change_over_time_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/change_over_time_metric_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/column_checks_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/column_configurations_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/columnset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/data_source_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/data_source_scan_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/distribution_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/file_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/for_each_column_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/for_each_dataset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/format_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/freshness_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/group_by_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/group_evolution_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/metric_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/metric_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/missing_and_valid_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/name_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/partition_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/reference_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/row_count_comparison_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/schema_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/sodacl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94517 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/sodacl_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/table_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/tableset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/threshold_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/user_defined_failed_rows_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.717960 soda_core-3.3.5/soda/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/telemetry/memory_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/telemetry/soda_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/telemetry/soda_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-23 22:50:11.000000 soda_core-3.3.5/soda/telemetry/soda_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:28.721960 soda_core-3.3.5/soda_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 22:50:28.000000 soda_core-3.3.5/soda_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-23 22:50:28.000000 soda_core-3.3.5/soda_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:50:28.000000 soda_core-3.3.5/soda_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 22:50:28.000000 soda_core-3.3.5/soda_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-23 22:50:28.000000 soda_core-3.3.5/soda_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:50:28.000000 soda_core-3.3.5/soda_core.egg-info/top_level.txt
```

### Comparing `soda_core-3.3.4/LICENSE` & `soda_core-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/PKG-INFO` & `soda_core-3.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-core
-Version: 3.3.4
+Version: 3.3.5
 Summary: Soda Core library & CLI
 Author: Soda Data N.V.
 Author-email: info@soda.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `soda_core-3.3.4/setup.py` & `soda_core-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_namespace_packages, setup
 
 package_name = "soda-core"
 # Managed by tbump - do not change manually
-package_version = "3.3.4"
+package_version = "3.3.5"
 description = "Soda Core"
 
 requires = [
     "markupsafe>=2.0.1,<=2.1.2",
     "Jinja2>=2.11,<4.0",
     "click~=8.0",
     "ruamel.yaml>=0.17.0,<0.18.0",
```

### Comparing `soda_core-3.3.4/soda/cli/cli.py` & `soda_core-3.3.5/soda/cli/cli.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/cloud/cloud.py` & `soda_core-3.3.5/soda/cloud/cloud.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/cloud/historic_descriptor.py` & `soda_core-3.3.5/soda/cloud/historic_descriptor.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/cloud/soda_cloud.py` & `soda_core-3.3.5/soda/cloud/soda_cloud.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/attributes_handler.py` & `soda_core-3.3.5/soda/common/attributes_handler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/aws_credentials.py` & `soda_core-3.3.5/soda/common/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/config_helper.py` & `soda_core-3.3.5/soda/common/config_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/exceptions.py` & `soda_core-3.3.5/soda/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/file_system.py` & `soda_core-3.3.5/soda/common/file_system.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/jinja.py` & `soda_core-3.3.5/soda/common/jinja.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/json_helper.py` & `soda_core-3.3.5/soda/common/json_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/log.py` & `soda_core-3.3.5/soda/common/log.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/logs.py` & `soda_core-3.3.5/soda/common/logs.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/parser.py` & `soda_core-3.3.5/soda/common/parser.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/query_helper.py` & `soda_core-3.3.5/soda/common/query_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/common/yaml_helper.py` & `soda_core-3.3.5/soda/common/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/configuration/configuration.py` & `soda_core-3.3.5/soda/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/configuration/configuration_parser.py` & `soda_core-3.3.5/soda/configuration/configuration_parser.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/core/api/data_source_utils.py` & `soda_core-3.3.5/soda/core/api/data_source_utils.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/anomaly_detection_metric_check.py` & `soda_core-3.3.5/soda/execution/check/anomaly_detection_metric_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/anomaly_metric_check.py` & `soda_core-3.3.5/soda/execution/check/anomaly_metric_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/automated_monitoring_run.py` & `soda_core-3.3.5/soda/execution/check/automated_monitoring_run.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/change_over_time_metric_check.py` & `soda_core-3.3.5/soda/execution/check/change_over_time_metric_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/check.py` & `soda_core-3.3.5/soda/execution/check/check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/discover_tables_run.py` & `soda_core-3.3.5/soda/execution/check/discover_tables_run.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/distribution_check.py` & `soda_core-3.3.5/soda/execution/check/distribution_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/freshness_check.py` & `soda_core-3.3.5/soda/execution/check/freshness_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/group_by_check.py` & `soda_core-3.3.5/soda/execution/check/group_by_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/group_evolution_check.py` & `soda_core-3.3.5/soda/execution/check/group_evolution_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/metric_check.py` & `soda_core-3.3.5/soda/execution/check/metric_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/profile_columns_run.py` & `soda_core-3.3.5/soda/execution/check/profile_columns_run.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/reference_check.py` & `soda_core-3.3.5/soda/execution/check/reference_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/row_count_comparison_check.py` & `soda_core-3.3.5/soda/execution/check/row_count_comparison_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/sample_tables_run.py` & `soda_core-3.3.5/soda/execution/check/sample_tables_run.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/schema_check.py` & `soda_core-3.3.5/soda/execution/check/schema_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/user_defined_failed_rows_check.py` & `soda_core-3.3.5/soda/execution/check/user_defined_failed_rows_check.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/check/user_defined_failed_rows_expression_check.py` & `soda_core-3.3.5/soda/execution/check/user_defined_failed_rows_expression_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,36 +40,43 @@
                 check=self,
             )
         )
 
     def evaluate(self, metrics: Dict[str, Metric], historic_values: Dict[str, object]):
         self.check_value: int = metrics.get(KEY_FAILED_ROWS_COUNT).value
 
-        self.outcome = CheckOutcome.FAIL
-
-        if self.check_value > 0:
+        # Thresholds path
+        if self.check_cfg.fail_threshold_cfg or self.check_cfg.warn_threshold_cfg:
             if self.check_cfg.fail_threshold_cfg and self.check_cfg.fail_threshold_cfg.is_bad(self.check_value):
                 self.outcome = CheckOutcome.FAIL
             elif self.check_cfg.warn_threshold_cfg and self.check_cfg.warn_threshold_cfg.is_bad(self.check_value):
                 self.outcome = CheckOutcome.WARN
+            else:
+                self.outcome = CheckOutcome.PASS
+        else:
+            # Original non-threshold path
+            if self.check_value > 0:
+                self.outcome = CheckOutcome.FAIL
+            else:
+                self.outcome = CheckOutcome.PASS
+
+        if self.check_value > 0:
             # Collect failed rows
             failed_rows_sql = self.get_failed_rows_sql()
             failed_rows_query = UserDefinedFailedRowsExpressionQuery(
                 data_source_scan=self.data_source_scan,
                 check_name=self.check_cfg.source_line,
                 sql=failed_rows_sql,
                 samples_limit=self.check_cfg.samples_limit,
                 partition=self.partition,
                 metric=self.metrics[KEY_FAILED_ROWS_COUNT],
             )
             failed_rows_query.execute()
             if failed_rows_query.sample_ref:
                 self.failed_rows_sample_ref = failed_rows_query.sample_ref
-        else:
-            self.outcome = CheckOutcome.PASS
 
     def get_failed_rows_sql(self) -> str:
         columns = ", ".join(
             self.data_source_scan.data_source.sql_select_all_column_names(self.partition.table.table_name)
         )
         sql = (
             f"SELECT {columns} \n"
```

### Comparing `soda_core-3.3.4/soda/execution/column.py` & `soda_core-3.3.5/soda/execution/column.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/data_source.py` & `soda_core-3.3.5/soda/execution/data_source.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/data_source_manager.py` & `soda_core-3.3.5/soda/execution/data_source_manager.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/data_source_scan.py` & `soda_core-3.3.5/soda/execution/data_source_scan.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/data_type.py` & `soda_core-3.3.5/soda/execution/data_type.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/derived_formula.py` & `soda_core-3.3.5/soda/execution/derived_formula.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/identity.py` & `soda_core-3.3.5/soda/execution/identity.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/column_metrics.py` & `soda_core-3.3.5/soda/execution/metric/column_metrics.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/derived_metric.py` & `soda_core-3.3.5/soda/execution/metric/derived_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/group_by_metric.py` & `soda_core-3.3.5/soda/execution/metric/group_by_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/group_evolution_metric.py` & `soda_core-3.3.5/soda/execution/metric/group_evolution_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/metric.py` & `soda_core-3.3.5/soda/execution/metric/metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/numeric_query_metric.py` & `soda_core-3.3.5/soda/execution/metric/numeric_query_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/query_metric.py` & `soda_core-3.3.5/soda/execution/metric/query_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/reference_metric.py` & `soda_core-3.3.5/soda/execution/metric/reference_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/schema_metric.py` & `soda_core-3.3.5/soda/execution/metric/schema_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/user_defined_failed_rows_metric.py` & `soda_core-3.3.5/soda/execution/metric/user_defined_failed_rows_metric.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/metric/user_defined_numeric_metric.py` & `soda_core-3.3.5/soda/execution/query/group_evolution_query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,28 @@
-from soda.execution.metric.query_metric import QueryMetric
-from soda.execution.query.user_defined_numeric_query import UserDefinedNumericQuery
+from __future__ import annotations
 
+from soda.execution.query.query import Query
 
-class UserDefinedNumericMetric(QueryMetric):
+
+class GroupEvolutionQuery(Query):
     def __init__(
         self,
-        data_source_scan: "DataSourceScan",
-        check_name: str,
-        sql: str,
-        check: "Check" = None,
+        data_source_scan: DataSourceScan,
+        metric: GroupEvolutionMetric,
+        partition: Partition,
+        location: Location | None = None,
+        samples_limit: int | None = None,
     ):
         super().__init__(
             data_source_scan=data_source_scan,
-            partition=None,
-            column=None,
-            name=check_name,
-            check=check,
-            identity_parts=[sql],
+            unqualified_query_name=f"group_evolution[{metric.name}]",
+            location=location,
+            samples_limit=samples_limit,
+            sql=metric.query,
+            partition=partition,
         )
-        self.sql = sql
-
-    def __str__(self):
-        return f'"{self.name}"'
+        self.metric = metric
 
-    def set_value(self, value):
-        if value is None or isinstance(value, float):
-            self.value = value
-        else:
-            self.value = float(value)
-
-    def ensure_query(self):
-        query = UserDefinedNumericQuery(
-            data_source_scan=self.data_source_scan,
-            check_name=self.name,
-            sql=self.sql,
-            metric=self,
-        )
-        self.queries.append(query)
-        self.data_source_scan.queries.append(query)
+    def execute(self):
+        self.fetchall()
+        # Only single value per group is supported and we skip nulls
+        self.metric.set_value([r[0] for r in self.rows if r[0] is not None])
```

### Comparing `soda_core-3.3.4/soda/execution/partition.py` & `soda_core-3.3.5/soda/execution/partition.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/aggregation_query.py` & `soda_core-3.3.5/soda/execution/query/aggregation_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/duplicates_query.py` & `soda_core-3.3.5/soda/execution/query/duplicates_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/group_by_query.py` & `soda_core-3.3.5/soda/execution/query/group_by_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/group_evolution_query.py` & `soda_core-3.3.5/soda/execution/query/user_defined_failed_rows_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
 from soda.execution.query.query import Query
 
 
-class GroupEvolutionQuery(Query):
+class UserDefinedFailedRowsQuery(Query):
     def __init__(
         self,
         data_source_scan: DataSourceScan,
-        metric: GroupEvolutionMetric,
+        metric: FailedRowsQueryMetric,
         partition: Partition,
         location: Location | None = None,
         samples_limit: int | None = None,
     ):
         super().__init__(
             data_source_scan=data_source_scan,
-            unqualified_query_name=f"group_evolution[{metric.name}]",
+            unqualified_query_name=f"failed_rows[{metric.name}]",
             location=location,
             samples_limit=samples_limit,
             sql=metric.query,
             partition=partition,
         )
         self.metric = metric
 
     def execute(self):
-        self.fetchall()
-        # Only single value per group is supported and we skip nulls
-        self.metric.set_value([r[0] for r in self.rows if r[0] is not None])
+        self.store()
+        if self.sample_ref:
+            self.metric.set_value(self.sample_ref.total_row_count)
+            self.metric.failed_rows_sample_ref = self.sample_ref
```

### Comparing `soda_core-3.3.4/soda/execution/query/query.py` & `soda_core-3.3.5/soda/execution/query/query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/reference_query.py` & `soda_core-3.3.5/soda/execution/query/reference_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/sample_query.py` & `soda_core-3.3.5/soda/execution/query/sample_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/schema_query.py` & `soda_core-3.3.5/soda/execution/query/schema_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/user_defined_failed_rows_expression_query.py` & `soda_core-3.3.5/soda/execution/query/user_defined_failed_rows_expression_query.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/query/user_defined_failed_rows_query.py` & `soda_core-3.3.5/soda/execution/query/user_defined_numeric_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
+from soda.execution.metric.metric import Metric
 from soda.execution.query.query import Query
 
 
-class UserDefinedFailedRowsQuery(Query):
+class UserDefinedNumericQuery(Query):
     def __init__(
         self,
         data_source_scan: DataSourceScan,
-        metric: FailedRowsQueryMetric,
-        partition: Partition,
-        location: Location | None = None,
-        samples_limit: int | None = None,
+        check_name: str,
+        sql: str,
+        metric: Metric,
     ):
         super().__init__(
-            data_source_scan=data_source_scan,
-            unqualified_query_name=f"failed_rows[{metric.name}]",
-            location=location,
-            samples_limit=samples_limit,
-            sql=metric.query,
-            partition=partition,
+            data_source_scan=data_source_scan, unqualified_query_name=f"user_defined_query[{check_name}]", sql=sql
         )
         self.metric = metric
 
     def execute(self):
-        self.store()
-        if self.sample_ref:
-            self.metric.set_value(self.sample_ref.total_row_count)
-            self.metric.failed_rows_sample_ref = self.sample_ref
+        self.fetchone()
+        if self.row is not None:
+            for index in range(len(self.description)):
+                if self.row[index] is not None:
+                    metric_value = float(self.row[index])
+                    self.metric.set_value(metric_value)
+
+            sample_query = self.metric.create_failed_rows_sample_query()
+            if sample_query:
+                self.metric.queries.append(sample_query)
+                sample_query.execute()
```

### Comparing `soda_core-3.3.4/soda/execution/schema_comparator.py` & `soda_core-3.3.5/soda/execution/schema_comparator.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/execution/table.py` & `soda_core-3.3.5/soda/execution/table.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/profiling/discover_table_result_table.py` & `soda_core-3.3.5/soda/profiling/discover_table_result_table.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/profiling/discover_tables_result.py` & `soda_core-3.3.5/soda/profiling/discover_tables_result.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/profiling/discover_tables_result_column.py` & `soda_core-3.3.5/soda/profiling/discover_tables_result_column.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/profiling/numeric_column_profiler.py` & `soda_core-3.3.5/soda/profiling/numeric_column_profiler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/profiling/profile_columns_result.py` & `soda_core-3.3.5/soda/profiling/profile_columns_result.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/profiling/sample_tables_result.py` & `soda_core-3.3.5/soda/profiling/sample_tables_result.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/profiling/text_column_profiler.py` & `soda_core-3.3.5/soda/profiling/text_column_profiler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sampler/db_sample.py` & `soda_core-3.3.5/soda/sampler/db_sample.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sampler/default_sampler.py` & `soda_core-3.3.5/soda/sampler/default_sampler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sampler/http_sampler.py` & `soda_core-3.3.5/soda/sampler/http_sampler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sampler/log_sampler.py` & `soda_core-3.3.5/soda/sampler/log_sampler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sampler/sample_context.py` & `soda_core-3.3.5/soda/sampler/sample_context.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sampler/sample_ref.py` & `soda_core-3.3.5/soda/sampler/sample_ref.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sampler/sample_schema.py` & `soda_core-3.3.5/soda/sampler/sample_schema.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sampler/soda_cloud_sampler.py` & `soda_core-3.3.5/soda/sampler/soda_cloud_sampler.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/scan.py` & `soda_core-3.3.5/soda/scan.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/anomaly_detection_metric_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/anomaly_detection_metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/anomaly_metric_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/anomaly_metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/antlr/SodaCLAntlrLexer.py` & `soda_core-3.3.5/soda/sodacl/antlr/SodaCLAntlrLexer.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/antlr/SodaCLAntlrListener.py` & `soda_core-3.3.5/soda/sodacl/antlr/SodaCLAntlrListener.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/antlr/SodaCLAntlrParser.py` & `soda_core-3.3.5/soda/sodacl/antlr/SodaCLAntlrParser.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/antlr/SodaCLAntlrVisitor.py` & `soda_core-3.3.5/soda/sodacl/antlr/SodaCLAntlrVisitor.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/change_over_time_cfg.py` & `soda_core-3.3.5/soda/sodacl/change_over_time_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/change_over_time_metric_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/change_over_time_metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/check_cfg.py` & `soda_core-3.3.5/soda/sodacl/check_cfg.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,22 +13,24 @@
         source_header: str,
         source_line: str,
         source_configurations: dict | None,
         location: Location,
         name: str | None,
         samples_limit: int | None = None,
         samples_columns: list | None = None,
+        failed_rows_query: str | None = None,
     ):
         self.source_header: str = source_header
         self.source_line: str = source_line
         self.source_configurations = source_configurations
         self.location: Location = location
         self.name: str | None = name
         self.samples_limit: int | None = samples_limit
         self.samples_columns: list | None = samples_columns
+        self.failed_rows_query: str | None = failed_rows_query
 
     def get_column_name(self) -> str | None:
         pass
 
     def instantiate_for_each_dataset(
         self, name: str, table_alias: str, table_name: str, partition_name: str
     ) -> CheckCfg:
```

### Comparing `soda_core-3.3.4/soda/sodacl/data_source_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/data_source_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/data_source_scan_cfg.py` & `soda_core-3.3.5/soda/sodacl/data_source_scan_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/distribution_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/distribution_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/format_cfg.py` & `soda_core-3.3.5/soda/sodacl/format_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/freshness_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/freshness_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/group_by_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/group_by_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/group_evolution_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/group_evolution_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/location.py` & `soda_core-3.3.5/soda/sodacl/location.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/metric_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/metric_check_cfg.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,16 +28,25 @@
         condition: str | None,
         metric_expression: str | None,
         metric_query: str | None,
         change_over_time_cfg: ChangeOverTimeCfg | None,
         fail_threshold_cfg: ThresholdCfg | None,
         warn_threshold_cfg: ThresholdCfg | None,
         samples_limit: int | None = None,
+        failed_rows_query: str | None = None,
     ):
-        super().__init__(source_header, source_line, source_configurations, location, name, samples_limit)
+        super().__init__(
+            source_header,
+            source_line,
+            source_configurations,
+            location,
+            name,
+            samples_limit,
+            failed_rows_query=failed_rows_query,
+        )
         self.metric_name: str = metric_name
         self.metric_args: list[object] | None = metric_args
         self.missing_and_valid_cfg: MissingAndValidCfg = missing_and_valid_cfg
         self.filter: str | None = filter
         self.condition: str | None = condition
         self.metric_expression: str | None = metric_expression
         self.metric_query: str | None = metric_query
```

### Comparing `soda_core-3.3.4/soda/sodacl/missing_and_valid_cfg.py` & `soda_core-3.3.5/soda/sodacl/missing_and_valid_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/partition_cfg.py` & `soda_core-3.3.5/soda/sodacl/partition_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/reference_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/reference_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/row_count_comparison_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/row_count_comparison_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/schema_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/schema_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/sodacl_cfg.py` & `soda_core-3.3.5/soda/sodacl/sodacl_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/sodacl_parser.py` & `soda_core-3.3.5/soda/sodacl/sodacl_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import functools
+import inspect
 import logging
 import os
 import re
 from datetime import timedelta
 from numbers import Number
 from textwrap import dedent
 from typing import List
@@ -615,14 +616,15 @@
         name = None
         filter = None
         method = None
         missing_and_valid_cfg = None
         condition = None
         metric_expression = None
         metric_query = None
+        failed_rows_query = None
         samples_limit = None
         samples_columns = None
         training_dataset_params: TrainingDatasetParameters = TrainingDatasetParameters()
         model_cfg: ModelConfigs = ModelConfigs()
         take_over_existing_anomaly_score_check = False
         severity_level_params: SeverityLevelParameters = SeverityLevelParameters()
 
@@ -653,14 +655,21 @@
                             else None
                         )
                         if configuration_metric_name != metric_name:
                             self.logs.error(
                                 f'In configuration "{configuration_key}" the metric name must match exactly the metric name in the check "{metric_name}"',
                                 location=self.location,
                             )
+                elif configuration_key == "failed rows query" or configuration_key == "failed rows sql_file":
+                    if configuration_key.endswith("sql_file"):
+                        fs = file_system()
+                        sql_file_path = fs.join(fs.dirname(self.path_stack.file_path), configuration_value.strip())
+                        failed_rows_query = dedent(fs.file_read_as_str(sql_file_path)).strip()
+                    else:
+                        failed_rows_query = dedent(configuration_value).strip()
                 elif configuration_key.endswith("query") or configuration_key.endswith("sql_file"):
                     if configuration_key.endswith("sql_file"):
                         fs = file_system()
                         sql_file_path = fs.join(fs.dirname(self.path_stack.file_path), configuration_value.strip())
                         metric_query = dedent(fs.file_read_as_str(sql_file_path)).strip()
                         configuration_metric_name = (
                             configuration_key[: -len(" sql_file")]
@@ -914,32 +923,47 @@
             and len(metric_args) > 1
             and metric_name not in MetricCheckCfg.MULTI_METRIC_CHECK_TYPES
         ):
             self.logs.warning(
                 f"Invalid syntax used in '{check_str}'. More than one check attribute is not supported. A check like this will be skipped in future versions of Soda Core"
             )
 
-        return metric_check_cfg_class(
-            source_header=header_str,
-            source_line=check_str,
-            source_configurations=check_configurations,
-            location=self.location,
-            name=name,
-            metric_name=metric_name,
-            metric_args=metric_args,
-            missing_and_valid_cfg=missing_and_valid_cfg,
-            filter=filter,
-            condition=condition,
-            metric_expression=metric_expression,
-            metric_query=metric_query,
-            change_over_time_cfg=change_over_time_cfg,
-            fail_threshold_cfg=fail_threshold_cfg,
-            warn_threshold_cfg=warn_threshold_cfg,
-            samples_limit=samples_limit,
-        )
+        def takes_keyword_argument(cls, keyword):
+            signature = inspect.signature(cls.__init__)
+            return keyword in signature.parameters
+
+        # Some arguments make no sense for certain metric checks, so we only pass the ones that are supported by the given class constructor.
+        # Do this instead of accepting kwargs and passing all arguments to the constructor, because it's easier to see what arguments are supported and they do not disappear in the constructor.
+        all_args = {
+            "source_header": header_str,
+            "source_line": check_str,
+            "source_configurations": check_configurations,
+            "location": self.location,
+            "name": name,
+            "metric_name": metric_name,
+            "metric_args": metric_args,
+            "missing_and_valid_cfg": missing_and_valid_cfg,
+            "filter": filter,
+            "condition": condition,
+            "metric_expression": metric_expression,
+            "metric_query": metric_query,
+            "change_over_time_cfg": change_over_time_cfg,
+            "fail_threshold_cfg": fail_threshold_cfg,
+            "warn_threshold_cfg": warn_threshold_cfg,
+            "samples_limit": samples_limit,
+            "failed_rows_query": failed_rows_query,
+        }
+
+        use_args = {}
+
+        for arg in all_args.keys():
+            if takes_keyword_argument(metric_check_cfg_class, arg):
+                use_args[arg] = all_args[arg]
+
+        return metric_check_cfg_class(**use_args)
 
     def __parse_configuration_threshold_condition(self, value) -> ThresholdCfg | None:
         if isinstance(value, str):
             if not value.startswith("when "):
                 self.logs.error(
                     'Value for fail must be "when {condition}"',
                     location=self.location,
```

### Comparing `soda_core-3.3.4/soda/sodacl/table_cfg.py` & `soda_core-3.3.5/soda/sodacl/table_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/threshold_cfg.py` & `soda_core-3.3.5/soda/sodacl/threshold_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/user_defined_failed_rows_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/user_defined_failed_rows_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py` & `soda_core-3.3.5/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/telemetry/memory_span_exporter.py` & `soda_core-3.3.5/soda/telemetry/memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/telemetry/soda_exporter.py` & `soda_core-3.3.5/soda/telemetry/soda_exporter.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/telemetry/soda_telemetry.py` & `soda_core-3.3.5/soda/telemetry/soda_telemetry.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda/telemetry/soda_tracer.py` & `soda_core-3.3.5/soda/telemetry/soda_tracer.py`

 * *Files identical despite different names*

### Comparing `soda_core-3.3.4/soda_core.egg-info/PKG-INFO` & `soda_core-3.3.5/soda_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-core
-Version: 3.3.4
+Version: 3.3.5
 Summary: Soda Core library & CLI
 Author: Soda Data N.V.
 Author-email: info@soda.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `soda_core-3.3.4/soda_core.egg-info/SOURCES.txt` & `soda_core-3.3.5/soda_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

