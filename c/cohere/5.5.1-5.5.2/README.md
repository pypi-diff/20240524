# Comparing `tmp/cohere-5.5.1.tar.gz` & `tmp/cohere-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.5.1.tar", max compression
+gzip compressed data, was "cohere-5.5.2.tar", max compression
```

## Comparing `cohere-5.5.1.tar` & `cohere-5.5.2.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0     1062 2024-05-22 14:34:21.058162 cohere-5.5.1/LICENSE
--rw-r--r--   0        0        0     2359 2024-05-22 14:34:21.058162 cohere-5.5.1/README.md
--rw-r--r--   0        0        0     1458 2024-05-22 14:34:21.066162 cohere-5.5.1/pyproject.toml
--rw-r--r--   0        0        0     8381 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/__init__.py
--rw-r--r--   0        0        0   211417 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/base_client.py
--rw-r--r--   0        0        0     9142 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/bedrock_client.py
--rw-r--r--   0        0        0    19723 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    53293 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/connectors/client.py
--rw-r--r--   0        0        0     1126 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      748 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/pydantic_utilities.py
--rw-r--r--   0        0        0     1266 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/query_encoder.py
--rw-r--r--   0        0        0      330 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/request_options.py
--rw-r--r--   0        0        0     7165 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/unchecked_base_model.py
--rw-r--r--   0        0        0      419 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    38300 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      578 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0     1265 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0     1665 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py
--rw-r--r--   0        0        0     1222 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1320 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0     1261 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    32495 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      169 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      160 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      326 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    65157 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1738 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      305 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1438 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1346 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1663 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2620 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1434 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     2086 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1752 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1795 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1726 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1840 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      402 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      193 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1653 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1440 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0      811 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/manually_maintained/cache.py
--rw-r--r--   0        0        0     3015 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/manually_maintained/tokenizers.py
--rw-r--r--   0        0        0       65 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    14701 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/py.typed
--rw-r--r--   0        0        0    10564 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1523 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0     1274 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1697 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0     1440 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/api_meta_tokens.py
--rw-r--r--   0        0        0      168 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     2192 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1390 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     2124 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1560 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1804 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      170 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1971 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0      189 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0     1443 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1510 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1916 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0     1318 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1680 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     2124 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      225 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0     1156 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      176 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1977 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0      195 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0     1365 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1331 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1303 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1268 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/check_api_key_response.py
--rw-r--r--   0        0        0     1267 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0     1234 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      171 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1400 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2823 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      214 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0     1234 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      220 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3646 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/connector.py
--rw-r--r--   0        0        0      163 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1923 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1988 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0     1223 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1458 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0     1310 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2472 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     2051 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      427 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      222 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1331 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1679 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2534 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1627 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      211 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     2127 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      201 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      156 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      168 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0     2831 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      184 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1998 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      222 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      185 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      171 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1460 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1364 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1574 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0     1160 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      191 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      177 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1575 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     4579 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1517 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generation.py
--rw-r--r--   0        0        0     1220 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     2413 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1519 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1358 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0     1256 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1450 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0     4531 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/message.py
--rw-r--r--   0        0        0     1393 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     1378 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/metrics_embed_data.py
--rw-r--r--   0        0        0     1417 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/metrics_embed_data_fields_item.py
--rw-r--r--   0        0        0     3203 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1343 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0     1237 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0     1264 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1463 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     2172 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1399 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     2081 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     2082 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1511 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0     1215 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     9119 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      179 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      170 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      173 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1464 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1390 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0     1204 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/too_many_requests_error_body.py
--rw-r--r--   0        0        0     2191 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1484 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1320 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool_message.py
--rw-r--r--   0        0        0     1594 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0     1258 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool_result.py
--rw-r--r--   0        0        0     1223 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10055 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/version.py
--rw-r--r--   0        0        0     3561 1970-01-01 00:00:00.000000 cohere-5.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-23 11:38:37.564954 cohere-5.5.2/LICENSE
+-rw-r--r--   0        0        0     2359 2024-05-23 11:38:37.564954 cohere-5.5.2/README.md
+-rw-r--r--   0        0        0     1458 2024-05-23 11:38:37.572954 cohere-5.5.2/pyproject.toml
+-rw-r--r--   0        0        0     8381 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/__init__.py
+-rw-r--r--   0        0        0   211417 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/base_client.py
+-rw-r--r--   0        0        0     9142 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/bedrock_client.py
+-rw-r--r--   0        0        0    19723 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    53293 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0     1126 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1266 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0     7165 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      419 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    38300 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      578 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0     1265 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0     1665 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py
+-rw-r--r--   0        0        0     1222 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1320 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0     1261 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    32495 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      160 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      326 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    65157 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1738 2024-05-23 11:38:37.572954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      305 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1438 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1346 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1663 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2620 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1434 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     2086 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1752 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1795 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1726 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1840 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      402 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      193 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1653 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1440 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     3834 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    14701 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/py.typed
+-rw-r--r--   0        0        0    10564 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1523 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1274 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1697 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0     1440 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/api_meta_tokens.py
+-rw-r--r--   0        0        0      168 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     2192 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1390 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     2124 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1560 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1804 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      170 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1971 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      189 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1443 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1510 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1916 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1318 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1680 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     2124 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      225 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0     1156 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      176 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1977 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      195 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1365 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1331 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1303 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1268 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/check_api_key_response.py
+-rw-r--r--   0        0        0     1267 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0     1234 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      171 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1400 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2823 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      214 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0     1234 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      220 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3646 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      163 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1923 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1988 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0     1223 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1458 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1310 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2472 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     2051 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      427 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      222 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1331 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1679 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2534 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1627 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      211 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     2127 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      201 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      156 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      168 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     2831 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      184 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1998 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      222 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      185 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      171 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1460 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1364 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1574 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0     1160 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      191 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      177 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1575 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     4579 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1517 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/generation.py
+-rw-r--r--   0        0        0     1220 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     2413 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1519 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1358 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0     1256 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1450 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     4531 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/message.py
+-rw-r--r--   0        0        0     1393 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     1378 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/metrics_embed_data.py
+-rw-r--r--   0        0        0     1417 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/metrics_embed_data_fields_item.py
+-rw-r--r--   0        0        0     3203 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1343 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0     1237 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1264 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1463 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     2172 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1399 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     2081 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     2082 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1511 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0     1215 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     9119 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      179 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      170 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      173 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1464 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1390 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0     1204 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0     2191 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1484 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1320 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/tool_message.py
+-rw-r--r--   0        0        0     1594 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0     1258 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/tool_result.py
+-rw-r--r--   0        0        0     1223 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10055 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-05-23 11:38:37.576954 cohere-5.5.2/src/cohere/version.py
+-rw-r--r--   0        0        0     3561 1970-01-01 00:00:00.000000 cohere-5.5.2/PKG-INFO
```

### Comparing `cohere-5.5.1/LICENSE` & `cohere-5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/README.md` & `cohere-5.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/pyproject.toml` & `cohere-5.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "5.5.1"
+version = "5.5.2"
 description = ""
 readme = "README.md"
 authors = []
 keywords = []
 
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `cohere-5.5.1/src/cohere/__init__.py` & `cohere-5.5.2/src/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/base_client.py` & `cohere-5.5.2/src/cohere/base_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/bedrock_client.py` & `cohere-5.5.2/src/cohere/bedrock_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/client.py` & `cohere-5.5.2/src/cohere/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/connectors/client.py` & `cohere-5.5.2/src/cohere/connectors/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/__init__.py` & `cohere-5.5.2/src/cohere/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/client_wrapper.py` & `cohere-5.5.2/src/cohere/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "cohere",
-            "X-Fern-SDK-Version": "5.5.1",
+            "X-Fern-SDK-Version": "5.5.2",
         }
         if self._client_name is not None:
             headers["X-Client-Name"] = self._client_name
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
```

