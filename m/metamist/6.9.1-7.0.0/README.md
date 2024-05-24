# Comparing `tmp/metamist-6.9.1.tar.gz` & `tmp/metamist-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-6.9.1.tar", last modified: Wed Apr 24 00:46:18 2024, max compression
+gzip compressed data, was "metamist-7.0.0.tar", last modified: Thu May 23 05:05:21 2024, max compression
```

## Comparing `metamist-6.9.1.tar` & `metamist-7.0.0.tar`

### file list

```diff
@@ -1,157 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.965452 metamist-6.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 00:41:25.000000 metamist-6.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 00:41:25.000000 metamist-6.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-24 00:46:18.965452 metamist-6.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-24 00:41:25.000000 metamist-6.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.945452 metamist-6.9.1/metamist/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.949452 metamist-6.9.1/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56280 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/analysis_runner_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23776 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    82010 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/billing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    51702 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28817 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47701 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    33023 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53117 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    47305 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18676 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.949452 metamist-6.9.1/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.949452 metamist-6.9.1/metamist/audit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/audit/audit_upload_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/audit/audithelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/audit/delete_assay_files_from_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/audit/generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.949452 metamist-6.9.1/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-24 00:44:23.000000 metamist-6.9.1/metamist/graphql/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.957452 metamist-6.9.1/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15388 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    13839 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_batch_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_cromwell_subworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_cromwell_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_seq_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_sku.py
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_total.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_cost_record_wdl_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    12972 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/assay.py
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/billing_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/billing_cost_budget_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/billing_cost_details_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/billing_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/billing_time_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/billing_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/billing_total_cost_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15404 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/billing_total_cost_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/body_get_assays_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/body_get_proportionate_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/family_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)    13138 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13524 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    16516 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/project_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/proportional_date_temporal_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14319 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12051 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/seqr_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/sequencing_group_meta_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/sequencing_group_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.957452 metamist-6.9.1/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.957452 metamist-6.9.1/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    55508 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-04-24 00:41:25.000000 metamist-6.9.1/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-04-24 00:44:11.000000 metamist-6.9.1/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.945452 metamist-6.9.1/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-24 00:46:18.000000 metamist-6.9.1/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-24 00:46:18.000000 metamist-6.9.1/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:46:18.000000 metamist-6.9.1/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 00:46:18.000000 metamist-6.9.1/metamist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:46:18.000000 metamist-6.9.1/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 00:46:18.000000 metamist-6.9.1/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 00:46:18.000000 metamist-6.9.1/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-24 00:41:25.000000 metamist-6.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:46:18.965452 metamist-6.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-24 00:41:25.000000 metamist-6.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:46:18.965452 metamist-6.9.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_analysis_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_api_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_audit_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_bq_billing_ar_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    32213 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_bq_billing_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_bq_billing_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_bq_billing_daily_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_bq_billing_gcp_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_bq_billing_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_bq_function_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_bq_generic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_generic_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_layers_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_metamist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    32146 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_project_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_update_participant_family.py
--rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19073 2024-04-24 00:41:25.000000 metamist-6.9.1/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-24 00:41:25.000000 metamist-6.9.1/test/testbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-24 00:41:25.000000 metamist-6.9.1/test/testbqbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.818431 metamist-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 05:02:20.000000 metamist-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 05:02:20.000000 metamist-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-23 05:05:21.818431 metamist-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-23 05:02:20.000000 metamist-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.798431 metamist-7.0.0/metamist/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.802431 metamist-7.0.0/metamist/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56146 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/analysis_runner_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/assay_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82373 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/billing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/cohort_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50382 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/enums_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29264 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48033 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32909 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/sequencing_group_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.802431 metamist-7.0.0/metamist/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.802431 metamist-7.0.0/metamist/audit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/audit_upload_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/audithelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/delete_assay_files_from_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.802431 metamist-7.0.0/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-23 05:03:55.000000 metamist-7.0.0/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.814431 metamist-7.0.0/metamist/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_batch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_cromwell_subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_cromwell_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_seq_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_sku.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_wdl_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13856 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15657 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/assay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/assay_query_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/assay_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_cost_budget_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_cost_details_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_time_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_total_cost_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_total_cost_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/body_create_cohort_from_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/body_get_proportionate_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/cohort_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/cohort_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/cohort_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/family.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/family_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/get_samples_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/nested_sequencing_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/new_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/project_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/proportional_date_temporal_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/query_participant_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sample_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/seqr_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sequencing_group_meta_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sequencing_group_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sequencing_group_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.814431 metamist-7.0.0/metamist/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.814431 metamist-7.0.0/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55508 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.798431 metamist-7.0.0/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-23 05:02:20.000000 metamist-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 05:05:21.818431 metamist-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-23 05:02:20.000000 metamist-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.818431 metamist-7.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_analysis_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_api_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_ar_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32213 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_daily_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_gcp_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_function_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_generic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18895 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_cohort_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_layers_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_metamist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32146 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_project_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_update_participant_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-23 05:02:20.000000 metamist-7.0.0/test/testbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 05:02:20.000000 metamist-7.0.0/test/testbqbase.py
```

### Comparing `metamist-6.9.1/LICENSE` & `metamist-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/PKG-INFO` & `metamist-7.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.9.1
+Version: 7.0.0
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/metamist
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -52,17 +52,17 @@
 
 3. **Installable Python Library**: Wraps the Python Web API using the OpenAPI generator, facilitating easier interaction with the system.
 
 ### Schema
 
 As of Jan 15, 2024 this schema should reflect the data structure on the tables:
 
-![Database Structure](resources/2024-01-15_db-diagram.png)
+![Database Structure](resources/schemav7.7.png)
 
