# Comparing `tmp/vellum_ai-0.5.2.tar.gz` & `tmp/vellum_ai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.5.2.tar", max compression
+gzip compressed data, was "vellum_ai-0.6.0.tar", max compression
```

## Comparing `vellum_ai-0.5.2.tar` & `vellum_ai-0.6.0.tar`

### file list

```diff
@@ -1,386 +1,434 @@
--rw-r--r--   0        0        0     1073 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/LICENSE
--rw-r--r--   0        0        0     2980 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/README.md
--rw-r--r--   0        0        0      632 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    35797 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/__init__.py
--rw-r--r--   0        0        0    97089 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/client.py
--rw-r--r--   0        0        0      853 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1697 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/core/request_options.py
--rw-r--r--   0        0        0      498 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/environment.py
--rw-r--r--   0        0        0      343 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/errors/not_found_error.py
--rw-r--r--   0        0        0       79 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/__init__.py
--rw-r--r--   0        0        0       77 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/test_suites/__init__.py
--rw-r--r--   0        0        0      116 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/test_suites/constants.py
--rw-r--r--   0        0        0       56 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/test_suites/exceptions.py
--rw-r--r--   0        0        0    12323 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/test_suites/resources.py
--rw-r--r--   0        0        0        0 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/utils/__init__.py
--rw-r--r--   0        0        0      298 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/utils/env.py
--rw-r--r--   0        0        0       49 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/utils/exceptions.py
--rw-r--r--   0        0        0      698 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/lib/utils/paginator.py
--rw-r--r--   0        0        0        0 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/py.typed
--rw-r--r--   0        0        0      730 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0      157 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/deployments/__init__.py
--rw-r--r--   0        0        0    19588 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/deployments/client.py
--rw-r--r--   0        0        0      183 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/deployments/types/__init__.py
--rw-r--r--   0        0        0      174 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/deployments/types/deployments_list_request_status.py
--rw-r--r--   0        0        0      165 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/document_indexes/__init__.py
--rw-r--r--   0        0        0    39845 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/document_indexes/client.py
--rw-r--r--   0        0        0      196 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/document_indexes/types/__init__.py
--rw-r--r--   0        0        0      178 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/document_indexes/types/document_indexes_list_request_status.py
--rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0    34010 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/folder_entities/__init__.py
--rw-r--r--   0        0        0     6435 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/folder_entities/client.py
--rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/sandboxes/__init__.py
--rw-r--r--   0        0        0    12738 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/sandboxes/client.py
--rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/test_suite_runs/__init__.py
--rw-r--r--   0        0        0    18728 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/test_suite_runs/client.py
--rw-r--r--   0        0        0       65 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/test_suites/__init__.py
--rw-r--r--   0        0        0    18982 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/test_suites/client.py
--rw-r--r--   0        0        0      173 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/__init__.py
--rw-r--r--   0        0        0    11158 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/client.py
--rw-r--r--   0        0        0      208 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/types/__init__.py
--rw-r--r--   0        0        0      182 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
--rw-r--r--   0        0        0      454 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/__init__.py
--rw-r--r--   0        0        0      473 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/_jsii/__init__.py
--rw-r--r--   0        0        0    15887 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz
--rw-r--r--   0        0        0       43 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/constraints.json
--rw-r--r--   0        0        0    21484 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/data_vellum_document_index/__init__.py
--rw-r--r--   0        0        0    25018 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/document_index/__init__.py
--rw-r--r--   0        0        0    10298 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/provider/__init__.py
--rw-r--r--   0        0        0        1 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/py.typed
--rw-r--r--   0        0        0       56 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/terraform/versions.json
--rw-r--r--   0        0        0    47652 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/__init__.py
--rw-r--r--   0        0        0      983 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/api_node_result.py
--rw-r--r--   0        0        0     1161 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/api_node_result_data.py
--rw-r--r--   0        0        0     1030 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_chat_message_content.py
--rw-r--r--   0        0        0     1297 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_item.py
--rw-r--r--   0        0        0     1421 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_item_request.py
--rw-r--r--   0        0        0     1059 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_request.py
--rw-r--r--   0        0        0      116 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_enum.py
--rw-r--r--   0        0        0     3002 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/array_variable_value_item.py
--rw-r--r--   0        0        0      129 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_history_enum.py
--rw-r--r--   0        0        0     1121 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_history_input_request.py
--rw-r--r--   0        0        0      945 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_history_variable_value.py
--rw-r--r--   0        0        0     1213 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_message.py
--rw-r--r--   0        0        0     1573 2024-05-08 19:20:42.752322 vellum_ai-0.5.2/src/vellum/types/chat_message_content.py
--rw-r--r--   0        0        0     1737 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/chat_message_content_request.py
--rw-r--r--   0        0        0     1242 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/chat_message_request.py
--rw-r--r--   0        0        0      182 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/chat_message_role.py
--rw-r--r--   0        0        0      996 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_array_result.py
--rw-r--r--   0        0        0      967 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_chat_history_result.py
--rw-r--r--   0        0        0      948 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_error_result.py
--rw-r--r--   0        0        0      958 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_function_call_result.py
--rw-r--r--   0        0        0      926 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_json_result.py
--rw-r--r--   0        0        0      905 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_number_result.py
--rw-r--r--   0        0        0     1034 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_result.py
--rw-r--r--   0        0        0     1016 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_result_data.py
--rw-r--r--   0        0        0     3377 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_result_output.py
--rw-r--r--   0        0        0      972 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_search_results_result.py
--rw-r--r--   0        0        0      903 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/code_execution_node_string_result.py
--rw-r--r--   0        0        0     1022 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/conditional_node_result.py
--rw-r--r--   0        0        0      898 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/conditional_node_result_data.py
--rw-r--r--   0        0        0      898 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/deployment_provider_payload_response.py
--rw-r--r--   0        0        0     1938 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/deployment_read.py
--rw-r--r--   0        0        0     1532 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1783 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/document_index_read.py
--rw-r--r--   0        0        0     2200 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/document_read.py
--rw-r--r--   0        0        0      122 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/document_status.py
--rw-r--r--   0        0        0     2108 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      158 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/entity_status.py
--rw-r--r--   0        0        0      179 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/environment_enum.py
--rw-r--r--   0        0        0      116 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/error_enum.py
--rw-r--r--   0        0        0      926 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/error_variable_value.py
--rw-r--r--   0        0        0      976 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/error_vellum_value.py
--rw-r--r--   0        0        0      948 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_prompt_api_error_response.py
--rw-r--r--   0        0        0     1636 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_prompt_event.py
--rw-r--r--   0        0        0      914 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_prompt_response.py
--rw-r--r--   0        0        0      947 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_workflow_error_response.py
--rw-r--r--   0        0        0     1085 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_workflow_response.py
--rw-r--r--   0        0        0      953 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_workflow_stream_error_response.py
--rw-r--r--   0        0        0     1067 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1099 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_array_vellum_value.py
--rw-r--r--   0        0        0     1070 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_chat_history_vellum_value.py
--rw-r--r--   0        0        0     1051 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_error_vellum_value.py
--rw-r--r--   0        0        0     1061 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_function_call_vellum_value.py
--rw-r--r--   0        0        0     1029 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_json_vellum_value.py
--rw-r--r--   0        0        0     1008 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_number_vellum_value.py
--rw-r--r--   0        0        0     1075 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_search_results_vellum_value.py
--rw-r--r--   0        0        0     1006 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_string_vellum_value.py
--rw-r--r--   0        0        0     3144 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/execution_vellum_value.py
--rw-r--r--   0        0        0     1125 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/external_test_case_execution.py
--rw-r--r--   0        0        0     1154 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/external_test_case_execution_request.py
--rw-r--r--   0        0        0      169 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      124 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_enum.py
--rw-r--r--   0        0        0     1235 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_prompt_event.py
--rw-r--r--   0        0        0     1457 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_prompt_response.py
--rw-r--r--   0        0        0     1089 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0      999 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_function_call.py
--rw-r--r--   0        0        0     1073 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_function_call_request.py
--rw-r--r--   0        0        0     1228 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_prompt_execution_meta.py
--rw-r--r--   0        0        0     1373 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/fulfilled_workflow_node_result_event.py
--rw-r--r--   0        0        0      813 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call.py
--rw-r--r--   0        0        0     1065 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content.py
--rw-r--r--   0        0        0     1094 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_request.py
--rw-r--r--   0        0        0     1013 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_value.py
--rw-r--r--   0        0        0     1020 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_value_request.py
--rw-r--r--   0        0        0      131 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_enum.py
--rw-r--r--   0        0        0      936 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_variable_value.py
--rw-r--r--   0        0        0      969 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/function_call_vellum_value.py
--rw-r--r--   0        0        0      940 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0     1079 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1572 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1342 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1394 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0     1087 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      949 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0      934 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_stream_response.py
--rw-r--r--   0        0        0     1101 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_stream_result.py
--rw-r--r--   0        0        0      991 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/generate_stream_result_data.py
--rw-r--r--   0        0        0      975 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/image_chat_message_content.py
--rw-r--r--   0        0        0     1004 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/image_chat_message_content_request.py
--rw-r--r--   0        0        0      116 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/image_enum.py
--rw-r--r--   0        0        0     1000 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/image_variable_value.py
--rw-r--r--   0        0        0      213 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      124 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/initiated_enum.py
--rw-r--r--   0        0        0     1134 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/initiated_execute_prompt_event.py
--rw-r--r--   0        0        0     1181 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/initiated_prompt_execution_meta.py
--rw-r--r--   0        0        0     1377 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/initiated_workflow_node_result_event.py
--rw-r--r--   0        0        0      114 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/json_enum.py
--rw-r--r--   0        0        0     1048 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/json_input_request.py
--rw-r--r--   0        0        0      904 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/json_variable_value.py
--rw-r--r--   0        0        0      959 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/json_vellum_value.py
--rw-r--r--   0        0        0      487 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/logical_operator.py
--rw-r--r--   0        0        0      151 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0     1355 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/metadata_filter_config_request.py
--rw-r--r--   0        0        0      165 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/metadata_filter_rule_combinator.py
--rw-r--r--   0        0        0     1371 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/metadata_filter_rule_request.py
--rw-r--r--   0        0        0     1086 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/ml_model_usage.py
--rw-r--r--   0        0        0     1098 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py
--rw-r--r--   0        0        0     1043 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_scenario_input_request.py
--rw-r--r--   0        0        0     1006 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_scenario_input_string_variable_value_request.py
--rw-r--r--   0        0        0     1044 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_chat_history_variable_value.py
--rw-r--r--   0        0        0     1073 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_chat_history_variable_value_request.py
--rw-r--r--   0        0        0     1018 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_error_variable_value.py
--rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_error_variable_value_request.py
--rw-r--r--   0        0        0     1064 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_function_call_variable_value.py
--rw-r--r--   0        0        0     1093 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_function_call_variable_value_request.py
--rw-r--r--   0        0        0      995 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_json_variable_value.py
--rw-r--r--   0        0        0     1002 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_json_variable_value_request.py
--rw-r--r--   0        0        0      976 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_number_variable_value.py
--rw-r--r--   0        0        0      983 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_number_variable_value_request.py
--rw-r--r--   0        0        0     1051 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_search_results_variable_value.py
--rw-r--r--   0        0        0     1080 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_search_results_variable_value_request.py
--rw-r--r--   0        0        0      974 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_string_variable_value.py
--rw-r--r--   0        0        0      981 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_string_variable_value_request.py
--rw-r--r--   0        0        0     3021 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_variable_value.py
--rw-r--r--   0        0        0     3280 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/named_test_case_variable_value_request.py
--rw-r--r--   0        0        0     1019 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_array_value.py
--rw-r--r--   0        0        0      990 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_chat_history_value.py
--rw-r--r--   0        0        0      971 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_error_value.py
--rw-r--r--   0        0        0      976 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_function_call.py
--rw-r--r--   0        0        0      949 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_json_value.py
--rw-r--r--   0        0        0      928 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_number_value.py
--rw-r--r--   0        0        0      995 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_search_results_value.py
--rw-r--r--   0        0        0      926 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_compiled_string_value.py
--rw-r--r--   0        0        0     3354 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_input_variable_compiled_value.py
--rw-r--r--   0        0        0     1220 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_array_value.py
--rw-r--r--   0        0        0     1198 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_chat_history_value.py
--rw-r--r--   0        0        0     1172 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_error_value.py
--rw-r--r--   0        0        0     1190 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_function_call_value.py
--rw-r--r--   0        0        0     1149 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_json_value.py
--rw-r--r--   0        0        0     1130 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_number_value.py
--rw-r--r--   0        0        0     1205 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_search_results_value.py
--rw-r--r--   0        0        0     1128 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_string_value.py
--rw-r--r--   0        0        0     3275 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/node_output_compiled_value.py
--rw-r--r--   0        0        0     1000 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0     1008 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      118 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/number_enum.py
--rw-r--r--   0        0        0      883 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/number_variable_value.py
--rw-r--r--   0        0        0     1091 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_document_index_read_list.py
--rw-r--r--   0        0        0     1095 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_slim_deployment_read_list.py
--rw-r--r--   0        0        0     1070 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0     1111 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_slim_workflow_deployment_list.py
--rw-r--r--   0        0        0     1060 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_test_suite_run_execution_list.py
--rw-r--r--   0        0        0     1044 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/paginated_test_suite_test_case_list.py
--rw-r--r--   0        0        0      195 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/processing_failure_reason_enum.py
--rw-r--r--   0        0        0      190 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0     2044 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_deployment_expand_meta_request_request.py
--rw-r--r--   0        0        0     1233 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_deployment_input_request.py
--rw-r--r--   0        0        0     1370 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_execution_meta.py
--rw-r--r--   0        0        0      997 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_node_result.py
--rw-r--r--   0        0        0      988 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_node_result_data.py
--rw-r--r--   0        0        0     1418 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/prompt_output.py
--rw-r--r--   0        0        0     1210 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/raw_prompt_execution_overrides_request.py
--rw-r--r--   0        0        0      122 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_enum.py
--rw-r--r--   0        0        0     1159 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_execute_prompt_event.py
--rw-r--r--   0        0        0     1417 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_execute_prompt_response.py
--rw-r--r--   0        0        0     1103 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1038 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_function_call.py
--rw-r--r--   0        0        0     1138 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_prompt_execution_meta.py
--rw-r--r--   0        0        0     1293 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/rejected_workflow_node_result_event.py
--rw-r--r--   0        0        0     1144 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/sandbox_scenario.py
--rw-r--r--   0        0        0      907 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/scenario_input.py
--rw-r--r--   0        0        0     1071 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/scenario_input_chat_history_variable_value.py
--rw-r--r--   0        0        0     1001 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/scenario_input_string_variable_value.py
--rw-r--r--   0        0        0      938 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0     1218 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0      997 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_node_result.py
--rw-r--r--   0        0        0     1143 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_node_result_data.py
--rw-r--r--   0        0        0     1622 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1304 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result.py
--rw-r--r--   0        0        0     1437 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result_document.py
--rw-r--r--   0        0        0     1365 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result_document_request.py
--rw-r--r--   0        0        0      972 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0     1333 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_result_request.py
--rw-r--r--   0        0        0      133 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_results_enum.py
--rw-r--r--   0        0        0      950 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_results_variable_value.py
--rw-r--r--   0        0        0     1128 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     1753 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/slim_deployment_read.py
--rw-r--r--   0        0        0     2975 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0     2104 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/slim_workflow_deployment.py
--rw-r--r--   0        0        0      124 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/streaming_enum.py
--rw-r--r--   0        0        0     1388 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/streaming_execute_prompt_event.py
--rw-r--r--   0        0        0     1030 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/streaming_prompt_execution_meta.py
--rw-r--r--   0        0        0     1383 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/streaming_workflow_node_result_event.py
--rw-r--r--   0        0        0      930 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_chat_message_content.py
--rw-r--r--   0        0        0      937 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_chat_message_content_request.py
--rw-r--r--   0        0        0      118 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_enum.py
--rw-r--r--   0        0        0     1026 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_input_request.py
--rw-r--r--   0        0        0      881 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_variable_value.py
--rw-r--r--   0        0        0      931 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/string_vellum_value.py
--rw-r--r--   0        0        0     1825 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      875 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0     1487 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/submit_workflow_execution_actual_request.py
--rw-r--r--   0        0        0      128 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/subworkflow_enum.py
--rw-r--r--   0        0        0      917 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/subworkflow_node_result.py
--rw-r--r--   0        0        0      993 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_array_result.py
--rw-r--r--   0        0        0      964 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_chat_history_result.py
--rw-r--r--   0        0        0      945 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_error_result.py
--rw-r--r--   0        0        0      955 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_function_call_result.py
--rw-r--r--   0        0        0      923 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_json_result.py
--rw-r--r--   0        0        0      902 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_number_result.py
--rw-r--r--   0        0        0     1017 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_result.py
--rw-r--r--   0        0        0      956 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_result_data.py
--rw-r--r--   0        0        0     3246 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_result_output.py
--rw-r--r--   0        0        0      969 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_search_results_result.py
--rw-r--r--   0        0        0      900 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/templating_node_string_result.py
--rw-r--r--   0        0        0     1142 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_array_result.py
--rw-r--r--   0        0        0     1113 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_chat_history_result.py
--rw-r--r--   0        0        0     1094 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_error_result.py
--rw-r--r--   0        0        0     1104 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_function_call_result.py
--rw-r--r--   0        0        0     1072 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_json_result.py
--rw-r--r--   0        0        0     1051 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_number_result.py
--rw-r--r--   0        0        0     1007 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_result.py
--rw-r--r--   0        0        0      948 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_result_data.py
--rw-r--r--   0        0        0     3164 2024-05-08 19:20:42.756322 vellum_ai-0.5.2/src/vellum/types/terminal_node_result_output.py
--rw-r--r--   0        0        0     1118 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/terminal_node_search_results_result.py
--rw-r--r--   0        0        0     1049 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/terminal_node_string_result.py
--rw-r--r--   0        0        0     1061 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_chat_history_variable_value.py
--rw-r--r--   0        0        0     1036 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_error_variable_value.py
--rw-r--r--   0        0        0     1081 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_function_call_variable_value.py
--rw-r--r--   0        0        0     1012 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_json_variable_value.py
--rw-r--r--   0        0        0      996 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_number_variable_value.py
--rw-r--r--   0        0        0     1068 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_search_results_variable_value.py
--rw-r--r--   0        0        0      991 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_string_variable_value.py
--rw-r--r--   0        0        0     2834 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_case_variable_value.py
--rw-r--r--   0        0        0     1373 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py
--rw-r--r--   0        0        0     1228 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py
--rw-r--r--   0        0        0     1235 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py
--rw-r--r--   0        0        0     1411 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py
--rw-r--r--   0        0        0      174 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_type_enum.py
--rw-r--r--   0        0        0     1483 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_exec_config.py
--rw-r--r--   0        0        0     1598 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_exec_config_request.py
--rw-r--r--   0        0        0     1158 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution.py
--rw-r--r--   0        0        0     1115 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_chat_history_output.py
--rw-r--r--   0        0        0     1089 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_error_output.py
--rw-r--r--   0        0        0     1135 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_function_call_output.py
--rw-r--r--   0        0        0     1066 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_json_output.py
--rw-r--r--   0        0        0      973 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_metric_definition.py
--rw-r--r--   0        0        0     1218 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_metric_result.py
--rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_number_output.py
--rw-r--r--   0        0        0     3057 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_output.py
--rw-r--r--   0        0        0     1122 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_search_results_output.py
--rw-r--r--   0        0        0     1045 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_string_output.py
--rw-r--r--   0        0        0     1331 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config.py
--rw-r--r--   0        0        0     1115 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_data.py
--rw-r--r--   0        0        0     1144 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_data_request.py
--rw-r--r--   0        0        0     1360 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_request.py
--rw-r--r--   0        0        0      148 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_type_enum.py
--rw-r--r--   0        0        0     1005 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_error_output.py
--rw-r--r--   0        0        0      144 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_error_output_type_enum.py
--rw-r--r--   0        0        0      963 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_number_output.py
--rw-r--r--   0        0        0      146 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_number_output_type_enum.py
--rw-r--r--   0        0        0     1291 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_output.py
--rw-r--r--   0        0        0      961 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_string_output.py
--rw-r--r--   0        0        0      146 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_string_output_type_enum.py
--rw-r--r--   0        0        0     1500 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_read.py
--rw-r--r--   0        0        0      197 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_state.py
--rw-r--r--   0        0        0      896 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_test_suite.py
--rw-r--r--   0        0        0     1367 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py
--rw-r--r--   0        0        0     1241 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py
--rw-r--r--   0        0        0     1248 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py
--rw-r--r--   0        0        0     1405 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py
--rw-r--r--   0        0        0      170 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_type_enum.py
--rw-r--r--   0        0        0     1086 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/test_suite_test_case.py
--rw-r--r--   0        0        0      866 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      946 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0      937 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_error.py
--rw-r--r--   0        0        0      233 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_error_code_enum.py
--rw-r--r--   0        0        0      944 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_error_request.py
--rw-r--r--   0        0        0      914 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_image.py
--rw-r--r--   0        0        0      921 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_image_request.py
--rw-r--r--   0        0        0      944 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_variable.py
--rw-r--r--   0        0        0      281 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/vellum_variable_type.py
--rw-r--r--   0        0        0     2110 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_deployment_read.py
--rw-r--r--   0        0        0      981 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_event_error.py
--rw-r--r--   0        0        0     2038 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_chat_history_request.py
--rw-r--r--   0        0        0     1975 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_json_request.py
--rw-r--r--   0        0        0     1952 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_string_request.py
--rw-r--r--   0        0        0      425 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_event_error_code.py
--rw-r--r--   0        0        0      170 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_event_type.py
--rw-r--r--   0        0        0     1139 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_node_result_event.py
--rw-r--r--   0        0        0     1134 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_execution_workflow_result_event.py
--rw-r--r--   0        0        0     2966 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_node_result_data.py
--rw-r--r--   0        0        0     1745 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_node_result_event.py
--rw-r--r--   0        0        0      209 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_node_result_event_state.py
--rw-r--r--   0        0        0     3212 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output.py
--rw-r--r--   0        0        0     1154 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_array.py
--rw-r--r--   0        0        0     1131 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_chat_history.py
--rw-r--r--   0        0        0     1106 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_error.py
--rw-r--r--   0        0        0     1123 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_function_call.py
--rw-r--r--   0        0        0     1106 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_image.py
--rw-r--r--   0        0        0     1082 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_json.py
--rw-r--r--   0        0        0     1063 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_number.py
--rw-r--r--   0        0        0     1138 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_search_results.py
--rw-r--r--   0        0        0     1061 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_output_string.py
--rw-r--r--   0        0        0     1137 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_chat_history_input_request.py
--rw-r--r--   0        0        0     1772 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_input_request.py
--rw-r--r--   0        0        0     1066 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_json_input_request.py
--rw-r--r--   0        0        0     1047 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_number_input_request.py
--rw-r--r--   0        0        0     1045 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_request_string_input_request.py
--rw-r--r--   0        0        0     1475 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event.py
--rw-r--r--   0        0        0     3529 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data.py
--rw-r--r--   0        0        0     1423 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_array.py
--rw-r--r--   0        0        0     1400 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_chat_history.py
--rw-r--r--   0        0        0     1375 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_error.py
--rw-r--r--   0        0        0     1392 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_function_call.py
--rw-r--r--   0        0        0     1351 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_json.py
--rw-r--r--   0        0        0     1332 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_number.py
--rw-r--r--   0        0        0     1407 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_search_results.py
--rw-r--r--   0        0        0     1482 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_string.py
--rw-r--r--   0        0        0      911 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/types/workflow_stream_event.py
--rw-r--r--   0        0        0       77 2024-05-08 19:20:42.760322 vellum_ai-0.5.2/src/vellum/version.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 vellum_ai-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2980 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/README.md
+-rw-r--r--   0        0        0      632 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    42011 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/__init__.py
+-rw-r--r--   0        0        0    97089 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/client.py
+-rw-r--r--   0        0        0      853 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1697 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/request_options.py
+-rw-r--r--   0        0        0      498 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/environment.py
+-rw-r--r--   0        0        0      343 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/not_found_error.py
+-rw-r--r--   0        0        0       79 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/test_suites/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/test_suites/constants.py
+-rw-r--r--   0        0        0       56 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/test_suites/exceptions.py
+-rw-r--r--   0        0        0    12323 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/test_suites/resources.py
+-rw-r--r--   0        0        0        0 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/utils/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/utils/env.py
+-rw-r--r--   0        0        0       49 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/utils/exceptions.py
+-rw-r--r--   0        0        0      698 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/utils/paginator.py
+-rw-r--r--   0        0        0        0 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/py.typed
+-rw-r--r--   0        0        0      730 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/deployments/__init__.py
+-rw-r--r--   0        0        0    19588 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/deployments/client.py
+-rw-r--r--   0        0        0      183 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/deployments/types/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/deployments/types/deployments_list_request_status.py
+-rw-r--r--   0        0        0      165 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/document_indexes/__init__.py
+-rw-r--r--   0        0        0    40388 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/document_indexes/client.py
+-rw-r--r--   0        0        0      196 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/document_indexes/types/__init__.py
+-rw-r--r--   0        0        0      178 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/document_indexes/types/document_indexes_list_request_status.py
+-rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0    34322 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/folder_entities/__init__.py
+-rw-r--r--   0        0        0     6435 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/folder_entities/client.py
+-rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/sandboxes/__init__.py
+-rw-r--r--   0        0        0    12738 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/sandboxes/client.py
+-rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/test_suite_runs/__init__.py
+-rw-r--r--   0        0        0    18728 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/test_suite_runs/client.py
+-rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/test_suites/__init__.py
+-rw-r--r--   0        0        0    18982 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/test_suites/client.py
+-rw-r--r--   0        0        0      173 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/__init__.py
+-rw-r--r--   0        0        0    11158 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/client.py
+-rw-r--r--   0        0        0      208 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/types/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
+-rw-r--r--   0        0        0      454 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/__init__.py
+-rw-r--r--   0        0        0      473 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/_jsii/__init__.py
+-rw-r--r--   0        0        0    15887 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz
+-rw-r--r--   0        0        0       43 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/constraints.json
+-rw-r--r--   0        0        0    21484 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/data_vellum_document_index/__init__.py
+-rw-r--r--   0        0        0    25018 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/document_index/__init__.py
+-rw-r--r--   0        0        0    10298 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/terraform/provider/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/terraform/py.typed
+-rw-r--r--   0        0        0       56 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/terraform/versions.json
+-rw-r--r--   0        0        0    56092 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/add_openai_api_key_enum.py
+-rw-r--r--   0        0        0      983 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/api_node_result.py
+-rw-r--r--   0        0        0     1161 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/api_node_result_data.py
+-rw-r--r--   0        0        0     1030 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_chat_message_content.py
+-rw-r--r--   0        0        0     1297 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_item.py
+-rw-r--r--   0        0        0     1421 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_item_request.py
+-rw-r--r--   0        0        0     1059 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_request.py
+-rw-r--r--   0        0        0      116 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_enum.py
+-rw-r--r--   0        0        0     2228 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_variable_value_item.py
+-rw-r--r--   0        0        0     2166 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_vellum_value_item.py
+-rw-r--r--   0        0        0     1004 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large.py
+-rw-r--r--   0        0        0     1011 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large_request.py
+-rw-r--r--   0        0        0     1036 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1.py
+-rw-r--r--   0        0        0     1043 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1_request.py
+-rw-r--r--   0        0        0     1036 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1.py
+-rw-r--r--   0        0        0     1043 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1_request.py
+-rw-r--r--   0        0        0      129 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_history_enum.py
+-rw-r--r--   0        0        0     1121 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_history_input_request.py
+-rw-r--r--   0        0        0     1213 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message.py
+-rw-r--r--   0        0        0     1573 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message_content.py
+-rw-r--r--   0        0        0     1737 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message_content_request.py
+-rw-r--r--   0        0        0     1242 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message_request.py
+-rw-r--r--   0        0        0      182 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message_role.py
+-rw-r--r--   0        0        0      996 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_array_result.py
+-rw-r--r--   0        0        0      967 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_chat_history_result.py
+-rw-r--r--   0        0        0      948 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_error_result.py
+-rw-r--r--   0        0        0      958 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_function_call_result.py
+-rw-r--r--   0        0        0      926 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_json_result.py
+-rw-r--r--   0        0        0      905 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_number_result.py
+-rw-r--r--   0        0        0     1034 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_result.py
+-rw-r--r--   0        0        0     1016 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_result_data.py
+-rw-r--r--   0        0        0     3377 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_result_output.py
+-rw-r--r--   0        0        0      972 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_search_results_result.py
+-rw-r--r--   0        0        0      903 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_string_result.py
+-rw-r--r--   0        0        0     1022 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/conditional_node_result.py
+-rw-r--r--   0        0        0      898 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/conditional_node_result_data.py
+-rw-r--r--   0        0        0      898 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/deployment_provider_payload_response.py
+-rw-r--r--   0        0        0     1938 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/deployment_read.py
+-rw-r--r--   0        0        0     1532 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1383 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_chunking.py
+-rw-r--r--   0        0        0     1498 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_chunking_request.py
+-rw-r--r--   0        0        0     1075 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_indexing_config.py
+-rw-r--r--   0        0        0     1126 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_indexing_config_request.py
+-rw-r--r--   0        0        0     1753 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_read.py
+-rw-r--r--   0        0        0     2200 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_read.py
+-rw-r--r--   0        0        0      122 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_status.py
+-rw-r--r--   0        0        0     2108 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      158 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/entity_status.py
+-rw-r--r--   0        0        0      179 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/environment_enum.py
+-rw-r--r--   0        0        0      116 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/error_enum.py
+-rw-r--r--   0        0        0      926 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/error_variable_value.py
+-rw-r--r--   0        0        0      976 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/error_vellum_value.py
+-rw-r--r--   0        0        0      948 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_prompt_api_error_response.py
+-rw-r--r--   0        0        0     1636 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_prompt_event.py
+-rw-r--r--   0        0        0      914 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_prompt_response.py
+-rw-r--r--   0        0        0      947 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_workflow_error_response.py
+-rw-r--r--   0        0        0     1085 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_workflow_response.py
+-rw-r--r--   0        0        0      953 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_workflow_stream_error_response.py
+-rw-r--r--   0        0        0     1067 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1099 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_array_vellum_value.py
+-rw-r--r--   0        0        0     1070 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_chat_history_vellum_value.py
+-rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_error_vellum_value.py
+-rw-r--r--   0        0        0     1061 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_function_call_vellum_value.py
+-rw-r--r--   0        0        0     1029 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_json_vellum_value.py
+-rw-r--r--   0        0        0     1008 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_number_vellum_value.py
+-rw-r--r--   0        0        0     1075 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_search_results_vellum_value.py
+-rw-r--r--   0        0        0     1006 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_string_vellum_value.py
+-rw-r--r--   0        0        0     3144 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_vellum_value.py
+-rw-r--r--   0        0        0     1125 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/external_test_case_execution.py
+-rw-r--r--   0        0        0     1154 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/external_test_case_execution_request.py
+-rw-r--r--   0        0        0      169 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      124 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_enum.py
+-rw-r--r--   0        0        0     1235 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_prompt_event.py
+-rw-r--r--   0        0        0     1457 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_prompt_response.py
+-rw-r--r--   0        0        0     1089 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1228 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1373 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1081 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call.py
+-rw-r--r--   0        0        0     1065 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content.py
+-rw-r--r--   0        0        0     1094 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_request.py
+-rw-r--r--   0        0        0     1013 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_value.py
+-rw-r--r--   0        0        0     1020 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_value_request.py
+-rw-r--r--   0        0        0      131 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_enum.py
+-rw-r--r--   0        0        0     1088 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_request.py
+-rw-r--r--   0        0        0      936 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_variable_value.py
+-rw-r--r--   0        0        0      993 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_vellum_value.py
+-rw-r--r--   0        0        0      940 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0     1079 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1572 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1342 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1394 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0     1087 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      949 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0      934 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_stream_response.py
+-rw-r--r--   0        0        0     1101 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_stream_result.py
+-rw-r--r--   0        0        0      991 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_stream_result_data.py
+-rw-r--r--   0        0        0      144 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/hkunlp_instructor_xl_enum.py
+-rw-r--r--   0        0        0     1017 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/hkunlp_instructor_xl_vectorizer.py
+-rw-r--r--   0        0        0     1046 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/hkunlp_instructor_xl_vectorizer_request.py
+-rw-r--r--   0        0        0      975 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_chat_message_content.py
+-rw-r--r--   0        0        0     1004 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_chat_message_content_request.py
+-rw-r--r--   0        0        0      116 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_enum.py
+-rw-r--r--   0        0        0     1000 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_variable_value.py
+-rw-r--r--   0        0        0      998 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_vellum_value.py
+-rw-r--r--   0        0        0     3802 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/indexing_config_vectorizer.py
+-rw-r--r--   0        0        0     4061 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/indexing_config_vectorizer_request.py
+-rw-r--r--   0        0        0      213 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      124 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/initiated_enum.py
+-rw-r--r--   0        0        0     1134 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/initiated_execute_prompt_event.py
+-rw-r--r--   0        0        0     1181 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/initiated_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1377 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/initiated_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1025 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/instructor_vectorizer_config.py
+-rw-r--r--   0        0        0     1032 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/instructor_vectorizer_config_request.py
+-rw-r--r--   0        0        0      163 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/intfloat_multilingual_e_5_large_enum.py
+-rw-r--r--   0        0        0      114 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/json_enum.py
+-rw-r--r--   0        0        0     1048 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/json_input_request.py
+-rw-r--r--   0        0        0      904 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/json_variable_value.py
+-rw-r--r--   0        0        0      959 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/json_vellum_value.py
+-rw-r--r--   0        0        0      487 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/logical_operator.py
+-rw-r--r--   0        0        0      151 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0     1355 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metadata_filter_config_request.py
+-rw-r--r--   0        0        0      165 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metadata_filter_rule_combinator.py
+-rw-r--r--   0        0        0     1371 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metadata_filter_rule_request.py
+-rw-r--r--   0        0        0      118 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metric_enum.py
+-rw-r--r--   0        0        0      907 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metric_node_result.py
+-rw-r--r--   0        0        0     1086 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/ml_model_usage.py
+-rw-r--r--   0        0        0     1098 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0     1043 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_scenario_input_request.py
+-rw-r--r--   0        0        0     1006 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_scenario_input_string_variable_value_request.py
+-rw-r--r--   0        0        0     1044 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1073 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0     1018 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_error_variable_value.py
+-rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_error_variable_value_request.py
+-rw-r--r--   0        0        0     1036 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_function_call_variable_value.py
+-rw-r--r--   0        0        0     1065 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_function_call_variable_value_request.py
+-rw-r--r--   0        0        0      995 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_json_variable_value.py
+-rw-r--r--   0        0        0     1002 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_json_variable_value_request.py
+-rw-r--r--   0        0        0      976 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_number_variable_value.py
+-rw-r--r--   0        0        0      983 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_number_variable_value_request.py
+-rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0     1080 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_search_results_variable_value_request.py
+-rw-r--r--   0        0        0      974 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_string_variable_value.py
+-rw-r--r--   0        0        0      981 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_string_variable_value_request.py
+-rw-r--r--   0        0        0     3021 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_variable_value.py
+-rw-r--r--   0        0        0     3280 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_variable_value_request.py
+-rw-r--r--   0        0        0     1019 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_array_value.py
+-rw-r--r--   0        0        0      990 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_chat_history_value.py
+-rw-r--r--   0        0        0      971 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_error_value.py
+-rw-r--r--   0        0        0      976 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_function_call.py
+-rw-r--r--   0        0        0      949 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_json_value.py
+-rw-r--r--   0        0        0      928 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_number_value.py
+-rw-r--r--   0        0        0      995 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_search_results_value.py
+-rw-r--r--   0        0        0      926 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_string_value.py
+-rw-r--r--   0        0        0     3354 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_variable_compiled_value.py
+-rw-r--r--   0        0        0     1214 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_array_value.py
+-rw-r--r--   0        0        0     1198 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_chat_history_value.py
+-rw-r--r--   0        0        0     1172 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_error_value.py
+-rw-r--r--   0        0        0     1190 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_function_call_value.py
+-rw-r--r--   0        0        0     1149 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_json_value.py
+-rw-r--r--   0        0        0     1130 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_number_value.py
+-rw-r--r--   0        0        0     1205 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_search_results_value.py
+-rw-r--r--   0        0        0     1128 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_string_value.py
+-rw-r--r--   0        0        0     3275 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_value.py
+-rw-r--r--   0        0        0     1000 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0     1008 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      118 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/number_enum.py
+-rw-r--r--   0        0        0      883 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/number_variable_value.py
+-rw-r--r--   0        0        0      933 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/number_vellum_value.py
+-rw-r--r--   0        0        0     1037 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_config.py
+-rw-r--r--   0        0        0     1044 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_config_request.py
+-rw-r--r--   0        0        0     1022 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_large.py
+-rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_large_request.py
+-rw-r--r--   0        0        0     1022 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_small.py
+-rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_small_request.py
+-rw-r--r--   0        0        0     1022 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002.py
+-rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002_request.py
+-rw-r--r--   0        0        0     1091 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/paginated_document_index_read_list.py
+-rw-r--r--   0        0        0     1095 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/paginated_slim_deployment_read_list.py
+-rw-r--r--   0        0        0     1070 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0     1111 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/paginated_slim_workflow_deployment_list.py
+-rw-r--r--   0        0        0     1060 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/paginated_test_suite_run_execution_list.py
+-rw-r--r--   0        0        0     1044 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/paginated_test_suite_test_case_list.py
+-rw-r--r--   0        0        0      195 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/processing_failure_reason_enum.py
+-rw-r--r--   0        0        0      190 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0     2044 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_deployment_expand_meta_request_request.py
+-rw-r--r--   0        0        0     1233 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_deployment_input_request.py
+-rw-r--r--   0        0        0     1370 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_execution_meta.py
+-rw-r--r--   0        0        0      997 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_node_result.py
+-rw-r--r--   0        0        0      988 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_node_result_data.py
+-rw-r--r--   0        0        0     1418 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_output.py
+-rw-r--r--   0        0        0     1210 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/raw_prompt_execution_overrides_request.py
+-rw-r--r--   0        0        0      948 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunker_config.py
+-rw-r--r--   0        0        0      955 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunker_config_request.py
+-rw-r--r--   0        0        0      135 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunker_enum.py
+-rw-r--r--   0        0        0      998 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunking.py
+-rw-r--r--   0        0        0     1027 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunking_request.py
+-rw-r--r--   0        0        0      122 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_enum.py
+-rw-r--r--   0        0        0     1159 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_execute_prompt_event.py
+-rw-r--r--   0        0        0     1417 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_execute_prompt_response.py
+-rw-r--r--   0        0        0     1103 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1138 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1293 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1144 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sandbox_scenario.py
+-rw-r--r--   0        0        0      907 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/scenario_input.py
+-rw-r--r--   0        0        0     1071 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/scenario_input_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1001 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/scenario_input_string_variable_value.py
+-rw-r--r--   0        0        0      938 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0     1218 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0      997 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_node_result.py
+-rw-r--r--   0        0        0     1143 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_node_result_data.py
+-rw-r--r--   0        0        0     1622 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1304 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0     1437 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result_document.py
+-rw-r--r--   0        0        0     1365 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result_document_request.py
+-rw-r--r--   0        0        0      972 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0     1333 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result_request.py
+-rw-r--r--   0        0        0      133 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_results_enum.py
+-rw-r--r--   0        0        0     1128 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     1003 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunker_config.py
+-rw-r--r--   0        0        0     1010 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunker_config_request.py
+-rw-r--r--   0        0        0      137 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunker_enum.py
+-rw-r--r--   0        0        0     1003 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunking.py
+-rw-r--r--   0        0        0     1032 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunking_request.py
+-rw-r--r--   0        0        0      195 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_transformers_multi_qa_mpnet_base_cos_v_1_enum.py
+-rw-r--r--   0        0        0      195 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_transformers_multi_qa_mpnet_base_dot_v_1_enum.py
+-rw-r--r--   0        0        0     1753 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/slim_deployment_read.py
+-rw-r--r--   0        0        0     2975 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0     2104 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/slim_workflow_deployment.py
+-rw-r--r--   0        0        0      124 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/streaming_enum.py
+-rw-r--r--   0        0        0     1388 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/streaming_execute_prompt_event.py
+-rw-r--r--   0        0        0     1030 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/streaming_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1383 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/streaming_workflow_node_result_event.py
+-rw-r--r--   0        0        0      930 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_chat_message_content.py
+-rw-r--r--   0        0        0      937 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_chat_message_content_request.py
+-rw-r--r--   0        0        0      118 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_enum.py
+-rw-r--r--   0        0        0     1026 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_input_request.py
+-rw-r--r--   0        0        0      881 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_variable_value.py
+-rw-r--r--   0        0        0      931 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_vellum_value.py
+-rw-r--r--   0        0        0     1825 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      875 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0     1487 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/submit_workflow_execution_actual_request.py
+-rw-r--r--   0        0        0      128 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/subworkflow_enum.py
+-rw-r--r--   0        0        0      917 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/subworkflow_node_result.py
+-rw-r--r--   0        0        0      993 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_array_result.py
+-rw-r--r--   0        0        0      964 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_chat_history_result.py
+-rw-r--r--   0        0        0      945 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_error_result.py
+-rw-r--r--   0        0        0      955 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_function_call_result.py
+-rw-r--r--   0        0        0      923 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_json_result.py
+-rw-r--r--   0        0        0      902 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_number_result.py
+-rw-r--r--   0        0        0     1017 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_result.py
+-rw-r--r--   0        0        0      956 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_result_data.py
+-rw-r--r--   0        0        0     3246 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_result_output.py
+-rw-r--r--   0        0        0      969 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_search_results_result.py
+-rw-r--r--   0        0        0      900 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_string_result.py
+-rw-r--r--   0        0        0     1142 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_array_result.py
+-rw-r--r--   0        0        0     1113 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_chat_history_result.py
+-rw-r--r--   0        0        0     1094 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_error_result.py
+-rw-r--r--   0        0        0     1104 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_function_call_result.py
+-rw-r--r--   0        0        0     1072 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_json_result.py
+-rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_number_result.py
+-rw-r--r--   0        0        0     1007 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_result.py
+-rw-r--r--   0        0        0      948 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_result_data.py
+-rw-r--r--   0        0        0     3164 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_result_output.py
+-rw-r--r--   0        0        0     1118 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_search_results_result.py
+-rw-r--r--   0        0        0     1049 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_string_result.py
+-rw-r--r--   0        0        0     1061 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1036 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_error_variable_value.py
+-rw-r--r--   0        0        0     1053 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_function_call_variable_value.py
+-rw-r--r--   0        0        0     1012 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_json_variable_value.py
+-rw-r--r--   0        0        0      996 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_number_variable_value.py
+-rw-r--r--   0        0        0     1068 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0      991 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_string_variable_value.py
+-rw-r--r--   0        0        0     2834 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_variable_value.py
+-rw-r--r--   0        0        0     1373 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py
+-rw-r--r--   0        0        0     1228 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py
+-rw-r--r--   0        0        0     1235 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py
+-rw-r--r--   0        0        0     1411 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py
+-rw-r--r--   0        0        0      174 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1483 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_exec_config.py
+-rw-r--r--   0        0        0     1598 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_exec_config_request.py
+-rw-r--r--   0        0        0     1158 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution.py
+-rw-r--r--   0        0        0     1115 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_chat_history_output.py
+-rw-r--r--   0        0        0     1089 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_error_output.py
+-rw-r--r--   0        0        0     1107 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_function_call_output.py
+-rw-r--r--   0        0        0     1066 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_json_output.py
+-rw-r--r--   0        0        0      973 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_metric_definition.py
+-rw-r--r--   0        0        0     1218 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_metric_result.py
+-rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_number_output.py
+-rw-r--r--   0        0        0     3057 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_output.py
+-rw-r--r--   0        0        0     1122 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_search_results_output.py
+-rw-r--r--   0        0        0     1045 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_string_output.py
+-rw-r--r--   0        0        0     1331 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config.py
+-rw-r--r--   0        0        0     1115 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_data.py
+-rw-r--r--   0        0        0     1144 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_data_request.py
+-rw-r--r--   0        0        0     1360 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_request.py
+-rw-r--r--   0        0        0      148 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1005 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_error_output.py
+-rw-r--r--   0        0        0      144 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_error_output_type_enum.py
+-rw-r--r--   0        0        0      963 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_number_output.py
+-rw-r--r--   0        0        0      146 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_number_output_type_enum.py
+-rw-r--r--   0        0        0     1291 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_output.py
+-rw-r--r--   0        0        0      961 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_string_output.py
+-rw-r--r--   0        0        0      146 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_string_output_type_enum.py
+-rw-r--r--   0        0        0     1500 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_read.py
+-rw-r--r--   0        0        0      197 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_state.py
+-rw-r--r--   0        0        0      896 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_test_suite.py
+-rw-r--r--   0        0        0     1367 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py
+-rw-r--r--   0        0        0     1241 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py
+-rw-r--r--   0        0        0     1248 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py
+-rw-r--r--   0        0        0     1405 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py
+-rw-r--r--   0        0        0      170 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1086 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_test_case.py
+-rw-r--r--   0        0        0      147 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/text_embedding_3_large_enum.py
+-rw-r--r--   0        0        0      147 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/text_embedding_3_small_enum.py
+-rw-r--r--   0        0        0      147 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/text_embedding_ada_002_enum.py
+-rw-r--r--   0        0        0     1025 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_config.py
+-rw-r--r--   0        0        0     1032 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_config_request.py
+-rw-r--r--   0        0        0      167 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_enum.py
+-rw-r--r--   0        0        0     1077 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunking.py
+-rw-r--r--   0        0        0     1106 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunking_request.py
+-rw-r--r--   0        0        0      866 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      946 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0      937 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_error.py
+-rw-r--r--   0        0        0      233 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_error_code_enum.py
+-rw-r--r--   0        0        0      944 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_error_request.py
+-rw-r--r--   0        0        0      914 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_image.py
+-rw-r--r--   0        0        0      921 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_image_request.py
+-rw-r--r--   0        0        0      944 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_variable.py
+-rw-r--r--   0        0        0      281 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_variable_type.py
+-rw-r--r--   0        0        0     2110 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_deployment_read.py
+-rw-r--r--   0        0        0      981 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_event_error.py
+-rw-r--r--   0        0        0     2223 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_chat_history_request.py
+-rw-r--r--   0        0        0     2160 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_json_request.py
+-rw-r--r--   0        0        0     2137 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_string_request.py
+-rw-r--r--   0        0        0      425 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_event_error_code.py
+-rw-r--r--   0        0        0      170 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_event_type.py
+-rw-r--r--   0        0        0     1139 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_node_result_event.py
+-rw-r--r--   0        0        0     1134 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_workflow_result_event.py
+-rw-r--r--   0        0        0     3299 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_node_result_data.py
+-rw-r--r--   0        0        0     1745 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_node_result_event.py
+-rw-r--r--   0        0        0      209 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_node_result_event_state.py
+-rw-r--r--   0        0        0     3212 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output.py
+-rw-r--r--   0        0        0     1148 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_array.py
+-rw-r--r--   0        0        0     1131 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_chat_history.py
+-rw-r--r--   0        0        0     1106 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_error.py
+-rw-r--r--   0        0        0     1123 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_function_call.py
+-rw-r--r--   0        0        0     1106 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_image.py
+-rw-r--r--   0        0        0     1082 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_json.py
+-rw-r--r--   0        0        0     1063 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_number.py
+-rw-r--r--   0        0        0     1138 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_search_results.py
+-rw-r--r--   0        0        0     1061 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_string.py
+-rw-r--r--   0        0        0     1137 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_chat_history_input_request.py
+-rw-r--r--   0        0        0     1772 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_input_request.py
+-rw-r--r--   0        0        0     1066 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_json_input_request.py
+-rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_number_input_request.py
+-rw-r--r--   0        0        0     1045 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_string_input_request.py
+-rw-r--r--   0        0        0     1475 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event.py
+-rw-r--r--   0        0        0     3529 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data.py
+-rw-r--r--   0        0        0     1423 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_array.py
+-rw-r--r--   0        0        0     1400 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_chat_history.py
+-rw-r--r--   0        0        0     1375 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_error.py
+-rw-r--r--   0        0        0     1392 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_function_call.py
+-rw-r--r--   0        0        0     1351 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_json.py
+-rw-r--r--   0        0        0     1332 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_number.py
+-rw-r--r--   0        0        0     1407 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_search_results.py
+-rw-r--r--   0        0        0     1482 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_string.py
+-rw-r--r--   0        0        0      911 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_stream_event.py
+-rw-r--r--   0        0        0       77 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/version.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 vellum_ai-0.6.0/PKG-INFO
```

### Comparing `vellum_ai-0.5.2/LICENSE` & `vellum_ai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/README.md` & `vellum_ai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/pyproject.toml` & `vellum_ai-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vellum-ai"
-version = "0.5.2"
+version = "0.6.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "vellum", from = "src"}
 ]
