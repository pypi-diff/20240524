# Comparing `tmp/metamist-7.0.0.tar.gz` & `tmp/metamist-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-7.0.0.tar", last modified: Thu May 23 05:05:21 2024, max compression
+gzip compressed data, was "metamist-7.0.1.tar", last modified: Fri May 24 00:06:04 2024, max compression
```

## Comparing `metamist-7.0.0.tar` & `metamist-7.0.1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.818431 metamist-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 05:02:20.000000 metamist-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 05:02:20.000000 metamist-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-23 05:05:21.818431 metamist-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-23 05:02:20.000000 metamist-7.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.798431 metamist-7.0.0/metamist/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.802431 metamist-7.0.0/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56146 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/analysis_runner_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    82373 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/billing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/cohort_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    50382 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29264 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    48033 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32909 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.802431 metamist-7.0.0/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.802431 metamist-7.0.0/metamist/audit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/audit_upload_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/audithelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/delete_assay_files_from_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/audit/generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.802431 metamist-7.0.0/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-23 05:03:55.000000 metamist-7.0.0/metamist/graphql/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.814431 metamist-7.0.0/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_batch_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_cromwell_subworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_cromwell_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_seq_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_sku.py
--rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_total.py
--rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_cost_record_wdl_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13856 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15657 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/assay.py
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/assay_query_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_cost_budget_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_cost_details_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_time_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_time_periods.py
--rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_total_cost_query_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/billing_total_cost_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-23 05:03:50.000000 metamist-7.0.0/metamist/model/body_create_cohort_from_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/body_get_proportionate_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/cohort_body.py
--rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/cohort_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/cohort_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/family.py
--rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/family_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/get_samples_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/new_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/project_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/proportional_date_temporal_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/query_participant_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/seqr_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sequencing_group_meta_update_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sequencing_group_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.814431 metamist-7.0.0/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.814431 metamist-7.0.0/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    55508 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-23 05:02:20.000000 metamist-7.0.0/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-23 05:03:51.000000 metamist-7.0.0/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.798431 metamist-7.0.0/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 05:05:21.000000 metamist-7.0.0/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-23 05:02:20.000000 metamist-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 05:05:21.818431 metamist-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-23 05:02:20.000000 metamist-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:05:21.818431 metamist-7.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_analysis_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_api_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_audit_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_ar_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    32213 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_daily_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_gcp_daily.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_billing_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_function_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_bq_generic_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18895 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_cohort_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_generic_auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_generic_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_layers_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_metamist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    32146 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_project_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_update_participant_family.py
--rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-05-23 05:02:20.000000 metamist-7.0.0/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-23 05:02:20.000000 metamist-7.0.0/test/testbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-23 05:02:20.000000 metamist-7.0.0/test/testbqbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.316694 metamist-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-24 00:03:11.000000 metamist-7.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 00:03:11.000000 metamist-7.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-24 00:06:04.316694 metamist-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-24 00:03:11.000000 metamist-7.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.292694 metamist-7.0.1/metamist/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.296694 metamist-7.0.1/metamist/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56146 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/analysis_runner_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/assay_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82373 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/billing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/cohort_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50382 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/enums_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29264 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48033 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32909 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48000 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/sequencing_group_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38210 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.296694 metamist-7.0.1/metamist/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.296694 metamist-7.0.1/metamist/audit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/audit/audit_upload_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/audit/audithelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/audit/delete_assay_files_from_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23865 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/audit/generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.300694 metamist-7.0.1/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-24 00:04:42.000000 metamist-7.0.1/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.308694 metamist-7.0.1/metamist/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15003 2024-05-24 00:04:36.000000 metamist-7.0.1/metamist/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_batch_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_cromwell_subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_cromwell_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_seq_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_sku.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_total.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12241 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_cost_record_wdl_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13856 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15657 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11993 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/assay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/assay_query_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12399 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/assay_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/billing_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/billing_cost_budget_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/billing_cost_details_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/billing_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/billing_time_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/billing_time_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/billing_total_cost_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19290 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/billing_total_cost_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/body_create_cohort_from_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/body_get_proportionate_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/cohort_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13341 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/cohort_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/cohort_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12506 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/family.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11591 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/family_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12441 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/get_samples_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13354 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13184 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/nested_sequencing_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/new_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16284 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/project_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/proportional_date_temporal_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/query_participant_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13993 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/sample_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/seqr_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/sequencing_group_meta_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/sequencing_group_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/sequencing_group_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82230 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.308694 metamist-7.0.1/metamist/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.308694 metamist-7.0.1/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35867 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55754 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-05-24 00:03:11.000000 metamist-7.0.1/metamist/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-05-24 00:04:37.000000 metamist-7.0.1/metamist/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.292694 metamist-7.0.1/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-24 00:06:04.000000 metamist-7.0.1/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-24 00:06:04.000000 metamist-7.0.1/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 00:06:04.000000 metamist-7.0.1/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-24 00:06:04.000000 metamist-7.0.1/metamist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 00:06:04.000000 metamist-7.0.1/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-24 00:06:04.000000 metamist-7.0.1/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 00:06:04.000000 metamist-7.0.1/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-24 00:03:11.000000 metamist-7.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 00:06:04.316694 metamist-7.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-24 00:03:11.000000 metamist-7.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 00:06:04.316694 metamist-7.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_analysis_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_api_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14169 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_bq_billing_ar_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32213 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_bq_billing_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_bq_billing_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_bq_billing_daily_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_bq_billing_gcp_daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_bq_billing_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_bq_function_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_bq_generic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18895 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_cohort_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28157 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_layers_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_metamist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_project_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_update_participant_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19049 2024-05-24 00:03:11.000000 metamist-7.0.1/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-24 00:03:11.000000 metamist-7.0.1/test/testbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-24 00:03:11.000000 metamist-7.0.1/test/testbqbase.py
```

### Comparing `metamist-7.0.0/LICENSE` & `metamist-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/PKG-INFO` & `metamist-7.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 7.0.0
+Version: 7.0.1
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/metamist
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-7.0.0/README.md` & `metamist-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/__init__.py` & `metamist-7.0.1/metamist/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `metamist-7.0.0/metamist/api/analysis_api.py` & `metamist-7.0.1/metamist/api/analysis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/analysis_runner_api.py` & `metamist-7.0.1/metamist/api/analysis_runner_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/assay_api.py` & `metamist-7.0.1/metamist/api/assay_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/billing_api.py` & `metamist-7.0.1/metamist/api/billing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/cohort_api.py` & `metamist-7.0.1/metamist/api/cohort_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/enums_api.py` & `metamist-7.0.1/metamist/api/enums_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/family_api.py` & `metamist-7.0.1/metamist/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/import_api.py` & `metamist-7.0.1/metamist/api/import_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/participant_api.py` & `metamist-7.0.1/metamist/api/participant_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/project_api.py` & `metamist-7.0.1/metamist/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/sample_api.py` & `metamist-7.0.1/metamist/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/seqr_api.py` & `metamist-7.0.1/metamist/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/sequencing_group_api.py` & `metamist-7.0.1/metamist/api/sequencing_group_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api/web_api.py` & `metamist-7.0.1/metamist/api/web_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/api_client.py` & `metamist-7.0.1/metamist/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `metamist-7.0.0/metamist/apis/__init__.py` & `metamist-7.0.1/metamist/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/audit/audit_upload_bucket.py` & `metamist-7.0.1/metamist/audit/audit_upload_bucket.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/audit/audithelper.py` & `metamist-7.0.1/metamist/audit/audithelper.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/audit/delete_assay_files_from_audit.py` & `metamist-7.0.1/metamist/audit/delete_assay_files_from_audit.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/audit/generic_auditor.py` & `metamist-7.0.1/metamist/audit/generic_auditor.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/configuration.py` & `metamist-7.0.1/metamist/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
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
-               "Version of the API: 7.0.0\n"\
+               "Version of the API: 7.0.1\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `metamist-7.0.0/metamist/exceptions.py` & `metamist-7.0.1/metamist/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `metamist-7.0.0/metamist/graphql/__init__.py` & `metamist-7.0.1/metamist/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/graphql/schema.graphql` & `metamist-7.0.1/metamist/graphql/schema.graphql`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/model/analysis.py` & `metamist-7.0.1/metamist/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record.py` & `metamist-7.0.1/metamist/model/analysis_cost_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_batch.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_batch_job.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_batch_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_category.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_cromwell_subworkflow.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_cromwell_subworkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_cromwell_workflow.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_cromwell_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_seq_group.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_seq_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_sku.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_sku.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_topic.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_topic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_total.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_total.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_cost_record_wdl_task.py` & `metamist-7.0.1/metamist/model/analysis_cost_record_wdl_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_internal.py` & `metamist-7.0.1/metamist/model/analysis_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_query_model.py` & `metamist-7.0.1/metamist/model/analysis_query_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_runner.py` & `metamist-7.0.1/metamist/model/analysis_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_status.py` & `metamist-7.0.1/metamist/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/analysis_update_model.py` & `metamist-7.0.1/metamist/model/analysis_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/assay.py` & `metamist-7.0.1/metamist/model/assay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/assay_query_criteria.py` & `metamist-7.0.1/metamist/model/assay_query_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/assay_upsert.py` & `metamist-7.0.1/metamist/model/assay_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/billing_column.py` & `metamist-7.0.1/metamist/model/billing_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/billing_cost_budget_record.py` & `metamist-7.0.1/metamist/model/billing_cost_budget_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/billing_cost_details_record.py` & `metamist-7.0.1/metamist/model/billing_cost_details_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/billing_source.py` & `metamist-7.0.1/metamist/model/billing_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/billing_time_column.py` & `metamist-7.0.1/metamist/model/billing_time_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/billing_time_periods.py` & `metamist-7.0.1/metamist/model/billing_time_periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/billing_total_cost_query_model.py` & `metamist-7.0.1/metamist/model/billing_total_cost_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/billing_total_cost_record.py` & `metamist-7.0.1/metamist/model/billing_total_cost_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/body_create_cohort_from_criteria.py` & `metamist-7.0.1/metamist/model/body_create_cohort_from_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/body_get_latest_complete_analysis_for_type_post.py` & `metamist-7.0.1/metamist/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/body_get_proportionate_map.py` & `metamist-7.0.1/metamist/model/body_get_proportionate_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/cohort_body.py` & `metamist-7.0.1/metamist/model/cohort_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/cohort_criteria.py` & `metamist-7.0.1/metamist/model/cohort_criteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/cohort_template.py` & `metamist-7.0.1/metamist/model/cohort_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/error_response.py` & `metamist-7.0.1/metamist/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/export_type.py` & `metamist-7.0.1/metamist/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/extra_participant_importer_handler.py` & `metamist-7.0.1/metamist/model/extra_participant_importer_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/family.py` & `metamist-7.0.1/metamist/model/family.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/family_search_response_data.py` & `metamist-7.0.1/metamist/model/family_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/family_simple.py` & `metamist-7.0.1/metamist/model/family_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/family_update_model.py` & `metamist-7.0.1/metamist/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/get_samples_criteria.py` & `metamist-7.0.1/metamist/model/get_samples_criteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/http_validation_error.py` & `metamist-7.0.1/metamist/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/meta_search_entity_prefix.py` & `metamist-7.0.1/metamist/model/meta_search_entity_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/nested_participant.py` & `metamist-7.0.1/metamist/model/nested_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/nested_sample.py` & `metamist-7.0.1/metamist/model/nested_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/nested_sequencing_group.py` & `metamist-7.0.1/metamist/model/nested_sequencing_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/new_cohort.py` & `metamist-7.0.1/metamist/model/new_cohort.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/paging_links.py` & `metamist-7.0.1/metamist/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/participant_search_response_data.py` & `metamist-7.0.1/metamist/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/participant_upsert.py` & `metamist-7.0.1/metamist/model/participant_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/project.py` & `metamist-7.0.1/metamist/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/project_summary.py` & `metamist-7.0.1/metamist/model/project_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/proportional_date_temporal_method.py` & `metamist-7.0.1/metamist/model/proportional_date_temporal_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/query_participant_criteria.py` & `metamist-7.0.1/metamist/model/query_participant_criteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/sample_search_response_data.py` & `metamist-7.0.1/metamist/model/sample_search_response_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/sample_upsert.py` & `metamist-7.0.1/metamist/model/sample_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/search_item.py` & `metamist-7.0.1/metamist/model/search_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/search_response.py` & `metamist-7.0.1/metamist/model/search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/search_response_model.py` & `metamist-7.0.1/metamist/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/search_response_type.py` & `metamist-7.0.1/metamist/model/search_response_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/seqr_dataset_type.py` & `metamist-7.0.1/metamist/model/seqr_dataset_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/sequencing_group_meta_update_model.py` & `metamist-7.0.1/metamist/model/sequencing_group_meta_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/sequencing_group_search_response_data.py` & `metamist-7.0.1/metamist/model/sequencing_group_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/sequencing_group_upsert.py` & `metamist-7.0.1/metamist/model/sequencing_group_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/validation_error.py` & `metamist-7.0.1/metamist/model/validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model/web_project.py` & `metamist-7.0.1/metamist/model/web_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-7.0.0/metamist/model_utils.py` & `metamist-7.0.1/metamist/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `metamist-7.0.0/metamist/models/__init__.py` & `metamist-7.0.1/metamist/models/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/parser/cloudhelper.py` & `metamist-7.0.1/metamist/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/metamist/parser/generic_metadata_parser.py` & `metamist-7.0.1/metamist/parser/generic_metadata_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=R0904,too-many-instance-attributes,too-many-locals,unused-argument,wrong-import-order,unused-argument,too-many-arguments,unused-import
 import asyncio
 import logging
 import re
 import shlex
 from functools import reduce