### Comparing `cohere-5.5.1/src/cohere/core/datetime_utils.py` & `cohere-5.5.2/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/file.py` & `cohere-5.5.2/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/http_client.py` & `cohere-5.5.2/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/jsonable_encoder.py` & `cohere-5.5.2/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/pydantic_utilities.py` & `cohere-5.5.2/src/cohere/core/pydantic_utilities.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/query_encoder.py` & `cohere-5.5.2/src/cohere/core/query_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/request_options.py` & `cohere-5.5.2/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/core/unchecked_base_model.py` & `cohere-5.5.2/src/cohere/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/datasets/client.py` & `cohere-5.5.2/src/cohere/datasets/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/datasets/types/__init__.py` & `cohere-5.5.2/src/cohere/datasets/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.5.2/src/cohere/datasets/types/datasets_create_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py` & `cohere-5.5.2/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.5.2/src/cohere/datasets/types/datasets_get_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.5.2/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.5.2/src/cohere/datasets/types/datasets_list_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/embed_jobs/client.py` & `cohere-5.5.2/src/cohere/embed_jobs/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/errors/__init__.py` & `cohere-5.5.2/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/__init__.py` & `cohere-5.5.2/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/client.py` & `cohere-5.5.2/src/cohere/finetuning/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/settings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.5.2/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/manually_maintained/cache.py` & `cohere-5.5.2/src/cohere/manually_maintained/cache.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/models/client.py` & `cohere-5.5.2/src/cohere/models/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/overrides.py` & `cohere-5.5.2/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/__init__.py` & `cohere-5.5.2/src/cohere/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/api_meta.py` & `cohere-5.5.2/src/cohere/types/api_meta.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/api_meta_api_version.py` & `cohere-5.5.2/src/cohere/types/api_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/api_meta_billed_units.py` & `cohere-5.5.2/src/cohere/types/api_meta_billed_units.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/api_meta_tokens.py` & `cohere-5.5.2/src/cohere/types/api_meta_tokens.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_citation.py` & `cohere-5.5.2/src/cohere/types/chat_citation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.5.2/src/cohere/types/chat_citation_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_connector.py` & `cohere-5.5.2/src/cohere/types/chat_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_data_metrics.py` & `cohere-5.5.2/src/cohere/types/chat_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_message.py` & `cohere-5.5.2/src/cohere/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.5.2/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.5.2/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_search_query.py` & `cohere-5.5.2/src/cohere/types/chat_search_query.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_search_result.py` & `cohere-5.5.2/src/cohere/types/chat_search_result.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_search_result_connector.py` & `cohere-5.5.2/src/cohere/types/chat_search_result_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_search_results_event.py` & `cohere-5.5.2/src/cohere/types/chat_search_results_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_stream_end_event.py` & `cohere-5.5.2/src/cohere/types/chat_stream_end_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_stream_event.py` & `cohere-5.5.2/src/cohere/types/chat_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.5.2/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_stream_start_event.py` & `cohere-5.5.2/src/cohere/types/chat_stream_start_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_text_generation_event.py` & `cohere-5.5.2/src/cohere/types/chat_text_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.5.2/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/check_api_key_response.py` & `cohere-5.5.2/src/cohere/types/check_api_key_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/classify_data_metrics.py` & `cohere-5.5.2/src/cohere/types/classify_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/classify_example.py` & `cohere-5.5.2/src/cohere/types/classify_example.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/classify_response.py` & `cohere-5.5.2/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.5.2/src/cohere/types/classify_response_classifications_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.5.2/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/connector.py` & `cohere-5.5.2/src/cohere/types/connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/connector_o_auth.py` & `cohere-5.5.2/src/cohere/types/connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/create_connector_o_auth.py` & `cohere-5.5.2/src/cohere/types/create_connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/create_connector_response.py` & `cohere-5.5.2/src/cohere/types/create_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/create_connector_service_auth.py` & `cohere-5.5.2/src/cohere/types/create_connector_service_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/create_embed_job_response.py` & `cohere-5.5.2/src/cohere/types/create_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/dataset.py` & `cohere-5.5.2/src/cohere/types/dataset.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/dataset_part.py` & `cohere-5.5.2/src/cohere/types/dataset_part.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/detokenize_response.py` & `cohere-5.5.2/src/cohere/types/detokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/embed_by_type_response.py` & `cohere-5.5.2/src/cohere/types/embed_by_type_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.5.2/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/embed_floats_response.py` & `cohere-5.5.2/src/cohere/types/embed_floats_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/embed_job.py` & `cohere-5.5.2/src/cohere/types/embed_job.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/embed_response.py` & `cohere-5.5.2/src/cohere/types/embed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.5.2/src/cohere/types/finetune_dataset_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/generate_stream_end.py` & `cohere-5.5.2/src/cohere/types/generate_stream_end.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/generate_stream_end_response.py` & `cohere-5.5.2/src/cohere/types/generate_stream_end_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/generate_stream_error.py` & `cohere-5.5.2/src/cohere/types/generate_stream_error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/generate_stream_event.py` & `cohere-5.5.2/src/cohere/types/generate_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/generate_stream_text.py` & `cohere-5.5.2/src/cohere/types/generate_stream_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/generate_streamed_response.py` & `cohere-5.5.2/src/cohere/types/generate_streamed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/generation.py` & `cohere-5.5.2/src/cohere/types/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/get_connector_response.py` & `cohere-5.5.2/src/cohere/types/get_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/get_model_response.py` & `cohere-5.5.2/src/cohere/types/get_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/label_metric.py` & `cohere-5.5.2/src/cohere/types/label_metric.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/list_connectors_response.py` & `cohere-5.5.2/src/cohere/types/list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/list_embed_job_response.py` & `cohere-5.5.2/src/cohere/types/list_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/list_models_response.py` & `cohere-5.5.2/src/cohere/types/list_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/message.py` & `cohere-5.5.2/src/cohere/types/message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/metrics.py` & `cohere-5.5.2/src/cohere/types/metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/metrics_embed_data.py` & `cohere-5.5.2/src/cohere/types/metrics_embed_data.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/metrics_embed_data_fields_item.py` & `cohere-5.5.2/src/cohere/types/metrics_embed_data_fields_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.5.2/src/cohere/types/non_streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.5.2/src/cohere/types/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/parse_info.py` & `cohere-5.5.2/src/cohere/types/parse_info.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.5.2/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/rerank_response.py` & `cohere-5.5.2/src/cohere/types/rerank_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/rerank_response_results_item.py` & `cohere-5.5.2/src/cohere/types/rerank_response_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.5.2/src/cohere/types/rerank_response_results_item_document.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/reranker_data_metrics.py` & `cohere-5.5.2/src/cohere/types/reranker_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/single_generation.py` & `cohere-5.5.2/src/cohere/types/single_generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/single_generation_in_stream.py` & `cohere-5.5.2/src/cohere/types/single_generation_in_stream.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/single_generation_token_likelihoods_item.py` & `cohere-5.5.2/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/streamed_chat_response.py` & `cohere-5.5.2/src/cohere/types/streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/summarize_response.py` & `cohere-5.5.2/src/cohere/types/summarize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/tokenize_response.py` & `cohere-5.5.2/src/cohere/types/tokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/too_many_requests_error_body.py` & `cohere-5.5.2/src/cohere/types/too_many_requests_error_body.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/tool.py` & `cohere-5.5.2/src/cohere/types/tool.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/tool_call.py` & `cohere-5.5.2/src/cohere/types/tool_call.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/tool_message.py` & `cohere-5.5.2/src/cohere/types/tool_message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/tool_parameter_definitions_value.py` & `cohere-5.5.2/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/tool_result.py` & `cohere-5.5.2/src/cohere/types/tool_result.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/types/update_connector_response.py` & `cohere-5.5.2/src/cohere/types/update_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/src/cohere/utils.py` & `cohere-5.5.2/src/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.1/PKG-INFO` & `cohere-5.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.5.1
+Version: 5.5.2
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
```