```

### Comparing `vellum_ai-0.5.2/src/vellum/__init__.py` & `vellum_ai-0.6.0/src/vellum/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
+    AddOpenaiApiKeyEnum,
     ApiNodeResult,
     ApiNodeResultData,
     ArrayChatMessageContent,
     ArrayChatMessageContentItem,
     ArrayChatMessageContentItemRequest,
     ArrayChatMessageContentItemRequest_FunctionCall,
     ArrayChatMessageContentItemRequest_Image,
     ArrayChatMessageContentItemRequest_String,
     ArrayChatMessageContentItem_FunctionCall,
     ArrayChatMessageContentItem_Image,
     ArrayChatMessageContentItem_String,
     ArrayChatMessageContentRequest,
     ArrayEnum,
     ArrayVariableValueItem,
-    ArrayVariableValueItem_ChatHistory,
     ArrayVariableValueItem_Error,
     ArrayVariableValueItem_FunctionCall,
     ArrayVariableValueItem_Image,
     ArrayVariableValueItem_Json,
     ArrayVariableValueItem_Number,
-    ArrayVariableValueItem_SearchResults,
     ArrayVariableValueItem_String,
+    ArrayVellumValueItem,
+    ArrayVellumValueItem_Error,
+    ArrayVellumValueItem_FunctionCall,
+    ArrayVellumValueItem_Image,
+    ArrayVellumValueItem_Json,
+    ArrayVellumValueItem_Number,
+    ArrayVellumValueItem_String,
+    BasicVectorizerIntfloatMultilingualE5Large,
+    BasicVectorizerIntfloatMultilingualE5LargeRequest,
+    BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1,
+    BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1Request,
+    BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1,
+    BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1Request,
     ChatHistoryEnum,
     ChatHistoryInputRequest,