-from typing import Any, Dict, List, Optional, Set, Tuple, Union
+from typing import Any
 
 import click
 
 from metamist.parser.generic_parser import (  # noqa
     DefaultSequencing,
     GenericParser,
     GroupedRow,
@@ -73,47 +73,57 @@
 
 
 class GenericMetadataParser(GenericParser):
     """Parser for GenericMetadataParser"""
 
     def __init__(
         self,
-        search_locations: List[str],
-        participant_meta_map: Dict[str, str],
-        sample_meta_map: Dict[str, str],
-        assay_meta_map: Dict[str, str],
-        qc_meta_map: Dict[str, str],
         project: str,
+        search_locations: list[str],
         sample_name_column: str,
-        participant_column: Optional[str] = None,
-        assay_id_column: Optional[str] = None,
-        reported_sex_column: Optional[str] = None,
-        reported_gender_column: Optional[str] = None,
-        karyotype_column: Optional[str] = None,
-        reads_column: Optional[str] = None,
-        checksum_column: Optional[str] = None,
-        seq_type_column: Optional[str] = None,
-        seq_technology_column: Optional[str] = None,
-        seq_platform_column: Optional[str] = None,
-        seq_facility_column: Optional[str] = None,
-        seq_library_column: Optional[str] = None,
-        read_end_type_column: Optional[str] = None,
-        read_length_column: Optional[str] = None,
-        gvcf_column: Optional[str] = None,
-        meta_column: Optional[str] = None,
-        seq_meta_column: Optional[str] = None,
-        batch_number: Optional[str] = None,
-        reference_assembly_location_column: Optional[str] = None,
-        default_reference_assembly_location: Optional[str] = None,
-        default_sample_type=None,
+
+        # Participant columns
+        participant_column: str | None = None,
+        reported_sex_column: str | None = None,
+        reported_gender_column: str | None = None,
+        karyotype_column: str | None = None,
+
+        # Sequencing metadata columns
+        seq_type_column: str | None = None,
+        seq_technology_column: str | None = None,
+        seq_platform_column: str | None = None,
+        seq_facility_column: str | None = None,
+        seq_library_column: str | None = None,
+
+        # Assay columns
+        assay_id_column: str | None = None,
+        reads_column: str | None = None,
+        checksum_column: str | None = None,
+        read_end_type_column: str | None = None,
+        read_length_column: str | None = None,
+        reference_assembly_location_column: str | None = None,
+
+        # GVCF columns
+        gvcf_column: str | None = None,
+
+        # Meta field key maps
+        participant_meta_map: dict[str, str] | None = None,
+        sample_meta_map: dict[str, str] | None = None,
+        assay_meta_map: dict[str, str] | None = None,
+        qc_meta_map: dict[str, str] | None = None,
+
+        # Default values
+        default_reference_assembly_location: str | None = None,
+        default_sample_type: str | None = None,
         default_sequencing=DefaultSequencing(
             seq_type='genome', technology='short-read', platform='illumina'
         ),
-        default_read_end_type: Optional[str] = None,
-        default_read_length: Optional[str | int] = None,
+        default_read_end_type: str | None = None,
+        default_read_length: str | int | None = None,
+        batch_number: str | None = None,
         allow_extra_files_in_search_path=False,
         **kwargs,
     ):
         super().__init__(
             path_prefix=None,
             search_paths=search_locations,
             project=project,
@@ -123,49 +133,57 @@
             default_read_length=default_read_length,
             **kwargs,
         )
 
         if not sample_name_column:
             raise ValueError('A sample name column MUST be provided')
 
-        self.cpg_id_column = 'Internal CPG Sample ID'
-
+        self.cpg_id_column = 'Internal CPG Sequencing Group ID'
         self.sample_name_column = sample_name_column
+
+        # Participant columns
         self.participant_column = participant_column
-        self.assay_id_column = assay_id_column
         self.reported_sex_column = reported_sex_column
         self.reported_gender_column = reported_gender_column
         self.karyotype_column = karyotype_column
+
+        # Sequencing metadata columns
         self.seq_type_column = seq_type_column
         self.seq_technology_column = seq_technology_column
         self.seq_platform_column = seq_platform_column
         self.seq_facility_column = seq_facility_column
         self.seq_library_column = seq_library_column
+
+        # Assay columns
+        self.assay_id_column = assay_id_column
+        self.reads_column = reads_column
+        self.checksum_column = checksum_column
         self.read_end_type_column = read_end_type_column
         self.read_length_column = read_length_column
         self.reference_assembly_location_column = reference_assembly_location_column
-        self.default_reference_assembly_location = default_reference_assembly_location
 
+        # Meta field key maps
         self.participant_meta_map = participant_meta_map or {}
         self.sample_meta_map = sample_meta_map or {}
         self.assay_meta_map = assay_meta_map or {}
         self.qc_meta_map = qc_meta_map or {}
-        self.reads_column = reads_column
-        self.checksum_column = checksum_column
+
+        # GVCF column
         self.gvcf_column = gvcf_column
-        self.meta_column = meta_column
-        self.seq_meta_column = seq_meta_column
-        self.allow_extra_files_in_search_path = allow_extra_files_in_search_path
+
+        # Default values
         self.batch_number = batch_number
+        self.default_reference_assembly_location = default_reference_assembly_location
+        self.allow_extra_files_in_search_path = allow_extra_files_in_search_path
 
     def get_sample_id(self, row: SingleRow) -> str:
         """Get external sample ID from row"""
         return row[self.sample_name_column].strip()
 
-    async def get_cpg_sample_id_from_row(self, row: SingleRow) -> Optional[str]:
+    async def get_cpg_sample_id_from_row(self, row: SingleRow) -> str | None:
         """Get internal cpg id from a row using get_sample_id and an api call"""
         return row.get(self.cpg_id_column, None)
 
     def get_sample_type(self, row: GroupedRow) -> str:
         """Get sample type from row"""
         if self.default_sample_type:
             return self.default_sample_type
@@ -253,26 +271,26 @@
         """Get read length from row"""
         value = (
             row.get(self.read_length_column, None) or self.default_read_length
         )
         value = int(value) if value else None
         return value
 
-    def get_assay_id(self, row: GroupedRow) -> Optional[dict[str, str]]:
+    def get_assay_id(self, row: GroupedRow) -> dict[str, str] | None:
         """Get external assay ID from row. Needs to be implemented per parser.
         NOTE: To be re-thought after assay group changes are applied"""
         return None
 
-    def get_participant_id(self, row: SingleRow) -> Optional[str]:
+    def get_participant_id(self, row: SingleRow) -> str | None:
         """Get external participant ID from row"""
         if not self.participant_column or self.participant_column not in row:
             raise ValueError('Participant column does not exist')
         return row[self.participant_column]
 
-    def get_reported_sex(self, row: GroupedRow) -> Optional[int]:
+    def get_reported_sex(self, row: GroupedRow) -> int | None:
         """Get reported sex from grouped row"""
 
         if not self.reported_sex_column:
             return None
 
         reported_sex = row[0].get(self.reported_sex_column, None)
 
@@ -285,19 +303,19 @@
         if reported_sex.lower() == 'male':
             return 1
 
         raise ValueError(
             f'{reported_sex} could not be identified as an input for reported_sex'
         )
 
-    def get_reported_gender(self, row: GroupedRow) -> Optional[str]:
+    def get_reported_gender(self, row: GroupedRow) -> str | None:
         """Get reported gender from grouped row"""
         return row[0].get(self.reported_gender_column, None)
 
-    def get_karyotype(self, row: GroupedRow) -> Optional[str]:
+    def get_karyotype(self, row: GroupedRow) -> str | None:
         """Get karyotype from grouped row"""
         return row[0].get(self.karyotype_column, None)
 
     def has_participants(self, rows: list[SingleRow]) -> bool:
         """Returns True if the file has a Participants column"""
         return self.participant_column in rows[0]
 
@@ -331,27 +349,27 @@
     async def get_all_files_from_row(self, sample_id: str, row):
         """Get all files from row, to allow subparsers to include other files"""
         fns = await self.get_read_filenames(sample_id, row)
 
         return self.flatten_irregular_list(fns)
 
     async def check_files_covered_by_rows(
-        self, rows: List[Dict[str, Any]]
-    ) -> List[str]:
+        self, rows: list[dict[str, Any]]
+    ) -> list[str]:
         """
         Check that the files in the search_paths are completely covered by the sample_map
         """
         filename_promises = []
         for grp in rows:
             for r in grp if isinstance(grp, list) else [grp]:
                 filename_promises.append(
                     self.get_all_files_from_row(self.get_sample_id(r), r)
                 )
 