-You can also find this at [DbDiagram](https://dbdiagram.io/d/Metamist-Schema-v6-6-2-65a48ac7ac844320aee60d16).
+You can also find this at [DbDiagram](https://dbdiagram.io/d/Metamist-Schema-v7-7-6600c875ae072629ced6a1fc).
 
 The codebase contains the following modules worth noting:
 
 - `models` -> General data models + enums
 - `db/python/tables` -> Interaction with MariaDB / BigQuery
 - `db/python/layers` -> Logic
 - `api/graphql` : GraphQL
```

### Comparing `metamist-6.9.1/README.md` & `metamist-7.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 
 3. **Installable Python Library**: Wraps the Python Web API using the OpenAPI generator, facilitating easier interaction with the system.
 
 ### Schema
 
 As of Jan 15, 2024 this schema should reflect the data structure on the tables:
 
-![Database Structure](resources/2024-01-15_db-diagram.png)
+![Database Structure](resources/schemav7.7.png)
 
-You can also find this at [DbDiagram](https://dbdiagram.io/d/Metamist-Schema-v6-6-2-65a48ac7ac844320aee60d16).
+You can also find this at [DbDiagram](https://dbdiagram.io/d/Metamist-Schema-v7-7-6600c875ae072629ced6a1fc).
 
 The codebase contains the following modules worth noting:
 
 - `models` -> General data models + enums
 - `db/python/tables` -> Interaction with MariaDB / BigQuery
 - `db/python/layers` -> Logic
 - `api/graphql` : GraphQL
```

### Comparing `metamist-6.9.1/metamist/__init__.py` & `metamist-7.0.0/metamist/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `metamist-6.9.1/metamist/api/analysis_api.py` & `metamist-7.0.0/metamist/api/analysis_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -19,14 +19,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
 from metamist.model.analysis import Analysis
+from metamist.model.analysis_internal import AnalysisInternal
 from metamist.model.analysis_query_model import AnalysisQueryModel
 from metamist.model.analysis_update_model import AnalysisUpdateModel
 from metamist.model.body_get_latest_complete_analysis_for_type_post import BodyGetLatestCompleteAnalysisForTypePost
 from metamist.model.body_get_proportionate_map import BodyGetProportionateMap
 from metamist.model.http_validation_error import HTTPValidationError
 
 
@@ -213,15 +214,15 @@
             },
             api_client=api_client
         )
 
         self.get_analysis_runner_log_async = async_wrap(self.get_analysis_runner_log)
         self.get_analysis_runner_log_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([AnalysisInternal],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/analysis/analysis-runner',
                 'operation_id': 'get_analysis_runner_log',
                 'http_method': 'GET',
                 'servers': None,
@@ -636,15 +637,15 @@
             },
             api_client=api_client
         )
 
         self.update_analysis_async = async_wrap(self.update_analysis)
         self.update_analysis_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': (bool,),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/analysis/{analysis_id}/',
                 'operation_id': 'update_analysis',
                 'http_method': 'PATCH',
                 'servers': None,
@@ -956,15 +957,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [AnalysisInternal]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1472,15 +1473,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            bool
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.9.1/metamist/api/analysis_runner_api.py` & `metamist-7.0.0/metamist/api/analysis_runner_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,14 +18,15 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
+from metamist.model.analysis_runner import AnalysisRunner
 from metamist.model.http_validation_error import HTTPValidationError
 
 
 class AnalysisRunnerApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -36,15 +37,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         self.create_analysis_runner_log_async = async_wrap(self.create_analysis_runner_log)
         self.create_analysis_runner_log_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': (str,),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/analysis-runner/{project}/',
                 'operation_id': 'create_analysis_runner_log',
                 'http_method': 'PUT',
                 'servers': None,
@@ -81,14 +82,16 @@
                     'environment',
                     'batch_url',
                     'submitting_user',
                     'output_path',
                     'request_body',
                 ],
                 'nullable': [
+                    'hail_version',
+                    'cwd',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -122,17 +125,17 @@
                     'submitting_user':
                         (str,),
                     'output_path':
                         (str,),
                     'request_body':
                         ({str: (str,)},),
                     'hail_version':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'cwd':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'ar_guid': 'ar_guid',
                     'access_level': 'access_level',
                     'repository': 'repository',
                     'commit': 'commit',
@@ -178,15 +181,15 @@
             },
             api_client=api_client
         )
 
         self.get_analysis_runner_logs_async = async_wrap(self.get_analysis_runner_logs)
         self.get_analysis_runner_logs_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([AnalysisRunner],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/analysis-runner/{project}/',
                 'operation_id': 'get_analysis_runner_logs',
                 'http_method': 'GET',
                 'servers': None,
@@ -200,14 +203,19 @@
                     'access_level',
                     'environment',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
+                    'ar_guid',
+                    'submitting_user',
+                    'repository',
+                    'access_level',
+                    'environment',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -215,23 +223,23 @@
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'ar_guid':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'submitting_user':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'repository':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'access_level':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'environment':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'ar_guid': 'ar_guid',
                     'submitting_user': 'submitting_user',
                     'repository': 'repository',
                     'access_level': 'access_level',
@@ -297,16 +305,16 @@
             environment (str):
             batch_url (str):
             submitting_user (str):
             output_path (str):
             request_body ({str: (str,)}):
 
         Keyword Args:
-            hail_version (str): [optional]
-            cwd (str): [optional]
+            hail_version (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            cwd (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -323,15 +331,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -396,19 +404,19 @@
         >>> thread = api.get_analysis_runner_logs(project, async_req=True)
         >>> result = thread.get()
 
         Args:
             project (str):
 
         Keyword Args:
-            ar_guid (str): [optional]
-            submitting_user (str): [optional]
-            repository (str): [optional]
-            access_level (str): [optional]
-            environment (str): [optional]
+            ar_guid (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            submitting_user (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            repository (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            access_level (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            environment (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -425,15 +433,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [AnalysisRunner]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.9.1/metamist/api/assay_api.py` & `metamist-7.0.0/metamist/api/assay_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,16 +18,16 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
+from metamist.model.assay_query_criteria import AssayQueryCriteria
 from metamist.model.assay_upsert import AssayUpsert
-from metamist.model.body_get_assays_by_criteria import BodyGetAssaysByCriteria
 from metamist.model.http_validation_error import HTTPValidationError
 
 
 class AssayApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -215,37 +215,39 @@
                 'endpoint_path': '/api/v1/assay/criteria',
                 'operation_id': 'get_assays_by_criteria',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'body_get_assays_by_criteria',
+                    'assay_query_criteria',
+                ],
+                'required': [
+                    'assay_query_criteria',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'body_get_assays_by_criteria':
-                        (BodyGetAssaysByCriteria,),
+                    'assay_query_criteria':
+                        (AssayQueryCriteria,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'body_get_assays_by_criteria': 'body',
+                    'assay_query_criteria': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -526,28 +528,30 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['assay_id'] = \
             assay_id
         return self.get_assay_by_id_endpoint.call_with_http_info(**kwargs)
 
     def get_assays_by_criteria(
         self,
+        assay_query_criteria,
         **kwargs
     ):
         """Get Assays By Criteria  # noqa: E501
 
         Get assays by criteria  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_assays_by_criteria(async_req=True)
+        >>> thread = api.get_assays_by_criteria(assay_query_criteria, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            assay_query_criteria (AssayQueryCriteria):
 
         Keyword Args:
-            body_get_assays_by_criteria (BodyGetAssaysByCriteria): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -589,14 +593,16 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['assay_query_criteria'] = \
+            assay_query_criteria
         return self.get_assays_by_criteria_endpoint.call_with_http_info(**kwargs)
 
     def update_assay(
         self,
         assay_upsert,
         **kwargs
     ):
```

### Comparing `metamist-6.9.1/metamist/api/billing_api.py` & `metamist-7.0.0/metamist/api/billing_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -21,15 +21,14 @@
     none_type,
     validate_and_convert_types,
     async_wrap
 )
 from metamist.model.analysis_cost_record import AnalysisCostRecord
 from metamist.model.billing_column import BillingColumn
 from metamist.model.billing_cost_budget_record import BillingCostBudgetRecord
-from metamist.model.billing_source import BillingSource
 from metamist.model.billing_total_cost_query_model import BillingTotalCostQueryModel
 from metamist.model.billing_total_cost_record import BillingTotalCostRecord
 from metamist.model.http_validation_error import HTTPValidationError
 
 
 class BillingApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -489,14 +488,16 @@
                     'invoice_month',
                     'source',
                 ],
                 'required': [
                     'field',
                 ],
                 'nullable': [
+                    'invoice_month',
+                    'source',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -504,17 +505,17 @@
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'field':
                         (BillingColumn,),
                     'invoice_month':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'source':
-                        (BillingSource,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'field': 'field',
                     'invoice_month': 'invoice_month',
                     'source': 'source',
                 },
                 'location_map': {
@@ -641,14 +642,15 @@
             params_map={
                 'all': [
                     'limit',
                     'offset',
                 ],
                 'required': [],
                 'nullable': [
+                    'offset',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -656,15 +658,15 @@
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'limit':
                         (int,),
                     'offset':
-                        (int,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'limit': 'limit',
                     'offset': 'offset',
                 },
                 'location_map': {
                     'limit': 'query',
@@ -1536,16 +1538,16 @@
         >>> thread = api.get_running_cost(field, async_req=True)
         >>> result = thread.get()
 
         Args:
             field (BillingColumn):
 
         Keyword Args:
-            invoice_month (str): [optional]
-            source (BillingSource): [optional]
+            invoice_month (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            source (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1739,15 +1741,15 @@
 
         >>> thread = api.get_skus(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
             limit (int): [optional] if omitted the server will use the default value of 10
-            offset (int): [optional]
+            offset (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `metamist-6.9.1/metamist/api/enums_api.py` & `metamist-7.0.0/metamist/api/enums_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -36,15 +36,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         self.get_analysis_types_async = async_wrap(self.get_analysis_types)
         self.get_analysis_types_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/analysis-type',
                 'operation_id': 'get_analysis_types',
                 'http_method': 'GET',
                 'servers': None,
@@ -82,15 +82,15 @@
             },
             api_client=api_client
         )
 
         self.get_assay_types_async = async_wrap(self.get_assay_types)
         self.get_assay_types_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/assay-type',
                 'operation_id': 'get_assay_types',
                 'http_method': 'GET',
                 'servers': None,
@@ -128,15 +128,15 @@
             },
             api_client=api_client
         )
 
         self.get_sample_types_async = async_wrap(self.get_sample_types)
         self.get_sample_types_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/sample-type',
                 'operation_id': 'get_sample_types',
                 'http_method': 'GET',
                 'servers': None,
@@ -174,15 +174,15 @@
             },
             api_client=api_client
         )
 
         self.get_sequencing_platforms_async = async_wrap(self.get_sequencing_platforms)
         self.get_sequencing_platforms_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/sequencing-platform',
                 'operation_id': 'get_sequencing_platforms',
                 'http_method': 'GET',
                 'servers': None,
@@ -220,15 +220,15 @@
             },
             api_client=api_client
         )
 
         self.get_sequencing_technologys_async = async_wrap(self.get_sequencing_technologys)
         self.get_sequencing_technologys_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/sequencing-technology',
                 'operation_id': 'get_sequencing_technologys',
                 'http_method': 'GET',
                 'servers': None,
@@ -266,15 +266,15 @@
             },
             api_client=api_client
         )
 
         self.get_sequencing_types_async = async_wrap(self.get_sequencing_types)
         self.get_sequencing_types_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/sequencing-type',
                 'operation_id': 'get_sequencing_types',
                 'http_method': 'GET',
                 'servers': None,
@@ -312,15 +312,15 @@
             },
             api_client=api_client
         )
 
         self.post_analysis_types_async = async_wrap(self.post_analysis_types)
         self.post_analysis_types_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/analysis-type',
                 'operation_id': 'post_analysis_types',
                 'http_method': 'POST',
                 'servers': None,
@@ -365,15 +365,15 @@
             },
             api_client=api_client
         )
 
         self.post_assay_types_async = async_wrap(self.post_assay_types)
         self.post_assay_types_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/assay-type',
                 'operation_id': 'post_assay_types',
                 'http_method': 'POST',
                 'servers': None,
@@ -418,15 +418,15 @@
             },
             api_client=api_client
         )
 
         self.post_sample_types_async = async_wrap(self.post_sample_types)
         self.post_sample_types_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/sample-type',
                 'operation_id': 'post_sample_types',
                 'http_method': 'POST',
                 'servers': None,
@@ -471,15 +471,15 @@
             },
             api_client=api_client
         )
 
         self.post_sequencing_platforms_async = async_wrap(self.post_sequencing_platforms)
         self.post_sequencing_platforms_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/sequencing-platform',
                 'operation_id': 'post_sequencing_platforms',
                 'http_method': 'POST',
                 'servers': None,
@@ -524,15 +524,15 @@
             },
             api_client=api_client
         )
 
         self.post_sequencing_technologys_async = async_wrap(self.post_sequencing_technologys)
         self.post_sequencing_technologys_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/sequencing-technology',
                 'operation_id': 'post_sequencing_technologys',
                 'http_method': 'POST',
                 'servers': None,
@@ -577,15 +577,15 @@
             },
             api_client=api_client
         )
 
         self.post_sequencing_types_async = async_wrap(self.post_sequencing_types)
         self.post_sequencing_types_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([str],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/enums/sequencing-type',
                 'operation_id': 'post_sequencing_types',
                 'http_method': 'POST',
                 'servers': None,
@@ -665,15 +665,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -730,15 +730,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -795,15 +795,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -860,15 +860,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -925,15 +925,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -990,15 +990,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1058,15 +1058,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1128,15 +1128,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1198,15 +1198,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1268,15 +1268,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1338,15 +1338,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -1408,15 +1408,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [str]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.9.1/metamist/api/family_api.py` & `metamist-7.0.0/metamist/api/family_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,14 +18,15 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
+from metamist.model.family import Family
 from metamist.model.family_update_model import FamilyUpdateModel
 from metamist.model.http_validation_error import HTTPValidationError
 
 
 class FamilyApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -37,15 +38,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         self.get_families_async = async_wrap(self.get_families)
         self.get_families_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([Family],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/family/{project}/',
                 'operation_id': 'get_families',
                 'http_method': 'GET',
                 'servers': None,
@@ -56,14 +57,16 @@
                     'participant_ids',
                     'sample_ids',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
+                    'participant_ids',
+                    'sample_ids',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -71,31 +74,29 @@
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'participant_ids':
-                        ([int],),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'sample_ids':
-                        ([str],),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'participant_ids': 'participant_ids',
                     'sample_ids': 'sample_ids',
                 },
                 'location_map': {
                     'project': 'path',
                     'participant_ids': 'query',
                     'sample_ids': 'query',
                 },
                 'collection_format_map': {
-                    'participant_ids': 'multi',
-                    'sample_ids': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
@@ -126,14 +127,15 @@
                     'empty_participant_value',
                     'include_participants_not_in_families',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
+                    'empty_participant_value',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -151,15 +153,15 @@
                     'replace_with_participant_external_ids':
                         (bool,),
                     'replace_with_family_external_ids':
                         (bool,),
                     'include_header':
                         (bool,),
                     'empty_participant_value':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'include_participants_not_in_families':
                         (bool,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'internal_family_ids': 'internal_family_ids',
                     'export_type': 'export_type',
@@ -212,14 +214,15 @@
                     'delimiter',
                 ],
                 'required': [
                     'project',
                     'file',
                 ],
                 'nullable': [
+                    'delimiter',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -231,15 +234,15 @@
                     'project':
                         (str,),
                     'file':
                         (file_type,),
                     'has_header':
                         (bool,),
                     'delimiter':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'file': 'file',
                     'has_header': 'has_header',
                     'delimiter': 'delimiter',
                 },
@@ -407,16 +410,16 @@
         >>> thread = api.get_families(project, async_req=True)
         >>> result = thread.get()
 
         Args:
             project (str):
 
         Keyword Args:
-            participant_ids ([int]): [optional]
-            sample_ids ([str]): [optional]
+            participant_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -433,15 +436,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [Family]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -485,15 +488,15 @@
 
         Keyword Args:
             internal_family_ids ([int]): [optional]
             export_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             replace_with_participant_external_ids (bool): [optional] if omitted the server will use the default value of True
             replace_with_family_external_ids (bool): [optional] if omitted the server will use the default value of True
             include_header (bool): [optional] if omitted the server will use the default value of True
-            empty_participant_value (str): [optional]
+            empty_participant_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             include_participants_not_in_families (bool): [optional] if omitted the server will use the default value of False
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -561,15 +564,15 @@
 
         Args:
             project (str):
             file (file_type):
 
         Keyword Args:
             has_header (bool): [optional] if omitted the server will use the default value of True
-            delimiter (str): [optional]
+            delimiter (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `metamist-6.9.1/metamist/api/import_api.py` & `metamist-7.0.0/metamist/api/import_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -57,14 +57,15 @@
                     'extra_participants_method',
                 ],
                 'required': [
                     'project',
                     'file',
                 ],
                 'nullable': [
+                    'delimiter',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -74,15 +75,15 @@
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'file':
                         (file_type,),
                     'delimiter':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'extra_participants_method':
                         (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'file': 'file',
                     'delimiter': 'delimiter',
@@ -124,15 +125,15 @@
         >>> result = thread.get()
 
         Args:
             project (str):
             file (file_type):
 
         Keyword Args:
-            delimiter (str): [optional]
+            delimiter (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             extra_participants_method (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
```

### Comparing `metamist-6.9.1/metamist/api/participant_api.py` & `metamist-7.0.0/metamist/api/participant_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,17 +18,17 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
-from metamist.model.body_get_participants import BodyGetParticipants
 from metamist.model.http_validation_error import HTTPValidationError
 from metamist.model.participant_upsert import ParticipantUpsert
+from metamist.model.query_participant_criteria import QueryParticipantCriteria
 
 
 class ParticipantApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -179,14 +179,15 @@
                     'external_participant_ids',
                     'replace_with_participant_external_ids',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
+                    'external_participant_ids',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -196,15 +197,15 @@
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'export_type':
                         (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'external_participant_ids':
-                        ([str],),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'replace_with_participant_external_ids':
                         (bool,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'export_type': 'export_type',
                     'external_participant_ids': 'external_participant_ids',
@@ -213,15 +214,14 @@
                 'location_map': {
                     'project': 'path',
                     'export_type': 'query',
                     'external_participant_ids': 'query',
                     'replace_with_participant_external_ids': 'query',
                 },
                 'collection_format_map': {
-                    'external_participant_ids': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
@@ -305,18 +305,19 @@
                 'operation_id': 'get_participants',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'project',
-                    'body_get_participants',
+                    'query_participant_criteria',
                 ],
                 'required': [
                     'project',
+                    'query_participant_criteria',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -325,23 +326,23 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'project':
                         (str,),
-                    'body_get_participants':
-                        (BodyGetParticipants,),
+                    'query_participant_criteria':
+                        (QueryParticipantCriteria,),
                 },
                 'attribute_map': {
                     'project': 'project',
                 },
                 'location_map': {
                     'project': 'path',
-                    'body_get_participants': 'body',
+                    'query_participant_criteria': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -752,15 +753,15 @@
         >>> result = thread.get()
 
         Args:
             project (str):
 
         Keyword Args:
             export_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
-            external_participant_ids ([str]): [optional]
+            external_participant_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             replace_with_participant_external_ids (bool): [optional] if omitted the server will use the default value of True
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -886,30 +887,31 @@
         kwargs['request_body'] = \
             request_body
         return self.get_participant_id_map_by_external_ids_endpoint.call_with_http_info(**kwargs)
 
     def get_participants(
         self,
         project,
+        query_participant_criteria,
         **kwargs
     ):
         """Get Participants  # noqa: E501
 
         Get participants, default ALL participants in project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_participants(project, async_req=True)
+        >>> thread = api.get_participants(project, query_participant_criteria, async_req=True)
         >>> result = thread.get()
 
         Args:
             project (str):
+            query_participant_criteria (QueryParticipantCriteria):
 
         Keyword Args:
-            body_get_participants (BodyGetParticipants): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -953,14 +955,16 @@
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['project'] = \
             project
+        kwargs['query_participant_criteria'] = \
+            query_participant_criteria
         return self.get_participants_endpoint.call_with_http_info(**kwargs)
 
     def update_many_participants(
         self,
         request_body,
         **kwargs
     ):
```

### Comparing `metamist-6.9.1/metamist/api/project_api.py` & `metamist-7.0.0/metamist/api/project_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -37,15 +37,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         self.create_project_async = async_wrap(self.create_project)
         self.create_project_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': (int,),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/project/',
                 'operation_id': 'create_project',
                 'http_method': 'PUT',
                 'servers': None,
@@ -465,15 +465,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            int
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.9.1/metamist/api/sample_api.py` & `metamist-7.0.0/metamist/api/sample_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,15 +18,15 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
-from metamist.model.body_get_samples import BodyGetSamples
+from metamist.model.get_samples_criteria import GetSamplesCriteria
 from metamist.model.http_validation_error import HTTPValidationError
 from metamist.model.sample_upsert import SampleUpsert
 
 
 class SampleApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -393,37 +393,39 @@
                 'endpoint_path': '/api/v1/sample/',
                 'operation_id': 'get_samples',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'body_get_samples',
+                    'get_samples_criteria',
+                ],
+                'required': [
+                    'get_samples_criteria',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'body_get_samples':
-                        (BodyGetSamples,),
+                    'get_samples_criteria':
+                        (GetSamplesCriteria,),
                 },
                 'attribute_map': {
                 },
                 'location_map': {
-                    'body_get_samples': 'body',
+                    'get_samples_criteria': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -1105,28 +1107,30 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['request_body'] = \
             request_body
         return self.get_sample_id_map_by_internal_endpoint.call_with_http_info(**kwargs)
 
     def get_samples(
         self,
+        get_samples_criteria,
         **kwargs
     ):
         """Get Samples  # noqa: E501
 
         Get list of samples (dict) by some mixture of (AND'd) criteria  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_samples(async_req=True)
+        >>> thread = api.get_samples(get_samples_criteria, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            get_samples_criteria (GetSamplesCriteria):
 
         Keyword Args:
-            body_get_samples (BodyGetSamples): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1168,14 +1172,16 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['get_samples_criteria'] = \
+            get_samples_criteria
         return self.get_samples_endpoint.call_with_http_info(**kwargs)
 
     def get_samples_create_date(
         self,
         request_body,
         **kwargs
     ):
```

### Comparing `metamist-6.9.1/metamist/api/seqr_api.py` & `metamist-7.0.0/metamist/api/seqr_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,14 +18,15 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
+from metamist.model.family import Family
 from metamist.model.http_validation_error import HTTPValidationError
 
 
 class SeqrApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -104,15 +105,15 @@
             },
             api_client=api_client
         )
 
         self.get_families_async = async_wrap(self.get_families)
         self.get_families_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ([Family],),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/family/{project}/',
                 'operation_id': 'get_families',
                 'http_method': 'GET',
                 'servers': None,
@@ -123,14 +124,16 @@
                     'participant_ids',
                     'sample_ids',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
+                    'participant_ids',
+                    'sample_ids',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -138,31 +141,29 @@
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'participant_ids':
-                        ([int],),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'sample_ids':
-                        ([str],),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'participant_ids': 'participant_ids',
                     'sample_ids': 'sample_ids',
                 },
                 'location_map': {
                     'project': 'path',
                     'participant_ids': 'query',
                     'sample_ids': 'query',
                 },
                 'collection_format_map': {
-                    'participant_ids': 'multi',
-                    'sample_ids': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
@@ -189,14 +190,15 @@
                     'external_participant_ids',
                     'replace_with_participant_external_ids',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
+                    'external_participant_ids',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -206,15 +208,15 @@
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'export_type':
                         (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'external_participant_ids':
-                        ([str],),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'replace_with_participant_external_ids':
                         (bool,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'export_type': 'export_type',
                     'external_participant_ids': 'external_participant_ids',
@@ -223,15 +225,14 @@
                 'location_map': {
                     'project': 'path',
                     'export_type': 'query',
                     'external_participant_ids': 'query',
                     'replace_with_participant_external_ids': 'query',
                 },
                 'collection_format_map': {
-                    'external_participant_ids': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
@@ -262,14 +263,15 @@
                     'empty_participant_value',
                     'include_participants_not_in_families',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
+                    'empty_participant_value',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -287,15 +289,15 @@
                     'replace_with_participant_external_ids':
                         (bool,),
                     'replace_with_family_external_ids':
                         (bool,),
                     'include_header':
                         (bool,),
                     'empty_participant_value':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'include_participants_not_in_families':
                         (bool,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'internal_family_ids': 'internal_family_ids',
                     'export_type': 'export_type',
@@ -412,14 +414,15 @@
                     'delimiter',
                 ],
                 'required': [
                     'project',
                     'file',
                 ],
                 'nullable': [
+                    'delimiter',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -431,15 +434,15 @@
                     'project':
                         (str,),
                     'file':
                         (file_type,),
                     'has_header':
                         (bool,),
                     'delimiter':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'file': 'file',
                     'has_header': 'has_header',
                     'delimiter': 'delimiter',
                 },
@@ -483,14 +486,15 @@
                     'extra_participants_method',
                 ],
                 'required': [
                     'project',
                     'file',
                 ],
                 'nullable': [
+                    'delimiter',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -500,15 +504,15 @@
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'file':
                         (file_type,),
                     'delimiter':
-                        (str,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                     'extra_participants_method':
                         (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'file': 'file',
                     'delimiter': 'delimiter',
@@ -698,16 +702,16 @@
         >>> thread = api.get_families(project, async_req=True)
         >>> result = thread.get()
 
         Args:
             project (str):
 
         Keyword Args:
-            participant_ids ([int]): [optional]
-            sample_ids ([str]): [optional]
+            participant_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
+            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -724,15 +728,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            [Family]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -772,15 +776,15 @@
         >>> result = thread.get()
 
         Args:
             project (str):
 
         Keyword Args:
             export_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
-            external_participant_ids ([str]): [optional]
+            external_participant_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             replace_with_participant_external_ids (bool): [optional] if omitted the server will use the default value of True
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -850,15 +854,15 @@
 
         Keyword Args:
             internal_family_ids ([int]): [optional]
             export_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             replace_with_participant_external_ids (bool): [optional] if omitted the server will use the default value of True
             replace_with_family_external_ids (bool): [optional] if omitted the server will use the default value of True
             include_header (bool): [optional] if omitted the server will use the default value of True
-            empty_participant_value (str): [optional]
+            empty_participant_value (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             include_participants_not_in_families (bool): [optional] if omitted the server will use the default value of False
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -999,15 +1003,15 @@
 
         Args:
             project (str):
             file (file_type):
 
         Keyword Args:
             has_header (bool): [optional] if omitted the server will use the default value of True
-            delimiter (str): [optional]
+            delimiter (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1075,15 +1079,15 @@
         >>> result = thread.get()
 
         Args:
             project (str):
             file (file_type):
 
         Keyword Args:
-            delimiter (str): [optional]
+            delimiter (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             extra_participants_method (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
```

### Comparing `metamist-6.9.1/metamist/api/sequencing_group_api.py` & `metamist-7.0.0/metamist/api/sequencing_group_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -37,15 +37,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         self.get_all_sequencing_group_ids_by_sample_by_type_async = async_wrap(self.get_all_sequencing_group_ids_by_sample_by_type)
         self.get_all_sequencing_group_ids_by_sample_by_type_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': ({str: ({str: ([str],)},)},),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/sequencing-group/project/{project}',
                 'operation_id': 'get_all_sequencing_group_ids_by_sample_by_type',
                 'http_method': 'GET',
                 'servers': None,
@@ -90,15 +90,15 @@
             },
             api_client=api_client
         )
 
         self.get_sequencing_group_async = async_wrap(self.get_sequencing_group)
         self.get_sequencing_group_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': (str,),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/sequencing-group{sequencing_group_id}',
                 'operation_id': 'get_sequencing_group',
                 'http_method': 'GET',
                 'servers': None,
@@ -143,15 +143,15 @@
             },
             api_client=api_client
         )
 
         self.update_sequencing_group_async = async_wrap(self.update_sequencing_group)
         self.update_sequencing_group_endpoint = _Endpoint(
             settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'response_type': (bool,),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/sequencing-group/project/{sequencing_group_id}',
                 'operation_id': 'update_sequencing_group',
                 'http_method': 'PATCH',
                 'servers': None,
@@ -248,15 +248,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            {str: ({str: ([str],)},)}
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -319,15 +319,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -394,15 +394,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
+            bool
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.9.1/metamist/api/web_api.py` & `metamist-7.0.0/metamist/api/web_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -61,14 +61,15 @@
                     'token',
                 ],
                 'required': [
                     'project',
                     'search_item',
                 ],
                 'nullable': [
+                    'token',
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
@@ -80,15 +81,15 @@
                     'project':
                         (str,),
                     'search_item':
                         ([SearchItem],),
                     'limit':
                         (int,),
                     'token':
-                        (int,),
+                        (bool, date, datetime, dict, float, int, list, str, none_type,),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'limit': 'limit',
                     'token': 'token',
                 },
                 'location_map': {
@@ -282,15 +283,15 @@
 
         Args:
             project (str):
             search_item ([SearchItem]):
 
         Keyword Args:
             limit (int): [optional] if omitted the server will use the default value of 20
-            token (int): [optional] if omitted the server will use the default value of 0
+            token (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `metamist-6.9.1/metamist/api_client.py` & `metamist-7.0.0/metamist/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `metamist-6.9.1/metamist/apis/__init__.py` & `metamist-7.0.0/metamist/apis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from metamist.api.analysis_api import AnalysisApi
 from metamist.api.analysis_runner_api import AnalysisRunnerApi
 from metamist.api.assay_api import AssayApi
 from metamist.api.billing_api import BillingApi
+from metamist.api.cohort_api import CohortApi
 from metamist.api.enums_api import EnumsApi
 from metamist.api.family_api import FamilyApi
 from metamist.api.import_api import ImportApi
 from metamist.api.participant_api import ParticipantApi
 from metamist.api.project_api import ProjectApi
 from metamist.api.sample_api import SampleApi
 from metamist.api.seqr_api import SeqrApi
```

### Comparing `metamist-6.9.1/metamist/audit/audit_upload_bucket.py` & `metamist-7.0.0/metamist/audit/audit_upload_bucket.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/metamist/audit/audithelper.py` & `metamist-7.0.0/metamist/audit/audithelper.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/metamist/audit/delete_assay_files_from_audit.py` & `metamist-7.0.0/metamist/audit/delete_assay_files_from_audit.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/metamist/audit/generic_auditor.py` & `metamist-7.0.0/metamist/audit/generic_auditor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/metamist/configuration.py` & `metamist-7.0.0/metamist/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -405,15 +405,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.9.1\n"\
+               "Version of the API: 7.0.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `metamist-6.9.1/metamist/exceptions.py` & `metamist-7.0.0/metamist/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `metamist-6.9.1/metamist/graphql/__init__.py` & `metamist-7.0.0/metamist/graphql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,18 @@
 
     (client or configure_sync_client(use_local_schema=use_local_schema)).validate(doc)
     return True
 
 
 # use older style typing to broaden supported Python versions
 @backoff.on_exception(
-    backoff.expo,
+    backoff.fibo,
     exception=(HTTPError, JSONDecodeError, TransportServerError),
-    max_time=10,
+    max_time=55,
+    max_value=55
 )
 def query(
     _query: str | DocumentNode,
     variables: Dict | None = None,
     client: Client | None = None,
     log_response: bool = False,
 ) -> Dict[str, Any]:
```

### Comparing `metamist-6.9.1/metamist/graphql/schema.graphql` & `metamist-7.0.0/metamist/graphql/schema.graphql`

 * *Files 12% similar despite different names*

```diff
@@ -11,49 +11,71 @@
   eq: AnalysisStatus = null
   in_: [AnalysisStatus!] = null
   nin: [AnalysisStatus!] = null
   gt: AnalysisStatus = null
   gte: AnalysisStatus = null
   lt: AnalysisStatus = null
   lte: AnalysisStatus = null
+  contains: AnalysisStatus = null
+  icontains: AnalysisStatus = null
 }
 
 """Filter for GraphQL queries"""
 input BoolGraphQLFilter {
   eq: Boolean = null
   in_: [Boolean!] = null
   nin: [Boolean!] = null
   gt: Boolean = null
   gte: Boolean = null
   lt: Boolean = null
   lte: Boolean = null
+  contains: Boolean = null
+  icontains: Boolean = null
+}
+
+"""Date (isoformat)"""
+scalar Date
+
+"""Filter for GraphQL queries"""
+input DateGraphQLFilter {
+  eq: Date = null
+  in_: [Date!] = null
+  nin: [Date!] = null
+  gt: Date = null
+  gte: Date = null
+  lt: Date = null
+  lte: Date = null
+  contains: Date = null
+  icontains: Date = null
 }
 
 """Date with time (isoformat)"""
 scalar DateTime
 
 """Filter for GraphQL queries"""
 input DatetimeGraphQLFilter {
   eq: DateTime = null
   in_: [DateTime!] = null
   nin: [DateTime!] = null
   gt: DateTime = null
   gte: DateTime = null
   lt: DateTime = null
   lte: DateTime = null
+  contains: DateTime = null
+  icontains: DateTime = null
 }
 
 type GraphQLAnalysis {
   id: Int!
   type: String!
   status: AnalysisStatus!
   output: String
   timestampCompleted: DateTime
   active: Boolean!
-  meta: JSON!
+  meta: JSON
   sequencingGroups: [GraphQLSequencingGroup!]!
   project: GraphQLProject!
   auditLogs: [GraphQLAuditLog!]!
 }
 
 type GraphQLAnalysisRunner {
   arGuid: String!
@@ -61,15 +83,15 @@
   timestamp: DateTime!
   accessLevel: String!
   repository: String!
   commit: String!
   script: String!
   description: String!
   driverImage: String!
-  configPath: String!
+  configPath: String
   cwd: String
   environment: String!
   hailVersion: String
   batchUrl: String!
   submittingUser: String!
   meta: JSON!
   project: GraphQLProject!
@@ -88,14 +110,32 @@
   author: String!
   timestamp: DateTime!
   arGuid: String
   comment: String
   meta: JSON!
 }
 
+type GraphQLCohort {
+  id: String!
+  name: String!
+  description: String!
+  author: String!
+  template: GraphQLCohortTemplate!
+  sequencingGroups: [GraphQLSequencingGroup!]!
+  analyses: [GraphQLAnalysis!]!
+  project: GraphQLProject!
+}
+
+type GraphQLCohortTemplate {
+  id: String!
+  name: String!
+  description: String!
+  criteria: JSON!
+}
+
 type GraphQLEnum {
   analysisType: [String!]!
   assayType: [String!]!
   sampleType: [String!]!
   sequencingPlatform: [String!]!
   sequencingTechnology: [String!]!
   sequencingType: [String!]!
@@ -104,52 +144,62 @@
 type GraphQLFamily {
   id: Int!
   externalId: String!
   description: String
   codedPhenotype: String
   project: GraphQLProject!
   participants: [GraphQLParticipant!]!
+  familyParticipants: [GraphQLFamilyParticipant!]!
+}
+
+type GraphQLFamilyParticipant {
+  affected: Int
+  notes: String
+  participant: GraphQLParticipant!
+  family: GraphQLFamily!
 }
 
 type GraphQLParticipant {
   id: Int!
   externalId: String!
   meta: JSON!
   reportedSex: Int
   reportedGender: String
   karyotype: String
   samples(type: StrGraphQLFilter = null, meta: JSON = null, active: BoolGraphQLFilter = null): [GraphQLSample!]!
   phenotypes: JSON!
   families: [GraphQLFamily!]!
+  familyParticipants: [GraphQLFamilyParticipant!]!
   project: GraphQLProject!
   auditLog: GraphQLAuditLog
 }
 
 type GraphQLProject {
   id: Int!
   name: String!
   dataset: String!
   meta: JSON!
   analysisRunner(arGuid: StrGraphQLFilter = null, author: StrGraphQLFilter = null, repository: StrGraphQLFilter = null, accessLevel: StrGraphQLFilter = null, environment: StrGraphQLFilter = null): [GraphQLAnalysisRunner!]!
   pedigree(internalFamilyIds: [Int!] = null, replaceWithParticipantExternalIds: Boolean! = true, replaceWithFamilyExternalIds: Boolean! = true, includeParticipantsNotInFamilies: Boolean! = false, emptyParticipantValue: String = null): [JSON!]!
-  families: [GraphQLFamily!]!
+  families(id: IntGraphQLFilter = null, externalId: StrGraphQLFilter = null): [GraphQLFamily!]!
   participants: [GraphQLParticipant!]!
   samples(type: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, id: StrGraphQLFilter = null, meta: JSON = null): [GraphQLSample!]!
   sequencingGroups(id: StrGraphQLFilter = null, externalId: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
   analyses(type: StrGraphQLFilter = null, status: AnalysisStatusGraphQLFilter = null, active: BoolGraphQLFilter = null, meta: JSON = null, timestampCompleted: DatetimeGraphQLFilter = null): [GraphQLAnalysis!]!
+  cohorts(id: IntGraphQLFilter = null, name: StrGraphQLFilter = null, author: StrGraphQLFilter = null, templateId: IntGraphQLFilter = null, timestamp: DatetimeGraphQLFilter = null): [GraphQLCohort!]!
 }
 
 type GraphQLSample {
   id: String!
   externalId: String!
   active: Boolean!
   meta: JSON!
   type: String!
   participant: GraphQLParticipant
-  assays(type: StrGraphQLFilter = null): [GraphQLAssay!]!
+  assays(type: StrGraphQLFilter = null, meta: JSON = null): [GraphQLAssay!]!
   project: GraphQLProject!
   sequencingGroups(id: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, meta: JSON = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
 }
 
 type GraphQLSequencingGroup {
   id: String!
   type: String!
@@ -167,26 +217,30 @@
   eq: Int = null
   in_: [Int!] = null
   nin: [Int!] = null
   gt: Int = null
   gte: Int = null
   lt: Int = null
   lte: Int = null
+  contains: Int = null
+  icontains: Int = null
 }
 
 """
-The `JSON` scalar type represents JSON values as specified by [ECMA-404](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf).
+The `JSON` scalar type represents JSON values as specified by [ECMA-404](https://ecma-international.org/wp-content/uploads/ECMA-404_2nd_edition_december_2017.pdf).
 """
-scalar JSON @specifiedBy(url: "http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf")
+scalar JSON @specifiedBy(url: "https://ecma-international.org/wp-content/uploads/ECMA-404_2nd_edition_december_2017.pdf")
 
 type Query {
   enum: GraphQLEnum!
+  cohortTemplates(id: StrGraphQLFilter = null, project: StrGraphQLFilter = null): [GraphQLCohortTemplate!]!
+  cohorts(id: StrGraphQLFilter = null, project: StrGraphQLFilter = null, name: StrGraphQLFilter = null, author: StrGraphQLFilter = null, templateId: IntGraphQLFilter = null): [GraphQLCohort!]!
   project(name: String!): GraphQLProject!
   sample(id: StrGraphQLFilter = null, project: StrGraphQLFilter = null, type: StrGraphQLFilter = null, meta: JSON = null, externalId: StrGraphQLFilter = null, participantId: IntGraphQLFilter = null, active: BoolGraphQLFilter = null): [GraphQLSample!]!
-  sequencingGroups(id: StrGraphQLFilter = null, project: StrGraphQLFilter = null, sampleId: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, activeOnly: BoolGraphQLFilter = null): [GraphQLSequencingGroup!]!
+  sequencingGroups(id: StrGraphQLFilter = null, project: StrGraphQLFilter = null, sampleId: StrGraphQLFilter = null, type: StrGraphQLFilter = null, technology: StrGraphQLFilter = null, platform: StrGraphQLFilter = null, activeOnly: BoolGraphQLFilter = null, createdOn: DateGraphQLFilter = null, assayMeta: JSON = null, hasCram: Boolean = null, hasGvcf: Boolean = null): [GraphQLSequencingGroup!]!
   assay(id: Int!): GraphQLAssay!
   participant(id: Int!): GraphQLParticipant!
   family(familyId: Int!): GraphQLFamily!
   myProjects: [GraphQLProject!]!
   analysisRunner(arGuid: String!): GraphQLAnalysisRunner!
 }
 
@@ -195,8 +249,10 @@
   eq: String = null
   in_: [String!] = null
   nin: [String!] = null
   gt: String = null
   gte: String = null
   lt: String = null
   lte: String = null
+  contains: String = null
+  icontains: String = null
 }
```

### Comparing `metamist-6.9.1/metamist/model/analysis.py` & `metamist-7.0.0/metamist/model/nested_participant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,19 +26,21 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from metamist.model.analysis_status import AnalysisStatus
-    globals()['AnalysisStatus'] = AnalysisStatus
+    from metamist.model.family_simple import FamilySimple
+    from metamist.model.nested_sample import NestedSample
+    globals()['FamilySimple'] = FamilySimple
+    globals()['NestedSample'] = NestedSample
 
 
-class Analysis(ModelNormal):
+class NestedParticipant(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,22 +62,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -83,57 +78,55 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'status': (AnalysisStatus,),  # noqa: E501
             'id': (int,),  # noqa: E501
-            'output': (str,),  # noqa: E501
-            'sequencing_group_ids': ([str],),  # noqa: E501
-            'author': (str,),  # noqa: E501
-            'timestamp_completed': (str,),  # noqa: E501
-            'project': (int,),  # noqa: E501
-            'active': (bool,),  # noqa: E501
             'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'samples': ([NestedSample],),  # noqa: E501
+            'families': ([FamilySimple],),  # noqa: E501
+            'external_id': (str,),  # noqa: E501
+            'reported_sex': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'reported_gender': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'karyotype': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'output': 'output',  # noqa: E501
-        'sequencing_group_ids': 'sequencing_group_ids',  # noqa: E501
-        'author': 'author',  # noqa: E501
-        'timestamp_completed': 'timestamp_completed',  # noqa: E501
-        'project': 'project',  # noqa: E501
-        'active': 'active',  # noqa: E501
         'meta': 'meta',  # noqa: E501
+        'samples': 'samples',  # noqa: E501
+        'families': 'families',  # noqa: E501
+        'external_id': 'external_id',  # noqa: E501
+        'reported_sex': 'reported_sex',  # noqa: E501
+        'reported_gender': 'reported_gender',  # noqa: E501
+        'karyotype': 'karyotype',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, status, *args, **kwargs):  # noqa: E501
-        """Analysis - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, meta, samples, families, *args, **kwargs):  # noqa: E501
+        """NestedParticipant - a model defined in OpenAPI
 
         Args:
-            type (str):
-            status (AnalysisStatus):
+            id (int):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            samples ([NestedSample]):
+            families ([FamilySimple]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -158,22 +151,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            output (str): [optional]  # noqa: E501
-            sequencing_group_ids ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
-            author (str): [optional]  # noqa: E501
-            timestamp_completed (str): [optional]  # noqa: E501
-            project (int): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
+            external_id (str): [optional]  # noqa: E501
+            reported_sex (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            reported_gender (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            karyotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -193,16 +182,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.status = status
+        self.id = id
+        self.meta = meta
+        self.samples = samples
+        self.families = families
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -215,20 +206,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, status, *args, **kwargs):  # noqa: E501
-        """Analysis - a model defined in OpenAPI
+    def __init__(self, id, meta, samples, families, *args, **kwargs):  # noqa: E501
+        """NestedParticipant - a model defined in OpenAPI
 
         Args:
-            type (str):
-            status (AnalysisStatus):
+            id (int):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            samples ([NestedSample]):
+            families ([FamilySimple]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,22 +246,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            output (str): [optional]  # noqa: E501
-            sequencing_group_ids ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
-            author (str): [optional]  # noqa: E501
-            timestamp_completed (str): [optional]  # noqa: E501
-            project (int): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional] if omitted the server will use the default value of {}  # noqa: E501
+            external_id (str): [optional]  # noqa: E501
+            reported_sex (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            reported_gender (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            karyotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -286,16 +275,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.status = status
+        self.id = id
+        self.meta = meta
+        self.samples = samples
+        self.families = families
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record.py` & `metamist-7.0.0/metamist/model/sample_upsert.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,36 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.analysis_cost_record_batch import AnalysisCostRecordBatch
-    from metamist.model.analysis_cost_record_category import AnalysisCostRecordCategory
-    from metamist.model.analysis_cost_record_cromwell_subworkflow import AnalysisCostRecordCromwellSubworkflow
-    from metamist.model.analysis_cost_record_cromwell_workflow import AnalysisCostRecordCromwellWorkflow
-    from metamist.model.analysis_cost_record_seq_group import AnalysisCostRecordSeqGroup
-    from metamist.model.analysis_cost_record_sku import AnalysisCostRecordSku
-    from metamist.model.analysis_cost_record_topic import AnalysisCostRecordTopic
-    from metamist.model.analysis_cost_record_total import AnalysisCostRecordTotal
-    from metamist.model.analysis_cost_record_wdl_task import AnalysisCostRecordWdlTask
-    globals()['AnalysisCostRecordBatch'] = AnalysisCostRecordBatch
-    globals()['AnalysisCostRecordCategory'] = AnalysisCostRecordCategory
-    globals()['AnalysisCostRecordCromwellSubworkflow'] = AnalysisCostRecordCromwellSubworkflow
-    globals()['AnalysisCostRecordCromwellWorkflow'] = AnalysisCostRecordCromwellWorkflow
-    globals()['AnalysisCostRecordSeqGroup'] = AnalysisCostRecordSeqGroup
-    globals()['AnalysisCostRecordSku'] = AnalysisCostRecordSku
-    globals()['AnalysisCostRecordTopic'] = AnalysisCostRecordTopic
-    globals()['AnalysisCostRecordTotal'] = AnalysisCostRecordTotal
-    globals()['AnalysisCostRecordWdlTask'] = AnalysisCostRecordWdlTask
 
-
-class AnalysisCostRecord(ModelNormal):
+class SampleUpsert(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,76 +56,66 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'total': (AnalysisCostRecordTotal,),  # noqa: E501
-            'topics': ([AnalysisCostRecordTopic],),  # noqa: E501
-            'categories': ([AnalysisCostRecordCategory],),  # noqa: E501
-            'batches': ([AnalysisCostRecordBatch],),  # noqa: E501
-            'skus': ([AnalysisCostRecordSku],),  # noqa: E501
-            'seq_groups': ([AnalysisCostRecordSeqGroup],),  # noqa: E501
-            'wdl_tasks': ([AnalysisCostRecordWdlTask],),  # noqa: E501
-            'cromwell_sub_workflows': ([AnalysisCostRecordCromwellSubworkflow],),  # noqa: E501
-            'cromwell_workflows': ([AnalysisCostRecordCromwellWorkflow],),  # noqa: E501
-            'dataproc': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'external_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'project': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'participant_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'active': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sequencing_groups': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'non_sequencing_assays': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'total': 'total',  # noqa: E501
-        'topics': 'topics',  # noqa: E501
-        'categories': 'categories',  # noqa: E501
-        'batches': 'batches',  # noqa: E501
-        'skus': 'skus',  # noqa: E501
-        'seq_groups': 'seq_groups',  # noqa: E501
-        'wdl_tasks': 'wdl_tasks',  # noqa: E501
-        'cromwell_sub_workflows': 'cromwell_sub_workflows',  # noqa: E501
-        'cromwell_workflows': 'cromwell_workflows',  # noqa: E501
-        'dataproc': 'dataproc',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'external_id': 'external_id',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
+        'project': 'project',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'participant_id': 'participant_id',  # noqa: E501
+        'active': 'active',  # noqa: E501
+        'sequencing_groups': 'sequencing_groups',  # noqa: E501
+        'non_sequencing_assays': 'non_sequencing_assays',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AnalysisCostRecord - a model defined in OpenAPI
+        """SampleUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -170,24 +140,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (AnalysisCostRecordTotal): [optional]  # noqa: E501
-            topics ([AnalysisCostRecordTopic]): [optional]  # noqa: E501
-            categories ([AnalysisCostRecordCategory]): [optional]  # noqa: E501
-            batches ([AnalysisCostRecordBatch]): [optional]  # noqa: E501
-            skus ([AnalysisCostRecordSku]): [optional]  # noqa: E501
-            seq_groups ([AnalysisCostRecordSeqGroup]): [optional]  # noqa: E501
-            wdl_tasks ([AnalysisCostRecordWdlTask]): [optional]  # noqa: E501
-            cromwell_sub_workflows ([AnalysisCostRecordCromwellSubworkflow]): [optional]  # noqa: E501
-            cromwell_workflows ([AnalysisCostRecordCromwellWorkflow]): [optional]  # noqa: E501
-            dataproc ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            project (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            participant_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sequencing_groups (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            non_sequencing_assays (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -228,15 +197,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AnalysisCostRecord - a model defined in OpenAPI
+        """SampleUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -261,24 +230,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            total (AnalysisCostRecordTotal): [optional]  # noqa: E501
-            topics ([AnalysisCostRecordTopic]): [optional]  # noqa: E501
-            categories ([AnalysisCostRecordCategory]): [optional]  # noqa: E501
-            batches ([AnalysisCostRecordBatch]): [optional]  # noqa: E501
-            skus ([AnalysisCostRecordSku]): [optional]  # noqa: E501
-            seq_groups ([AnalysisCostRecordSeqGroup]): [optional]  # noqa: E501
-            wdl_tasks ([AnalysisCostRecordWdlTask]): [optional]  # noqa: E501
-            cromwell_sub_workflows ([AnalysisCostRecordCromwellSubworkflow]): [optional]  # noqa: E501
-            cromwell_workflows ([AnalysisCostRecordCromwellWorkflow]): [optional]  # noqa: E501
-            dataproc ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            project (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            participant_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sequencing_groups (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            non_sequencing_assays (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_batch.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_batch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -64,22 +64,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -88,53 +81,54 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'batch_id': (str,),  # noqa: E501
+            'batch_name': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'cost': (float,),  # noqa: E501
             'usage_start_time': (datetime,),  # noqa: E501
             'usage_end_time': (datetime,),  # noqa: E501
             'jobs_cnt': (int,),  # noqa: E501
             'skus': ([AnalysisCostRecordSku],),  # noqa: E501
             'jobs': ([AnalysisCostRecordBatchJob],),  # noqa: E501
             'seq_groups': ([AnalysisCostRecordSeqGroup],),  # noqa: E501
-            'batch_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'batch_id': 'batch_id',  # noqa: E501
+        'batch_name': 'batch_name',  # noqa: E501
         'cost': 'cost',  # noqa: E501
         'usage_start_time': 'usage_start_time',  # noqa: E501
         'usage_end_time': 'usage_end_time',  # noqa: E501
         'jobs_cnt': 'jobs_cnt',  # noqa: E501
         'skus': 'skus',  # noqa: E501
         'jobs': 'jobs',  # noqa: E501
         'seq_groups': 'seq_groups',  # noqa: E501
-        'batch_name': 'batch_name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, batch_id, cost, usage_start_time, usage_end_time, jobs_cnt, skus, jobs, seq_groups, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, batch_id, batch_name, cost, usage_start_time, usage_end_time, jobs_cnt, skus, jobs, seq_groups, *args, **kwargs):  # noqa: E501
         """AnalysisCostRecordBatch - a model defined in OpenAPI
 
         Args:
             batch_id (str):
+            batch_name (bool, date, datetime, dict, float, int, list, str, none_type):
             cost (float):
             usage_start_time (datetime):
             usage_end_time (datetime):
             jobs_cnt (int):
             skus ([AnalysisCostRecordSku]):
             jobs ([AnalysisCostRecordBatchJob]):
             seq_groups ([AnalysisCostRecordSeqGroup]):
@@ -166,15 +160,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            batch_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,14 +188,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.batch_id = batch_id
+        self.batch_name = batch_name
         self.cost = cost
         self.usage_start_time = usage_start_time
         self.usage_end_time = usage_end_time
         self.jobs_cnt = jobs_cnt
         self.skus = skus
         self.jobs = jobs
         self.seq_groups = seq_groups
@@ -222,19 +216,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, batch_id, cost, usage_start_time, usage_end_time, jobs_cnt, skus, jobs, seq_groups, *args, **kwargs):  # noqa: E501
+    def __init__(self, batch_id, batch_name, cost, usage_start_time, usage_end_time, jobs_cnt, skus, jobs, seq_groups, *args, **kwargs):  # noqa: E501
         """AnalysisCostRecordBatch - a model defined in OpenAPI
 
         Args:
             batch_id (str):
+            batch_name (bool, date, datetime, dict, float, int, list, str, none_type):
             cost (float):
             usage_start_time (datetime):
             usage_end_time (datetime):
             jobs_cnt (int):
             skus ([AnalysisCostRecordSku]):
             jobs ([AnalysisCostRecordBatchJob]):
             seq_groups ([AnalysisCostRecordSeqGroup]):
@@ -266,15 +261,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            batch_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -293,14 +287,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.batch_id = batch_id
+        self.batch_name = batch_name
         self.cost = cost
         self.usage_start_time = usage_start_time
         self.usage_end_time = usage_end_time
         self.jobs_cnt = jobs_cnt
         self.skus = skus
         self.jobs = jobs
         self.seq_groups = seq_groups
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_batch_job.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_batch_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -84,47 +77,48 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'job_id': (str,),  # noqa: E501
+            'job_name': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'skus': ([AnalysisCostRecordSku],),  # noqa: E501
             'cost': (float,),  # noqa: E501
             'usage_start_time': (datetime,),  # noqa: E501
             'usage_end_time': (datetime,),  # noqa: E501
-            'job_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'job_id': 'job_id',  # noqa: E501
+        'job_name': 'job_name',  # noqa: E501
         'skus': 'skus',  # noqa: E501
         'cost': 'cost',  # noqa: E501
         'usage_start_time': 'usage_start_time',  # noqa: E501
         'usage_end_time': 'usage_end_time',  # noqa: E501
-        'job_name': 'job_name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, job_id, skus, cost, usage_start_time, usage_end_time, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, job_id, job_name, skus, cost, usage_start_time, usage_end_time, *args, **kwargs):  # noqa: E501
         """AnalysisCostRecordBatchJob - a model defined in OpenAPI
 
         Args:
             job_id (str):
+            job_name (bool, date, datetime, dict, float, int, list, str, none_type):
             skus ([AnalysisCostRecordSku]):
             cost (float):
             usage_start_time (datetime):
             usage_end_time (datetime):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -153,15 +147,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            job_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,14 +175,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.job_id = job_id
+        self.job_name = job_name
         self.skus = skus
         self.cost = cost
         self.usage_start_time = usage_start_time
         self.usage_end_time = usage_end_time
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
@@ -206,19 +200,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, job_id, skus, cost, usage_start_time, usage_end_time, *args, **kwargs):  # noqa: E501
+    def __init__(self, job_id, job_name, skus, cost, usage_start_time, usage_end_time, *args, **kwargs):  # noqa: E501
         """AnalysisCostRecordBatchJob - a model defined in OpenAPI
 
         Args:
             job_id (str):
+            job_name (bool, date, datetime, dict, float, int, list, str, none_type):
             skus ([AnalysisCostRecordSku]):
             cost (float):
             usage_start_time (datetime):
             usage_end_time (datetime):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -247,15 +242,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            job_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -274,14 +268,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.job_id = job_id
+        self.job_name = job_name
         self.skus = skus
         self.cost = cost
         self.usage_start_time = usage_start_time
         self.usage_end_time = usage_end_time
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_category.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_category.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -79,15 +73,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'category': (str,),  # noqa: E501
             'cost': (float,),  # noqa: E501
-            'workflows': (int,),  # noqa: E501
+            'workflows': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -100,20 +94,21 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, category, cost, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, category, cost, workflows, *args, **kwargs):  # noqa: E501
         """AnalysisCostRecordCategory - a model defined in OpenAPI
 
         Args:
             category (str):
             cost (float):
+            workflows (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +133,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            workflows (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,14 +162,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.category = category
         self.cost = cost
+        self.workflows = workflows
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -188,20 +183,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, category, cost, *args, **kwargs):  # noqa: E501
+    def __init__(self, category, cost, workflows, *args, **kwargs):  # noqa: E501
         """AnalysisCostRecordCategory - a model defined in OpenAPI
 
         Args:
             category (str):
             cost (float):
+            workflows (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +222,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            workflows (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -254,14 +249,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.category = category
         self.cost = cost
+        self.workflows = workflows
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_cromwell_subworkflow.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_cromwell_subworkflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_cromwell_workflow.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_cromwell_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_seq_group.py` & `metamist-7.0.0/metamist/model/web_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class AnalysisCostRecordSeqGroup(ModelNormal):
+class WebProject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,63 +56,62 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'cost': (float,),  # noqa: E501
-            'sequencing_group': (str,),  # noqa: E501
-            'stage': (str,),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'dataset': (str,),  # noqa: E501
+            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'cost': 'cost',  # noqa: E501
-        'sequencing_group': 'sequencing_group',  # noqa: E501
-        'stage': 'stage',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'dataset': 'dataset',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, cost, *args, **kwargs):  # noqa: E501
-        """AnalysisCostRecordSeqGroup - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
+        """WebProject - a model defined in OpenAPI
 
         Args:
-            cost (float):
+            id (int):
+            name (str):
+            dataset (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,16 +136,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sequencing_group (str): [optional]  # noqa: E501
-            stage (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -166,15 +163,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.cost = cost
+        self.id = id
+        self.name = name
+        self.dataset = dataset
+        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -187,19 +187,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, cost, *args, **kwargs):  # noqa: E501
-        """AnalysisCostRecordSeqGroup - a model defined in OpenAPI
+    def __init__(self, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
+        """WebProject - a model defined in OpenAPI
 
         Args:
-            cost (float):
+            id (int):
+            name (str):
+            dataset (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +227,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sequencing_group (str): [optional]  # noqa: E501
-            stage (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,15 +252,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.cost = cost
+        self.id = id
+        self.name = name
+        self.dataset = dataset
+        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_sku.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_sku.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_topic.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_topic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_total.py` & `metamist-7.0.0/metamist/model/assay.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class AnalysisCostRecordTotal(ModelNormal):
+class Assay(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,62 +56,65 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'ar_guid': (str,),  # noqa: E501
-            'cost': (float,),  # noqa: E501
-            'usage_start_time': (datetime,),  # noqa: E501
-            'usage_end_time': (datetime,),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'external_ids': ({str: (str,)},),  # noqa: E501
+            'sample_id': (str,),  # noqa: E501
+            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'ar_guid': 'ar_guid',  # noqa: E501
-        'cost': 'cost',  # noqa: E501
-        'usage_start_time': 'usage_start_time',  # noqa: E501
-        'usage_end_time': 'usage_end_time',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'external_ids': 'external_ids',  # noqa: E501
+        'sample_id': 'sample_id',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AnalysisCostRecordTotal - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, external_ids, sample_id, meta, type, *args, **kwargs):  # noqa: E501
+        """Assay - a model defined in OpenAPI
+
+        Args:
+            id (int):
+            external_ids ({str: (str,)}):
+            sample_id (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,18 +139,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ar_guid (str): [optional]  # noqa: E501
-            cost (float): [optional]  # noqa: E501
-            usage_start_time (datetime): [optional]  # noqa: E501
-            usage_end_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -167,14 +166,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.external_ids = external_ids
+        self.sample_id = sample_id
+        self.meta = meta
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -187,16 +191,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """AnalysisCostRecordTotal - a model defined in OpenAPI
+    def __init__(self, id, external_ids, sample_id, meta, type, *args, **kwargs):  # noqa: E501
+        """Assay - a model defined in OpenAPI
+
+        Args:
+            id (int):
+            external_ids ({str: (str,)}):
+            sample_id (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,18 +232,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ar_guid (str): [optional]  # noqa: E501
-            cost (float): [optional]  # noqa: E501
-            usage_start_time (datetime): [optional]  # noqa: E501
-            usage_end_time (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -250,14 +257,19 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.external_ids = external_ids
+        self.sample_id = sample_id
+        self.meta = meta
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/analysis_cost_record_wdl_task.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_wdl_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/analysis_query_model.py` & `metamist-7.0.0/metamist/model/assay_upsert.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.analysis_status import AnalysisStatus
-    globals()['AnalysisStatus'] = AnalysisStatus
 
-
-class AnalysisQueryModel(ModelNormal):
+class AssayUpsert(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,75 +56,58 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'projects': ([str],),  # noqa: E501
-            'sample_ids': ([str],),  # noqa: E501
-            'sequencing_group_ids': ([str],),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'status': (AnalysisStatus,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'output': (str,),  # noqa: E501
-            'active': (bool,),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'external_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sample_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'projects': 'projects',  # noqa: E501
-        'sample_ids': 'sample_ids',  # noqa: E501
-        'sequencing_group_ids': 'sequencing_group_ids',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'status': 'status',  # noqa: E501
+        'external_ids': 'external_ids',  # noqa: E501
+        'sample_id': 'sample_id',  # noqa: E501
         'meta': 'meta',  # noqa: E501
-        'output': 'output',  # noqa: E501
-        'active': 'active',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, projects, *args, **kwargs):  # noqa: E501
-        """AnalysisQueryModel - a model defined in OpenAPI
-
-        Args:
-            projects ([str]):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """AssayUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,21 +132,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sample_ids ([str]): [optional]  # noqa: E501
-            sequencing_group_ids ([str]): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            status (AnalysisStatus): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            output (str): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +164,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.projects = projects
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -208,19 +184,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, projects, *args, **kwargs):  # noqa: E501
-        """AnalysisQueryModel - a model defined in OpenAPI
-
-        Args:
-            projects ([str]):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """AssayUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -245,21 +218,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sample_ids ([str]): [optional]  # noqa: E501
-            sequencing_group_ids ([str]): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            status (AnalysisStatus): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            output (str): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -277,15 +248,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.projects = projects
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/analysis_status.py` & `metamist-7.0.0/metamist/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/analysis_update_model.py` & `metamist-7.0.0/metamist/model/analysis_update_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -84,17 +84,17 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'status': (AnalysisStatus,),  # noqa: E501
-            'output': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'active': (bool,),  # noqa: E501
+            'output': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'active': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -145,17 +145,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            output (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
+            output (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -233,17 +233,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            output (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
+            output (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/assay.py` & `metamist-7.0.0/metamist/model/new_cohort.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class Assay(ModelNormal):
+class NewCohort(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,71 +56,58 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (int,),  # noqa: E501
-            'external_ids': ({str: (str,)},),  # noqa: E501
-            'sample_id': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'type': (str,),  # noqa: E501
+            'cohort_id': (str,),  # noqa: E501
+            'sequencing_group_ids': ([str],),  # noqa: E501
+            'dry_run': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'external_ids': 'external_ids',  # noqa: E501
-        'sample_id': 'sample_id',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'cohort_id': 'cohort_id',  # noqa: E501
+        'sequencing_group_ids': 'sequencing_group_ids',  # noqa: E501
+        'dry_run': 'dry_run',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, external_ids, sample_id, meta, type, *args, **kwargs):  # noqa: E501
-        """Assay - a model defined in OpenAPI
+    def _from_openapi_data(cls, cohort_id, sequencing_group_ids, *args, **kwargs):  # noqa: E501
+        """NewCohort - a model defined in OpenAPI
 
         Args:
-            id (int):
-            external_ids ({str: (str,)}):
-            sample_id (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
-            type (str):
+            cohort_id (str):
+            sequencing_group_ids ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,14 +132,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            dry_run (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -172,19 +160,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.external_ids = external_ids
-        self.sample_id = sample_id
-        self.meta = meta
-        self.type = type
+        self.cohort_id = cohort_id
+        self.sequencing_group_ids = sequencing_group_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -197,23 +182,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, external_ids, sample_id, meta, type, *args, **kwargs):  # noqa: E501
-        """Assay - a model defined in OpenAPI
+    def __init__(self, cohort_id, sequencing_group_ids, *args, **kwargs):  # noqa: E501
+        """NewCohort - a model defined in OpenAPI
 
         Args:
-            id (int):
-            external_ids ({str: (str,)}):
-            sample_id (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
-            type (str):
+            cohort_id (str):
+            sequencing_group_ids ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -238,14 +220,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            dry_run (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -263,19 +246,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.external_ids = external_ids
-        self.sample_id = sample_id
-        self.meta = meta
-        self.type = type
+        self.cohort_id = cohort_id
+        self.sequencing_group_ids = sequencing_group_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/assay_upsert.py` & `metamist-7.0.0/metamist/model/get_samples_criteria.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class AssayUpsert(ModelNormal):
+class GetSamplesCriteria(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,64 +56,58 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'external_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'sample_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sample_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'participant_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'project_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'active': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'external_ids': 'external_ids',  # noqa: E501
-        'sample_id': 'sample_id',  # noqa: E501
+        'sample_ids': 'sample_ids',  # noqa: E501
         'meta': 'meta',  # noqa: E501
+        'participant_ids': 'participant_ids',  # noqa: E501
+        'project_ids': 'project_ids',  # noqa: E501
+        'active': 'active',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AssayUpsert - a model defined in OpenAPI
+        """GetSamplesCriteria - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,19 +132,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            external_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            sample_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            participant_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            project_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            active (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +185,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AssayUpsert - a model defined in OpenAPI
+        """GetSamplesCriteria - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,19 +218,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            external_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            sample_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            participant_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            project_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            active (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/billing_column.py` & `metamist-7.0.0/metamist/model/billing_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/billing_cost_budget_record.py` & `metamist-7.0.0/metamist/model/billing_cost_details_record.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.billing_cost_details_record import BillingCostDetailsRecord
-    globals()['BillingCostDetailsRecord'] = BillingCostDetailsRecord
 
-
-class BillingCostBudgetRecord(ModelNormal):
+class BillingCostDetailsRecord(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,78 +56,62 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'field': (str,),  # noqa: E501
-            'total_monthly': (float,),  # noqa: E501
-            'total_daily': (float,),  # noqa: E501
-            'compute_monthly': (float,),  # noqa: E501
-            'compute_daily': (float,),  # noqa: E501
-            'storage_monthly': (float,),  # noqa: E501
-            'storage_daily': (float,),  # noqa: E501
-            'details': ([BillingCostDetailsRecord],),  # noqa: E501
-            'budget_spent': (float,),  # noqa: E501
-            'budget': (float,),  # noqa: E501
-            'last_loaded_day': (str,),  # noqa: E501
+            'cost_group': (str,),  # noqa: E501
+            'cost_category': (str,),  # noqa: E501
+            'daily_cost': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'monthly_cost': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'field': 'field',  # noqa: E501
-        'total_monthly': 'total_monthly',  # noqa: E501
-        'total_daily': 'total_daily',  # noqa: E501
-        'compute_monthly': 'compute_monthly',  # noqa: E501
-        'compute_daily': 'compute_daily',  # noqa: E501
-        'storage_monthly': 'storage_monthly',  # noqa: E501
-        'storage_daily': 'storage_daily',  # noqa: E501
-        'details': 'details',  # noqa: E501
-        'budget_spent': 'budget_spent',  # noqa: E501
-        'budget': 'budget',  # noqa: E501
-        'last_loaded_day': 'last_loaded_day',  # noqa: E501
+        'cost_group': 'cost_group',  # noqa: E501
+        'cost_category': 'cost_category',  # noqa: E501
+        'daily_cost': 'daily_cost',  # noqa: E501
+        'monthly_cost': 'monthly_cost',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BillingCostBudgetRecord - a model defined in OpenAPI
+    def _from_openapi_data(cls, cost_group, cost_category, daily_cost, monthly_cost, *args, **kwargs):  # noqa: E501
+        """BillingCostDetailsRecord - a model defined in OpenAPI
+
+        Args:
+            cost_group (str):
+            cost_category (str):
+            daily_cost (bool, date, datetime, dict, float, int, list, str, none_type):
+            monthly_cost (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -156,25 +136,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            field (str): [optional]  # noqa: E501
-            total_monthly (float): [optional]  # noqa: E501
-            total_daily (float): [optional]  # noqa: E501
-            compute_monthly (float): [optional]  # noqa: E501
-            compute_daily (float): [optional]  # noqa: E501
-            storage_monthly (float): [optional]  # noqa: E501
-            storage_daily (float): [optional]  # noqa: E501
-            details ([BillingCostDetailsRecord]): [optional]  # noqa: E501
-            budget_spent (float): [optional]  # noqa: E501
-            budget (float): [optional]  # noqa: E501
-            last_loaded_day (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -194,14 +163,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.cost_group = cost_group
+        self.cost_category = cost_category
+        self.daily_cost = daily_cost
+        self.monthly_cost = monthly_cost
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -214,16 +187,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """BillingCostBudgetRecord - a model defined in OpenAPI
+    def __init__(self, cost_group, cost_category, daily_cost, monthly_cost, *args, **kwargs):  # noqa: E501
+        """BillingCostDetailsRecord - a model defined in OpenAPI
+
+        Args:
+            cost_group (str):
+            cost_category (str):
+            daily_cost (bool, date, datetime, dict, float, int, list, str, none_type):
+            monthly_cost (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -248,25 +227,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            field (str): [optional]  # noqa: E501
-            total_monthly (float): [optional]  # noqa: E501
-            total_daily (float): [optional]  # noqa: E501
-            compute_monthly (float): [optional]  # noqa: E501
-            compute_daily (float): [optional]  # noqa: E501
-            storage_monthly (float): [optional]  # noqa: E501
-            storage_daily (float): [optional]  # noqa: E501
-            details ([BillingCostDetailsRecord]): [optional]  # noqa: E501
-            budget_spent (float): [optional]  # noqa: E501
-            budget (float): [optional]  # noqa: E501
-            last_loaded_day (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -284,14 +252,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.cost_group = cost_group
+        self.cost_category = cost_category
+        self.daily_cost = daily_cost
+        self.monthly_cost = monthly_cost
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/billing_cost_details_record.py` & `metamist-7.0.0/metamist/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class BillingCostDetailsRecord(ModelNormal):
+class BodyGetLatestCompleteAnalysisForTypePost(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,45 +77,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'cost_group': (str,),  # noqa: E501
-            'cost_category': (str,),  # noqa: E501
-            'daily_cost': (float,),  # noqa: E501
-            'monthly_cost': (float,),  # noqa: E501
+            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'cost_group': 'cost_group',  # noqa: E501
-        'cost_category': 'cost_category',  # noqa: E501
-        'daily_cost': 'daily_cost',  # noqa: E501
-        'monthly_cost': 'monthly_cost',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, cost_group, cost_category, *args, **kwargs):  # noqa: E501
-        """BillingCostDetailsRecord - a model defined in OpenAPI
+    def _from_openapi_data(cls, meta, *args, **kwargs):  # noqa: E501
+        """BodyGetLatestCompleteAnalysisForTypePost - a model defined in OpenAPI
 
         Args:
-            cost_group (str):
-            cost_category (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,16 +133,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            daily_cost (float): [optional]  # noqa: E501
-            monthly_cost (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -169,16 +160,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.cost_group = cost_group
-        self.cost_category = cost_category
+        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -191,20 +181,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, cost_group, cost_category, *args, **kwargs):  # noqa: E501
-        """BillingCostDetailsRecord - a model defined in OpenAPI
+    def __init__(self, meta, *args, **kwargs):  # noqa: E501
+        """BodyGetLatestCompleteAnalysisForTypePost - a model defined in OpenAPI
 
         Args:
-            cost_group (str):
-            cost_category (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -229,16 +218,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            daily_cost (float): [optional]  # noqa: E501
-            monthly_cost (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -256,16 +243,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.cost_group = cost_group
-        self.cost_category = cost_category
+        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/billing_source.py` & `metamist-7.0.0/metamist/model/billing_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/billing_time_column.py` & `metamist-7.0.0/metamist/model/billing_time_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/billing_time_periods.py` & `metamist-7.0.0/metamist/model/billing_time_periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/billing_total_cost_query_model.py` & `metamist-7.0.0/metamist/model/billing_total_cost_query_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,21 +27,15 @@
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from metamist.model.billing_column import BillingColumn
-    from metamist.model.billing_source import BillingSource
-    from metamist.model.billing_time_column import BillingTimeColumn
-    from metamist.model.billing_time_periods import BillingTimePeriods
     globals()['BillingColumn'] = BillingColumn
-    globals()['BillingSource'] = BillingSource
-    globals()['BillingTimeColumn'] = BillingTimeColumn
-    globals()['BillingTimePeriods'] = BillingTimePeriods
 
 
 class BillingTotalCostQueryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -66,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -92,24 +79,24 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'fields': ([BillingColumn],),  # noqa: E501
             'start_date': (str,),  # noqa: E501
             'end_date': (str,),  # noqa: E501
-            'source': (BillingSource,),  # noqa: E501
-            'filters': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'filters_op': (str,),  # noqa: E501
+            'source': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'filters': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'filters_op': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'group_by': (bool,),  # noqa: E501
-            'order_by': ({str: (bool,)},),  # noqa: E501
-            'limit': (int,),  # noqa: E501
-            'offset': (int,),  # noqa: E501
-            'time_column': (BillingTimeColumn,),  # noqa: E501
-            'time_periods': (BillingTimePeriods,),  # noqa: E501
-            'min_cost': (float,),  # noqa: E501
+            'order_by': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'limit': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'offset': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'time_column': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'time_periods': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'min_cost': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -171,24 +158,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            source (BillingSource): [optional]  # noqa: E501
-            filters ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            filters_op (str): [optional]  # noqa: E501
+            source (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            filters (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            filters_op (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             group_by (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
-            order_by ({str: (bool,)}): [optional]  # noqa: E501
-            limit (int): [optional]  # noqa: E501
-            offset (int): [optional]  # noqa: E501
-            time_column (BillingTimeColumn): [optional]  # noqa: E501
-            time_periods (BillingTimePeriods): [optional]  # noqa: E501
-            min_cost (float): [optional]  # noqa: E501
+            order_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            limit (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            offset (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            time_column (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            time_periods (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            min_cost (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -270,24 +257,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            source (BillingSource): [optional]  # noqa: E501
-            filters ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            filters_op (str): [optional]  # noqa: E501
+            source (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            filters (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            filters_op (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             group_by (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
-            order_by ({str: (bool,)}): [optional]  # noqa: E501
-            limit (int): [optional]  # noqa: E501
-            offset (int): [optional]  # noqa: E501
-            time_column (BillingTimeColumn): [optional]  # noqa: E501
-            time_periods (BillingTimePeriods): [optional]  # noqa: E501
-            min_cost (float): [optional]  # noqa: E501
+            order_by (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            limit (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            offset (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            time_column (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            time_periods (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            min_cost (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/body_get_assays_by_criteria.py` & `metamist-7.0.0/metamist/model/assay_query_criteria.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class BodyGetAssaysByCriteria(ModelNormal):
+class AssayQueryCriteria(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,42 +56,36 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'sample_ids': ([str],),  # noqa: E501
-            'assay_ids': ([int],),  # noqa: E501
-            'external_assay_ids': ([str],),  # noqa: E501
-            'assay_meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'sample_meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'projects': ([str],),  # noqa: E501
-            'assay_types': ([str],),  # noqa: E501
+            'sample_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'assay_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'external_assay_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'assay_meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sample_meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'projects': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'assay_types': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -109,15 +103,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BodyGetAssaysByCriteria - a model defined in OpenAPI
+        """AssayQueryCriteria - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,21 +136,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sample_ids ([str]): [optional]  # noqa: E501
-            assay_ids ([int]): [optional]  # noqa: E501
-            external_assay_ids ([str]): [optional]  # noqa: E501
-            assay_meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            sample_meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            projects ([str]): [optional]  # noqa: E501
-            assay_types ([str]): [optional]  # noqa: E501
+            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            assay_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_assay_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            assay_meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            projects (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            assay_types (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -197,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BodyGetAssaysByCriteria - a model defined in OpenAPI
+        """AssayQueryCriteria - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,21 +224,21 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sample_ids ([str]): [optional]  # noqa: E501
-            assay_ids ([int]): [optional]  # noqa: E501
-            external_assay_ids ([str]): [optional]  # noqa: E501
-            assay_meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            sample_meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            projects ([str]): [optional]  # noqa: E501
-            assay_types ([str]): [optional]  # noqa: E501
+            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            assay_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_assay_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            assay_meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            projects (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            assay_types (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/body_get_latest_complete_analysis_for_type_post.py` & `metamist-7.0.0/metamist/model/sequencing_group_meta_update_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class BodyGetLatestCompleteAnalysisForTypePost(ModelNormal):
+class SequencingGroupMetaUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,15 +77,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -96,19 +96,16 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, meta, *args, **kwargs):  # noqa: E501
-        """BodyGetLatestCompleteAnalysisForTypePost - a model defined in OpenAPI
-
-        Args:
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """SequencingGroupMetaUpdateModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,14 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -160,15 +158,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -181,19 +178,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, meta, *args, **kwargs):  # noqa: E501
-        """BodyGetLatestCompleteAnalysisForTypePost - a model defined in OpenAPI
-
-        Args:
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """SequencingGroupMetaUpdateModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,14 +212,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -243,15 +238,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/body_get_participants.py` & `metamist-7.0.0/metamist/model/paging_links.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class BodyGetParticipants(ModelNormal):
+class PagingLinks(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,58 +56,59 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'external_participant_ids': ([str],),  # noqa: E501
-            'internal_participant_ids': ([int],),  # noqa: E501
+            '_self': (str,),  # noqa: E501
+            'next': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'token': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'external_participant_ids': 'external_participant_ids',  # noqa: E501
-        'internal_participant_ids': 'internal_participant_ids',  # noqa: E501
+        '_self': 'self',  # noqa: E501
+        'next': 'next',  # noqa: E501
+        'token': 'token',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BodyGetParticipants - a model defined in OpenAPI
+    def _from_openapi_data(cls, _self, next, token, *args, **kwargs):  # noqa: E501
+        """PagingLinks - a model defined in OpenAPI
+
+        Args:
+            _self (str):
+            next (bool, date, datetime, dict, float, int, list, str, none_type):
+            token (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -132,16 +133,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            external_participant_ids ([str]): [optional]  # noqa: E501
-            internal_participant_ids ([int]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -161,14 +160,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self._self = _self
+        self.next = next
+        self.token = token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -181,16 +183,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """BodyGetParticipants - a model defined in OpenAPI
+    def __init__(self, _self, next, token, *args, **kwargs):  # noqa: E501
+        """PagingLinks - a model defined in OpenAPI
+
+        Args:
+            _self (str):
+            next (bool, date, datetime, dict, float, int, list, str, none_type):
+            token (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -215,16 +222,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            external_participant_ids ([str]): [optional]  # noqa: E501
-            internal_participant_ids ([int]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -242,14 +247,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self._self = _self
+        self.next = next
+        self.token = token
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/body_get_proportionate_map.py` & `metamist-7.0.0/metamist/model/body_get_proportionate_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -85,15 +85,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'projects': ([str],),  # noqa: E501
             'temporal_methods': ([ProportionalDateTemporalMethod],),  # noqa: E501
-            'sequencing_types': ([str],),  # noqa: E501
+            'sequencing_types': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -144,15 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sequencing_types ([str]): [optional]  # noqa: E501
+            sequencing_types (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -232,15 +232,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sequencing_types ([str]): [optional]  # noqa: E501
+            sequencing_types (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/body_get_samples.py` & `metamist-7.0.0/metamist/model/family_update_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class BodyGetSamples(ModelNormal):
+class FamilyUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,43 +77,44 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'sample_ids': ([str],),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'participant_ids': ([int],),  # noqa: E501
-            'project_ids': ([str],),  # noqa: E501
-            'active': (bool,),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'external_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'description': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'coded_phenotype': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'sample_ids': 'sample_ids',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
-        'participant_ids': 'participant_ids',  # noqa: E501
-        'project_ids': 'project_ids',  # noqa: E501
-        'active': 'active',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'external_id': 'external_id',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'coded_phenotype': 'coded_phenotype',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BodyGetSamples - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
+        """FamilyUpdateModel - a model defined in OpenAPI
+
+        Args:
+            id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,19 +139,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sample_ids ([str]): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            participant_ids ([int]): [optional]  # noqa: E501
-            project_ids ([str]): [optional]  # noqa: E501
-            active (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
+            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            description (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            coded_phenotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,14 +169,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,16 +190,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """BodyGetSamples - a model defined in OpenAPI
+    def __init__(self, id, *args, **kwargs):  # noqa: E501
+        """FamilyUpdateModel - a model defined in OpenAPI
+
+        Args:
+            id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,19 +227,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            sample_ids ([str]): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            participant_ids ([int]): [optional]  # noqa: E501
-            project_ids ([str]): [optional]  # noqa: E501
-            active (bool): [optional] if omitted the server will use the default value of True  # noqa: E501
+            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            description (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            coded_phenotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -254,14 +255,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/error_response.py` & `metamist-7.0.0/metamist/model/error_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/export_type.py` & `metamist-7.0.0/metamist/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/extra_participant_importer_handler.py` & `metamist-7.0.0/metamist/model/extra_participant_importer_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/family_search_response_data.py` & `metamist-7.0.0/metamist/model/family_search_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/family_simple.py` & `metamist-7.0.0/metamist/model/family_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/family_update_model.py` & `metamist-7.0.0/metamist/model/http_validation_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from metamist.model.validation_error import ValidationError
+    globals()['ValidationError'] = ValidationError
 
-class FamilyUpdateModel(ModelNormal):
+
+class HTTPValidationError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,59 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (int,),  # noqa: E501
-            'external_id': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
-            'coded_phenotype': (str,),  # noqa: E501
+            'detail': ([ValidationError],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'external_id': 'external_id',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'coded_phenotype': 'coded_phenotype',  # noqa: E501
+        'detail': 'detail',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, *args, **kwargs):  # noqa: E501
-        """FamilyUpdateModel - a model defined in OpenAPI
-
-        Args:
-            id (int):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """HTTPValidationError - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,17 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            external_id (str): [optional]  # noqa: E501
-            description (str): [optional]  # noqa: E501
-            coded_phenotype (str): [optional]  # noqa: E501
+            detail ([ValidationError]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -169,15 +164,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,19 +184,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, *args, **kwargs):  # noqa: E501
-        """FamilyUpdateModel - a model defined in OpenAPI
-
-        Args:
-            id (int):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """HTTPValidationError - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,17 +218,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            external_id (str): [optional]  # noqa: E501
-            description (str): [optional]  # noqa: E501
-            coded_phenotype (str): [optional]  # noqa: E501
+            detail ([ValidationError]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -255,15 +244,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/http_validation_error.py` & `metamist-7.0.0/metamist/model/cohort_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,19 +26,19 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from metamist.model.validation_error import ValidationError
-    globals()['ValidationError'] = ValidationError
+    from metamist.model.cohort_criteria import CohortCriteria
+    globals()['CohortCriteria'] = CohortCriteria
 
 
-class HTTPValidationError(ModelNormal):
+class CohortTemplate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -83,35 +76,47 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'detail': ([ValidationError],),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'criteria': (CohortCriteria,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'detail': 'detail',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'criteria': 'criteria',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """HTTPValidationError - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, description, criteria, *args, **kwargs):  # noqa: E501
+        """CohortTemplate - a model defined in OpenAPI
+
+        Args:
+            id (bool, date, datetime, dict, float, int, list, str, none_type):
+            name (str):
+            description (str):
+            criteria (CohortCriteria):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +141,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            detail ([ValidationError]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -164,14 +168,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.name = name
+        self.description = description
+        self.criteria = criteria
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -184,16 +192,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """HTTPValidationError - a model defined in OpenAPI
+    def __init__(self, id, name, description, criteria, *args, **kwargs):  # noqa: E501
+        """CohortTemplate - a model defined in OpenAPI
+
+        Args:
+            id (bool, date, datetime, dict, float, int, list, str, none_type):
+            name (str):
+            description (str):
+            criteria (CohortCriteria):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -218,15 +232,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            detail ([ValidationError]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -244,14 +257,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.id = id
+        self.name = name
+        self.description = description
+        self.criteria = criteria
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/meta_search_entity_prefix.py` & `metamist-7.0.0/metamist/model/meta_search_entity_prefix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/nested_participant.py` & `metamist-7.0.0/metamist/model/family.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,22 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.family_simple import FamilySimple
-    from metamist.model.nested_sample import NestedSample
-    globals()['FamilySimple'] = FamilySimple
-    globals()['NestedSample'] = NestedSample
 
-
-class NestedParticipant(ModelNormal):
+class Family(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -68,72 +62,63 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'id': (int,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'samples': ([NestedSample],),  # noqa: E501
-            'families': ([FamilySimple],),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'external_id': (str,),  # noqa: E501
-            'reported_sex': (int,),  # noqa: E501
-            'reported_gender': (str,),  # noqa: E501
-            'karyotype': (str,),  # noqa: E501
+            'project': (int,),  # noqa: E501
+            'description': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'coded_phenotype': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
-        'samples': 'samples',  # noqa: E501
-        'families': 'families',  # noqa: E501
         'external_id': 'external_id',  # noqa: E501
-        'reported_sex': 'reported_sex',  # noqa: E501
-        'reported_gender': 'reported_gender',  # noqa: E501
-        'karyotype': 'karyotype',  # noqa: E501
+        'project': 'project',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'coded_phenotype': 'coded_phenotype',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, meta, samples, families, *args, **kwargs):  # noqa: E501
-        """NestedParticipant - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, external_id, project, *args, **kwargs):  # noqa: E501
+        """Family - a model defined in OpenAPI
 
         Args:
-            id (int):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
-            samples ([NestedSample]):
-            families ([FamilySimple]):
+            id (bool, date, datetime, dict, float, int, list, str, none_type):
+            external_id (str):
+            project (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -158,18 +143,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            external_id (str): [optional]  # noqa: E501
-            reported_sex (int): [optional]  # noqa: E501
-            reported_gender (str): [optional]  # noqa: E501
-            karyotype (str): [optional]  # noqa: E501
+            description (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            coded_phenotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,17 +173,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.meta = meta
-        self.samples = samples
-        self.families = families
+        self.external_id = external_id
+        self.project = project
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -213,22 +195,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, meta, samples, families, *args, **kwargs):  # noqa: E501
-        """NestedParticipant - a model defined in OpenAPI
+    def __init__(self, id, external_id, project, *args, **kwargs):  # noqa: E501
+        """Family - a model defined in OpenAPI
 
         Args:
-            id (int):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
-            samples ([NestedSample]):
-            families ([FamilySimple]):
+            id (bool, date, datetime, dict, float, int, list, str, none_type):
+            external_id (str):
+            project (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,18 +234,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            external_id (str): [optional]  # noqa: E501
-            reported_sex (int): [optional]  # noqa: E501
-            reported_gender (str): [optional]  # noqa: E501
-            karyotype (str): [optional]  # noqa: E501
+            description (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            coded_phenotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -283,17 +262,16 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.meta = meta
-        self.samples = samples
-        self.families = families
+        self.external_id = external_id
+        self.project = project
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/nested_sample.py` & `metamist-7.0.0/metamist/model/nested_sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,17 +27,15 @@
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from metamist.model.assay import Assay
-    from metamist.model.nested_sequencing_group import NestedSequencingGroup
     globals()['Assay'] = Assay
-    globals()['NestedSequencingGroup'] = NestedSequencingGroup
 
 
 class NestedSample(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -62,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -88,49 +79,51 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'external_id': (str,),  # noqa: E501
             'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'created_date': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'non_sequencing_assays': ([Assay],),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'created_date': (str,),  # noqa: E501
-            'sequencing_groups': ([NestedSequencingGroup],),  # noqa: E501
+            'sequencing_groups': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'external_id': 'external_id',  # noqa: E501
         'meta': 'meta',  # noqa: E501
-        'non_sequencing_assays': 'non_sequencing_assays',  # noqa: E501
         'type': 'type',  # noqa: E501
         'created_date': 'created_date',  # noqa: E501
+        'non_sequencing_assays': 'non_sequencing_assays',  # noqa: E501
         'sequencing_groups': 'sequencing_groups',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, external_id, meta, non_sequencing_assays, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, external_id, meta, type, created_date, non_sequencing_assays, *args, **kwargs):  # noqa: E501
         """NestedSample - a model defined in OpenAPI
 
         Args:
             id (str):
             external_id (str):
             meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            type (bool, date, datetime, dict, float, int, list, str, none_type):
+            created_date (bool, date, datetime, dict, float, int, list, str, none_type):
             non_sequencing_assays ([Assay]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -156,17 +149,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            created_date (str): [optional]  # noqa: E501
-            sequencing_groups ([NestedSequencingGroup]): [optional]  # noqa: E501
+            sequencing_groups (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,14 +180,16 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.external_id = external_id
         self.meta = meta
+        self.type = type
+        self.created_date = created_date
         self.non_sequencing_assays = non_sequencing_assays
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
@@ -210,21 +203,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, external_id, meta, non_sequencing_assays, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, external_id, meta, type, created_date, non_sequencing_assays, *args, **kwargs):  # noqa: E501
         """NestedSample - a model defined in OpenAPI
 
         Args:
             id (str):
             external_id (str):
             meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            type (bool, date, datetime, dict, float, int, list, str, none_type):
+            created_date (bool, date, datetime, dict, float, int, list, str, none_type):
             non_sequencing_assays ([Assay]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -250,17 +245,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            created_date (str): [optional]  # noqa: E501
-            sequencing_groups ([NestedSequencingGroup]): [optional]  # noqa: E501
+            sequencing_groups (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -281,14 +274,16 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.external_id = external_id
         self.meta = meta
+        self.type = type
+        self.created_date = created_date
         self.non_sequencing_assays = non_sequencing_assays
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `metamist-6.9.1/metamist/model/nested_sequencing_group.py` & `metamist-7.0.0/metamist/model/nested_sequencing_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,18 +25,14 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.assay import Assay
-    globals()['Assay'] = Assay
-
 
 class NestedSequencingGroup(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -60,44 +56,36 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'technology': (str,),  # noqa: E501
             'platform': (str,),  # noqa: E501
             'meta': ({str: (str,)},),  # noqa: E501
             'external_ids': ({str: (str,)},),  # noqa: E501
-            'assays': ([Assay],),  # noqa: E501
+            'assays': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -156,15 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            assays ([Assay]): [optional]  # noqa: E501
+            assays (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -252,15 +240,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            assays ([Assay]): [optional]  # noqa: E501
+            assays (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/paging_links.py` & `metamist-7.0.0/metamist/model/body_create_cohort_from_criteria.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from metamist.model.cohort_body import CohortBody
+    globals()['CohortBody'] = CohortBody
 
-class PagingLinks(ModelNormal):
+
+class BodyCreateCohortFromCriteria(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,57 +66,57 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            '_self': (str,),  # noqa: E501
-            'next': (str,),  # noqa: E501
-            'token': (str,),  # noqa: E501
+            'cohort_spec': (CohortBody,),  # noqa: E501
+            'cohort_criteria': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        '_self': 'self',  # noqa: E501
-        'next': 'next',  # noqa: E501
-        'token': 'token',  # noqa: E501
+        'cohort_spec': 'cohort_spec',  # noqa: E501
+        'cohort_criteria': 'cohort_criteria',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, _self, *args, **kwargs):  # noqa: E501
-        """PagingLinks - a model defined in OpenAPI
+    def _from_openapi_data(cls, cohort_spec, *args, **kwargs):  # noqa: E501
+        """BodyCreateCohortFromCriteria - a model defined in OpenAPI
 
         Args:
-            _self (str):
+            cohort_spec (CohortBody):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -137,16 +141,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            next (str): [optional]  # noqa: E501
-            token (str): [optional]  # noqa: E501
+            cohort_criteria (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -166,15 +169,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self._self = _self
+        self.cohort_spec = cohort_spec
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -187,19 +190,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, _self, *args, **kwargs):  # noqa: E501
-        """PagingLinks - a model defined in OpenAPI
+    def __init__(self, cohort_spec, *args, **kwargs):  # noqa: E501
+        """BodyCreateCohortFromCriteria - a model defined in OpenAPI
 
         Args:
-            _self (str):
+            cohort_spec (CohortBody):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,16 +227,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            next (str): [optional]  # noqa: E501
-            token (str): [optional]  # noqa: E501
+            cohort_criteria (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,15 +253,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self._self = _self
+        self.cohort_spec = cohort_spec
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/participant_search_response_data.py` & `metamist-7.0.0/metamist/model/participant_search_response_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/participant_upsert.py` & `metamist-7.0.0/metamist/model/participant_upsert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,18 +25,14 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.sample_upsert import SampleUpsert
-    globals()['SampleUpsert'] = SampleUpsert
-
 
 class ParticipantUpsert(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -60,44 +56,36 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'external_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'reported_sex': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'reported_gender': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'karyotype': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'samples': ([SampleUpsert],),  # noqa: E501
+            'samples': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -154,15 +142,15 @@
                                 _visited_composed_classes = (Animal,)
             id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             reported_sex (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             reported_gender (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             karyotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            samples ([SampleUpsert]): [optional]  # noqa: E501
+            samples (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -242,15 +230,15 @@
                                 _visited_composed_classes = (Animal,)
             id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             reported_sex (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             reported_gender (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             karyotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            samples ([SampleUpsert]): [optional]  # noqa: E501
+            samples (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/project.py` & `metamist-7.0.0/metamist/model/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,41 +56,35 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'dataset': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'read_group_id': (int,),  # noqa: E501
-            'write_group_id': (int,),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'name': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'dataset': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'read_group_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'write_group_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -140,20 +134,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            dataset (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            read_group_id (int): [optional]  # noqa: E501
-            write_group_id (int): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            name (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            dataset (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            read_group_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            write_group_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -227,20 +221,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            dataset (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            read_group_id (int): [optional]  # noqa: E501
-            write_group_id (int): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            name (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            dataset (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            read_group_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            write_group_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/project_summary.py` & `metamist-7.0.0/metamist/model/project_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -27,18 +27,16 @@
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from metamist.model.nested_participant import NestedParticipant
-    from metamist.model.paging_links import PagingLinks
     from metamist.model.web_project import WebProject
     globals()['NestedParticipant'] = NestedParticipant
-    globals()['PagingLinks'] = PagingLinks
     globals()['WebProject'] = WebProject
 
 
 class ProjectSummary(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -64,22 +62,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -102,15 +93,15 @@
             'participants': ([NestedParticipant],),  # noqa: E501
             'participant_keys': ([list],),  # noqa: E501
             'sample_keys': ([list],),  # noqa: E501
             'sequencing_group_keys': ([list],),  # noqa: E501
             'assay_keys': ([list],),  # noqa: E501
             'seqr_links': ({str: (str,)},),  # noqa: E501
             'seqr_sync_types': ([str],),  # noqa: E501
-            'links': (PagingLinks,),  # noqa: E501
+            'links': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -126,25 +117,25 @@
         'participants': 'participants',  # noqa: E501
         'participant_keys': 'participant_keys',  # noqa: E501
         'sample_keys': 'sample_keys',  # noqa: E501
         'sequencing_group_keys': 'sequencing_group_keys',  # noqa: E501
         'assay_keys': 'assay_keys',  # noqa: E501
         'seqr_links': 'seqr_links',  # noqa: E501
         'seqr_sync_types': 'seqr_sync_types',  # noqa: E501
-        'links': '_links',  # noqa: E501
+        'links': 'links',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, project, total_samples, total_samples_in_query, total_participants, total_sequencing_groups, total_assays, cram_seqr_stats, batch_sequencing_group_stats, participants, participant_keys, sample_keys, sequencing_group_keys, assay_keys, seqr_links, seqr_sync_types, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, project, total_samples, total_samples_in_query, total_participants, total_sequencing_groups, total_assays, cram_seqr_stats, batch_sequencing_group_stats, participants, participant_keys, sample_keys, sequencing_group_keys, assay_keys, seqr_links, seqr_sync_types, links, *args, **kwargs):  # noqa: E501
         """ProjectSummary - a model defined in OpenAPI
 
         Args:
             project (WebProject):
             total_samples (int):
             total_samples_in_query (int):
             total_participants (int):
@@ -155,14 +146,15 @@
             participants ([NestedParticipant]):
             participant_keys ([list]):
             sample_keys ([list]):
             sequencing_group_keys ([list]):
             assay_keys ([list]):
             seqr_links ({str: (str,)}):
             seqr_sync_types ([str]):
+            links (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -187,15 +179,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            links (PagingLinks): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -230,14 +221,15 @@
         self.participants = participants
         self.participant_keys = participant_keys
         self.sample_keys = sample_keys
         self.sequencing_group_keys = sequencing_group_keys
         self.assay_keys = assay_keys
         self.seqr_links = seqr_links
         self.seqr_sync_types = seqr_sync_types
+        self.links = links
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -250,15 +242,15 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, project, total_samples, total_samples_in_query, total_participants, total_sequencing_groups, total_assays, cram_seqr_stats, batch_sequencing_group_stats, participants, participant_keys, sample_keys, sequencing_group_keys, assay_keys, seqr_links, seqr_sync_types, *args, **kwargs):  # noqa: E501
+    def __init__(self, project, total_samples, total_samples_in_query, total_participants, total_sequencing_groups, total_assays, cram_seqr_stats, batch_sequencing_group_stats, participants, participant_keys, sample_keys, sequencing_group_keys, assay_keys, seqr_links, seqr_sync_types, links, *args, **kwargs):  # noqa: E501
         """ProjectSummary - a model defined in OpenAPI
 
         Args:
             project (WebProject):
             total_samples (int):
             total_samples_in_query (int):
             total_participants (int):
@@ -269,14 +261,15 @@
             participants ([NestedParticipant]):
             participant_keys ([list]):
             sample_keys ([list]):
             sequencing_group_keys ([list]):
             assay_keys ([list]):
             seqr_links ({str: (str,)}):
             seqr_sync_types ([str]):
+            links (bool, date, datetime, dict, float, int, list, str, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -301,15 +294,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            links (PagingLinks): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -342,14 +334,15 @@
         self.participants = participants
         self.participant_keys = participant_keys
         self.sample_keys = sample_keys
         self.sequencing_group_keys = sequencing_group_keys
         self.assay_keys = assay_keys
         self.seqr_links = seqr_links
         self.seqr_sync_types = seqr_sync_types
+        self.links = links
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/proportional_date_temporal_method.py` & `metamist-7.0.0/metamist/model/proportional_date_temporal_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/sample_search_response_data.py` & `metamist-7.0.0/metamist/model/sample_search_response_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -78,45 +72,46 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'project': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'family_external_ids': ([str],),  # noqa: E501
             'participant_external_ids': ([str],),  # noqa: E501
             'sample_external_ids': ([str],),  # noqa: E501
-            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'project': 'project',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'family_external_ids': 'family_external_ids',  # noqa: E501
         'participant_external_ids': 'participant_external_ids',  # noqa: E501
         'sample_external_ids': 'sample_external_ids',  # noqa: E501
-        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, project, family_external_ids, participant_external_ids, sample_external_ids, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, project, id, family_external_ids, participant_external_ids, sample_external_ids, *args, **kwargs):  # noqa: E501
         """SampleSearchResponseData - a model defined in OpenAPI
 
         Args:
             project (bool, date, datetime, dict, float, int, list, str, none_type):
+            id (bool, date, datetime, dict, float, int, list, str, none_type):
             family_external_ids ([str]):
             participant_external_ids ([str]):
             sample_external_ids ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -144,15 +139,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -173,14 +167,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.project = project
+        self.id = id
         self.family_external_ids = family_external_ids
         self.participant_external_ids = participant_external_ids
         self.sample_external_ids = sample_external_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
@@ -196,19 +191,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, project, family_external_ids, participant_external_ids, sample_external_ids, *args, **kwargs):  # noqa: E501
+    def __init__(self, project, id, family_external_ids, participant_external_ids, sample_external_ids, *args, **kwargs):  # noqa: E501
         """SampleSearchResponseData - a model defined in OpenAPI
 
         Args:
             project (bool, date, datetime, dict, float, int, list, str, none_type):
+            id (bool, date, datetime, dict, float, int, list, str, none_type):
             family_external_ids ([str]):
             participant_external_ids ([str]):
             sample_external_ids ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -236,15 +232,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -263,14 +258,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.project = project
+        self.id = id
         self.family_external_ids = family_external_ids
         self.participant_external_ids = participant_external_ids
         self.sample_external_ids = sample_external_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
```

### Comparing `metamist-6.9.1/metamist/model/sample_upsert.py` & `metamist-7.0.0/metamist/model/analysis_query_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,22 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.assay_upsert import AssayUpsert
-    from metamist.model.sequencing_group_upsert import SequencingGroupUpsert
-    globals()['AssayUpsert'] = AssayUpsert
-    globals()['SequencingGroupUpsert'] = SequencingGroupUpsert
 
-
-class SampleUpsert(ModelNormal):
+class AnalysisQueryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -68,68 +62,68 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'external_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'project': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sequencing_group_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'projects': ([str],),  # noqa: E501
+            'sample_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'participant_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'output': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'active': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'sequencing_groups': ([SequencingGroupUpsert],),  # noqa: E501
-            'non_sequencing_assays': ([AssayUpsert],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'external_id': 'external_id',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
-        'project': 'project',  # noqa: E501
+        'sequencing_group_ids': 'sequencing_group_ids',  # noqa: E501
+        'projects': 'projects',  # noqa: E501
+        'sample_ids': 'sample_ids',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'participant_id': 'participant_id',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
+        'output': 'output',  # noqa: E501
         'active': 'active',  # noqa: E501
-        'sequencing_groups': 'sequencing_groups',  # noqa: E501
-        'non_sequencing_assays': 'non_sequencing_assays',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SampleUpsert - a model defined in OpenAPI
+    def _from_openapi_data(cls, sequencing_group_ids, projects, *args, **kwargs):  # noqa: E501
+        """AnalysisQueryModel - a model defined in OpenAPI
+
+        Args:
+            sequencing_group_ids (bool, date, datetime, dict, float, int, list, str, none_type):
+            projects ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,23 +148,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            project (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            participant_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            output (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            sequencing_groups ([SequencingGroupUpsert]): [optional]  # noqa: E501
-            non_sequencing_assays ([AssayUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,14 +181,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.sequencing_group_ids = sequencing_group_ids
+        self.projects = projects
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -210,16 +203,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """SampleUpsert - a model defined in OpenAPI
+    def __init__(self, sequencing_group_ids, projects, *args, **kwargs):  # noqa: E501
+        """AnalysisQueryModel - a model defined in OpenAPI
+
+        Args:
+            sequencing_group_ids (bool, date, datetime, dict, float, int, list, str, none_type):
+            projects ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,23 +241,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            project (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            participant_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            output (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            sequencing_groups ([SequencingGroupUpsert]): [optional]  # noqa: E501
-            non_sequencing_assays ([AssayUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -278,14 +272,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.sequencing_group_ids = sequencing_group_ids
+        self.projects = projects
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/search_item.py` & `metamist-7.0.0/metamist/model/search_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -60,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -83,44 +76,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'model_type': (MetaSearchEntityPrefix,),  # noqa: E501
+            'type': (MetaSearchEntityPrefix,),  # noqa: E501
             'query': (str,),  # noqa: E501
             'field': (str,),  # noqa: E501
             'is_meta': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'model_type': 'model_type',  # noqa: E501
+        'type': 'type',  # noqa: E501
         'query': 'query',  # noqa: E501
         'field': 'field',  # noqa: E501
         'is_meta': 'is_meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, model_type, query, field, is_meta, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, type, query, field, is_meta, *args, **kwargs):  # noqa: E501
         """SearchItem - a model defined in OpenAPI
 
         Args:
-            model_type (MetaSearchEntityPrefix):
+            type (MetaSearchEntityPrefix):
             query (str):
             field (str):
             is_meta (bool):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -175,15 +168,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.model_type = model_type
+        self.type = type
         self.query = query
         self.field = field
         self.is_meta = is_meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
@@ -199,19 +192,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, model_type, query, field, is_meta, *args, **kwargs):  # noqa: E501
+    def __init__(self, type, query, field, is_meta, *args, **kwargs):  # noqa: E501
         """SearchItem - a model defined in OpenAPI
 
         Args:
-            model_type (MetaSearchEntityPrefix):
+            type (MetaSearchEntityPrefix):
             query (str):
             field (str):
             is_meta (bool):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -264,15 +257,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.model_type = model_type
+        self.type = type
         self.query = query
         self.field = field
         self.is_meta = is_meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
```

### Comparing `metamist-6.9.1/metamist/model/search_response.py` & `metamist-7.0.0/metamist/model/search_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,17 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from metamist.model.error_response import ErrorResponse
     from metamist.model.search_response_type import SearchResponseType
-    globals()['ErrorResponse'] = ErrorResponse
     globals()['SearchResponseType'] = SearchResponseType
 
 
 class SearchResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -62,22 +60,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        lazy_import()
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -88,15 +79,15 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'type': (SearchResponseType,),  # noqa: E501
             'title': (str,),  # noqa: E501
             'data': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'error': (ErrorResponse,),  # noqa: E501
+            'error': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -149,15 +140,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            error (ErrorResponse): [optional]  # noqa: E501
+            error (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -239,15 +230,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            error (ErrorResponse): [optional]  # noqa: E501
+            error (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.9.1/metamist/model/search_response_model.py` & `metamist-7.0.0/metamist/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/search_response_type.py` & `metamist-7.0.0/metamist/model/search_response_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/seqr_dataset_type.py` & `metamist-7.0.0/metamist/model/seqr_dataset_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.9.1/metamist/model/sequencing_group_meta_update_model.py` & `metamist-7.0.0/metamist/model/validation_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class SequencingGroupMetaUpdateModel(ModelNormal):
+class ValidationError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,35 +77,44 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'loc': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
+            'msg': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'meta': 'meta',  # noqa: E501
+        'loc': 'loc',  # noqa: E501
+        'msg': 'msg',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SequencingGroupMetaUpdateModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, loc, msg, type, *args, **kwargs):  # noqa: E501
+        """ValidationError - a model defined in OpenAPI
+
+        Args:
+            loc ([bool, date, datetime, dict, float, int, list, str, none_type]):
+            msg (str):
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +139,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -158,14 +166,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.loc = loc
+        self.msg = msg
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -178,16 +189,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """SequencingGroupMetaUpdateModel - a model defined in OpenAPI
+    def __init__(self, loc, msg, type, *args, **kwargs):  # noqa: E501
+        """ValidationError - a model defined in OpenAPI
+
+        Args:
+            loc ([bool, date, datetime, dict, float, int, list, str, none_type]):
+            msg (str):
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -212,15 +228,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -238,14 +253,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.loc = loc
+        self.msg = msg
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/sequencing_group_search_response_data.py` & `metamist-7.0.0/metamist/model/sequencing_group_search_response_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
@@ -78,43 +72,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'project': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'sample_external_id': (str,),  # noqa: E501
             'sg_external_id': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'project': 'project',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'sample_external_id': 'sample_external_id',  # noqa: E501
         'sg_external_id': 'sg_external_id',  # noqa: E501
-        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, project, sample_external_id, sg_external_id, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, project, id, sample_external_id, sg_external_id, *args, **kwargs):  # noqa: E501
         """SequencingGroupSearchResponseData - a model defined in OpenAPI
 
         Args:
             project (bool, date, datetime, dict, float, int, list, str, none_type):
+            id (bool, date, datetime, dict, float, int, list, str, none_type):
             sample_external_id (str):
             sg_external_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -141,15 +136,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,14 +164,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.project = project
+        self.id = id
         self.sample_external_id = sample_external_id
         self.sg_external_id = sg_external_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
@@ -192,19 +187,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, project, sample_external_id, sg_external_id, *args, **kwargs):  # noqa: E501
+    def __init__(self, project, id, sample_external_id, sg_external_id, *args, **kwargs):  # noqa: E501
         """SequencingGroupSearchResponseData - a model defined in OpenAPI
 
         Args:
             project (bool, date, datetime, dict, float, int, list, str, none_type):
+            id (bool, date, datetime, dict, float, int, list, str, none_type):
             sample_external_id (str):
             sg_external_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -231,15 +227,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,14 +253,15 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.project = project
+        self.id = id
         self.sample_external_id = sample_external_id
         self.sg_external_id = sg_external_id
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
```

### Comparing `metamist-6.9.1/metamist/model/sequencing_group_upsert.py` & `metamist-7.0.0/metamist/model/sequencing_group_upsert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -56,21 +56,15 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
```

### Comparing `metamist-6.9.1/metamist/model/validation_error.py` & `metamist-7.0.0/metamist/model/cohort_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class ValidationError(ModelNormal):
+class CohortBody(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,65 +56,58 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'loc': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
-            'msg': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'template_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'loc': 'loc',  # noqa: E501
-        'msg': 'msg',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'template_id': 'template_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, loc, msg, type, *args, **kwargs):  # noqa: E501
-        """ValidationError - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, description, *args, **kwargs):  # noqa: E501
+        """CohortBody - a model defined in OpenAPI
 
         Args:
-            loc ([bool, date, datetime, dict, float, int, list, str, none_type]):
-            msg (str):
-            type (str):
+            name (str):
+            description (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,14 +132,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            template_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -166,17 +160,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.loc = loc
-        self.msg = msg
-        self.type = type
+        self.name = name
+        self.description = description
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,21 +182,20 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, loc, msg, type, *args, **kwargs):  # noqa: E501
-        """ValidationError - a model defined in OpenAPI
+    def __init__(self, name, description, *args, **kwargs):  # noqa: E501
+        """CohortBody - a model defined in OpenAPI
 
         Args:
-            loc ([bool, date, datetime, dict, float, int, list, str, none_type]):
-            msg (str):
-            type (str):
+            name (str):
+            description (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,14 +220,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            template_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -253,17 +246,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.loc = loc
-        self.msg = msg
-        self.type = type
+        self.name = name
+        self.description = description
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model/web_project.py` & `metamist-7.0.0/metamist/model/analysis_cost_record_seq_group.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class WebProject(ModelNormal):
+class AnalysisCostRecordSeqGroup(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,68 +56,59 @@
 
     allowed_values = {
     }
 
     validations = {
     }
 
-    @cached_property
-    def additional_properties_type():
-        """
-        This must be a method because a model may have properties that are
-        of type self, this must run after the class is loaded
-        """
-        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
+    additional_properties_type = None
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'dataset': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'sequencing_group': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'stage': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'cost': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'dataset': 'dataset',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
+        'sequencing_group': 'sequencing_group',  # noqa: E501
+        'stage': 'stage',  # noqa: E501
+        'cost': 'cost',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
-        """WebProject - a model defined in OpenAPI
+    def _from_openapi_data(cls, sequencing_group, stage, cost, *args, **kwargs):  # noqa: E501
+        """AnalysisCostRecordSeqGroup - a model defined in OpenAPI
 
         Args:
-            id (int):
-            name (str):
-            dataset (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            sequencing_group (bool, date, datetime, dict, float, int, list, str, none_type):
+            stage (bool, date, datetime, dict, float, int, list, str, none_type):
+            cost (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -169,18 +160,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
-        self.dataset = dataset
-        self.meta = meta
+        self.sequencing_group = sequencing_group
+        self.stage = stage
+        self.cost = cost
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,22 +183,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
-        """WebProject - a model defined in OpenAPI
+    def __init__(self, sequencing_group, stage, cost, *args, **kwargs):  # noqa: E501
+        """AnalysisCostRecordSeqGroup - a model defined in OpenAPI
 
         Args:
-            id (int):
-            name (str):
-            dataset (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+            sequencing_group (bool, date, datetime, dict, float, int, list, str, none_type):
+            stage (bool, date, datetime, dict, float, int, list, str, none_type):
+            cost (float):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -258,18 +247,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
-        self.dataset = dataset
-        self.meta = meta
+        self.sequencing_group = sequencing_group
+        self.stage = stage
+        self.cost = cost
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.9.1/metamist/model_utils.py` & `metamist-7.0.0/metamist/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `metamist-6.9.1/metamist/models/__init__.py` & `metamist-7.0.0/metamist/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,49 +17,57 @@
 from metamist.model.analysis_cost_record_cromwell_subworkflow import AnalysisCostRecordCromwellSubworkflow
 from metamist.model.analysis_cost_record_cromwell_workflow import AnalysisCostRecordCromwellWorkflow
 from metamist.model.analysis_cost_record_seq_group import AnalysisCostRecordSeqGroup
 from metamist.model.analysis_cost_record_sku import AnalysisCostRecordSku
 from metamist.model.analysis_cost_record_topic import AnalysisCostRecordTopic
 from metamist.model.analysis_cost_record_total import AnalysisCostRecordTotal
 from metamist.model.analysis_cost_record_wdl_task import AnalysisCostRecordWdlTask
+from metamist.model.analysis_internal import AnalysisInternal
 from metamist.model.analysis_query_model import AnalysisQueryModel
+from metamist.model.analysis_runner import AnalysisRunner
 from metamist.model.analysis_status import AnalysisStatus
 from metamist.model.analysis_update_model import AnalysisUpdateModel
 from metamist.model.assay import Assay
+from metamist.model.assay_query_criteria import AssayQueryCriteria
 from metamist.model.assay_upsert import AssayUpsert
 from metamist.model.billing_column import BillingColumn
 from metamist.model.billing_cost_budget_record import BillingCostBudgetRecord
 from metamist.model.billing_cost_details_record import BillingCostDetailsRecord
 from metamist.model.billing_source import BillingSource
 from metamist.model.billing_time_column import BillingTimeColumn
 from metamist.model.billing_time_periods import BillingTimePeriods
 from metamist.model.billing_total_cost_query_model import BillingTotalCostQueryModel
 from metamist.model.billing_total_cost_record import BillingTotalCostRecord
-from metamist.model.body_get_assays_by_criteria import BodyGetAssaysByCriteria
+from metamist.model.body_create_cohort_from_criteria import BodyCreateCohortFromCriteria
 from metamist.model.body_get_latest_complete_analysis_for_type_post import BodyGetLatestCompleteAnalysisForTypePost
-from metamist.model.body_get_participants import BodyGetParticipants
 from metamist.model.body_get_proportionate_map import BodyGetProportionateMap
-from metamist.model.body_get_samples import BodyGetSamples
+from metamist.model.cohort_body import CohortBody
+from metamist.model.cohort_criteria import CohortCriteria
+from metamist.model.cohort_template import CohortTemplate
 from metamist.model.error_response import ErrorResponse
 from metamist.model.export_type import ExportType
 from metamist.model.extra_participant_importer_handler import ExtraParticipantImporterHandler
+from metamist.model.family import Family
 from metamist.model.family_search_response_data import FamilySearchResponseData
 from metamist.model.family_simple import FamilySimple
 from metamist.model.family_update_model import FamilyUpdateModel
+from metamist.model.get_samples_criteria import GetSamplesCriteria
 from metamist.model.http_validation_error import HTTPValidationError
 from metamist.model.meta_search_entity_prefix import MetaSearchEntityPrefix
 from metamist.model.nested_participant import NestedParticipant
 from metamist.model.nested_sample import NestedSample
 from metamist.model.nested_sequencing_group import NestedSequencingGroup
+from metamist.model.new_cohort import NewCohort
 from metamist.model.paging_links import PagingLinks
 from metamist.model.participant_search_response_data import ParticipantSearchResponseData
 from metamist.model.participant_upsert import ParticipantUpsert
 from metamist.model.project import Project
 from metamist.model.project_summary import ProjectSummary
 from metamist.model.proportional_date_temporal_method import ProportionalDateTemporalMethod
+from metamist.model.query_participant_criteria import QueryParticipantCriteria
 from metamist.model.sample_search_response_data import SampleSearchResponseData
 from metamist.model.sample_upsert import SampleUpsert
 from metamist.model.search_item import SearchItem
 from metamist.model.search_response import SearchResponse
 from metamist.model.search_response_model import SearchResponseModel
 from metamist.model.search_response_type import SearchResponseType
 from metamist.model.seqr_dataset_type import SeqrDatasetType
```

### Comparing `metamist-6.9.1/metamist/parser/cloudhelper.py` & `metamist-7.0.0/metamist/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/metamist/parser/generic_metadata_parser.py` & `metamist-7.0.0/metamist/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/metamist/parser/generic_parser.py` & `metamist-7.0.0/metamist/parser/generic_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/metamist/parser/sample_file_map_parser.py` & `metamist-7.0.0/metamist/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/metamist/rest.py` & `metamist-7.0.0/metamist/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.9.1
+    The version of the OpenAPI document: 7.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `metamist-6.9.1/metamist.egg-info/PKG-INFO` & `metamist-7.0.0/metamist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.9.1
+Version: 7.0.0
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/metamist
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -52,17 +52,17 @@
 
 3. **Installable Python Library**: Wraps the Python Web API using the OpenAPI generator, facilitating easier interaction with the system.
 
 ### Schema
 
 As of Jan 15, 2024 this schema should reflect the data structure on the tables:
 
-![Database Structure](resources/2024-01-15_db-diagram.png)
+![Database Structure](resources/schemav7.7.png)
 
-You can also find this at [DbDiagram](https://dbdiagram.io/d/Metamist-Schema-v6-6-2-65a48ac7ac844320aee60d16).
+You can also find this at [DbDiagram](https://dbdiagram.io/d/Metamist-Schema-v7-7-6600c875ae072629ced6a1fc).
 
 The codebase contains the following modules worth noting:
 
 - `models` -> General data models + enums
 - `db/python/tables` -> Interaction with MariaDB / BigQuery
 - `db/python/layers` -> Logic
 - `api/graphql` : GraphQL
```

### Comparing `metamist-6.9.1/metamist.egg-info/SOURCES.txt` & `metamist-7.0.0/metamist.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 metamist.egg-info/requires.txt
 metamist.egg-info/top_level.txt
 metamist/api/__init__.py
 metamist/api/analysis_api.py
 metamist/api/analysis_runner_api.py
 metamist/api/assay_api.py
 metamist/api/billing_api.py
+metamist/api/cohort_api.py
 metamist/api/enums_api.py
 metamist/api/family_api.py
 metamist/api/import_api.py
 metamist/api/participant_api.py
 metamist/api/project_api.py
 metamist/api/sample_api.py
 metamist/api/seqr_api.py
@@ -47,49 +48,57 @@
 metamist/model/analysis_cost_record_cromwell_subworkflow.py
 metamist/model/analysis_cost_record_cromwell_workflow.py
 metamist/model/analysis_cost_record_seq_group.py
 metamist/model/analysis_cost_record_sku.py
 metamist/model/analysis_cost_record_topic.py
 metamist/model/analysis_cost_record_total.py
 metamist/model/analysis_cost_record_wdl_task.py
+metamist/model/analysis_internal.py
 metamist/model/analysis_query_model.py
+metamist/model/analysis_runner.py
 metamist/model/analysis_status.py
 metamist/model/analysis_update_model.py
 metamist/model/assay.py
+metamist/model/assay_query_criteria.py
 metamist/model/assay_upsert.py
 metamist/model/billing_column.py
 metamist/model/billing_cost_budget_record.py
 metamist/model/billing_cost_details_record.py
 metamist/model/billing_source.py
 metamist/model/billing_time_column.py
 metamist/model/billing_time_periods.py
 metamist/model/billing_total_cost_query_model.py
 metamist/model/billing_total_cost_record.py
-metamist/model/body_get_assays_by_criteria.py
+metamist/model/body_create_cohort_from_criteria.py
 metamist/model/body_get_latest_complete_analysis_for_type_post.py
-metamist/model/body_get_participants.py
 metamist/model/body_get_proportionate_map.py
-metamist/model/body_get_samples.py
+metamist/model/cohort_body.py
+metamist/model/cohort_criteria.py
+metamist/model/cohort_template.py
 metamist/model/error_response.py
 metamist/model/export_type.py
 metamist/model/extra_participant_importer_handler.py
+metamist/model/family.py
 metamist/model/family_search_response_data.py
 metamist/model/family_simple.py
 metamist/model/family_update_model.py
+metamist/model/get_samples_criteria.py
 metamist/model/http_validation_error.py
 metamist/model/meta_search_entity_prefix.py
 metamist/model/nested_participant.py
 metamist/model/nested_sample.py
 metamist/model/nested_sequencing_group.py
+metamist/model/new_cohort.py
 metamist/model/paging_links.py
 metamist/model/participant_search_response_data.py
 metamist/model/participant_upsert.py
 metamist/model/project.py
 metamist/model/project_summary.py
 metamist/model/proportional_date_temporal_method.py
+metamist/model/query_participant_criteria.py
 metamist/model/sample_search_response_data.py
 metamist/model/sample_upsert.py
 metamist/model/search_item.py
 metamist/model/search_response.py
 metamist/model/search_response_model.py
 metamist/model/search_response_type.py
 metamist/model/seqr_dataset_type.py
@@ -114,14 +123,16 @@
 test/test_bq_billing_base.py
 test/test_bq_billing_daily.py
 test/test_bq_billing_daily_extended.py
 test/test_bq_billing_gcp_daily.py
 test/test_bq_billing_raw.py
 test/test_bq_function_filter.py
 test/test_bq_generic_filter.py
+test/test_cohort.py
+test/test_cohort_builder.py
 test/test_generate_data.py
 test/test_generic_auditor.py
 test/test_generic_filters.py
 test/test_get_participants.py
 test/test_graphql.py
 test/test_import_individual_metadata.py
 test/test_layers_billing.py
```

### Comparing `metamist-6.9.1/pyproject.toml` & `metamist-7.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/setup.py` & `metamist-7.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='6.9.1',
+    version='7.0.0',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/metamist',
     license='MIT',
     packages=all_packages,
     install_requires=[
@@ -35,15 +35,15 @@
         'urllib3 >= 1.25.3',
         'python-dateutil',
         'requests',
         'typing-extensions',
         # for get id-token
         'cpg-utils >= 5.0.5',
         'gql[aiohttp,requests]',
-        'tabulate >= 0.9.0'
+        'tabulate >= 0.9.0',
     ],
     entry_points={
         'metamist_parser': [
             'GenericMetadataParser = metamist.parser.generic_metadata_parser:GenericMetadataParser',
             'SampleFileMapParser = metamist.parser.sample_file_map_parser:SampleFileMapParser',
         ],
     },
```

### Comparing `metamist-6.9.1/test/test_analysis.py` & `metamist-7.0.0/test/test_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,22 @@
 
         analysis = await self.al.get_analysis_by_id(analysis_id)
         self.assertEqual(analysis_id, analysis.id)
         self.assertEqual('cram', analysis.type)
         self.assertEqual(AnalysisStatus.COMPLETED, analysis.status)
 
     @run_as_sync
+    async def test_empty_query(self):
+        """
+        Test empty IDs to see the query construction
+        """
+        analyses = await self.al.query(AnalysisFilter(id=GenericFilter(in_=[])))
+        self.assertEqual(len(analyses), 0)
+
+    @run_as_sync
     async def test_add_cram(self):
         """
         Test adding an analysis of type CRAM
         """
 
         analysis_id = await self.al.create_analysis(
             AnalysisInternal(
@@ -143,14 +151,15 @@
         )
         expected = [
             AnalysisInternal(
                 id=a_id,
                 type='analysis-runner',
                 status=AnalysisStatus.UNKNOWN,
                 sequencing_group_ids=[],
+                cohort_ids=[],
                 output=None,
                 timestamp_completed=None,
                 project=1,
                 meta={},
                 active=True,
                 author=None,
             )
```

### Comparing `metamist-6.9.1/test/test_analysis_runner.py` & `metamist-7.0.0/test/test_analysis_runner.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_api_billing.py` & `metamist-7.0.0/test/test_api_billing.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_api_utils.py` & `metamist-7.0.0/test/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_assay.py` & `metamist-7.0.0/test/test_assay.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_audit_log.py` & `metamist-7.0.0/test/test_audit_log.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_bq_billing_ar_batch.py` & `metamist-7.0.0/test/test_bq_billing_ar_batch.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_bq_billing_base.py` & `metamist-7.0.0/test/test_bq_billing_base.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_bq_billing_daily.py` & `metamist-7.0.0/test/test_bq_billing_daily.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_bq_billing_daily_extended.py` & `metamist-7.0.0/test/test_bq_billing_daily_extended.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_bq_billing_gcp_daily.py` & `metamist-7.0.0/test/test_bq_billing_gcp_daily.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_bq_billing_raw.py` & `metamist-7.0.0/test/test_bq_billing_raw.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_bq_function_filter.py` & `metamist-7.0.0/test/test_bq_function_filter.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_bq_generic_filter.py` & `metamist-7.0.0/test/test_bq_generic_filter.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_generate_data.py` & `metamist-7.0.0/test/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_generic_auditor.py` & `metamist-7.0.0/test/test_generic_auditor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_generic_filters.py` & `metamist-7.0.0/test/test_generic_filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,14 +20,46 @@
         """Test that the basic filter converts to SQL as expected"""
         filter_ = GenericFilterTest(test_string=GenericFilter(eq='test'))
         sql, values = filter_.to_sql()
 
         self.assertEqual('test_string = :test_string_eq', sql)
         self.assertDictEqual({'test_string_eq': 'test'}, values)
 
+    def test_contains_case_sensitive(self):
+        """Test that the basic filter converts to SQL as expected"""
+        filter_ = GenericFilterTest(test_string=GenericFilter(contains='test'))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('test_string LIKE :test_string_contains', sql)
+        self.assertDictEqual({'test_string_contains': '%test%'}, values)
+
+    def test_malicious_contains(self):
+        """Test that a contains-% filter converts to SQL by appropriately encoding _ and %"""
+        filter_ = GenericFilterTest(test_string=GenericFilter(contains='per%ce_nt'))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('test_string LIKE :test_string_contains', sql)
+        self.assertDictEqual({'test_string_contains': r'%per\%ce\_nt%'}, values)
+
+    def test_icontains_is_not_case_sensitive(self):
+        """Test that the basic filter converts to SQL as expected"""
+        filter_ = GenericFilterTest(test_string=GenericFilter(icontains='test'))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('LOWER(test_string) LIKE LOWER(:test_string_icontains)', sql)
+        self.assertDictEqual({'test_string_icontains': '%test%'}, values)
+
+    def test_malicious_icontains(self):
+        """Test that an icontains-% filter converts to SQL by appropriately encoding _ and %"""
+        filter_ = GenericFilterTest(test_string=GenericFilter(icontains='per%ce_nt'))
+        sql, values = filter_.to_sql()
+
+        self.assertEqual('LOWER(test_string) LIKE LOWER(:test_string_icontains)', sql)
+        self.assertDictEqual({'test_string_icontains': r'%per\%ce\_nt%'}, values)
+
     def test_basic_override(self):
         """Test that the basic filter with an override converts to SQL as expected"""
         filter_ = GenericFilterTest(test_string=GenericFilter(eq='test'))
         sql, values = filter_.to_sql({'test_string': 't.string'})
 
         self.assertEqual('t.string = :t_string_eq', sql)
         self.assertDictEqual({'t_string_eq': 'test'}, values)
```

### Comparing `metamist-6.9.1/test/test_get_participants.py` & `metamist-7.0.0/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_graphql.py` & `metamist-7.0.0/test/test_graphql.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from test.testbase import DbIsolatedTest, run_as_sync
 
 from graphql.error import GraphQLError, GraphQLSyntaxError
 
 import api.graphql.schema
 from db.python.layers import AnalysisLayer, ParticipantLayer
+from db.python.layers.family import FamilyLayer
 from metamist.graphql import configure_sync_client, gql, validate
 from models.enums import AnalysisStatus
 from models.models import (
     AnalysisInternal,
     AssayUpsertInternal,
     ParticipantUpsertInternal,
     SampleUpsertInternal,
@@ -187,14 +188,53 @@
             1, len(participants[0]['samples'][0]['sequencingGroups'][0]['assays'])
         )
         self.assertEqual(
             p.samples[0].sequencing_groups[0].assays[0].id, assays[0]['id']
         )
 
     @run_as_sync
+    async def test_query_sample_by_meta(self):
+        """Test querying a participant"""
+        await self.player.upsert_participant(
+            ParticipantUpsertInternal(
+                meta={},
+                external_id='Demeter',
+                samples=[
+                    SampleUpsertInternal(
+                        external_id='sample_id001',
+                        meta={'thisKey': 'value'},
+                    )
+                ],
+            )
+        )
+        q = """
+    query MyQuery($project: String!, $meta: JSON!) {
+        project(name: $project) {
+            participants {
+                samples(meta: $meta) {
+                    id
+                }
+            }
+        }
+    }"""
+        values = await self.run_graphql_query_async(
+            q, {'project': self.project_name, 'meta': {'thisKey': 'value'}}
+        )
+        assert values
+
+        self.assertEqual(1, len(values['project']['participants'][0]['samples']))
+
+        values2 = await self.run_graphql_query_async(
+            q, {'project': self.project_name, 'meta': {'thisKeyDoesNotExistEver': '-1'}}
+        )
+        assert values2
+
+        self.assertEqual(0, len(values2['project']['participants'][0]['samples']))
+
+    @run_as_sync
     async def test_sg_analyses_query(self):
         """Example graphql query of analyses from sequencing-group"""
         p = await self.player.upsert_participant(_get_single_participant_upsert())
         sg_id = p.samples[0].sequencing_groups[0].id
 
         alayer = AnalysisLayer(self.connection)
         await alayer.create_analysis(
@@ -253,7 +293,103 @@
 }"""
 
         resp = await self.run_graphql_query_async(q, {'pid': p.id})
 
         self.assertIn('participant', resp)
         self.assertIn('phenotypes', resp['participant'])
         self.assertDictEqual(phenotypes, resp['participant']['phenotypes'])
+
+    @run_as_sync
+    async def test_family_participants(self):
+        """Test inserting + querying family participants from different directions"""
+        family_layer = FamilyLayer(self.connection)
+
+        family_eid = 'family1'
+
+        rows = [
+            [family_eid, 'individual1', 'paternal1', 'maternal1', 'm', '1', 'note1'],
+            [family_eid, 'paternal1', None, None, 'm', '0', 'note2'],
+            [family_eid, 'maternal1', None, None, 'f', '1', 'note3'],
+        ]
+
+        await family_layer.import_pedigree(None, rows, create_missing_participants=True)
+
+        q = """
+query MyQuery($project: String!) {
+    project(name: $project) {
+        participants {
+            externalId
+            familyParticipants {
+                affected
+                notes
+                family {
+                    externalId
+                }
+            }
+            families {
+                externalId
+            }
+        }
+        families {
+            externalId
+            familyParticipants {
+                affected
+                notes
+                participant {
+                    externalId
+                }
+            }
+        }
+    }
+}
+"""
+
+        resp = await self.run_graphql_query_async(q, {'project': self.project_name})
+        assert resp is not None
+
+        family_simple_obj = {'family': {'externalId': family_eid}}
+
+        participants = resp['project']['participants']
+        families = resp['project']['families']
+
+        participants_by_eid = {p['externalId']: p for p in participants}
+        self.assertEqual(3, len(participants))
+
+        self.assertDictEqual(
+            {
+                'externalId': 'individual1',
+                'families': [{'externalId': family_eid}],
+                'familyParticipants': [
+                    {'affected': 1, 'notes': 'note1', **family_simple_obj}
+                ],
+            },
+            participants_by_eid['individual1'],
+        )
+        self.assertEqual(1, len(participants_by_eid['individual1']['families']))
+
+        self.assertEqual(1, len(families))
+        self.assertEqual(family_eid, families[0]['externalId'])
+
+        sorted_fps = sorted(
+            families[0]['familyParticipants'],
+            key=lambda x: x['participant']['externalId'],
+        )
+        self.assertListEqual(
+            sorted_fps,
+            [
+                {
+                    'affected': 1,
+                    'notes': 'note1',
+                    'participant': {'externalId': 'individual1'},
+                },
+                {
+                    'affected': 1,
+                    'notes': 'note3',
+                    'participant': {'externalId': 'maternal1'},
+                },
+                {
+                    'affected': 0,
+                    'notes': 'note2',
+                    'participant': {'externalId': 'paternal1'},
+                },
+            ],
+        )
```

### Comparing `metamist-6.9.1/test/test_import_individual_metadata.py` & `metamist-7.0.0/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_layers_billing.py` & `metamist-7.0.0/test/test_layers_billing.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_metamist.py` & `metamist-7.0.0/test/test_metamist.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_models.py` & `metamist-7.0.0/test/test_models.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_parse_existing_cohort.py` & `metamist-7.0.0/test/test_parse_existing_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_parse_file_map.py` & `metamist-7.0.0/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_parse_generic_metadata.py` & `metamist-7.0.0/test/test_parse_generic_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_parse_ont_processor.py` & `metamist-7.0.0/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_parse_ont_sheet.py` & `metamist-7.0.0/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_pedigree.py` & `metamist-7.0.0/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_project_groups.py` & `metamist-7.0.0/test/test_project_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_sample.py` & `metamist-7.0.0/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_search.py` & `metamist-7.0.0/test/test_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,18 +200,19 @@
             ParticipantUpsertInternal(external_id='X:PART01')
         )
         f_id = await self.flayer.create_family(external_id='X:FAM01')
         await fptable.create_rows(
             [
                 PedRowInternal(
                     family_id=f_id,
-                    participant_id=p.id,
+                    individual_id=p.id,
                     paternal_id=None,
                     maternal_id=None,
                     affected=0,
+                    sex=0,
                     notes=None,
                 )
             ]
         )
 
         sample = await self.slayer.upsert_sample(
             SampleUpsertInternal(
```

### Comparing `metamist-6.9.1/test/test_update_participant_family.py` & `metamist-7.0.0/test/test_update_participant_family.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,29 @@
 
         fl = FamilyLayer(self.connection)
 
         self.fid_1 = await fl.create_family(external_id='FAM01')
         self.fid_2 = await fl.create_family(external_id='FAM02')
 
         pl = ParticipantLayer(self.connection)
-        self.pid = (await pl.upsert_participant(ParticipantUpsertInternal(external_id='EX01', reported_sex=2))).id
-        self.pat_pid = (await pl.upsert_participant(
-            ParticipantUpsertInternal(external_id='EX01_pat', reported_sex=1)
-        )).id
-        self.mat_pid = (await pl.upsert_participant(
-            ParticipantUpsertInternal(external_id='EX01_mat', reported_sex=2)
-        )).id
+        self.pid = (
+            await pl.upsert_participant(
+                ParticipantUpsertInternal(external_id='EX01', reported_sex=2)
+            )
+        ).id
+        self.pat_pid = (
+            await pl.upsert_participant(
+                ParticipantUpsertInternal(external_id='EX01_pat', reported_sex=1)
+            )
+        ).id
+        self.mat_pid = (
+            await pl.upsert_participant(
+                ParticipantUpsertInternal(external_id='EX01_mat', reported_sex=2)
+            )
+        ).id
 
         await pl.add_participant_to_family(
             family_id=self.fid_1,
             participant_id=self.pid,
             paternal_id=self.pat_pid,
             maternal_id=self.mat_pid,
             affected=2,
@@ -50,42 +58,44 @@
         expected_fp_row = {
             'family_id': self.fid_1,
             'individual_id': self.pid,
             'paternal_id': self.pat_pid,
             'maternal_id': self.mat_pid,
             'sex': 2,
             'affected': 2,
+            'notes': None,
         }
-        self.assertDictEqual(fp_row, expected_fp_row)
+        self.assertDictEqual(expected_fp_row, fp_row.to_dict())
 
         await pl.remove_participant_from_family(
             family_id=self.fid_1, participant_id=self.pid
         )
 
         await pl.add_participant_to_family(
             family_id=self.fid_2,
             participant_id=self.pid,
-            paternal_id=fp_row['paternal_id'],
-            maternal_id=fp_row['maternal_id'],
-            affected=fp_row['affected'],
+            paternal_id=fp_row.paternal_id,
+            maternal_id=fp_row.maternal_id,
+            affected=fp_row.affected,
         )
 
         updated_fp_row = await pl.get_family_participant_data(
             family_id=self.fid_2, participant_id=self.pid
         )
 
         expected_updated_fp_row = {
             'family_id': self.fid_2,
             'individual_id': self.pid,
             'paternal_id': self.pat_pid,
             'maternal_id': self.mat_pid,
             'sex': 2,
             'affected': 2,
+            'notes': None,
         }
-        self.assertDictEqual(updated_fp_row, expected_updated_fp_row)
+        self.assertDictEqual(expected_updated_fp_row, updated_fp_row.to_dict())
 
         await pl.remove_participant_from_family(
             family_id=self.fid_2, participant_id=self.pid
         )
 
     @run_as_sync
     async def test_update_participant_family(self):
@@ -102,16 +112,17 @@
         expected_updated_fp_row = {
             'family_id': self.fid_2,
             'individual_id': self.pid,
             'paternal_id': self.pat_pid,
             'maternal_id': self.mat_pid,
             'sex': 2,
             'affected': 2,
+            'notes': None,
         }
-        self.assertDictEqual(updated_fp_row, expected_updated_fp_row)
+        self.assertDictEqual(expected_updated_fp_row, updated_fp_row.to_dict())
 
         await pl.remove_participant_from_family(
             family_id=self.fid_2, participant_id=self.pid
         )
 
     @run_as_sync
     async def test_update_participant_to_nonexistent_family(self):
@@ -124,21 +135,22 @@
         expected_fp_row = {
             'family_id': self.fid_1,
             'individual_id': self.pid,
             'paternal_id': self.pat_pid,
             'maternal_id': self.mat_pid,
             'sex': 2,
             'affected': 2,
+            'notes': None,
         }
-        self.assertDictEqual(fp_row, expected_fp_row)
+        self.assertDictEqual(expected_fp_row, fp_row.to_dict())
 
         with self.assertRaises(IntegrityError):
             await pl.update_participant_family(
                 participant_id=self.pid, old_family_id=self.fid_1, new_family_id=-99
             )
 
         rollback_fp_row = await pl.get_family_participant_data(
             family_id=self.fid_1, participant_id=self.pid
         )
 
         # Update transaction should rollback, so no change expected
-        self.assertDictEqual(rollback_fp_row, expected_fp_row)
+        self.assertDictEqual(expected_fp_row, rollback_fp_row.to_dict())
```

### Comparing `metamist-6.9.1/test/test_upsert.py` & `metamist-7.0.0/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/test_web.py` & `metamist-7.0.0/test/test_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         """Project grid but with test filter, that shows results"""
         await self.partl.upsert_participants(participants=[get_test_participant()])
 
         filtered_result_success = await self.webl.get_project_summary(
             token=0,
             grid_filter=[
                 SearchItem(
-                    model_type=MetaSearchEntityPrefix.ASSAY,
+                    type=MetaSearchEntityPrefix.ASSAY,
                     query='M001',
                     field='batch',
                     is_meta=True,
                 )
             ],
         )
         filtered_result_success.participants = []
@@ -294,15 +294,15 @@
     @run_as_sync
     async def project_summary_with_filter_no_results(self):
         """Project grid but with test filter, that doesn't have results"""
         filtered_result_empty = await self.webl.get_project_summary(
             token=0,
             grid_filter=[
                 SearchItem(
-                    model_type=MetaSearchEntityPrefix.ASSAY,
+                    type=MetaSearchEntityPrefix.ASSAY,
                     query='M002',
                     field='batch',
                     is_meta=True,
                 )
             ],
         )
         empty_result = ProjectSummaryInternal(
@@ -423,15 +423,15 @@
             seqr_sync_types=[],
         )
 
         two_samples_result_filtered = await self.webl.get_project_summary(
             token=0,
             grid_filter=[
                 SearchItem(
-                    model_type=MetaSearchEntityPrefix.SAMPLE,
+                    type=MetaSearchEntityPrefix.SAMPLE,
                     query='sample_id002',
                     field='external_id',
                     is_meta=False,
                 )
             ],
         )
         two_samples_result_filtered.participants = []
@@ -447,15 +447,15 @@
             participants=[get_test_participant(), get_test_participant_2()]
         )
         print(await self.connection.connection.fetch_all('SELECT * FROM assay'))
         test_field_with_space = await self.webl.get_project_summary(
             token=0,
             grid_filter=[
                 SearchItem(
-                    model_type=MetaSearchEntityPrefix.ASSAY,
+                    type=MetaSearchEntityPrefix.ASSAY,
                     query='field wi',
                     field='field with spaces',
                     is_meta=True,
                 )
             ],
         )
         self.assertEqual(1, len(test_field_with_space.participants))
```

### Comparing `metamist-6.9.1/test/testbase.py` & `metamist-7.0.0/test/testbase.py`

 * *Files identical despite different names*

### Comparing `metamist-6.9.1/test/testbqbase.py` & `metamist-7.0.0/test/testbqbase.py`

 * *Files identical despite different names*