-    ChatHistoryVariableValue,
     ChatMessage,
     ChatMessageContent,
     ChatMessageContentRequest,
     ChatMessageContentRequest_Array,
     ChatMessageContentRequest_FunctionCall,
     ChatMessageContentRequest_Image,
     ChatMessageContentRequest_String,
@@ -59,14 +70,24 @@
     CodeExecutionNodeSearchResultsResult,
     CodeExecutionNodeStringResult,
     ConditionalNodeResult,
     ConditionalNodeResultData,
     DeploymentProviderPayloadResponse,
     DeploymentRead,
     DocumentDocumentToDocumentIndex,
+    DocumentIndexChunking,
+    DocumentIndexChunkingRequest,
+    DocumentIndexChunkingRequest_ReductoChunker,
+    DocumentIndexChunkingRequest_SentenceChunker,
+    DocumentIndexChunkingRequest_TokenOverlappingWindowChunker,
+    DocumentIndexChunking_ReductoChunker,
+    DocumentIndexChunking_SentenceChunker,
+    DocumentIndexChunking_TokenOverlappingWindowChunker,
+    DocumentIndexIndexingConfig,
+    DocumentIndexIndexingConfigRequest,
     DocumentIndexRead,
     DocumentRead,
     DocumentStatus,
     EnrichedNormalizedCompletion,
     EntityStatus,
     EnvironmentEnum,
     ErrorEnum,
@@ -107,56 +128,78 @@
     ExternalTestCaseExecution,
     ExternalTestCaseExecutionRequest,
     FinishReasonEnum,
     FulfilledEnum,
     FulfilledExecutePromptEvent,
     FulfilledExecutePromptResponse,
     FulfilledExecuteWorkflowWorkflowResultEvent,
-    FulfilledFunctionCall,
-    FulfilledFunctionCallRequest,
     FulfilledPromptExecutionMeta,
     FulfilledWorkflowNodeResultEvent,
     FunctionCall,
     FunctionCallChatMessageContent,
     FunctionCallChatMessageContentRequest,
     FunctionCallChatMessageContentValue,
     FunctionCallChatMessageContentValueRequest,
     FunctionCallEnum,
+    FunctionCallRequest,
     FunctionCallVariableValue,
     FunctionCallVellumValue,
-    FunctionCall_Fulfilled,
-    FunctionCall_Rejected,
     GenerateErrorResponse,
     GenerateOptionsRequest,
     GenerateRequest,
     GenerateResponse,
     GenerateResult,
     GenerateResultData,
     GenerateResultError,
     GenerateStreamResponse,
     GenerateStreamResult,
     GenerateStreamResultData,
+    HkunlpInstructorXlEnum,
+    HkunlpInstructorXlVectorizer,
+    HkunlpInstructorXlVectorizerRequest,
     ImageChatMessageContent,
     ImageChatMessageContentRequest,
     ImageEnum,
     ImageVariableValue,