-        files_from_rows: List[str] = sum(await asyncio.gather(*filename_promises), [])
+        files_from_rows: list[str] = sum(await asyncio.gather(*filename_promises), [])
         filenames_from_rows = set(f.strip() for f in files_from_rows if f and f.strip())
         relevant_extensions = ('.cram', '.fastq.gz', '.fastq', 'fq.gz', '.fq', '.bam')
 
         # we need to explicitly filter filenames from rows not to include absolute
         # paths, otherwise the below check will flag it as missing
         absolute_path_starts = ('/', 'gs://', 'https://')
         filenames_from_rows = set(
@@ -384,15 +402,15 @@
                 logger.warning(m)
             else:
                 errors.append(m)
 
         return errors
 
     @staticmethod
-    def merge_dicts(a: Dict, b: Dict):
+    def merge_dicts(a: dict, b: dict):
         """
         Recursively merge two dictionaries:
         - collapse equal values
         - put differing values into a list (not guaranteeing order)
         """
         if b is None:
             return a
@@ -417,15 +435,15 @@
                     res[key] = [a_val, b_val]
             else:
                 res[key] = a_val or b_val
 
         return res
 
     @staticmethod
-    def collapse_arbitrary_meta(key_map: Dict[str, str], row: GroupedRow):
+    def collapse_arbitrary_meta(key_map: dict[str, str], row: GroupedRow):
         """
         This is a little bit tricky
 
         >>> GenericMetadataParser.collapse_arbitrary_meta({'key1': 'new_key'}, {'key1': True})
         {'new_key': True}
 
         >>> GenericMetadataParser.collapse_arbitrary_meta({'key1': 'new_key'}, [{'key1': True}, {'key1': True}])
@@ -446,44 +464,59 @@
         # multiple keys sometimes is ordered, so check the sorted(dict.items())
         >>> import json; json.dumps(GenericMetadataParser.collapse_arbitrary_meta({'key1': 'new.key', 'key2': 'new.another'}, [{'key1': 1}, {'key1': 2}, {'key2': False}]), sort_keys=True)
         '{"new": {"another": false, "key": [1, 2]}}'
         """
         if not key_map or not row:
             return {}
 
-        def prepare_dict_from_keys(key_parts: List[str], val):
+        def unstring_value(value: Any) -> bool:
+            """Convert strings to boolean or number if possible"""
+            if not isinstance(value, str):
+                return value
+            if value.lower() == 'true':
+                return True
+            if value.lower() == 'false':
+                return False
+            try:
+                return int(value)
+            except ValueError:
+                try:
+                    return float(value)
+                except ValueError:
+                    return value
+
+        def prepare_dict_from_keys(key_parts: list[str], val):
             """Recursive production of dictionary"""
             if len(key_parts) == 1:
                 return {key_parts[0]: val}
             return {key_parts[0]: prepare_dict_from_keys(key_parts[1:], val)}
 
         dicts = []
         for row_key, dict_key in key_map.items():
             if isinstance(row, list):
-                inner_values = [r[row_key] for r in row if r.get(row_key) is not None]
+                inner_values = [unstring_value(r[row_key]) for r in row if r.get(row_key) is not None]
                 if any(isinstance(inner, list) for inner in inner_values):
                     # lists are unhashable
                     value = inner_values
                 else:
-                    value = list(set(inner_values))
+                    value = sorted(set(inner_values), key=str)  # sorted for unit test consistency
                     if len(value) == 0:
                         continue
                     if len(value) == 1:
-                        value = value[0]
+                        value = unstring_value(value[0])
             else:
                 if row_key not in row:
                     continue
-                value = row[row_key]
-
+                value = unstring_value(row[row_key])
             dicts.append(prepare_dict_from_keys(dict_key.split('.'), value))
 
         return reduce(GenericMetadataParser.merge_dicts, dicts)
 
     @staticmethod
-    def process_filename_value(string: Union[str, List[str]]) -> List[str]:
+    def process_filename_value(string: str | list[str]) -> list[str]:
         """
         Split on multiple delimiters, ;,
 
         >>> GenericMetadataParser.process_filename_value('Filename1-fastq.gz;Filename2.fastq.gz')
         ['Filename1-fastq.gz', 'Filename2.fastq.gz']
 
         >>> GenericMetadataParser.process_filename_value('Filename1-fastq.gz, Filename2.fastq.gz')
@@ -515,43 +548,43 @@
                 'Whitespace detected in filenames: '
                 + ','.join(shlex.quote(str(s)) for s in whitespace_filenames)
             )
 
         return filenames
 
     async def get_read_filenames(
-        self, sample_id: Optional[str], row: SingleRow
-    ) -> List[str]:
+        self, sample_id: str | None, row: SingleRow
+    ) -> list[str]:
         """Get paths to reads from a row"""
         if not self.reads_column or self.reads_column not in row:
             return []
         # more post-processing
         return self.process_filename_value(row[self.reads_column])
 
     async def get_checksums_from_row(
-        self, sample_id: Optional[str], row: SingleRow, read_filenames: List[str]
-    ) -> Optional[List[Optional[str]]]:
+        self, sample_id: str | None, row: SingleRow, read_filenames: list[str]
+    ) -> list[str | None] | None:
         """
         Get checksums for some row, you must either return:
             - no elements, or
             - number of elements equal to read_filenames
 
         Each element should be a string or None.
         """
         if not self.checksum_column or self.checksum_column not in row:
             return []
 
         return self.process_filename_value(row[self.checksum_column])
 
-    async def get_gvcf_filenames(self, sample_id: str, row: GroupedRow) -> List[str]:
+    async def get_gvcf_filenames(self, sample_id: str, row: GroupedRow) -> list[str]:
         """Get paths to gvcfs from a row"""
         if not self.gvcf_column:
             return []
 
-        gvcf_filenames: List[str] = []
+        gvcf_filenames: list[str] = []
         for r in row if isinstance(row, list) else [row]:
             if self.gvcf_column in r:
                 gvcf_filenames.extend(self.process_filename_value(r[self.gvcf_column]))
 
         return gvcf_filenames
 
     async def get_sample_meta_from_group(self, rows: GroupedRow):
@@ -569,49 +602,49 @@
         meta: dict[str, Any] = {}
 
         if not sequencing_group.sample.external_sid:
             sequencing_group.sample.external_sid = (
                 await self.get_cpg_sample_id_from_row(sequencing_group.rows[0])
             )
 
-        gvcf_filenames: List[str] = []
+        gvcf_filenames: list[str] = []
 
         for r in sequencing_group.rows:
             if self.gvcf_column and self.gvcf_column in r:
                 gvcf_filenames.extend(self.process_filename_value(r[self.gvcf_column]))
 
         # strip in case collaborator put "file1, file2"
-        full_gvcf_filenames: List[str] = []
+        full_gvcf_filenames: list[str] = []
 
         if gvcf_filenames:
             full_gvcf_filenames.extend(
                 self.file_path(f.strip()) for f in gvcf_filenames if f.strip()
             )
 
-        variant_file_types: Dict[str, Dict[str, List]] = await self.parse_files(
+        variant_file_types: dict[str, dict[str, list]] = await self.parse_files(
             sequencing_group.sample.external_sid, full_gvcf_filenames, None
         )
-        variants: Dict[str, List] = variant_file_types.get('variants')
+        variants: dict[str, list] = variant_file_types.get('variants')
 
         if variants:
             if 'gvcf' in variants:
                 meta['gvcfs'] = variants.get('gvcf')
                 meta['gvcf_types'] = 'gvcf'
 
             if 'vcf' in variants:
                 meta['vcfs'] = variants['vcf']
                 meta['vcf_type'] = 'vcf'
 
         return meta
 
     async def get_read_and_ref_files_and_checksums(self, sample_id: str, rows: GroupedRow) -> (
-            Tuple[List[str], List[str], Set[str]]):
+            tuple[list[str], list[str], set[str]]):
         """Get read filenames and checksums from rows."""
-        read_filenames: List[str] = []
-        read_checksums: List[str] = []
+        read_filenames: list[str] = []
+        read_checksums: list[str] = []
         reference_assemblies: set[str] = set()
         for r in rows:
             _rfilenames = await self.get_read_filenames(sample_id=sample_id, row=r)
             read_filenames.extend(_rfilenames)
             if self.checksum_column and self.checksum_column in r:
                 checksums = await self.get_checksums_from_row(sample_id, r, _rfilenames)
                 if not checksums:
@@ -667,23 +700,23 @@
         assays = []
 
         read_filenames, read_checksums, reference_assemblies = await self.get_read_and_ref_files_and_checksums(
             sample.external_sid, rows
         )
 
         # strip in case collaborator put "file1, file2"
-        full_read_filenames: List[str] = []
+        full_read_filenames: list[str] = []
         if read_filenames:
             full_read_filenames.extend(
                 self.file_path(f.strip()) for f in read_filenames if f.strip()
             )
-        read_file_types: Dict[str, Dict[str, List]] = await self.parse_files(
+        read_file_types: dict[str, dict[str, list]] = await self.parse_files(
             sample.external_sid, full_read_filenames, read_checksums
         )
-        reads: Dict[str, List] = read_file_types.get('reads')
+        reads: dict[str, list] = read_file_types.get('reads')
         if not reads:
             return []
 
         keys = list(reads.keys())
         if len(keys) > 1:
             # 2021-12-14 mfranklin: In future we should return multiple
             #       assay meta, and handle that in the generic parser
@@ -780,44 +813,39 @@
 
 @click.command(help=__DOC)
 @click.option(
     '--project',
     required=True,
     help='The metamist project ($DATASET) to import manifest into',
 )
+@click.option('--search-path', multiple=True, required=True)
 @click.option('--sample-name-column', required=True)
 @click.option(
     '--participant-column',
     help='Column where the external participant id is held',
 )
 @click.option(
-    '--reads-column',
-    help='Column where the reads information is held, comma-separated if multiple',
-)
-@click.option(
-    '--gvcf-column',
-    help='Column where the reads information is held, comma-separated if multiple',
-)
-@click.option(
     '--reported-sex-column',
     help='Column where the reported sex is held',
 )
 @click.option(
     '--reported-gender-column',
     help='Column where the reported gender is held',
 )
 @click.option(
     '--karyotype-column',
     help='Column where the karyotype is held',
 )
 @click.option(
-    '--qc-meta-field-map',
-    nargs=2,
-    multiple=True,
-    help='Two arguments per listing, eg: --qc-meta-field "name-in-manifest" "name-in-analysis.meta"',
+    '--reads-column',
+    help='Column where the reads information is held, comma-separated if multiple',
+)
+@click.option(
+    '--gvcf-column',
+    help='Column where the reads information is held, comma-separated if multiple',
 )
 @click.option(
     '--participant-meta-field',
     multiple=True,
     help='Single argument, key to pull out of row to put in participant.meta',
 )
 @click.option(
@@ -844,55 +872,58 @@
 )
 @click.option(
     '--assay-meta-field-map',
     nargs=2,
     multiple=True,
     help='Two arguments per listing, eg: --assay-meta-field "name-in-manifest" "name-in-assay.meta"',
 )
+@click.option(
+    '--qc-meta-field-map',
+    nargs=2,
+    multiple=True,
+    help='Two arguments per listing, eg: --qc-meta-field "name-in-manifest" "name-in-analysis.meta"',
+)
 @click.option('--default-sample-type', default='blood')
-@click.option('--default-assay-type', default='wgs')
 @click.option(
     '--confirm', is_flag=True, help='Confirm with user input before updating server'
 )
-@click.option('--search-path', multiple=True, required=True)
 @click.argument('manifests', nargs=-1)
 @run_as_sync
 async def main(
     manifests,
-    search_path: list[str],
     project,
+    search_path: list[str],
     sample_name_column: str,
-    participant_meta_field: List[str],
-    participant_meta_field_map: List[Tuple[str, str]],
-    sample_meta_field: List[str],
-    sample_meta_field_map: List[Tuple[str, str]],
-    assay_meta_field: List[str],
-    assay_meta_field_map: List[Tuple[str, str]],
-    qc_meta_field_map: List[Tuple[str, str]] = None,
-    reads_column: Optional[str] = None,
-    gvcf_column: Optional[str] = None,
-    participant_column: Optional[str] = None,
-    reported_sex_column: Optional[str] = None,
-    reported_gender_column: Optional[str] = None,
-    karyotype_column: Optional[str] = None,
-    default_sample_type: Optional[str] = None,
-    default_assay_type='sequencing',
+    participant_column: str | None = None,
+    reported_sex_column: str | None = None,
+    reported_gender_column: str | None = None,
+    karyotype_column: str | None = None,
+    participant_meta_field: list[str] | None = None,
+    participant_meta_field_map: list[tuple[str, str]] | None = None,
+    sample_meta_field: list[str] | None = None,
+    sample_meta_field_map: list[tuple[str, str]] | None = None,
+    assay_meta_field: list[str] | None = None,
+    assay_meta_field_map: list[tuple[str, str]] | None = None,
+    qc_meta_field_map: list[tuple[str, str]] = None,
+    reads_column: str | None = None,
+    gvcf_column: str | None = None,
+    default_sample_type: str | None = None,
     confirm=False,
 ):
     """Run script from CLI arguments"""
     if not manifests:
         raise ValueError('Expected at least 1 manifest')
 
     extra_search_paths = [m for m in manifests if m.startswith('gs://')]
     if extra_search_paths:
         search_path = list(set(search_path).union(set(extra_search_paths)))
 
-    participant_meta_map: Dict[Any, Any] = {}
-    sample_meta_map: Dict[Any, Any] = {}
-    assay_meta_map: Dict[Any, Any] = {}
+    participant_meta_map: dict[Any, Any] = {}
+    sample_meta_map: dict[Any, Any] = {}
+    assay_meta_map: dict[Any, Any] = {}
 
     qc_meta_map = dict(qc_meta_field_map or {})
     if participant_meta_field_map:
         participant_meta_map.update(dict(participant_meta_map))
     if participant_meta_field:
         participant_meta_map.update({k: k for k in participant_meta_field})
     if sample_meta_field_map:
@@ -904,23 +935,23 @@
     if assay_meta_field:
         assay_meta_map.update({k: k for k in assay_meta_field})
 
     parser = GenericMetadataParser(
         project=project,
         sample_name_column=sample_name_column,
         participant_column=participant_column,
+        reported_sex_column=reported_sex_column,
+        reported_gender_column=reported_gender_column,
+        karyotype_column=karyotype_column,
         participant_meta_map=participant_meta_map,
         sample_meta_map=sample_meta_map,
         assay_meta_map=assay_meta_map,
         qc_meta_map=qc_meta_map,
         reads_column=reads_column,
         gvcf_column=gvcf_column,
-        reported_sex_column=reported_sex_column,
-        reported_gender_column=reported_gender_column,
-        karyotype_column=karyotype_column,
         default_sample_type=default_sample_type,
         default_sequencing=DefaultSequencing(
             seq_type='genome', technology='short-read', platform='illumina'
         ),
         search_locations=search_path,
     )
     for manifest in manifests:
```

### Comparing `metamist-7.0.0/metamist/parser/generic_parser.py` & `metamist-7.0.1/metamist/parser/generic_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1080,14 +1080,17 @@
             elif assay.meta.get('sequencing_type') in RNA_SEQ_TYPES:
                 keys = (
                     'sequencing_facility',
                     'sequencing_library',
                     'read_end_type',
                     'read_length',
                 )
+            elif assay.meta.get('sequencing_technology') == 'long-read':
+                # lift all assay meta into the sequencing group meta for long-read
+                keys = [k for k in assay.meta.keys() if k not in ('reads', 'reads_type')]
             else:
                 continue
             for key in keys:
                 if assay.meta.get(key) is not None:
                     meta[key] = assay.meta[key]
         return meta
```

### Comparing `metamist-7.0.0/metamist/parser/sample_file_map_parser.py` & `metamist-7.0.1/metamist/parser/sample_file_map_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #!/usr/bin/env python3
-# pylint: disable=too-many-instance-attributes,too-many-locals,unused-argument,wrong-import-order,unused-argument
 import logging
-from typing import List
 
 import click
 
 from metamist.parser.generic_metadata_parser import GenericMetadataParser, run_as_sync
 from metamist.parser.generic_parser import DefaultSequencing, SingleRow
 
 PARTICIPANT_COL_NAME = 'individual_id'
@@ -91,25 +89,26 @@
 
 
 class SampleFileMapParser(GenericMetadataParser):
     """Parser for SampleFileMap"""
 
     def __init__(
         self,
-        search_locations: List[str],
+        search_locations: list[str],
         project: str,
         default_sample_type='blood',
         default_sequencing=DefaultSequencing(
             seq_type='genome', technology='short-read', platform='illumina'
         ),
         default_read_end_type: str = None,
         default_read_length: str | int = None,
         allow_extra_files_in_search_path=False,
         default_reference_assembly_location: str | None = None,
         verbose=True,
+        **kwargs,
     ):
         super().__init__(
             search_locations=search_locations,
             project=project,
             participant_column=PARTICIPANT_COL_NAME,
             sample_name_column=SAMPLE_ID_COL_NAME,
             reads_column=READS_COL_NAME,
@@ -120,21 +119,18 @@
             read_end_type_column=READ_END_TYPE_COL_NAME,
             read_length_column=READ_LENGTH_COL_NAME,
             default_sample_type=default_sample_type,
             default_sequencing=default_sequencing,
             default_read_end_type=default_read_end_type,
             default_read_length=default_read_length,
             default_reference_assembly_location=default_reference_assembly_location,
-            participant_meta_map={},
-            sample_meta_map={},
-            assay_meta_map={},
-            qc_meta_map={},
             allow_extra_files_in_search_path=allow_extra_files_in_search_path,
             key_map=KeyMap,
             verbose=verbose,
+            **kwargs,
         )
 
     def get_sample_id(self, row: SingleRow) -> str:
         """Get external sample ID from row"""
 
         if self.sample_name_column and self.sample_name_column in row:
             return row[self.sample_name_column]
@@ -188,15 +184,15 @@
     '--dry-run', is_flag=True, help='Just prepare the run, without comitting it'
 )
 @click.option('--verbose', '-v', is_flag=True, help='Verbose output')
 @click.argument('manifests', nargs=-1)
 @run_as_sync
 async def main(  # pylint: disable=too-many-arguments
     manifests,
-    search_path: List[str],
+    search_path: list[str],
     project,
     default_sample_type='blood',
     default_sequencing_type='genome',
     default_sequencing_technology='short-read',
     default_sequencing_platform='illumina',
     default_sequencing_facility: str = None,
     default_sequencing_library: str = None,
```

### Comparing `metamist-7.0.0/metamist/rest.py` & `metamist-7.0.1/metamist/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 7.0.0
+    The version of the OpenAPI document: 7.0.1
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `metamist-7.0.0/metamist.egg-info/PKG-INFO` & `metamist-7.0.1/metamist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 7.0.0
+Version: 7.0.1
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/metamist
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-7.0.0/metamist.egg-info/SOURCES.txt` & `metamist-7.0.1/metamist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/pyproject.toml` & `metamist-7.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/setup.py` & `metamist-7.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='7.0.0',
+    version='7.0.1',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/metamist',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `metamist-7.0.0/test/test_analysis.py` & `metamist-7.0.1/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_analysis_runner.py` & `metamist-7.0.1/test/test_analysis_runner.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_api_billing.py` & `metamist-7.0.1/test/test_api_billing.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_api_utils.py` & `metamist-7.0.1/test/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_assay.py` & `metamist-7.0.1/test/test_assay.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_audit_log.py` & `metamist-7.0.1/test/test_audit_log.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_bq_billing_ar_batch.py` & `metamist-7.0.1/test/test_bq_billing_ar_batch.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_bq_billing_base.py` & `metamist-7.0.1/test/test_bq_billing_base.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_bq_billing_daily.py` & `metamist-7.0.1/test/test_bq_billing_daily.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_bq_billing_daily_extended.py` & `metamist-7.0.1/test/test_bq_billing_daily_extended.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_bq_billing_gcp_daily.py` & `metamist-7.0.1/test/test_bq_billing_gcp_daily.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_bq_billing_raw.py` & `metamist-7.0.1/test/test_bq_billing_raw.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_bq_function_filter.py` & `metamist-7.0.1/test/test_bq_function_filter.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_bq_generic_filter.py` & `metamist-7.0.1/test/test_bq_generic_filter.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_cohort.py` & `metamist-7.0.1/test/test_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_cohort_builder.py` & `metamist-7.0.1/test/test_cohort_builder.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_generate_data.py` & `metamist-7.0.1/test/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_generic_auditor.py` & `metamist-7.0.1/test/test_generic_auditor.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_generic_filters.py` & `metamist-7.0.1/test/test_generic_filters.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_get_participants.py` & `metamist-7.0.1/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_graphql.py` & `metamist-7.0.1/test/test_graphql.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_import_individual_metadata.py` & `metamist-7.0.1/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_layers_billing.py` & `metamist-7.0.1/test/test_layers_billing.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_metamist.py` & `metamist-7.0.1/test/test_metamist.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_models.py` & `metamist-7.0.1/test/test_models.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_parse_existing_cohort.py` & `metamist-7.0.1/test/test_parse_existing_cohort.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,16 @@
         self.assertEqual(0, summary['assays']['update'])
 
         sample_to_add = participants[0].samples[0]
         self.assertEqual('EXTID1234', sample_to_add.external_sid)
         expected_sequence_dict = {
             'reference_genome': 'hg38',
             'platform': 'App',
-            'concentration': '100',
-            'volume': '100',
+            'concentration': 100,
+            'volume': 100,
             'fluid_x_tube_id': '220405_FLUIDX1234',
             'reads_type': 'fastq',
             'reads': [
                 {
                     'location': '/path/to/HG3F_2_220405_FLUIDX1234_Homo-sapiens_AAC-TAT_R_220208_VB_BLAH_M002_R1.fastq',
                     'basename': 'HG3F_2_220405_FLUIDX1234_Homo-sapiens_AAC-TAT_R_220208_VB_BLAH_M002_R1.fastq',
                     'class': 'File',
@@ -364,16 +364,16 @@
                     StringIO(file_contents), delimiter='\t', dry_run=True
                 )
 
                 sample_to_add = participants[0].samples[0]
                 expected_sequence_dict = {
                     'reference_genome': 'hg38',
                     'platform': 'App',
-                    'concentration': '100',
-                    'volume': '100',
+                    'concentration': 100,
+                    'volume': 100,
                     'fluid_x_tube_id': '220405_FLUIDX1234',
                     'reads_type': 'fastq',
                     'reads': [
                         {
                             'location': '/path/to/HG3F_2_220405_FLUIDX1234_Homo-sapiens_AAC-TAT_R_220208_VB_BLAH_M002_R1.fastq',
                             'basename': 'HG3F_2_220405_FLUIDX1234_Homo-sapiens_AAC-TAT_R_220208_VB_BLAH_M002_R1.fastq',
                             'class': 'File',
```

### Comparing `metamist-7.0.0/test/test_parse_file_map.py` & `metamist-7.0.1/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_parse_generic_metadata.py` & `metamist-7.0.1/test/test_parse_generic_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from io import StringIO
 from test.testbase import DbIsolatedTest, run_as_sync
 from unittest.mock import patch
 
 import api.graphql.schema
 from db.python.layers import ParticipantLayer
 from metamist.graphql import configure_sync_client, validate
-from metamist.parser.generic_metadata_parser import GenericMetadataParser
+from metamist.parser.generic_metadata_parser import (
+    DefaultSequencing,
+    GenericMetadataParser,
+)
 from metamist.parser.generic_parser import (
     QUERY_MATCH_ASSAYS,
     QUERY_MATCH_PARTICIPANTS,
     QUERY_MATCH_SAMPLES,
     QUERY_MATCH_SEQUENCING_GROUPS,
     ParsedParticipant,
     ParsedSample,
@@ -228,18 +231,18 @@
         self.assertEqual(0, summary['samples']['update'])
         self.assertEqual(0, summary['assays']['update'])
         self.assertEqual(1, summary['analyses']['insert'])
 
         self.assertDictEqual({'centre': 'KCCG'}, samples[0].meta)
         expected_assay_dict = {
             'qc': {
-                'median_insert_size': '400',
-                'median_coverage': '30',
-                'freemix': '0.01',
-                'pct_chimeras': '0.01',
+                'median_insert_size': 400,
+                'median_coverage': 30,
+                'freemix': 0.01,
+                'pct_chimeras': 0.01,
             },
             'reads_type': 'bam',
             'reads': {
                 'location': '/path/to/<sample-id>.bam',
                 'basename': '<sample-id>.bam',
                 'class': 'File',
                 'checksum': None,
@@ -267,18 +270,18 @@
         self.assertDictEqual(assay_group_dict, samples[0].sequencing_groups[0].meta)
         self.assertDictEqual(
             expected_assay_dict, samples[0].sequencing_groups[0].assays[0].meta
         )
         analysis = samples[0].sequencing_groups[0].analyses[0]
         self.assertDictEqual(
             {
-                'median_insert_size': '400',
-                'median_coverage': '30',
-                'freemix': '0.01',
-                'pct_chimeras': '0.01',
+                'median_insert_size': 400,
+                'median_coverage': 30,
+                'freemix': 0.01,
+                'pct_chimeras': 0.01,
             },
             analysis.meta,
         )
 
     @run_as_sync
     @patch('metamist.parser.generic_parser.query_async')
     async def test_rows_with_participants(self, mock_graphql_query):
@@ -478,14 +481,133 @@
             await parser.parse_manifest(
                 StringIO(file_contents), delimiter='\t', dry_run=True
             )
         return
 
     @run_as_sync
     @patch('metamist.parser.generic_parser.query_async')
+    async def test_lrs_rows_with_arbitrary_assay_meta_columns(
+        self,
+        mock_graphql_query
+    ):
+        """
+        Test importing a single row of long read sequencing data with arbitrary assay metadata columns
+        """
+        mock_graphql_query.side_effect = self.run_graphql_query_async
+        self.maxDiff = None
+        rows = [
+            'Individual ID\tSample ID\tFilename\tAssay Meta 1\tAssay Meta 2',
+            'Athena\tsample_id003\t"sample_id003.filename-01-R1.fastq.gz,sample_id003.filename-01-R2.fastq.gz"\tTrue\tsome_value',
+            'Athena\tsample_id003\t"sample_id003.filename-02-R1.fastq.gz,sample_id003.filename-02-R2.fastq.gz"\t5\tFalse',
+        ]
+        parser = GenericMetadataParser(
+            search_locations=[],
+            participant_column='Individual ID',
+            sample_name_column='Sample ID',
+            reads_column='Filename',
+            assay_meta_map={'Assay Meta 1': 'assay_meta1', 'Assay Meta 2': 'assay_meta2'},
+            default_sequencing=DefaultSequencing(
+                seq_type='genome',
+                technology='long-read',
+                platform='pacbio',
+            ),
+            # doesn't matter, we're going to mock the call anyway
+            project=self.project_name,
+            skip_checking_gcs_objects=True,
+        )
+
+        parser.filename_map = {
+            'sample_id003.filename-01-R1.fastq.gz': '/path/to/sample_id003.filename-01-R1.fastq.gz',
+            'sample_id003.filename-01-R2.fastq.gz': '/path/to/sample_id003.filename-01-R2.fastq.gz',
+            'sample_id003.filename-02-R1.fastq.gz': '/path/to/sample_id003.filename-02-R1.fastq.gz',
+            'sample_id003.filename-02-R2.fastq.gz': '/path/to/sample_id003.filename-02-R2.fastq.gz',
+        }
+
+        # Call generic parser
+        file_contents = '\n'.join(rows)
+
+        _, prows = await parser.parse_manifest(
+            StringIO(file_contents), delimiter='\t', dry_run=True
+        )
+
+        participants: list[ParsedParticipant] = prows
+
+        expected_assay_1_dict = {
+            'reads': [
+                {
+                    'basename': 'sample_id003.filename-01-R1.fastq.gz',
+                    'checksum': None,
+                    'class': 'File',
+                    'location': '/path/to/sample_id003.filename-01-R1.fastq.gz',
+                    'size': None,
+                    'datetime_added': None,
+                },
+                {
+                    'basename': 'sample_id003.filename-01-R2.fastq.gz',
+                    'checksum': None,
+                    'class': 'File',
+                    'location': '/path/to/sample_id003.filename-01-R2.fastq.gz',
+                    'size': None,
+                    'datetime_added': None,
+                },
+            ],
+            'reads_type': 'fastq',
+            'sequencing_platform': 'pacbio',
+            'sequencing_technology': 'long-read',
+            'sequencing_type': 'genome',
+            'assay_meta1': [5, True],
+            'assay_meta2': [False, 'some_value'],
+        }
+
+        expected_assay_2_dict = {
+            'reads': [
+                {
+                    'basename': 'sample_id003.filename-02-R1.fastq.gz',
+                    'checksum': None,
+                    'class': 'File',
+                    'location': '/path/to/sample_id003.filename-02-R1.fastq.gz',
+                    'size': None,
+                    'datetime_added': None,
+                },
+                {
+                    'basename': 'sample_id003.filename-02-R2.fastq.gz',
+                    'checksum': None,
+                    'class': 'File',
+                    'location': '/path/to/sample_id003.filename-02-R2.fastq.gz',
+                    'size': None,
+                    'datetime_added': None,
+                },
+            ],
+            'reads_type': 'fastq',
+            'sequencing_platform': 'pacbio',
+            'sequencing_technology': 'long-read',
+            'sequencing_type': 'genome',
+            'assay_meta1': [5, True],
+            'assay_meta2': [False, 'some_value'],
+        }
+
+        expected_sg_dict = {
+            'sequencing_platform': 'pacbio',
+            'sequencing_technology': 'long-read',
+            'sequencing_type': 'genome',
+            'assay_meta1': [5, True],
+            'assay_meta2': [False, 'some_value'],
+        }
+
+        assay_1 = participants[0].samples[0].sequencing_groups[0].assays[0]
+        assay_2 = participants[0].samples[0].sequencing_groups[0].assays[1]
+        sg = participants[0].samples[0].sequencing_groups[0]
+
+        self.assertDictEqual(expected_assay_1_dict, assay_1.meta)
+        self.assertDictEqual(expected_assay_2_dict, assay_2.meta)
+        self.assertDictEqual(expected_sg_dict, sg.meta)
+        return
+
+    @run_as_sync
+    @patch('metamist.parser.generic_parser.query_async')
     @patch('metamist.parser.cloudhelper.CloudHelper.file_exists')
     @patch('metamist.parser.cloudhelper.CloudHelper.file_size')
     @patch('metamist.parser.cloudhelper.CloudHelper.file_contents')
     async def test_cram_with_no_reference(
         self,
         mock_filecontents,
         mock_filesize,
```

### Comparing `metamist-7.0.0/test/test_parse_ont_processor.py` & `metamist-7.0.1/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_parse_ont_sheet.py` & `metamist-7.0.1/test/test_parse_ont_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         meta_dict = {
             'barcoding': 'None',
             'basecalling': '4.0.11+f1071ce',
             'device': 'PromethION',
             'experiment_name': 'PBXP_Awesome',
             'flow_cell': 'PRO002',
             'flowcell_id': 'XYZ1',
-            'mux_total': '7107',
+            'mux_total': 7107,
             'protocol': 'LSK1',
             'reads': [
                 {
                     'basename': 'Sample01_pass.fastq.gz',
                     'checksum': None,
                     'class': 'File',
                     'location': 'gs://BUCKET/FAKE/Sample01_pass.fastq.gz',
```

### Comparing `metamist-7.0.0/test/test_pedigree.py` & `metamist-7.0.1/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_project_groups.py` & `metamist-7.0.1/test/test_project_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_sample.py` & `metamist-7.0.1/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_search.py` & `metamist-7.0.1/test/test_search.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_sequencing_groups.py` & `metamist-7.0.1/test/test_sequencing_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_update_participant_family.py` & `metamist-7.0.1/test/test_update_participant_family.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_upsert.py` & `metamist-7.0.1/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/test_web.py` & `metamist-7.0.1/test/test_web.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/testbase.py` & `metamist-7.0.1/test/testbase.py`

 * *Files identical despite different names*

### Comparing `metamist-7.0.0/test/testbqbase.py` & `metamist-7.0.1/test/testbqbase.py`

 * *Files identical despite different names*