+    ImageVellumValue,
+    IndexingConfigVectorizer,
+    IndexingConfigVectorizerRequest,
+    IndexingConfigVectorizerRequest_HkunlpInstructorXl,
+    IndexingConfigVectorizerRequest_IntfloatMultilingualE5Large,
+    IndexingConfigVectorizerRequest_SentenceTransformersMultiQaMpnetBaseCosV1,
+    IndexingConfigVectorizerRequest_SentenceTransformersMultiQaMpnetBaseDotV1,
+    IndexingConfigVectorizerRequest_TextEmbedding3Large,
+    IndexingConfigVectorizerRequest_TextEmbedding3Small,
+    IndexingConfigVectorizerRequest_TextEmbeddingAda002,
+    IndexingConfigVectorizer_HkunlpInstructorXl,
+    IndexingConfigVectorizer_IntfloatMultilingualE5Large,
+    IndexingConfigVectorizer_SentenceTransformersMultiQaMpnetBaseCosV1,
+    IndexingConfigVectorizer_SentenceTransformersMultiQaMpnetBaseDotV1,
+    IndexingConfigVectorizer_TextEmbedding3Large,
+    IndexingConfigVectorizer_TextEmbedding3Small,
+    IndexingConfigVectorizer_TextEmbeddingAda002,
     IndexingStateEnum,
     InitiatedEnum,
     InitiatedExecutePromptEvent,
     InitiatedPromptExecutionMeta,
     InitiatedWorkflowNodeResultEvent,
+    InstructorVectorizerConfig,
+    InstructorVectorizerConfigRequest,
+    IntfloatMultilingualE5LargeEnum,
     JsonEnum,
     JsonInputRequest,
     JsonVariableValue,
     JsonVellumValue,
     LogicalOperator,
     LogprobsEnum,
     MetadataFilterConfigRequest,
     MetadataFilterRuleCombinator,
     MetadataFilterRuleRequest,
+    MetricEnum,
+    MetricNodeResult,
     MlModelUsage,
     NamedScenarioInputChatHistoryVariableValueRequest,
     NamedScenarioInputRequest,
     NamedScenarioInputRequest_ChatHistory,
     NamedScenarioInputRequest_String,
     NamedScenarioInputStringVariableValueRequest,
     NamedTestCaseChatHistoryVariableValue,
@@ -223,14 +266,23 @@
     NodeOutputCompiledValue_Number,
     NodeOutputCompiledValue_SearchResults,
     NodeOutputCompiledValue_String,
     NormalizedLogProbs,
     NormalizedTokenLogProbs,
     NumberEnum,
     NumberVariableValue,
+    NumberVellumValue,
+    OpenAiVectorizerConfig,
+    OpenAiVectorizerConfigRequest,
+    OpenAiVectorizerTextEmbedding3Large,
+    OpenAiVectorizerTextEmbedding3LargeRequest,
+    OpenAiVectorizerTextEmbedding3Small,
+    OpenAiVectorizerTextEmbedding3SmallRequest,
+    OpenAiVectorizerTextEmbeddingAda002,
+    OpenAiVectorizerTextEmbeddingAda002Request,
     PaginatedDocumentIndexReadList,
     PaginatedSlimDeploymentReadList,
     PaginatedSlimDocumentList,
     PaginatedSlimWorkflowDeploymentList,
     PaginatedTestSuiteRunExecutionList,
     PaginatedTestSuiteTestCaseList,
     ProcessingFailureReasonEnum,
@@ -245,19 +297,23 @@
     PromptNodeResultData,
     PromptOutput,
     PromptOutput_Error,
     PromptOutput_FunctionCall,
     PromptOutput_Json,
     PromptOutput_String,
     RawPromptExecutionOverridesRequest,
+    ReductoChunkerConfig,
+    ReductoChunkerConfigRequest,
+    ReductoChunkerEnum,
+    ReductoChunking,
+    ReductoChunkingRequest,
     RejectedEnum,
     RejectedExecutePromptEvent,
     RejectedExecutePromptResponse,
     RejectedExecuteWorkflowWorkflowResultEvent,
-    RejectedFunctionCall,
     RejectedPromptExecutionMeta,
     RejectedWorkflowNodeResultEvent,
     SandboxScenario,
     ScenarioInput,
     ScenarioInputChatHistoryVariableValue,
     ScenarioInputStringVariableValue,
     ScenarioInput_ChatHistory,
@@ -270,16 +326,22 @@
     SearchResponse,
     SearchResult,
     SearchResultDocument,
     SearchResultDocumentRequest,
     SearchResultMergingRequest,
     SearchResultRequest,
     SearchResultsEnum,
-    SearchResultsVariableValue,
     SearchWeightsRequest,
+    SentenceChunkerConfig,
+    SentenceChunkerConfigRequest,
+    SentenceChunkerEnum,
+    SentenceChunking,
+    SentenceChunkingRequest,
+    SentenceTransformersMultiQaMpnetBaseCosV1Enum,
+    SentenceTransformersMultiQaMpnetBaseDotV1Enum,
     SlimDeploymentRead,
     SlimDocument,
     SlimWorkflowDeployment,
     StreamingEnum,
     StreamingExecutePromptEvent,
     StreamingPromptExecutionMeta,
     StreamingWorkflowNodeResultEvent,
@@ -401,14 +463,22 @@
     TestSuiteRunTestSuite,
     TestSuiteRunWorkflowReleaseTagExecConfig,
     TestSuiteRunWorkflowReleaseTagExecConfigData,
     TestSuiteRunWorkflowReleaseTagExecConfigDataRequest,
     TestSuiteRunWorkflowReleaseTagExecConfigRequest,
     TestSuiteRunWorkflowReleaseTagExecConfigTypeEnum,
     TestSuiteTestCase,
+    TextEmbedding3LargeEnum,
+    TextEmbedding3SmallEnum,
+    TextEmbeddingAda002Enum,
+    TokenOverlappingWindowChunkerConfig,
+    TokenOverlappingWindowChunkerConfigRequest,
+    TokenOverlappingWindowChunkerEnum,
+    TokenOverlappingWindowChunking,
+    TokenOverlappingWindowChunkingRequest,
     UploadDocumentErrorResponse,
     UploadDocumentResponse,
     VellumError,
     VellumErrorCodeEnum,
     VellumErrorRequest,
     VellumImage,
     VellumImageRequest,
@@ -423,14 +493,15 @@
     WorkflowExecutionEventType,
     WorkflowExecutionNodeResultEvent,
     WorkflowExecutionWorkflowResultEvent,
     WorkflowNodeResultData,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
+    WorkflowNodeResultData_Metric,
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
     WorkflowNodeResultData_Subworkflow,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_Terminal,
     WorkflowNodeResultEvent,
     WorkflowNodeResultEventState,
@@ -502,40 +573,51 @@
     test_suites,
     workflow_deployments,
 )
 from .environment import VellumEnvironment
 from .version import __version__
 
 __all__ = [
+    "AddOpenaiApiKeyEnum",
     "ApiNodeResult",
     "ApiNodeResultData",
     "ArrayChatMessageContent",
     "ArrayChatMessageContentItem",
     "ArrayChatMessageContentItemRequest",
     "ArrayChatMessageContentItemRequest_FunctionCall",
     "ArrayChatMessageContentItemRequest_Image",
     "ArrayChatMessageContentItemRequest_String",
     "ArrayChatMessageContentItem_FunctionCall",
     "ArrayChatMessageContentItem_Image",
     "ArrayChatMessageContentItem_String",
     "ArrayChatMessageContentRequest",
     "ArrayEnum",
     "ArrayVariableValueItem",
-    "ArrayVariableValueItem_ChatHistory",
     "ArrayVariableValueItem_Error",
     "ArrayVariableValueItem_FunctionCall",
     "ArrayVariableValueItem_Image",
     "ArrayVariableValueItem_Json",
     "ArrayVariableValueItem_Number",
-    "ArrayVariableValueItem_SearchResults",
     "ArrayVariableValueItem_String",
+    "ArrayVellumValueItem",
+    "ArrayVellumValueItem_Error",
+    "ArrayVellumValueItem_FunctionCall",
+    "ArrayVellumValueItem_Image",
+    "ArrayVellumValueItem_Json",
+    "ArrayVellumValueItem_Number",
+    "ArrayVellumValueItem_String",
     "BadRequestError",
+    "BasicVectorizerIntfloatMultilingualE5Large",
+    "BasicVectorizerIntfloatMultilingualE5LargeRequest",
+    "BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1",
+    "BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1Request",
+    "BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1",
+    "BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1Request",
     "ChatHistoryEnum",
     "ChatHistoryInputRequest",
-    "ChatHistoryVariableValue",
     "ChatMessage",
     "ChatMessageContent",
     "ChatMessageContentRequest",
     "ChatMessageContentRequest_Array",
     "ChatMessageContentRequest_FunctionCall",
     "ChatMessageContentRequest_Image",
     "ChatMessageContentRequest_String",
@@ -566,14 +648,24 @@
     "CodeExecutionNodeStringResult",
     "ConditionalNodeResult",
     "ConditionalNodeResultData",
     "DeploymentProviderPayloadResponse",
     "DeploymentRead",
     "DeploymentsListRequestStatus",
     "DocumentDocumentToDocumentIndex",
+    "DocumentIndexChunking",
+    "DocumentIndexChunkingRequest",
+    "DocumentIndexChunkingRequest_ReductoChunker",
+    "DocumentIndexChunkingRequest_SentenceChunker",
+    "DocumentIndexChunkingRequest_TokenOverlappingWindowChunker",
+    "DocumentIndexChunking_ReductoChunker",
+    "DocumentIndexChunking_SentenceChunker",
+    "DocumentIndexChunking_TokenOverlappingWindowChunker",
+    "DocumentIndexIndexingConfig",
+    "DocumentIndexIndexingConfigRequest",
     "DocumentIndexRead",
     "DocumentIndexesListRequestStatus",
     "DocumentRead",
     "DocumentStatus",
     "EnrichedNormalizedCompletion",
     "EntityStatus",
     "EnvironmentEnum",
@@ -616,57 +708,79 @@
     "ExternalTestCaseExecutionRequest",
     "FinishReasonEnum",
     "ForbiddenError",
     "FulfilledEnum",
     "FulfilledExecutePromptEvent",
     "FulfilledExecutePromptResponse",
     "FulfilledExecuteWorkflowWorkflowResultEvent",
-    "FulfilledFunctionCall",
-    "FulfilledFunctionCallRequest",
     "FulfilledPromptExecutionMeta",
     "FulfilledWorkflowNodeResultEvent",
     "FunctionCall",
     "FunctionCallChatMessageContent",
     "FunctionCallChatMessageContentRequest",
     "FunctionCallChatMessageContentValue",
     "FunctionCallChatMessageContentValueRequest",
     "FunctionCallEnum",
+    "FunctionCallRequest",
     "FunctionCallVariableValue",
     "FunctionCallVellumValue",
-    "FunctionCall_Fulfilled",
-    "FunctionCall_Rejected",
     "GenerateErrorResponse",
     "GenerateOptionsRequest",
     "GenerateRequest",
     "GenerateResponse",
     "GenerateResult",
     "GenerateResultData",
     "GenerateResultError",
     "GenerateStreamResponse",
     "GenerateStreamResult",
     "GenerateStreamResultData",
+    "HkunlpInstructorXlEnum",
+    "HkunlpInstructorXlVectorizer",
+    "HkunlpInstructorXlVectorizerRequest",
     "ImageChatMessageContent",
     "ImageChatMessageContentRequest",
     "ImageEnum",
     "ImageVariableValue",
+    "ImageVellumValue",
+    "IndexingConfigVectorizer",
+    "IndexingConfigVectorizerRequest",
+    "IndexingConfigVectorizerRequest_HkunlpInstructorXl",
+    "IndexingConfigVectorizerRequest_IntfloatMultilingualE5Large",
+    "IndexingConfigVectorizerRequest_SentenceTransformersMultiQaMpnetBaseCosV1",
+    "IndexingConfigVectorizerRequest_SentenceTransformersMultiQaMpnetBaseDotV1",
+    "IndexingConfigVectorizerRequest_TextEmbedding3Large",
+    "IndexingConfigVectorizerRequest_TextEmbedding3Small",
+    "IndexingConfigVectorizerRequest_TextEmbeddingAda002",
+    "IndexingConfigVectorizer_HkunlpInstructorXl",
+    "IndexingConfigVectorizer_IntfloatMultilingualE5Large",
+    "IndexingConfigVectorizer_SentenceTransformersMultiQaMpnetBaseCosV1",
+    "IndexingConfigVectorizer_SentenceTransformersMultiQaMpnetBaseDotV1",
+    "IndexingConfigVectorizer_TextEmbedding3Large",
+    "IndexingConfigVectorizer_TextEmbedding3Small",
+    "IndexingConfigVectorizer_TextEmbeddingAda002",
     "IndexingStateEnum",
     "InitiatedEnum",
     "InitiatedExecutePromptEvent",
     "InitiatedPromptExecutionMeta",
     "InitiatedWorkflowNodeResultEvent",
+    "InstructorVectorizerConfig",
+    "InstructorVectorizerConfigRequest",
     "InternalServerError",
+    "IntfloatMultilingualE5LargeEnum",
     "JsonEnum",
     "JsonInputRequest",
     "JsonVariableValue",
     "JsonVellumValue",
     "LogicalOperator",
     "LogprobsEnum",
     "MetadataFilterConfigRequest",
     "MetadataFilterRuleCombinator",
     "MetadataFilterRuleRequest",
+    "MetricEnum",
+    "MetricNodeResult",
     "MlModelUsage",
     "NamedScenarioInputChatHistoryVariableValueRequest",
     "NamedScenarioInputRequest",
     "NamedScenarioInputRequest_ChatHistory",
     "NamedScenarioInputRequest_String",
     "NamedScenarioInputStringVariableValueRequest",
     "NamedTestCaseChatHistoryVariableValue",
@@ -734,14 +848,23 @@
     "NodeOutputCompiledValue_SearchResults",
     "NodeOutputCompiledValue_String",
     "NormalizedLogProbs",
     "NormalizedTokenLogProbs",
     "NotFoundError",
     "NumberEnum",
     "NumberVariableValue",
+    "NumberVellumValue",
+    "OpenAiVectorizerConfig",
+    "OpenAiVectorizerConfigRequest",
+    "OpenAiVectorizerTextEmbedding3Large",
+    "OpenAiVectorizerTextEmbedding3LargeRequest",
+    "OpenAiVectorizerTextEmbedding3Small",
+    "OpenAiVectorizerTextEmbedding3SmallRequest",
+    "OpenAiVectorizerTextEmbeddingAda002",
+    "OpenAiVectorizerTextEmbeddingAda002Request",
     "PaginatedDocumentIndexReadList",
     "PaginatedSlimDeploymentReadList",
     "PaginatedSlimDocumentList",
     "PaginatedSlimWorkflowDeploymentList",
     "PaginatedTestSuiteRunExecutionList",
     "PaginatedTestSuiteTestCaseList",
     "ProcessingFailureReasonEnum",
@@ -756,19 +879,23 @@
     "PromptNodeResultData",
     "PromptOutput",
     "PromptOutput_Error",
     "PromptOutput_FunctionCall",
     "PromptOutput_Json",
     "PromptOutput_String",
     "RawPromptExecutionOverridesRequest",
+    "ReductoChunkerConfig",
+    "ReductoChunkerConfigRequest",
+    "ReductoChunkerEnum",
+    "ReductoChunking",
+    "ReductoChunkingRequest",
     "RejectedEnum",
     "RejectedExecutePromptEvent",
     "RejectedExecutePromptResponse",
     "RejectedExecuteWorkflowWorkflowResultEvent",
-    "RejectedFunctionCall",
     "RejectedPromptExecutionMeta",
     "RejectedWorkflowNodeResultEvent",
     "SandboxScenario",
     "ScenarioInput",
     "ScenarioInputChatHistoryVariableValue",
     "ScenarioInputStringVariableValue",
     "ScenarioInput_ChatHistory",
@@ -781,16 +908,22 @@
     "SearchResponse",
     "SearchResult",
     "SearchResultDocument",
     "SearchResultDocumentRequest",
     "SearchResultMergingRequest",
     "SearchResultRequest",
     "SearchResultsEnum",
-    "SearchResultsVariableValue",
     "SearchWeightsRequest",
+    "SentenceChunkerConfig",
+    "SentenceChunkerConfigRequest",
+    "SentenceChunkerEnum",
+    "SentenceChunking",
+    "SentenceChunkingRequest",
+    "SentenceTransformersMultiQaMpnetBaseCosV1Enum",
+    "SentenceTransformersMultiQaMpnetBaseDotV1Enum",
     "SlimDeploymentRead",
     "SlimDocument",
     "SlimWorkflowDeployment",
     "StreamingEnum",
     "StreamingExecutePromptEvent",
     "StreamingPromptExecutionMeta",
     "StreamingWorkflowNodeResultEvent",
@@ -912,14 +1045,22 @@
     "TestSuiteRunTestSuite",
     "TestSuiteRunWorkflowReleaseTagExecConfig",
     "TestSuiteRunWorkflowReleaseTagExecConfigData",
     "TestSuiteRunWorkflowReleaseTagExecConfigDataRequest",
     "TestSuiteRunWorkflowReleaseTagExecConfigRequest",
     "TestSuiteRunWorkflowReleaseTagExecConfigTypeEnum",
     "TestSuiteTestCase",
+    "TextEmbedding3LargeEnum",
+    "TextEmbedding3SmallEnum",
+    "TextEmbeddingAda002Enum",
+    "TokenOverlappingWindowChunkerConfig",
+    "TokenOverlappingWindowChunkerConfigRequest",
+    "TokenOverlappingWindowChunkerEnum",
+    "TokenOverlappingWindowChunking",
+    "TokenOverlappingWindowChunkingRequest",
     "UploadDocumentErrorResponse",
     "UploadDocumentResponse",
     "VellumEnvironment",
     "VellumError",
     "VellumErrorCodeEnum",
     "VellumErrorRequest",
     "VellumImage",
@@ -936,14 +1077,15 @@
     "WorkflowExecutionEventType",
     "WorkflowExecutionNodeResultEvent",
     "WorkflowExecutionWorkflowResultEvent",
     "WorkflowNodeResultData",
     "WorkflowNodeResultData_Api",
     "WorkflowNodeResultData_CodeExecution",
     "WorkflowNodeResultData_Conditional",
+    "WorkflowNodeResultData_Metric",
     "WorkflowNodeResultData_Prompt",
     "WorkflowNodeResultData_Search",
     "WorkflowNodeResultData_Subworkflow",
     "WorkflowNodeResultData_Templating",
     "WorkflowNodeResultData_Terminal",
     "WorkflowNodeResultEvent",
     "WorkflowNodeResultEventState",
```

### Comparing `vellum_ai-0.5.2/src/vellum/client.py` & `vellum_ai-0.6.0/src/vellum/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/core/__init__.py` & `vellum_ai-0.6.0/src/vellum/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/core/client_wrapper.py` & `vellum_ai-0.6.0/src/vellum/core/client_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self._environment = environment
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "vellum-ai",
-            "X-Fern-SDK-Version": "0.5.2",
+            "X-Fern-SDK-Version": "0.6.0",
         }
         headers["X_API_KEY"] = self.api_key
         return headers
 
     def get_environment(self) -> VellumEnvironment:
         return self._environment
```

### Comparing `vellum_ai-0.5.2/src/vellum/core/datetime_utils.py` & `vellum_ai-0.6.0/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/core/file.py` & `vellum_ai-0.6.0/src/vellum/core/file.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/core/http_client.py` & `vellum_ai-0.6.0/src/vellum/core/http_client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.6.0/src/vellum/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/core/request_options.py` & `vellum_ai-0.6.0/src/vellum/core/request_options.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/lib/test_suites/resources.py` & `vellum_ai-0.6.0/src/vellum/lib/test_suites/resources.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/lib/utils/paginator.py` & `vellum_ai-0.6.0/src/vellum/lib/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/resources/__init__.py` & `vellum_ai-0.6.0/src/vellum/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/resources/deployments/client.py` & `vellum_ai-0.6.0/src/vellum/resources/deployments/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/resources/document_indexes/client.py` & `vellum_ai-0.6.0/src/vellum/resources/document_indexes/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from ...core.api_error import ApiError
 from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.pydantic_utilities import pydantic_v1
 from ...core.remove_none_from_dict import remove_none_from_dict
 from ...core.request_options import RequestOptions
+from ...types.document_index_indexing_config_request import DocumentIndexIndexingConfigRequest
 from ...types.document_index_read import DocumentIndexRead
 from ...types.entity_status import EntityStatus
 from ...types.environment_enum import EnvironmentEnum
 from ...types.paginated_document_index_read_list import PaginatedDocumentIndexReadList
 from .types.document_indexes_list_request_status import DocumentIndexesListRequestStatus
 
 # this is used as the default value for optional parameters
@@ -26,28 +27,31 @@
 
     def list(
         self,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         ordering: typing.Optional[str] = None,
+        search: typing.Optional[str] = None,
         status: typing.Optional[DocumentIndexesListRequestStatus] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> PaginatedDocumentIndexReadList:
         """
         Used to retrieve a list of Document Indexes.
 
         Parameters:
             - limit: typing.Optional[int]. Number of results to return per page.
 
             - offset: typing.Optional[int]. The initial index from which to return the results.
 
             - ordering: typing.Optional[str]. Which field to use when ordering the results.
 
-            - status: typing.Optional[DocumentIndexesListRequestStatus]. The current status of the document index
+            - search: typing.Optional[str]. Search for document indices by name or label
+
+            - status: typing.Optional[DocumentIndexesListRequestStatus]. Filter down to only document indices that have a status matching the status specified
 
                                                                          - `ACTIVE` - Active
                                                                          - `ARCHIVED` - Archived
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import Vellum
 
@@ -61,14 +65,15 @@
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/document-indexes"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "limit": limit,
                         "offset": offset,
                         "ordering": ordering,
+                        "search": search,
                         "status": status,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
@@ -99,15 +104,15 @@
     def create(
         self,
         *,
         label: str,
         name: str,
         status: typing.Optional[EntityStatus] = OMIT,
         environment: typing.Optional[EnvironmentEnum] = OMIT,
-        indexing_config: typing.Dict[str, typing.Any],
+        indexing_config: DocumentIndexIndexingConfigRequest,
         copy_documents_from_index_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DocumentIndexRead:
         """
         Creates a new document index.
 
         Parameters:
@@ -120,45 +125,40 @@
                                                      * `ACTIVE` - Active
                                                      * `ARCHIVED` - Archived
             - environment: typing.Optional[EnvironmentEnum]. The environment this document index is used in
 
                                                              * `DEVELOPMENT` - Development
                                                              * `STAGING` - Staging
                                                              * `PRODUCTION` - Production
-            - indexing_config: typing.Dict[str, typing.Any]. Configuration representing how documents should be indexed
+            - indexing_config: DocumentIndexIndexingConfigRequest.
 
             - copy_documents_from_index_id: typing.Optional[str]. Optionally specify the id of a document index from which you'd like to copy and re-index its documents into this newly created index
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from vellum import (
+            DocumentIndexChunkingRequest_ReductoChunker,
+            DocumentIndexIndexingConfigRequest,
+            IndexingConfigVectorizerRequest_TextEmbedding3Small,
+        )
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
         client.document_indexes.create(
-            label="My Document Index",
-            name="my-document-index",
-            indexing_config={
-                "chunking": {
-                    "chunker_name": "sentence-chunker",
-                    "chunker_config": {
-                        "character_limit": 1000,
-                        "min_overlap_ratio": 0.5,
-                    },
-                },
-                "vectorizer": {
-                    "model_name": "hkunlp/instructor-xl",
-                    "config": {
-                        "instruction_domain": "",
-                        "instruction_document_text_type": "plain_text",
-                        "instruction_query_text_type": "plain_text",
-                    },
-                },
-            },
+            label="string",
+            name="string",
+            status="ACTIVE",
+            environment="DEVELOPMENT",
+            indexing_config=DocumentIndexIndexingConfigRequest(
+                vectorizer=IndexingConfigVectorizerRequest_TextEmbedding3Small(),
+                chunking=DocumentIndexChunkingRequest_ReductoChunker(),
+            ),
+            copy_documents_from_index_id="string",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"label": label, "name": name, "indexing_config": indexing_config}
         if status is not OMIT:
             _request["status"] = status
         if environment is not OMIT:
             _request["environment"] = environment
@@ -209,15 +209,15 @@
         ---
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
         client.document_indexes.retrieve(
-            id="id",
+            id="string",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/document-indexes/{jsonable_encoder(id)}"
             ),
@@ -276,16 +276,18 @@
         ---
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
         client.document_indexes.update(
-            id="id",
-            label="label",
+            id="string",
+            label="string",
+            status="ACTIVE",
+            environment="DEVELOPMENT",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"label": label}
         if status is not OMIT:
             _request["status"] = status
         if environment is not OMIT:
             _request["environment"] = environment
@@ -403,15 +405,18 @@
         ---
         from vellum.client import Vellum
 
         client = Vellum(
             api_key="YOUR_API_KEY",
         )
         client.document_indexes.partial_update(
-            id="id",
+            id="string",
+            label="string",
+            status="ACTIVE",
+            environment="DEVELOPMENT",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if label is not OMIT:
             _request["label"] = label
         if status is not OMIT:
             _request["status"] = status
@@ -460,28 +465,31 @@
 
     async def list(
         self,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         ordering: typing.Optional[str] = None,
+        search: typing.Optional[str] = None,
         status: typing.Optional[DocumentIndexesListRequestStatus] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> PaginatedDocumentIndexReadList:
         """
         Used to retrieve a list of Document Indexes.
 
         Parameters:
             - limit: typing.Optional[int]. Number of results to return per page.
 
             - offset: typing.Optional[int]. The initial index from which to return the results.
 
             - ordering: typing.Optional[str]. Which field to use when ordering the results.
 
-            - status: typing.Optional[DocumentIndexesListRequestStatus]. The current status of the document index
+            - search: typing.Optional[str]. Search for document indices by name or label
+
+            - status: typing.Optional[DocumentIndexesListRequestStatus]. Filter down to only document indices that have a status matching the status specified
 
                                                                          - `ACTIVE` - Active
                                                                          - `ARCHIVED` - Archived
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import AsyncVellum
 
@@ -495,14 +503,15 @@
             url=urllib.parse.urljoin(f"{self._client_wrapper.get_environment().default}/", "v1/document-indexes"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         "limit": limit,
                         "offset": offset,
                         "ordering": ordering,
+                        "search": search,
                         "status": status,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
@@ -533,15 +542,15 @@
     async def create(
         self,
         *,
         label: str,
         name: str,
         status: typing.Optional[EntityStatus] = OMIT,
         environment: typing.Optional[EnvironmentEnum] = OMIT,
-        indexing_config: typing.Dict[str, typing.Any],
+        indexing_config: DocumentIndexIndexingConfigRequest,
         copy_documents_from_index_id: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DocumentIndexRead:
         """
         Creates a new document index.
 
         Parameters:
@@ -554,45 +563,40 @@
                                                      * `ACTIVE` - Active
                                                      * `ARCHIVED` - Archived
             - environment: typing.Optional[EnvironmentEnum]. The environment this document index is used in
 
                                                              * `DEVELOPMENT` - Development
                                                              * `STAGING` - Staging
                                                              * `PRODUCTION` - Production
-            - indexing_config: typing.Dict[str, typing.Any]. Configuration representing how documents should be indexed
+            - indexing_config: DocumentIndexIndexingConfigRequest.
 
             - copy_documents_from_index_id: typing.Optional[str]. Optionally specify the id of a document index from which you'd like to copy and re-index its documents into this newly created index
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
+        from vellum import (
+            DocumentIndexChunkingRequest_ReductoChunker,
+            DocumentIndexIndexingConfigRequest,
+            IndexingConfigVectorizerRequest_TextEmbedding3Small,
+        )
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
         await client.document_indexes.create(
-            label="My Document Index",
-            name="my-document-index",
-            indexing_config={
-                "chunking": {
-                    "chunker_name": "sentence-chunker",
-                    "chunker_config": {
-                        "character_limit": 1000,
-                        "min_overlap_ratio": 0.5,
-                    },
-                },
-                "vectorizer": {
-                    "model_name": "hkunlp/instructor-xl",
-                    "config": {
-                        "instruction_domain": "",
-                        "instruction_document_text_type": "plain_text",
-                        "instruction_query_text_type": "plain_text",
-                    },
-                },
-            },
+            label="string",
+            name="string",
+            status="ACTIVE",
+            environment="DEVELOPMENT",
+            indexing_config=DocumentIndexIndexingConfigRequest(
+                vectorizer=IndexingConfigVectorizerRequest_TextEmbedding3Small(),
+                chunking=DocumentIndexChunkingRequest_ReductoChunker(),
+            ),
+            copy_documents_from_index_id="string",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"label": label, "name": name, "indexing_config": indexing_config}
         if status is not OMIT:
             _request["status"] = status
         if environment is not OMIT:
             _request["environment"] = environment
@@ -643,15 +647,15 @@
         ---
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
         await client.document_indexes.retrieve(
-            id="id",
+            id="string",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             method="GET",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/", f"v1/document-indexes/{jsonable_encoder(id)}"
             ),
@@ -710,16 +714,18 @@
         ---
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
         await client.document_indexes.update(
-            id="id",
-            label="label",
+            id="string",
+            label="string",
+            status="ACTIVE",
+            environment="DEVELOPMENT",
         )
         """
         _request: typing.Dict[str, typing.Any] = {"label": label}
         if status is not OMIT:
             _request["status"] = status
         if environment is not OMIT:
             _request["environment"] = environment
@@ -837,15 +843,18 @@
         ---
         from vellum.client import AsyncVellum
 
         client = AsyncVellum(
             api_key="YOUR_API_KEY",
         )
         await client.document_indexes.partial_update(
-            id="id",
+            id="string",
+            label="string",
+            status="ACTIVE",
+            environment="DEVELOPMENT",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if label is not OMIT:
             _request["label"] = label
         if status is not OMIT:
             _request["status"] = status
```

### Comparing `vellum_ai-0.5.2/src/vellum/resources/documents/client.py` & `vellum_ai-0.6.0/src/vellum/resources/documents/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DocumentRead:
         """
-        Retrieve a Document via its Vellum-generated ID.
+        Retrieve a Document, keying off of either its Vellum-generated ID or its external ID.
 
         Parameters:
             - id: str. A UUID string identifying this document.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import Vellum
@@ -143,14 +143,16 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def destroy(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
+        Delete a Document, keying off of either its Vellum-generated ID or its external ID.
+
         Parameters:
             - id: str. A UUID string identifying this document.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import Vellum
 
@@ -197,15 +199,15 @@
         *,
         label: typing.Optional[str] = OMIT,
         status: typing.Optional[DocumentStatus] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DocumentRead:
         """
-        Update a Document, keying off of its Vellum-generated ID. Particularly useful for updating its metadata.
+        Update a Document, keying off of either its Vellum-generated ID or its external ID. Particularly useful for updating its metadata.
 
         Parameters:
             - id: str. A UUID string identifying this document.
 
             - label: typing.Optional[str]. A human-readable label for the document. Defaults to the originally uploaded file's file name.
 
             - status: typing.Optional[DocumentStatus]. The current status of the document
@@ -449,15 +451,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DocumentRead:
         """
-        Retrieve a Document via its Vellum-generated ID.
+        Retrieve a Document, keying off of either its Vellum-generated ID or its external ID.
 
         Parameters:
             - id: str. A UUID string identifying this document.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import AsyncVellum
@@ -497,14 +499,16 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def destroy(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
+        Delete a Document, keying off of either its Vellum-generated ID or its external ID.
+
         Parameters:
             - id: str. A UUID string identifying this document.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from vellum.client import AsyncVellum
 
@@ -551,15 +555,15 @@
         *,
         label: typing.Optional[str] = OMIT,
         status: typing.Optional[DocumentStatus] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DocumentRead:
         """
-        Update a Document, keying off of its Vellum-generated ID. Particularly useful for updating its metadata.
+        Update a Document, keying off of either its Vellum-generated ID or its external ID. Particularly useful for updating its metadata.
 
         Parameters:
             - id: str. A UUID string identifying this document.
 
             - label: typing.Optional[str]. A human-readable label for the document. Defaults to the originally uploaded file's file name.
 
             - status: typing.Optional[DocumentStatus]. The current status of the document
```

### Comparing `vellum_ai-0.5.2/src/vellum/resources/folder_entities/client.py` & `vellum_ai-0.6.0/src/vellum/resources/folder_entities/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/resources/sandboxes/client.py` & `vellum_ai-0.6.0/src/vellum/resources/sandboxes/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/resources/test_suite_runs/client.py` & `vellum_ai-0.6.0/src/vellum/resources/test_suite_runs/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/resources/test_suites/client.py` & `vellum_ai-0.6.0/src/vellum/resources/test_suites/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/resources/workflow_deployments/client.py` & `vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz` & `vellum_ai-0.6.0/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/terraform/data_vellum_document_index/__init__.py` & `vellum_ai-0.6.0/src/vellum/terraform/data_vellum_document_index/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/terraform/document_index/__init__.py` & `vellum_ai-0.6.0/src/vellum/terraform/document_index/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/terraform/provider/__init__.py` & `vellum_ai-0.6.0/src/vellum/terraform/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/__init__.py` & `vellum_ai-0.6.0/src/vellum/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .add_openai_api_key_enum import AddOpenaiApiKeyEnum
 from .api_node_result import ApiNodeResult
 from .api_node_result_data import ApiNodeResultData
 from .array_chat_message_content import ArrayChatMessageContent
 from .array_chat_message_content_item import (
     ArrayChatMessageContentItem,
     ArrayChatMessageContentItem_FunctionCall,
     ArrayChatMessageContentItem_Image,
@@ -15,26 +16,46 @@
     ArrayChatMessageContentItemRequest_Image,
     ArrayChatMessageContentItemRequest_String,
 )
 from .array_chat_message_content_request import ArrayChatMessageContentRequest
 from .array_enum import ArrayEnum
 from .array_variable_value_item import (
     ArrayVariableValueItem,
-    ArrayVariableValueItem_ChatHistory,
     ArrayVariableValueItem_Error,
     ArrayVariableValueItem_FunctionCall,
     ArrayVariableValueItem_Image,
     ArrayVariableValueItem_Json,
     ArrayVariableValueItem_Number,
-    ArrayVariableValueItem_SearchResults,
     ArrayVariableValueItem_String,
 )
+from .array_vellum_value_item import (
+    ArrayVellumValueItem,
+    ArrayVellumValueItem_Error,
+    ArrayVellumValueItem_FunctionCall,
+    ArrayVellumValueItem_Image,
+    ArrayVellumValueItem_Json,
+    ArrayVellumValueItem_Number,
+    ArrayVellumValueItem_String,
+)
+from .basic_vectorizer_intfloat_multilingual_e_5_large import BasicVectorizerIntfloatMultilingualE5Large
+from .basic_vectorizer_intfloat_multilingual_e_5_large_request import BasicVectorizerIntfloatMultilingualE5LargeRequest
+from .basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1 import (
+    BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1,
+)
+from .basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1_request import (
+    BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1Request,
+)
+from .basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1 import (
+    BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1,
+)
+from .basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1_request import (
+    BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1Request,
+)
 from .chat_history_enum import ChatHistoryEnum
 from .chat_history_input_request import ChatHistoryInputRequest
-from .chat_history_variable_value import ChatHistoryVariableValue
 from .chat_message import ChatMessage
 from .chat_message_content import (
     ChatMessageContent,
     ChatMessageContent_Array,
     ChatMessageContent_FunctionCall,
     ChatMessageContent_Image,
     ChatMessageContent_String,
@@ -70,14 +91,28 @@
 from .code_execution_node_search_results_result import CodeExecutionNodeSearchResultsResult
 from .code_execution_node_string_result import CodeExecutionNodeStringResult
 from .conditional_node_result import ConditionalNodeResult
 from .conditional_node_result_data import ConditionalNodeResultData
 from .deployment_provider_payload_response import DeploymentProviderPayloadResponse
 from .deployment_read import DeploymentRead
 from .document_document_to_document_index import DocumentDocumentToDocumentIndex
+from .document_index_chunking import (
+    DocumentIndexChunking,
+    DocumentIndexChunking_ReductoChunker,
+    DocumentIndexChunking_SentenceChunker,
+    DocumentIndexChunking_TokenOverlappingWindowChunker,
+)
+from .document_index_chunking_request import (
+    DocumentIndexChunkingRequest,
+    DocumentIndexChunkingRequest_ReductoChunker,
+    DocumentIndexChunkingRequest_SentenceChunker,
+    DocumentIndexChunkingRequest_TokenOverlappingWindowChunker,
+)
+from .document_index_indexing_config import DocumentIndexIndexingConfig
+from .document_index_indexing_config_request import DocumentIndexIndexingConfigRequest
 from .document_index_read import DocumentIndexRead
 from .document_read import DocumentRead
 from .document_status import DocumentStatus
 from .enriched_normalized_completion import EnrichedNormalizedCompletion
 from .entity_status import EntityStatus
 from .environment_enum import EnvironmentEnum
 from .error_enum import ErrorEnum
@@ -126,54 +161,82 @@
 from .external_test_case_execution import ExternalTestCaseExecution
 from .external_test_case_execution_request import ExternalTestCaseExecutionRequest
 from .finish_reason_enum import FinishReasonEnum
 from .fulfilled_enum import FulfilledEnum
 from .fulfilled_execute_prompt_event import FulfilledExecutePromptEvent
 from .fulfilled_execute_prompt_response import FulfilledExecutePromptResponse
 from .fulfilled_execute_workflow_workflow_result_event import FulfilledExecuteWorkflowWorkflowResultEvent
-from .fulfilled_function_call import FulfilledFunctionCall
-from .fulfilled_function_call_request import FulfilledFunctionCallRequest
 from .fulfilled_prompt_execution_meta import FulfilledPromptExecutionMeta
 from .fulfilled_workflow_node_result_event import FulfilledWorkflowNodeResultEvent
-from .function_call import FunctionCall, FunctionCall_Fulfilled, FunctionCall_Rejected
+from .function_call import FunctionCall
 from .function_call_chat_message_content import FunctionCallChatMessageContent
 from .function_call_chat_message_content_request import FunctionCallChatMessageContentRequest
 from .function_call_chat_message_content_value import FunctionCallChatMessageContentValue
 from .function_call_chat_message_content_value_request import FunctionCallChatMessageContentValueRequest
 from .function_call_enum import FunctionCallEnum
+from .function_call_request import FunctionCallRequest
 from .function_call_variable_value import FunctionCallVariableValue
 from .function_call_vellum_value import FunctionCallVellumValue
 from .generate_error_response import GenerateErrorResponse
 from .generate_options_request import GenerateOptionsRequest
 from .generate_request import GenerateRequest
 from .generate_response import GenerateResponse
 from .generate_result import GenerateResult
 from .generate_result_data import GenerateResultData
 from .generate_result_error import GenerateResultError
 from .generate_stream_response import GenerateStreamResponse
 from .generate_stream_result import GenerateStreamResult
 from .generate_stream_result_data import GenerateStreamResultData
+from .hkunlp_instructor_xl_enum import HkunlpInstructorXlEnum
+from .hkunlp_instructor_xl_vectorizer import HkunlpInstructorXlVectorizer
+from .hkunlp_instructor_xl_vectorizer_request import HkunlpInstructorXlVectorizerRequest
 from .image_chat_message_content import ImageChatMessageContent
 from .image_chat_message_content_request import ImageChatMessageContentRequest
 from .image_enum import ImageEnum
 from .image_variable_value import ImageVariableValue
+from .image_vellum_value import ImageVellumValue
+from .indexing_config_vectorizer import (
+    IndexingConfigVectorizer,
+    IndexingConfigVectorizer_HkunlpInstructorXl,
+    IndexingConfigVectorizer_IntfloatMultilingualE5Large,
+    IndexingConfigVectorizer_SentenceTransformersMultiQaMpnetBaseCosV1,
+    IndexingConfigVectorizer_SentenceTransformersMultiQaMpnetBaseDotV1,
+    IndexingConfigVectorizer_TextEmbedding3Large,
+    IndexingConfigVectorizer_TextEmbedding3Small,
+    IndexingConfigVectorizer_TextEmbeddingAda002,
+)
+from .indexing_config_vectorizer_request import (
+    IndexingConfigVectorizerRequest,
+    IndexingConfigVectorizerRequest_HkunlpInstructorXl,
+    IndexingConfigVectorizerRequest_IntfloatMultilingualE5Large,
+    IndexingConfigVectorizerRequest_SentenceTransformersMultiQaMpnetBaseCosV1,
+    IndexingConfigVectorizerRequest_SentenceTransformersMultiQaMpnetBaseDotV1,
+    IndexingConfigVectorizerRequest_TextEmbedding3Large,
+    IndexingConfigVectorizerRequest_TextEmbedding3Small,
+    IndexingConfigVectorizerRequest_TextEmbeddingAda002,
+)
 from .indexing_state_enum import IndexingStateEnum
 from .initiated_enum import InitiatedEnum
 from .initiated_execute_prompt_event import InitiatedExecutePromptEvent
 from .initiated_prompt_execution_meta import InitiatedPromptExecutionMeta
 from .initiated_workflow_node_result_event import InitiatedWorkflowNodeResultEvent
+from .instructor_vectorizer_config import InstructorVectorizerConfig
+from .instructor_vectorizer_config_request import InstructorVectorizerConfigRequest
+from .intfloat_multilingual_e_5_large_enum import IntfloatMultilingualE5LargeEnum
 from .json_enum import JsonEnum
 from .json_input_request import JsonInputRequest
 from .json_variable_value import JsonVariableValue
 from .json_vellum_value import JsonVellumValue
 from .logical_operator import LogicalOperator
 from .logprobs_enum import LogprobsEnum
 from .metadata_filter_config_request import MetadataFilterConfigRequest
 from .metadata_filter_rule_combinator import MetadataFilterRuleCombinator
 from .metadata_filter_rule_request import MetadataFilterRuleRequest
+from .metric_enum import MetricEnum
+from .metric_node_result import MetricNodeResult
 from .ml_model_usage import MlModelUsage
 from .named_scenario_input_chat_history_variable_value_request import NamedScenarioInputChatHistoryVariableValueRequest
 from .named_scenario_input_request import (
     NamedScenarioInputRequest,
     NamedScenarioInputRequest_ChatHistory,
     NamedScenarioInputRequest_String,
 )
@@ -250,14 +313,23 @@
     NodeOutputCompiledValue_SearchResults,
     NodeOutputCompiledValue_String,
 )
 from .normalized_log_probs import NormalizedLogProbs
 from .normalized_token_log_probs import NormalizedTokenLogProbs
 from .number_enum import NumberEnum
 from .number_variable_value import NumberVariableValue
+from .number_vellum_value import NumberVellumValue
+from .open_ai_vectorizer_config import OpenAiVectorizerConfig
+from .open_ai_vectorizer_config_request import OpenAiVectorizerConfigRequest
+from .open_ai_vectorizer_text_embedding_3_large import OpenAiVectorizerTextEmbedding3Large
+from .open_ai_vectorizer_text_embedding_3_large_request import OpenAiVectorizerTextEmbedding3LargeRequest
+from .open_ai_vectorizer_text_embedding_3_small import OpenAiVectorizerTextEmbedding3Small
+from .open_ai_vectorizer_text_embedding_3_small_request import OpenAiVectorizerTextEmbedding3SmallRequest
+from .open_ai_vectorizer_text_embedding_ada_002 import OpenAiVectorizerTextEmbeddingAda002
+from .open_ai_vectorizer_text_embedding_ada_002_request import OpenAiVectorizerTextEmbeddingAda002Request
 from .paginated_document_index_read_list import PaginatedDocumentIndexReadList
 from .paginated_slim_deployment_read_list import PaginatedSlimDeploymentReadList
 from .paginated_slim_document_list import PaginatedSlimDocumentList
 from .paginated_slim_workflow_deployment_list import PaginatedSlimWorkflowDeploymentList
 from .paginated_test_suite_run_execution_list import PaginatedTestSuiteRunExecutionList
 from .paginated_test_suite_test_case_list import PaginatedTestSuiteTestCaseList
 from .processing_failure_reason_enum import ProcessingFailureReasonEnum
@@ -276,19 +348,23 @@
     PromptOutput,
     PromptOutput_Error,
     PromptOutput_FunctionCall,
     PromptOutput_Json,
     PromptOutput_String,
 )
 from .raw_prompt_execution_overrides_request import RawPromptExecutionOverridesRequest
+from .reducto_chunker_config import ReductoChunkerConfig
+from .reducto_chunker_config_request import ReductoChunkerConfigRequest
+from .reducto_chunker_enum import ReductoChunkerEnum
+from .reducto_chunking import ReductoChunking
+from .reducto_chunking_request import ReductoChunkingRequest
 from .rejected_enum import RejectedEnum
 from .rejected_execute_prompt_event import RejectedExecutePromptEvent
 from .rejected_execute_prompt_response import RejectedExecutePromptResponse
 from .rejected_execute_workflow_workflow_result_event import RejectedExecuteWorkflowWorkflowResultEvent
-from .rejected_function_call import RejectedFunctionCall
 from .rejected_prompt_execution_meta import RejectedPromptExecutionMeta
 from .rejected_workflow_node_result_event import RejectedWorkflowNodeResultEvent
 from .sandbox_scenario import SandboxScenario
 from .scenario_input import ScenarioInput, ScenarioInput_ChatHistory, ScenarioInput_String
 from .scenario_input_chat_history_variable_value import ScenarioInputChatHistoryVariableValue
 from .scenario_input_string_variable_value import ScenarioInputStringVariableValue
 from .search_error_response import SearchErrorResponse
@@ -299,16 +375,22 @@
 from .search_response import SearchResponse
 from .search_result import SearchResult
 from .search_result_document import SearchResultDocument
 from .search_result_document_request import SearchResultDocumentRequest
 from .search_result_merging_request import SearchResultMergingRequest
 from .search_result_request import SearchResultRequest
 from .search_results_enum import SearchResultsEnum
-from .search_results_variable_value import SearchResultsVariableValue
 from .search_weights_request import SearchWeightsRequest
+from .sentence_chunker_config import SentenceChunkerConfig
+from .sentence_chunker_config_request import SentenceChunkerConfigRequest
+from .sentence_chunker_enum import SentenceChunkerEnum
+from .sentence_chunking import SentenceChunking
+from .sentence_chunking_request import SentenceChunkingRequest
+from .sentence_transformers_multi_qa_mpnet_base_cos_v_1_enum import SentenceTransformersMultiQaMpnetBaseCosV1Enum
+from .sentence_transformers_multi_qa_mpnet_base_dot_v_1_enum import SentenceTransformersMultiQaMpnetBaseDotV1Enum
 from .slim_deployment_read import SlimDeploymentRead
 from .slim_document import SlimDocument
 from .slim_workflow_deployment import SlimWorkflowDeployment
 from .streaming_enum import StreamingEnum
 from .streaming_execute_prompt_event import StreamingExecutePromptEvent
 from .streaming_prompt_execution_meta import StreamingPromptExecutionMeta
 from .streaming_workflow_node_result_event import StreamingWorkflowNodeResultEvent
@@ -452,14 +534,22 @@
 from .test_suite_run_workflow_release_tag_exec_config_data import TestSuiteRunWorkflowReleaseTagExecConfigData
 from .test_suite_run_workflow_release_tag_exec_config_data_request import (
     TestSuiteRunWorkflowReleaseTagExecConfigDataRequest,
 )
 from .test_suite_run_workflow_release_tag_exec_config_request import TestSuiteRunWorkflowReleaseTagExecConfigRequest
 from .test_suite_run_workflow_release_tag_exec_config_type_enum import TestSuiteRunWorkflowReleaseTagExecConfigTypeEnum
 from .test_suite_test_case import TestSuiteTestCase
+from .text_embedding_3_large_enum import TextEmbedding3LargeEnum
+from .text_embedding_3_small_enum import TextEmbedding3SmallEnum
+from .text_embedding_ada_002_enum import TextEmbeddingAda002Enum
+from .token_overlapping_window_chunker_config import TokenOverlappingWindowChunkerConfig
+from .token_overlapping_window_chunker_config_request import TokenOverlappingWindowChunkerConfigRequest
+from .token_overlapping_window_chunker_enum import TokenOverlappingWindowChunkerEnum
+from .token_overlapping_window_chunking import TokenOverlappingWindowChunking
+from .token_overlapping_window_chunking_request import TokenOverlappingWindowChunkingRequest
 from .upload_document_error_response import UploadDocumentErrorResponse
 from .upload_document_response import UploadDocumentResponse
 from .vellum_error import VellumError
 from .vellum_error_code_enum import VellumErrorCodeEnum
 from .vellum_error_request import VellumErrorRequest
 from .vellum_image import VellumImage
 from .vellum_image_request import VellumImageRequest
@@ -475,14 +565,15 @@
 from .workflow_execution_node_result_event import WorkflowExecutionNodeResultEvent
 from .workflow_execution_workflow_result_event import WorkflowExecutionWorkflowResultEvent
 from .workflow_node_result_data import (
     WorkflowNodeResultData,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
+    WorkflowNodeResultData_Metric,
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
     WorkflowNodeResultData_Subworkflow,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_Terminal,
 )
 from .workflow_node_result_event import (
@@ -544,39 +635,50 @@
 from .workflow_result_event_output_data_json import WorkflowResultEventOutputDataJson
 from .workflow_result_event_output_data_number import WorkflowResultEventOutputDataNumber
 from .workflow_result_event_output_data_search_results import WorkflowResultEventOutputDataSearchResults
 from .workflow_result_event_output_data_string import WorkflowResultEventOutputDataString
 from .workflow_stream_event import WorkflowStreamEvent, WorkflowStreamEvent_Node, WorkflowStreamEvent_Workflow
 
 __all__ = [
+    "AddOpenaiApiKeyEnum",
     "ApiNodeResult",
     "ApiNodeResultData",
     "ArrayChatMessageContent",
     "ArrayChatMessageContentItem",
     "ArrayChatMessageContentItemRequest",
     "ArrayChatMessageContentItemRequest_FunctionCall",
     "ArrayChatMessageContentItemRequest_Image",
     "ArrayChatMessageContentItemRequest_String",
     "ArrayChatMessageContentItem_FunctionCall",
     "ArrayChatMessageContentItem_Image",
     "ArrayChatMessageContentItem_String",
     "ArrayChatMessageContentRequest",
     "ArrayEnum",
     "ArrayVariableValueItem",
-    "ArrayVariableValueItem_ChatHistory",
     "ArrayVariableValueItem_Error",
     "ArrayVariableValueItem_FunctionCall",
     "ArrayVariableValueItem_Image",
     "ArrayVariableValueItem_Json",
     "ArrayVariableValueItem_Number",
-    "ArrayVariableValueItem_SearchResults",
     "ArrayVariableValueItem_String",
+    "ArrayVellumValueItem",
+    "ArrayVellumValueItem_Error",
+    "ArrayVellumValueItem_FunctionCall",
+    "ArrayVellumValueItem_Image",
+    "ArrayVellumValueItem_Json",
+    "ArrayVellumValueItem_Number",
+    "ArrayVellumValueItem_String",
+    "BasicVectorizerIntfloatMultilingualE5Large",
+    "BasicVectorizerIntfloatMultilingualE5LargeRequest",
+    "BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1",
+    "BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1Request",
+    "BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1",
+    "BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1Request",
     "ChatHistoryEnum",
     "ChatHistoryInputRequest",
-    "ChatHistoryVariableValue",
     "ChatMessage",
     "ChatMessageContent",
     "ChatMessageContentRequest",
     "ChatMessageContentRequest_Array",
     "ChatMessageContentRequest_FunctionCall",
     "ChatMessageContentRequest_Image",
     "ChatMessageContentRequest_String",
@@ -606,14 +708,24 @@
     "CodeExecutionNodeSearchResultsResult",
     "CodeExecutionNodeStringResult",
     "ConditionalNodeResult",
     "ConditionalNodeResultData",
     "DeploymentProviderPayloadResponse",
     "DeploymentRead",
     "DocumentDocumentToDocumentIndex",
+    "DocumentIndexChunking",
+    "DocumentIndexChunkingRequest",
+    "DocumentIndexChunkingRequest_ReductoChunker",
+    "DocumentIndexChunkingRequest_SentenceChunker",
+    "DocumentIndexChunkingRequest_TokenOverlappingWindowChunker",
+    "DocumentIndexChunking_ReductoChunker",
+    "DocumentIndexChunking_SentenceChunker",
+    "DocumentIndexChunking_TokenOverlappingWindowChunker",
+    "DocumentIndexIndexingConfig",
+    "DocumentIndexIndexingConfigRequest",
     "DocumentIndexRead",
     "DocumentRead",
     "DocumentStatus",
     "EnrichedNormalizedCompletion",
     "EntityStatus",
     "EnvironmentEnum",
     "ErrorEnum",
@@ -654,56 +766,78 @@
     "ExternalTestCaseExecution",
     "ExternalTestCaseExecutionRequest",
     "FinishReasonEnum",
     "FulfilledEnum",
     "FulfilledExecutePromptEvent",
     "FulfilledExecutePromptResponse",
     "FulfilledExecuteWorkflowWorkflowResultEvent",
-    "FulfilledFunctionCall",
-    "FulfilledFunctionCallRequest",
     "FulfilledPromptExecutionMeta",
     "FulfilledWorkflowNodeResultEvent",
     "FunctionCall",
     "FunctionCallChatMessageContent",
     "FunctionCallChatMessageContentRequest",
     "FunctionCallChatMessageContentValue",
     "FunctionCallChatMessageContentValueRequest",
     "FunctionCallEnum",
+    "FunctionCallRequest",
     "FunctionCallVariableValue",
     "FunctionCallVellumValue",
-    "FunctionCall_Fulfilled",
-    "FunctionCall_Rejected",
     "GenerateErrorResponse",
     "GenerateOptionsRequest",
     "GenerateRequest",
     "GenerateResponse",
     "GenerateResult",
     "GenerateResultData",
     "GenerateResultError",
     "GenerateStreamResponse",
     "GenerateStreamResult",
     "GenerateStreamResultData",
+    "HkunlpInstructorXlEnum",
+    "HkunlpInstructorXlVectorizer",
+    "HkunlpInstructorXlVectorizerRequest",
     "ImageChatMessageContent",
     "ImageChatMessageContentRequest",
     "ImageEnum",
     "ImageVariableValue",
+    "ImageVellumValue",
+    "IndexingConfigVectorizer",
+    "IndexingConfigVectorizerRequest",
+    "IndexingConfigVectorizerRequest_HkunlpInstructorXl",
+    "IndexingConfigVectorizerRequest_IntfloatMultilingualE5Large",
+    "IndexingConfigVectorizerRequest_SentenceTransformersMultiQaMpnetBaseCosV1",
+    "IndexingConfigVectorizerRequest_SentenceTransformersMultiQaMpnetBaseDotV1",
+    "IndexingConfigVectorizerRequest_TextEmbedding3Large",
+    "IndexingConfigVectorizerRequest_TextEmbedding3Small",
+    "IndexingConfigVectorizerRequest_TextEmbeddingAda002",
+    "IndexingConfigVectorizer_HkunlpInstructorXl",
+    "IndexingConfigVectorizer_IntfloatMultilingualE5Large",
+    "IndexingConfigVectorizer_SentenceTransformersMultiQaMpnetBaseCosV1",
+    "IndexingConfigVectorizer_SentenceTransformersMultiQaMpnetBaseDotV1",
+    "IndexingConfigVectorizer_TextEmbedding3Large",
+    "IndexingConfigVectorizer_TextEmbedding3Small",
+    "IndexingConfigVectorizer_TextEmbeddingAda002",
     "IndexingStateEnum",
     "InitiatedEnum",
     "InitiatedExecutePromptEvent",
     "InitiatedPromptExecutionMeta",
     "InitiatedWorkflowNodeResultEvent",
+    "InstructorVectorizerConfig",
+    "InstructorVectorizerConfigRequest",
+    "IntfloatMultilingualE5LargeEnum",
     "JsonEnum",
     "JsonInputRequest",
     "JsonVariableValue",
     "JsonVellumValue",
     "LogicalOperator",
     "LogprobsEnum",
     "MetadataFilterConfigRequest",
     "MetadataFilterRuleCombinator",
     "MetadataFilterRuleRequest",
+    "MetricEnum",
+    "MetricNodeResult",
     "MlModelUsage",
     "NamedScenarioInputChatHistoryVariableValueRequest",
     "NamedScenarioInputRequest",
     "NamedScenarioInputRequest_ChatHistory",
     "NamedScenarioInputRequest_String",
     "NamedScenarioInputStringVariableValueRequest",
     "NamedTestCaseChatHistoryVariableValue",
@@ -770,14 +904,23 @@
     "NodeOutputCompiledValue_Number",
     "NodeOutputCompiledValue_SearchResults",
     "NodeOutputCompiledValue_String",
     "NormalizedLogProbs",
     "NormalizedTokenLogProbs",
     "NumberEnum",
     "NumberVariableValue",
+    "NumberVellumValue",
+    "OpenAiVectorizerConfig",
+    "OpenAiVectorizerConfigRequest",
+    "OpenAiVectorizerTextEmbedding3Large",
+    "OpenAiVectorizerTextEmbedding3LargeRequest",
+    "OpenAiVectorizerTextEmbedding3Small",
+    "OpenAiVectorizerTextEmbedding3SmallRequest",
+    "OpenAiVectorizerTextEmbeddingAda002",
+    "OpenAiVectorizerTextEmbeddingAda002Request",
     "PaginatedDocumentIndexReadList",
     "PaginatedSlimDeploymentReadList",
     "PaginatedSlimDocumentList",
     "PaginatedSlimWorkflowDeploymentList",
     "PaginatedTestSuiteRunExecutionList",
     "PaginatedTestSuiteTestCaseList",
     "ProcessingFailureReasonEnum",
@@ -792,19 +935,23 @@
     "PromptNodeResultData",
     "PromptOutput",
     "PromptOutput_Error",
     "PromptOutput_FunctionCall",
     "PromptOutput_Json",
     "PromptOutput_String",
     "RawPromptExecutionOverridesRequest",
+    "ReductoChunkerConfig",
+    "ReductoChunkerConfigRequest",
+    "ReductoChunkerEnum",
+    "ReductoChunking",
+    "ReductoChunkingRequest",
     "RejectedEnum",
     "RejectedExecutePromptEvent",
     "RejectedExecutePromptResponse",
     "RejectedExecuteWorkflowWorkflowResultEvent",
-    "RejectedFunctionCall",
     "RejectedPromptExecutionMeta",
     "RejectedWorkflowNodeResultEvent",
     "SandboxScenario",
     "ScenarioInput",
     "ScenarioInputChatHistoryVariableValue",
     "ScenarioInputStringVariableValue",
     "ScenarioInput_ChatHistory",
@@ -817,16 +964,22 @@
     "SearchResponse",
     "SearchResult",
     "SearchResultDocument",
     "SearchResultDocumentRequest",
     "SearchResultMergingRequest",
     "SearchResultRequest",
     "SearchResultsEnum",
-    "SearchResultsVariableValue",
     "SearchWeightsRequest",
+    "SentenceChunkerConfig",
+    "SentenceChunkerConfigRequest",
+    "SentenceChunkerEnum",
+    "SentenceChunking",
+    "SentenceChunkingRequest",
+    "SentenceTransformersMultiQaMpnetBaseCosV1Enum",
+    "SentenceTransformersMultiQaMpnetBaseDotV1Enum",
     "SlimDeploymentRead",
     "SlimDocument",
     "SlimWorkflowDeployment",
     "StreamingEnum",
     "StreamingExecutePromptEvent",
     "StreamingPromptExecutionMeta",
     "StreamingWorkflowNodeResultEvent",
@@ -948,14 +1101,22 @@
     "TestSuiteRunTestSuite",
     "TestSuiteRunWorkflowReleaseTagExecConfig",
     "TestSuiteRunWorkflowReleaseTagExecConfigData",
     "TestSuiteRunWorkflowReleaseTagExecConfigDataRequest",
     "TestSuiteRunWorkflowReleaseTagExecConfigRequest",
     "TestSuiteRunWorkflowReleaseTagExecConfigTypeEnum",
     "TestSuiteTestCase",
+    "TextEmbedding3LargeEnum",
+    "TextEmbedding3SmallEnum",
+    "TextEmbeddingAda002Enum",
+    "TokenOverlappingWindowChunkerConfig",
+    "TokenOverlappingWindowChunkerConfigRequest",
+    "TokenOverlappingWindowChunkerEnum",
+    "TokenOverlappingWindowChunking",
+    "TokenOverlappingWindowChunkingRequest",
     "UploadDocumentErrorResponse",
     "UploadDocumentResponse",
     "VellumError",
     "VellumErrorCodeEnum",
     "VellumErrorRequest",
     "VellumImage",
     "VellumImageRequest",
@@ -970,14 +1131,15 @@
     "WorkflowExecutionEventType",
     "WorkflowExecutionNodeResultEvent",
     "WorkflowExecutionWorkflowResultEvent",
     "WorkflowNodeResultData",
     "WorkflowNodeResultData_Api",
     "WorkflowNodeResultData_CodeExecution",
     "WorkflowNodeResultData_Conditional",
+    "WorkflowNodeResultData_Metric",
     "WorkflowNodeResultData_Prompt",
     "WorkflowNodeResultData_Search",
     "WorkflowNodeResultData_Subworkflow",
     "WorkflowNodeResultData_Templating",
     "WorkflowNodeResultData_Terminal",
     "WorkflowNodeResultEvent",
     "WorkflowNodeResultEventState",
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/api_node_result.py` & `vellum_ai-0.6.0/src/vellum/types/api_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/api_node_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/api_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/array_chat_message_content.py` & `vellum_ai-0.6.0/src/vellum/types/array_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_item.py` & `vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_item.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_item_request.py` & `vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_item_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/array_chat_message_content_request.py` & `vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/array_variable_value_item.py` & `vellum_ai-0.6.0/src/vellum/types/array_variable_value_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from __future__ import annotations
 
 import typing
 
-from .chat_history_variable_value import ChatHistoryVariableValue
 from .error_variable_value import ErrorVariableValue
 from .function_call_variable_value import FunctionCallVariableValue
 from .image_variable_value import ImageVariableValue
 from .json_variable_value import JsonVariableValue
 from .number_variable_value import NumberVariableValue
-from .search_results_variable_value import SearchResultsVariableValue
 from .string_variable_value import StringVariableValue
 
 
 class ArrayVariableValueItem_String(StringVariableValue):
     type: typing.Literal["STRING"] = "STRING"
 
     class Config:
@@ -40,34 +38,14 @@
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
 
 
-class ArrayVariableValueItem_ChatHistory(ChatHistoryVariableValue):
-    type: typing.Literal["CHAT_HISTORY"] = "CHAT_HISTORY"
-
-    class Config:
-        frozen = True
-        smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
-
-
-class ArrayVariableValueItem_SearchResults(SearchResultsVariableValue):
-    type: typing.Literal["SEARCH_RESULTS"] = "SEARCH_RESULTS"
-
-    class Config:
-        frozen = True
-        smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
-
-
 class ArrayVariableValueItem_Error(ErrorVariableValue):
     type: typing.Literal["ERROR"] = "ERROR"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
@@ -94,13 +72,11 @@
         populate_by_name = True
 
 
 ArrayVariableValueItem = typing.Union[
     ArrayVariableValueItem_String,
     ArrayVariableValueItem_Number,
     ArrayVariableValueItem_Json,
-    ArrayVariableValueItem_ChatHistory,
-    ArrayVariableValueItem_SearchResults,
     ArrayVariableValueItem_Error,
     ArrayVariableValueItem_FunctionCall,
     ArrayVariableValueItem_Image,
 ]
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/chat_history_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/chat_history_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/chat_history_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_chat_history_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .chat_message import ChatMessage
 
 
-class ChatHistoryVariableValue(pydantic_v1.BaseModel):
+class TemplatingNodeChatHistoryResult(pydantic_v1.BaseModel):
+    id: str
     value: typing.Optional[typing.List[ChatMessage]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/chat_message.py` & `vellum_ai-0.6.0/src/vellum/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/chat_message_content.py` & `vellum_ai-0.6.0/src/vellum/types/chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/chat_message_content_request.py` & `vellum_ai-0.6.0/src/vellum/types/chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/chat_message_request.py` & `vellum_ai-0.6.0/src/vellum/types/chat_message_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_array_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_chat_history_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_error_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_function_call_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_function_call_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_json_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_number_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_result_output.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_search_results_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/code_execution_node_string_result.py` & `vellum_ai-0.6.0/src/vellum/types/code_execution_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/conditional_node_result.py` & `vellum_ai-0.6.0/src/vellum/types/conditional_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/conditional_node_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/conditional_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/deployment_provider_payload_response.py` & `vellum_ai-0.6.0/src/vellum/types/deployment_provider_payload_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/deployment_read.py` & `vellum_ai-0.6.0/src/vellum/types/deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.6.0/src/vellum/types/document_document_to_document_index.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/document_index_read.py` & `vellum_ai-0.6.0/src/vellum/types/document_index_read.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .document_index_indexing_config import DocumentIndexIndexingConfig
 from .entity_status import EntityStatus
 from .environment_enum import EnvironmentEnum
 
 
 class DocumentIndexRead(pydantic_v1.BaseModel):
     id: str
     created: dt.datetime
@@ -35,18 +36,15 @@
     The environment this document index is used in
     
     - `DEVELOPMENT` - Development
     - `STAGING` - Staging
     - `PRODUCTION` - Production
     """
 
-    indexing_config: typing.Dict[str, typing.Any] = pydantic_v1.Field()
-    """
-    Configuration representing how documents should be indexed
-    """
+    indexing_config: DocumentIndexIndexingConfig
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/document_read.py` & `vellum_ai-0.6.0/src/vellum/types/document_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.6.0/src/vellum/types/enriched_normalized_completion.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/error_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/error_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/error_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execute_prompt_api_error_response.py` & `vellum_ai-0.6.0/src/vellum/types/execute_prompt_api_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execute_prompt_event.py` & `vellum_ai-0.6.0/src/vellum/types/execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execute_prompt_response.py` & `vellum_ai-0.6.0/src/vellum/types/execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execute_workflow_error_response.py` & `vellum_ai-0.6.0/src/vellum/types/execute_workflow_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execute_workflow_response.py` & `vellum_ai-0.6.0/src/vellum/types/execute_workflow_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execute_workflow_stream_error_response.py` & `vellum_ai-0.6.0/src/vellum/types/execute_workflow_stream_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execute_workflow_workflow_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_array_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_array_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_chat_history_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_chat_history_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_error_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_error_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_function_call_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_function_call_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_json_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_json_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_number_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_number_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_search_results_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_search_results_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_string_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_string_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/execution_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/execution_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/external_test_case_execution.py` & `vellum_ai-0.6.0/src/vellum/types/external_test_case_execution.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/external_test_case_execution_request.py` & `vellum_ai-0.6.0/src/vellum/types/external_test_case_execution_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_prompt_event.py` & `vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_prompt_response.py` & `vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/fulfilled_function_call.py` & `vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_value.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class FulfilledFunctionCall(pydantic_v1.BaseModel):
+class FunctionCallChatMessageContentValue(pydantic_v1.BaseModel):
     """
     The final resolved function call value.
     """
 
+    name: str
     arguments: typing.Dict[str, typing.Any]
     id: typing.Optional[str] = None
-    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/fulfilled_function_call_request.py` & `vellum_ai-0.6.0/src/vellum/types/function_call_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .fulfilled_enum import FulfilledEnum
 
 
-class FulfilledFunctionCallRequest(pydantic_v1.BaseModel):
+class FunctionCallRequest(pydantic_v1.BaseModel):
     """
     The final resolved function call value.
     """
 
-    state: FulfilledEnum
     arguments: typing.Dict[str, typing.Any]
     id: typing.Optional[str] = None
     name: str
+    state: typing.Optional[FulfilledEnum] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/fulfilled_prompt_execution_meta.py` & `vellum_ai-0.6.0/src/vellum/types/fulfilled_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/fulfilled_workflow_node_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/fulfilled_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content.py` & `vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_request.py` & `vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_value.py` & `vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_value_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class FunctionCallChatMessageContentValue(pydantic_v1.BaseModel):
+class FunctionCallChatMessageContentValueRequest(pydantic_v1.BaseModel):
     """
     The final resolved function call value.
     """
 
     name: str
     arguments: typing.Dict[str, typing.Any]
     id: typing.Optional[str] = None
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/function_call_chat_message_content_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class FunctionCallChatMessageContentValueRequest(pydantic_v1.BaseModel):
+class TokenOverlappingWindowChunkerConfig(pydantic_v1.BaseModel):
     """
-    The final resolved function call value.
+    Configuration for token overlapping window chunking
     """
 
-    name: str
-    arguments: typing.Dict[str, typing.Any]
-    id: typing.Optional[str] = None
+    token_limit: typing.Optional[int] = None
+    overlap_ratio: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/function_call_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/function_call_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/function_call_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_function_call_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .function_call import FunctionCall
 
 
-class FunctionCallVellumValue(pydantic_v1.BaseModel):
+class TerminalNodeFunctionCallResult(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = None
+    name: str = pydantic_v1.Field()
     """
-    A value representing a Function Call.
+    The unique name given to the terminal node that produced this output.
     """
 
-    value: FunctionCall
+    value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_error_response.py` & `vellum_ai-0.6.0/src/vellum/types/generate_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_options_request.py` & `vellum_ai-0.6.0/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_request.py` & `vellum_ai-0.6.0/src/vellum/types/generate_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_response.py` & `vellum_ai-0.6.0/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_result.py` & `vellum_ai-0.6.0/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/generate_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_result_error.py` & `vellum_ai-0.6.0/src/vellum/types/generate_result_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_stream_response.py` & `vellum_ai-0.6.0/src/vellum/types/generate_stream_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_stream_result.py` & `vellum_ai-0.6.0/src/vellum/types/generate_stream_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/generate_stream_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/generate_stream_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/image_chat_message_content.py` & `vellum_ai-0.6.0/src/vellum/types/image_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/image_chat_message_content_request.py` & `vellum_ai-0.6.0/src/vellum/types/image_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/image_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/image_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/initiated_execute_prompt_event.py` & `vellum_ai-0.6.0/src/vellum/types/initiated_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/initiated_prompt_execution_meta.py` & `vellum_ai-0.6.0/src/vellum/types/initiated_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/initiated_workflow_node_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/initiated_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/json_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/json_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/json_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/json_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/json_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/metadata_filter_config_request.py` & `vellum_ai-0.6.0/src/vellum/types/metadata_filter_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/metadata_filter_rule_request.py` & `vellum_ai-0.6.0/src/vellum/types/metadata_filter_rule_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/ml_model_usage.py` & `vellum_ai-0.6.0/src/vellum/types/ml_model_usage.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_scenario_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_scenario_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_scenario_input_string_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_scenario_input_string_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_chat_history_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_chat_history_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_chat_history_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_error_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_error_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_error_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_function_call_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_case_function_call_variable_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .fulfilled_function_call import FulfilledFunctionCall
+from .function_call import FunctionCall
 
 
-class NamedTestCaseFunctionCallVariableValue(pydantic_v1.BaseModel):
+class TestCaseFunctionCallVariableValue(pydantic_v1.BaseModel):
     """
-    Named Test Case value that is of type FUNCTION_CALL
+    A function call value for a variable in a Test Case.
     """
 
-    value: typing.Optional[FulfilledFunctionCall] = None
+    variable_id: str
     name: str
+    value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_function_call_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_search_results_variable_value_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .fulfilled_function_call_request import FulfilledFunctionCallRequest
+from .search_result_request import SearchResultRequest
 
 
-class NamedTestCaseFunctionCallVariableValueRequest(pydantic_v1.BaseModel):
+class NamedTestCaseSearchResultsVariableValueRequest(pydantic_v1.BaseModel):
     """
-    Named Test Case value that is of type FUNCTION_CALL
+    Named Test Case value that is of type SEARCH_RESULTS
     """
 
-    value: typing.Optional[FulfilledFunctionCallRequest] = None
+    value: typing.Optional[typing.List[SearchResultRequest]] = None
     name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_json_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_json_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_json_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_number_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_number_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_number_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_search_results_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_search_results_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_search_results_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_string_variable_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .search_result_request import SearchResultRequest
 
 
-class NamedTestCaseSearchResultsVariableValueRequest(pydantic_v1.BaseModel):
+class NamedTestCaseStringVariableValue(pydantic_v1.BaseModel):
     """
-    Named Test Case value that is of type SEARCH_RESULTS
+    Named Test Case value that is of type STRING
     """
 
-    value: typing.Optional[typing.List[SearchResultRequest]] = None
+    value: typing.Optional[str] = None
     name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_string_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/search_result_merging_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class NamedTestCaseStringVariableValue(pydantic_v1.BaseModel):
+class SearchResultMergingRequest(pydantic_v1.BaseModel):
+    enabled: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
-    Named Test Case value that is of type STRING
+    Whether to enable merging results
     """
 
-    value: typing.Optional[str] = None
-    name: str
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_string_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_string_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/named_test_case_variable_value_request.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_array_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_array_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_chat_history_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_chat_history_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_error_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_error_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_function_call.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_json_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_json_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_number_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_number_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_search_results_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_search_results_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_compiled_string_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_string_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_input_variable_compiled_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_input_variable_compiled_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_array_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_array_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .array_variable_value_item import ArrayVariableValueItem
+from .array_vellum_value_item import ArrayVellumValueItem
 from .workflow_node_result_event_state import WorkflowNodeResultEventState
 
 
 class NodeOutputCompiledArrayValue(pydantic_v1.BaseModel):
     """
     An output returned by a node that is of type ARRAY.
     """
 
-    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
+    value: typing.Optional[typing.List[ArrayVellumValueItem]] = None
     node_output_id: str
     state: typing.Optional[WorkflowNodeResultEventState] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_chat_history_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_chat_history_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_error_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_error_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_function_call_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_function_call_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_json_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_json_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_number_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_number_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_search_results_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_search_results_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_string_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_string_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/node_output_compiled_value.py` & `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.6.0/src/vellum/types/normalized_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.6.0/src/vellum/types/normalized_token_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/number_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/paginated_document_index_read_list.py` & `vellum_ai-0.6.0/src/vellum/types/paginated_document_index_read_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/paginated_slim_deployment_read_list.py` & `vellum_ai-0.6.0/src/vellum/types/paginated_slim_deployment_read_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.6.0/src/vellum/types/paginated_slim_document_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/paginated_slim_workflow_deployment_list.py` & `vellum_ai-0.6.0/src/vellum/types/paginated_slim_workflow_deployment_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/paginated_test_suite_run_execution_list.py` & `vellum_ai-0.6.0/src/vellum/types/paginated_test_suite_run_execution_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/paginated_test_suite_test_case_list.py` & `vellum_ai-0.6.0/src/vellum/types/paginated_test_suite_test_case_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/prompt_deployment_expand_meta_request_request.py` & `vellum_ai-0.6.0/src/vellum/types/prompt_deployment_expand_meta_request_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/prompt_deployment_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/prompt_deployment_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/prompt_execution_meta.py` & `vellum_ai-0.6.0/src/vellum/types/prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/prompt_node_result.py` & `vellum_ai-0.6.0/src/vellum/types/prompt_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/prompt_node_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/prompt_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/prompt_output.py` & `vellum_ai-0.6.0/src/vellum/types/prompt_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/raw_prompt_execution_overrides_request.py` & `vellum_ai-0.6.0/src/vellum/types/raw_prompt_execution_overrides_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/rejected_execute_prompt_event.py` & `vellum_ai-0.6.0/src/vellum/types/rejected_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/rejected_execute_prompt_response.py` & `vellum_ai-0.6.0/src/vellum/types/rejected_execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/rejected_execute_workflow_workflow_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/rejected_execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/rejected_function_call.py` & `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .vellum_error import VellumError
 
 
-class RejectedFunctionCall(pydantic_v1.BaseModel):
+class BasicVectorizerSentenceTransformersMultiQaMpnetBaseCosV1(pydantic_v1.BaseModel):
     """
-    Returned if the function call failed to parse for some reason.
+    Basic vectorizer for sentence-transformers/multi-qa-mpnet-base-cos-v1.
     """
 
-    error: VellumError
-    id: typing.Optional[str] = None
-    name: str
+    config: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/rejected_prompt_execution_meta.py` & `vellum_ai-0.6.0/src/vellum/types/rejected_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/rejected_workflow_node_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/rejected_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/sandbox_scenario.py` & `vellum_ai-0.6.0/src/vellum/types/sandbox_scenario.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/scenario_input.py` & `vellum_ai-0.6.0/src/vellum/types/scenario_input.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/scenario_input_chat_history_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/scenario_input_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/scenario_input_string_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/scenario_input_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_error_response.py` & `vellum_ai-0.6.0/src/vellum/types/search_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_filters_request.py` & `vellum_ai-0.6.0/src/vellum/types/search_filters_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_node_result.py` & `vellum_ai-0.6.0/src/vellum/types/search_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_node_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/search_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.6.0/src/vellum/types/search_request_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_response.py` & `vellum_ai-0.6.0/src/vellum/types/search_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_result.py` & `vellum_ai-0.6.0/src/vellum/types/search_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_result_document.py` & `vellum_ai-0.6.0/src/vellum/types/search_result_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_result_document_request.py` & `vellum_ai-0.6.0/src/vellum/types/search_result_document_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class SearchResultMergingRequest(pydantic_v1.BaseModel):
-    enabled: typing.Optional[bool] = pydantic_v1.Field(default=None)
+class BasicVectorizerIntfloatMultilingualE5Large(pydantic_v1.BaseModel):
     """
-    Whether to enable merging results
+    Basic vectorizer for intfloat/multilingual-e5-large.
     """
 
+    config: typing.Optional[typing.Dict[str, typing.Any]] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_result_request.py` & `vellum_ai-0.6.0/src/vellum/types/search_result_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_results_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_search_results_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .search_result import SearchResult
 
 
-class SearchResultsVariableValue(pydantic_v1.BaseModel):
+class TemplatingNodeSearchResultsResult(pydantic_v1.BaseModel):
+    id: str
     value: typing.Optional[typing.List[SearchResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/search_weights_request.py` & `vellum_ai-0.6.0/src/vellum/types/search_weights_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/slim_deployment_read.py` & `vellum_ai-0.6.0/src/vellum/types/slim_deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/slim_document.py` & `vellum_ai-0.6.0/src/vellum/types/slim_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/slim_workflow_deployment.py` & `vellum_ai-0.6.0/src/vellum/types/slim_workflow_deployment.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/streaming_execute_prompt_event.py` & `vellum_ai-0.6.0/src/vellum/types/streaming_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/streaming_prompt_execution_meta.py` & `vellum_ai-0.6.0/src/vellum/types/streaming_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/streaming_workflow_node_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/streaming_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/string_chat_message_content.py` & `vellum_ai-0.6.0/src/vellum/types/string_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/string_chat_message_content_request.py` & `vellum_ai-0.6.0/src/vellum/types/string_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/string_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/string_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/string_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/string_vellum_value.py` & `vellum_ai-0.6.0/src/vellum/types/string_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.6.0/src/vellum/types/submit_completion_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.6.0/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/submit_workflow_execution_actual_request.py` & `vellum_ai-0.6.0/src/vellum/types/submit_workflow_execution_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/subworkflow_node_result.py` & `vellum_ai-0.6.0/src/vellum/types/subworkflow_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_array_result.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_chat_history_result.py` & `vellum_ai-0.6.0/src/vellum/types/upload_document_error_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .chat_message import ChatMessage
 
 
-class TemplatingNodeChatHistoryResult(pydantic_v1.BaseModel):
-    id: str
-    value: typing.Optional[typing.List[ChatMessage]] = None
+class UploadDocumentErrorResponse(pydantic_v1.BaseModel):
+    detail: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_error_result.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_function_call_result.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_function_call_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_json_result.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_number_result.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_result.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_result_output.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_search_results_result.py` & `vellum_ai-0.6.0/src/vellum/types/reducto_chunker_config_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .search_result import SearchResult
 
 
-class TemplatingNodeSearchResultsResult(pydantic_v1.BaseModel):
-    id: str
-    value: typing.Optional[typing.List[SearchResult]] = None
+class ReductoChunkerConfigRequest(pydantic_v1.BaseModel):
+    """
+    Configuration for Reducto chunking
+    """
+
+    character_limit: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/templating_node_string_result.py` & `vellum_ai-0.6.0/src/vellum/types/templating_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_array_result.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_chat_history_result.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_error_result.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_function_call_result.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output_function_call.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .function_call import FunctionCall
 
 
-class TerminalNodeFunctionCallResult(pydantic_v1.BaseModel):
-    id: typing.Optional[str] = None
+class WorkflowOutputFunctionCall(pydantic_v1.BaseModel):
+    """
+    A function call output from a Workflow execution.
+    """
+
+    id: str
     name: str = pydantic_v1.Field()
     """
-    The unique name given to the terminal node that produced this output.
+    The output's name, as defined in the workflow
     """
 
     value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_json_result.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_number_result.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_result.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_result_output.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_search_results_result.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/terminal_node_string_result.py` & `vellum_ai-0.6.0/src/vellum/types/terminal_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_case_chat_history_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_case_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_case_error_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_case_error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_case_function_call_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_case_number_variable_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .fulfilled_function_call import FulfilledFunctionCall
 
 
-class TestCaseFunctionCallVariableValue(pydantic_v1.BaseModel):
+class TestCaseNumberVariableValue(pydantic_v1.BaseModel):
     """
-    A function call value for a variable in a Test Case.
+    A numerical value for a variable in a Test Case.
     """
 
     variable_id: str
     name: str
-    value: typing.Optional[FulfilledFunctionCall] = None
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_case_json_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_case_json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_case_number_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_string_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class TestCaseNumberVariableValue(pydantic_v1.BaseModel):
+class TestSuiteRunMetricStringOutput(pydantic_v1.BaseModel):
     """
-    A numerical value for a variable in a Test Case.
+    Output for a test suite run metric that is of type STRING
     """
 
-    variable_id: str
+    value: str
     name: str
-    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_case_search_results_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_case_search_results_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_case_string_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_case_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_case_variable_value.py` & `vellum_ai-0.6.0/src/vellum/types/test_case_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_exec_config.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_exec_config_request.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_chat_history_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_chat_history_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_error_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_error_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_function_call_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_function_call_output.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .fulfilled_function_call import FulfilledFunctionCall
+from .function_call import FunctionCall
 
 
 class TestSuiteRunExecutionFunctionCallOutput(pydantic_v1.BaseModel):
     """
     Execution output of an entity evaluated during a Test Suite Run that is of type FUNCTION_CALL
     """
 
     name: str
-    value: typing.Optional[FulfilledFunctionCall] = None
+    value: typing.Optional[FunctionCall] = None
     output_variable_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_json_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_json_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_metric_definition.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_metric_definition.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_metric_result.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_metric_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_number_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_number_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_search_results_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_search_results_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_execution_string_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_string_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_data.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_data_request.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_external_exec_config_request.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_error_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_error_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_number_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_number_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_output.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_metric_string_output.py` & `vellum_ai-0.6.0/src/vellum/types/upload_document_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class TestSuiteRunMetricStringOutput(pydantic_v1.BaseModel):
+class UploadDocumentResponse(pydantic_v1.BaseModel):
+    document_id: str = pydantic_v1.Field()
     """
-    Output for a test suite run metric that is of type STRING
+    The ID of the newly created document.
     """
 
-    value: str
-    name: str
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_read.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_test_suite.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_test_suite.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/test_suite_test_case.py` & `vellum_ai-0.6.0/src/vellum/types/test_suite_test_case.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.6.0/src/vellum/types/number_vellum_value.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class UploadDocumentErrorResponse(pydantic_v1.BaseModel):
-    detail: str
+class NumberVellumValue(pydantic_v1.BaseModel):
+    """
+    A value representing a number.
+    """
+
+    value: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/upload_document_response.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_event_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .workflow_execution_event_error_code import WorkflowExecutionEventErrorCode
 
 
-class UploadDocumentResponse(pydantic_v1.BaseModel):
-    document_id: str = pydantic_v1.Field()
-    """
-    The ID of the newly created document.
-    """
+class WorkflowEventError(pydantic_v1.BaseModel):
+    message: str
+    code: WorkflowExecutionEventErrorCode
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/vellum_error.py` & `vellum_ai-0.6.0/src/vellum/types/vellum_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/vellum_error_request.py` & `vellum_ai-0.6.0/src/vellum/types/vellum_error_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/vellum_image.py` & `vellum_ai-0.6.0/src/vellum/types/vellum_image.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/vellum_image_request.py` & `vellum_ai-0.6.0/src/vellum/types/vellum_image_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/vellum_variable.py` & `vellum_ai-0.6.0/src/vellum/types/vellum_variable.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_deployment_read.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_event_error.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_execution_workflow_result_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .workflow_execution_event_error_code import WorkflowExecutionEventErrorCode
+from .workflow_result_event import WorkflowResultEvent
 
 
-class WorkflowEventError(pydantic_v1.BaseModel):
-    message: str
-    code: WorkflowExecutionEventErrorCode
+class WorkflowExecutionWorkflowResultEvent(pydantic_v1.BaseModel):
+    """
+    A WORKFLOW-level event emitted from the workflow's execution.
+    """
+
+    execution_id: str
+    run_id: typing.Optional[str] = None
+    external_id: typing.Optional[str] = None
+    data: WorkflowResultEvent
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_chat_history_request.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_chat_history_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,19 @@
     """
 
     quality: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best.
     """
 
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide additional metadata about the feedback submission.
+    """
+
     timestamp: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes.
     """
 
     desired_output_value: typing.Optional[typing.List[ChatMessageRequest]] = pydantic_v1.Field(default=None)
     """
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_json_request.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_json_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     """
 
     quality: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best.
     """
 
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide additional metadata about the feedback submission.
+    """
+
     timestamp: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes.
     """
 
     desired_output_value: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_execution_actual_string_request.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_string_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     """
 
     quality: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Optionally provide a decimal number between 0.0 and 1.0 (inclusive) representing the quality of the output. 0 is the worst, 1 is the best.
     """
 
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide additional metadata about the feedback submission.
+    """
+
     timestamp: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes.
     """
 
     desired_output_value: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_execution_node_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_execution_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_execution_workflow_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .workflow_result_event import WorkflowResultEvent
 
 
-class WorkflowExecutionWorkflowResultEvent(pydantic_v1.BaseModel):
+class BasicVectorizerSentenceTransformersMultiQaMpnetBaseDotV1(pydantic_v1.BaseModel):
     """
-    A WORKFLOW-level event emitted from the workflow's execution.
+    Basic vectorizer for sentence-transformers/multi-qa-mpnet-base-dot-v1.
     """
 
-    execution_id: str
-    run_id: typing.Optional[str] = None
-    external_id: typing.Optional[str] = None
-    data: WorkflowResultEvent
+    config: typing.Optional[typing.Dict[str, typing.Any]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_node_result_data.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_node_result_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import typing
 
 from .api_node_result import ApiNodeResult
 from .code_execution_node_result import CodeExecutionNodeResult
 from .conditional_node_result import ConditionalNodeResult
+from .metric_node_result import MetricNodeResult
 from .prompt_node_result import PromptNodeResult
 from .search_node_result import SearchNodeResult
 from .subworkflow_node_result import SubworkflowNodeResult
 from .templating_node_result import TemplatingNodeResult
 from .terminal_node_result import TerminalNodeResult
 
 
@@ -90,17 +91,28 @@
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
 
 
+class WorkflowNodeResultData_Metric(MetricNodeResult):
+    type: typing.Literal["METRIC"] = "METRIC"
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+
+
 WorkflowNodeResultData = typing.Union[
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_Terminal,
     WorkflowNodeResultData_Subworkflow,
+    WorkflowNodeResultData_Metric,
 ]
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_node_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_array.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output_string.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .array_variable_value_item import ArrayVariableValueItem
 
 
-class WorkflowOutputArray(pydantic_v1.BaseModel):
+class WorkflowOutputString(pydantic_v1.BaseModel):
     """
-    An array output from a Workflow execution.
+    A string output from a Workflow execution.
     """
 
     id: str
     name: str = pydantic_v1.Field()
     """
     The output's name, as defined in the workflow
     """
 
-    value: typing.Optional[typing.List[ArrayVariableValueItem]] = None
+    value: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_chat_history.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output_chat_history.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_error.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_function_call.py` & `vellum_ai-0.6.0/src/vellum/types/function_call_vellum_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,17 @@
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from .function_call import FunctionCall
 
 
-class WorkflowOutputFunctionCall(pydantic_v1.BaseModel):
+class FunctionCallVellumValue(pydantic_v1.BaseModel):
     """
-    A function call output from a Workflow execution.
-    """
-
-    id: str
-    name: str = pydantic_v1.Field()
-    """
-    The output's name, as defined in the workflow
+    A value representing a Function Call.
     """
 
     value: typing.Optional[FunctionCall] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_image.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output_image.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_json.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output_json.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_number.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output_number.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_search_results.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_output_search_results.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_output_string.py` & `vellum_ai-0.6.0/src/vellum/types/named_test_case_function_call_variable_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .function_call import FunctionCall
 
 
-class WorkflowOutputString(pydantic_v1.BaseModel):
+class NamedTestCaseFunctionCallVariableValue(pydantic_v1.BaseModel):
     """
-    A string output from a Workflow execution.
+    Named Test Case value that is of type FUNCTION_CALL
     """
 
-    id: str
-    name: str = pydantic_v1.Field()
-    """
-    The output's name, as defined in the workflow
-    """
-
-    value: typing.Optional[str] = None
+    value: typing.Optional[FunctionCall] = None
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_request_chat_history_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_request_chat_history_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_request_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_request_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_request_json_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_request_json_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_request_number_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_request_number_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_request_string_input_request.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_request_string_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_array.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_array.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_chat_history.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_chat_history.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_error.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_function_call.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_json.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_json.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_number.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_number.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_search_results.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_search_results.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_result_event_output_data_string.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_string.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/src/vellum/types/workflow_stream_event.py` & `vellum_ai-0.6.0/src/vellum/types/workflow_stream_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.5.2/PKG-INFO` & `vellum_ai-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vellum-ai
-Version: 0.5.2
+Version: 0.6.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

