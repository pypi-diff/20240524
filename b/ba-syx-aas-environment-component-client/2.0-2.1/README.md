# Comparing `tmp/ba_syx_aas_environment_component_client-2.0.tar.gz` & `tmp/ba_syx_aas_environment_component_client-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ba_syx_aas_environment_component_client-2.0.tar", max compression
+gzip compressed data, was "ba_syx_aas_environment_component_client-2.1.tar", max compression
```

## Comparing `ba_syx_aas_environment_component_client-2.0.tar` & `ba_syx_aas_environment_component_client-2.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0      182 2024-05-21 16:30:55.230448 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/__init__.py
--rw-r--r--   0        0        0       46 2024-05-21 16:30:55.235610 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-21 16:30:53.185516 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/__init__.py
--rw-r--r--   0        0        0     5429 2024-05-21 16:30:55.679637 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/delete_file_by_path.py
--rw-r--r--   0        0        0     5350 2024-05-21 16:30:55.679637 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/get_file_by_path.py
--rw-r--r--   0        0        0     6800 2024-05-21 16:30:55.708748 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/put_file_by_path.py
--rw-r--r--   0        0        0        0 2024-05-21 16:30:53.200857 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/__init__.py
--rw-r--r--   0        0        0     4711 2024-05-21 16:30:55.716235 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_asset_administration_shell_by_id.py
--rw-r--r--   0        0        0     5683 2024-05-21 16:30:55.708748 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_submodel_reference_by_id_aas_repository.py
--rw-r--r--   0        0        0     4462 2024-05-21 16:30:55.676500 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_thumbnail_aas_repository.py
--rw-r--r--   0        0        0     8256 2024-05-21 16:30:55.642266 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_all_asset_administration_shells.py
--rw-r--r--   0        0        0     6715 2024-05-21 16:30:55.723562 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_all_submodel_references_aas_repository.py
--rw-r--r--   0        0        0     4619 2024-05-21 16:30:55.688600 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_asset_administration_shell_by_id.py
--rw-r--r--   0        0        0     4573 2024-05-21 16:30:55.654653 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_asset_information_aas_repository.py
--rw-r--r--   0        0        0     4641 2024-05-21 16:30:55.621955 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_thumbnail_aas_repository.py
--rw-r--r--   0        0        0     5369 2024-05-21 16:30:55.594896 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/post_asset_administration_shell.py
--rw-r--r--   0        0        0     5718 2024-05-21 16:30:55.562780 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/post_submodel_reference_aas_repository.py
--rw-r--r--   0        0        0     5590 2024-05-21 16:30:55.530974 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_asset_administration_shell_by_id.py
--rw-r--r--   0        0        0     5451 2024-05-21 16:30:55.501471 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_asset_information_aas_repository.py
--rw-r--r--   0        0        0     5965 2024-05-21 16:30:55.530974 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_thumbnail_aas_repository.py
--rw-r--r--   0        0        0        0 2024-05-21 16:30:53.276850 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/__init__.py
--rw-r--r--   0        0        0     4674 2024-05-21 16:30:55.501471 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/delete_concept_description_by_id.py
--rw-r--r--   0        0        0     7716 2024-05-21 16:30:55.476430 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/get_all_concept_descriptions.py
--rw-r--r--   0        0        0     4441 2024-05-21 16:30:55.442955 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/get_concept_description_by_id.py
--rw-r--r--   0        0        0     5076 2024-05-21 16:30:55.419463 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/post_concept_description.py
--rw-r--r--   0        0        0     5345 2024-05-21 16:30:55.391913 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/put_concept_description_by_id.py
--rw-r--r--   0        0        0        0 2024-05-21 16:30:53.316443 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/environment_api/__init__.py
--rw-r--r--   0        0        0     4549 2024-05-21 16:30:55.507038 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/environment_api/upload_environment.py
--rw-r--r--   0        0        0        0 2024-05-21 16:30:53.328230 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/registry_and_discovery_interface/__init__.py
--rw-r--r--   0        0        0     4041 2024-05-21 16:30:55.421216 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/registry_and_discovery_interface/get_description.py
--rw-r--r--   0        0        0        0 2024-05-21 16:30:53.320597 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/serialization_api/__init__.py
--rw-r--r--   0        0        0     7009 2024-05-21 16:30:55.372942 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/serialization_api/generate_serialization_by_ids.py
--rw-r--r--   0        0        0        0 2024-05-21 16:30:52.845186 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/__init__.py
--rw-r--r--   0        0        0     4873 2024-05-21 16:30:55.445954 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/delete_submodel_by_id.py
--rw-r--r--   0        0        0     5576 2024-05-21 16:30:55.285157 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/delete_submodel_element_by_path_submodel_repo.py
--rw-r--r--   0        0        0     9384 2024-05-21 16:30:55.729075 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_all_submodel_elements.py
--rw-r--r--   0        0        0     9242 2024-05-21 16:30:55.606423 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_all_submodels.py
--rw-r--r--   0        0        0     7350 2024-05-21 16:30:55.314155 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id.py
--rw-r--r--   0        0        0     6195 2024-05-21 16:30:55.604820 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id_metadata.py
--rw-r--r--   0        0        0     7672 2024-05-21 16:30:55.647096 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id_value_only.py
--rw-r--r--   0        0        0     9039 2024-05-21 16:30:55.237235 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_element_by_path_submodel_repo.py
--rw-r--r--   0        0        0     9339 2024-05-21 16:30:55.233099 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_element_by_path_value_only_submodel_repo.py
--rw-r--r--   0        0        0     6855 2024-05-21 16:30:55.464912 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/invoke_operation_submodel_repo.py
--rw-r--r--   0        0        0    10207 2024-05-21 16:30:55.338292 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/patch_submodel_by_id_value_only.py
--rw-r--r--   0        0        0     8095 2024-05-21 16:30:55.333048 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/patch_submodel_element_by_path_value_only_submodel_repo.py
--rw-r--r--   0        0        0     4946 2024-05-21 16:30:55.287396 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel.py
--rw-r--r--   0        0        0    12245 2024-05-21 16:30:55.553230 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel_element_by_path_submodel_repo.py
--rw-r--r--   0        0        0     8117 2024-05-21 16:30:55.512791 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel_element_submodel_repo.py
--rw-r--r--   0        0        0     6649 2024-05-21 16:30:55.493926 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/put_submodel_by_id.py
--rw-r--r--   0        0        0    10186 2024-05-21 16:30:55.422842 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/put_submodel_element_by_path_submodel_repo.py
--rw-r--r--   0        0        0    12685 2024-05-21 16:30:55.233099 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/client.py
--rw-r--r--   0        0        0      562 2024-05-21 16:30:55.352018 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/errors.py
--rw-r--r--   0        0        0     7350 2024-05-21 16:30:55.262473 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/__init__.py
--rw-r--r--   0        0        0     4470 2024-05-21 16:30:55.350678 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/administrative_information.py
--rw-r--r--   0        0        0    10044 2024-05-21 16:30:55.716235 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/asset_administration_shell.py
--rw-r--r--   0        0        0     4784 2024-05-21 16:30:55.756286 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/asset_information.py
--rw-r--r--   0        0        0      222 2024-05-21 16:30:54.647454 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/asset_information_asset_kind.py
--rw-r--r--   0        0        0     2075 2024-05-21 16:30:55.649987 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/base_64_url_encoded_cursor.py
--rw-r--r--   0        0        0     8454 2024-05-21 16:30:55.688600 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/concept_description.py
--rw-r--r--   0        0        0     1291 2024-05-21 16:30:55.659676 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/data_specification_content.py
--rw-r--r--   0        0        0     3450 2024-05-21 16:30:55.634611 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/embedded_data_specification.py
--rw-r--r--   0        0        0    12350 2024-05-21 16:30:55.604820 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/entity.py
--rw-r--r--   0        0        0      222 2024-05-21 16:30:55.080311 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/entity_entity_type.py
--rw-r--r--   0        0        0     5254 2024-05-21 16:30:55.654653 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/extension.py
--rw-r--r--   0        0        0      996 2024-05-21 16:30:55.049052 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/extension_value_type.py
--rw-r--r--   0        0        0      167 2024-05-21 16:30:55.021443 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_asset_administration_shells_limit.py
--rw-r--r--   0        0        0      161 2024-05-21 16:30:55.095953 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_concept_descriptions_limit.py
--rw-r--r--   0        0        0      220 2024-05-21 16:30:55.028730 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_submodel_elements_extent.py
--rw-r--r--   0        0        0      177 2024-05-21 16:30:55.017433 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_submodel_elements_level.py
--rw-r--r--   0        0        0      158 2024-05-21 16:30:54.964213 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_submodel_elements_limit.py
--rw-r--r--   0        0        0      173 2024-05-21 16:30:54.872331 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_submodel_references_aas_repository_limit.py
--rw-r--r--   0        0        0      213 2024-05-21 16:30:55.042932 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_submodels_extent.py
--rw-r--r--   0        0        0      170 2024-05-21 16:30:55.102957 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_submodels_level.py
--rw-r--r--   0        0        0      151 2024-05-21 16:30:55.014407 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_all_submodels_limit.py
--rw-r--r--   0        0        0     3366 2024-05-21 16:30:55.512791 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_asset_administration_shells_result.py
--rw-r--r--   0        0        0      213 2024-05-21 16:30:54.918289 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_by_id_extent.py
--rw-r--r--   0        0        0      170 2024-05-21 16:30:54.901163 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_by_id_level.py
--rw-r--r--   0        0        0      178 2024-05-21 16:30:54.880888 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_by_id_metadata_level.py
--rw-r--r--   0        0        0      222 2024-05-21 16:30:54.850590 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_by_id_value_only_extent.py
--rw-r--r--   0        0        0      179 2024-05-21 16:30:54.777050 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_by_id_value_only_level.py
--rw-r--r--   0        0        0      234 2024-05-21 16:30:54.736704 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_element_by_path_submodel_repo_extent.py
--rw-r--r--   0        0        0      191 2024-05-21 16:30:54.717630 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_element_by_path_submodel_repo_level.py
--rw-r--r--   0        0        0      243 2024-05-21 16:30:54.691478 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_element_by_path_value_only_submodel_repo_extent.py
--rw-r--r--   0        0        0      200 2024-05-21 16:30:54.663426 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_submodel_element_by_path_value_only_submodel_repo_level.py
--rw-r--r--   0        0        0     2059 2024-05-21 16:30:55.231286 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/key.py
--rw-r--r--   0        0        0     1087 2024-05-21 16:30:54.588433 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/key_type.py
--rw-r--r--   0        0        0     1880 2024-05-21 16:30:55.516808 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/lang_string_name_type.py
--rw-r--r--   0        0        0     1880 2024-05-21 16:30:55.512791 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/lang_string_text_type.py
--rw-r--r--   0        0        0     3139 2024-05-21 16:30:55.512791 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/message.py
--rw-r--r--   0        0        0      224 2024-05-21 16:30:54.953636 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/message_message_type.py
--rw-r--r--   0        0        0    12315 2024-05-21 16:30:55.386849 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation.py
--rw-r--r--   0        0        0     4740 2024-05-21 16:30:55.350678 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation_request.py
--rw-r--r--   0        0        0     4434 2024-05-21 16:30:55.642266 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation_request_client_timeout_duration.py
--rw-r--r--   0        0        0     2421 2024-05-21 16:30:55.751331 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation_request_client_timeout_duration_xmlschema_type.py
--rw-r--r--   0        0        0     2088 2024-05-21 16:30:55.362703 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation_variable.py
--rw-r--r--   0        0        0     1717 2024-05-21 16:30:55.312407 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/paged_result_paging_metadata.py
--rw-r--r--   0        0        0      181 2024-05-21 16:30:54.670311 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/patch_submodel_by_id_value_only_level.py
--rw-r--r--   0        0        0      183 2024-05-21 16:30:54.642001 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/patch_submodel_element_by_path_value_only_submodel_repo_level.py
--rw-r--r--   0        0        0      235 2024-05-21 16:30:54.620949 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/post_submodel_element_by_path_submodel_repo_extent.py
--rw-r--r--   0        0        0      192 2024-05-21 16:30:54.609863 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/post_submodel_element_by_path_submodel_repo_level.py
--rw-r--r--   0        0        0     2020 2024-05-21 16:30:55.232098 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/put_file_by_path_body.py
--rw-r--r--   0        0        0      151 2024-05-21 16:30:54.563148 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/put_submodel_by_id_level.py
--rw-r--r--   0        0        0      172 2024-05-21 16:30:54.521063 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/put_submodel_element_by_path_submodel_repo_level.py
--rw-r--r--   0        0        0     2080 2024-05-21 16:30:55.333048 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/put_thumbnail_aas_repository_body.py
--rw-r--r--   0        0        0     5626 2024-05-21 16:30:55.327298 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/qualifier.py
--rw-r--r--   0        0        0      258 2024-05-21 16:30:54.922441 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/qualifier_kind.py
--rw-r--r--   0        0        0      996 2024-05-21 16:30:54.903483 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/qualifier_value_type.py
--rw-r--r--   0        0        0     3449 2024-05-21 16:30:55.541648 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/reference.py
--rw-r--r--   0        0        0      213 2024-05-21 16:30:54.836965 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/reference_type.py
--rw-r--r--   0        0        0    10356 2024-05-21 16:30:55.464098 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/relationship_element.py
--rw-r--r--   0        0        0     1863 2024-05-21 16:30:55.422842 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/resource.py
--rw-r--r--   0        0        0     2188 2024-05-21 16:30:55.391913 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/result.py
--rw-r--r--   0        0        0     2576 2024-05-21 16:30:55.362703 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/service_description.py
--rw-r--r--   0        0        0     3468 2024-05-21 16:30:55.313689 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/service_description_profiles_item.py
--rw-r--r--   0        0        0     4591 2024-05-21 16:30:55.284407 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/specific_asset_id.py
--rw-r--r--   0        0        0    12023 2024-05-21 16:30:55.252009 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel.py
--rw-r--r--   0        0        0     9232 2024-05-21 16:30:55.677057 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element.py
--rw-r--r--   0        0        0    10115 2024-05-21 16:30:55.416914 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_collection.py
--rw-r--r--   0        0        0    13431 2024-05-21 16:30:55.415223 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_list.py
--rw-r--r--   0        0        0      826 2024-05-21 16:30:54.981373 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_list_type_value_list_element.py
--rw-r--r--   0        0        0     1017 2024-05-21 16:30:54.987077 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_list_value_type_list_element.py
--rw-r--r--   0        0        0     1271 2024-05-21 16:30:55.310199 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_value.py
--rw-r--r--   0        0        0      178 2024-05-21 16:30:54.978861 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_kind.py
--rw-r--r--   0        0        0     2670 2024-05-21 16:30:55.252009 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_value_only.py
--rw-r--r--   0        0        0     1889 2024-05-21 16:30:55.314155 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_value_only_values_only_map.py
--rw-r--r--   0        0        0     1654 2024-05-21 16:30:55.284407 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/upload_environment_body.py
--rw-r--r--   0        0        0       25 2024-05-21 16:30:51.964161 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/py.typed
--rw-r--r--   0        0        0     1030 2024-05-21 16:30:55.231286 ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/types.py
--rw-r--r--   0        0        0      657 2024-05-21 16:30:52.034166 ba_syx_aas_environment_component_client-2.0/pyproject.toml
--rw-r--r--   0        0        0     5433 2024-05-21 16:30:52.065800 ba_syx_aas_environment_component_client-2.0/README.md
--rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 ba_syx_aas_environment_component_client-2.0/PKG-INFO
+-rw-r--r--   0        0        0      182 2024-05-21 16:30:55.230448 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/__init__.py
+-rw-r--r--   0        0        0       46 2024-05-21 16:30:55.235610 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:30:53.185516 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/__init__.py
+-rw-r--r--   0        0        0     5429 2024-05-21 16:30:55.679637 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/delete_file_by_path.py
+-rw-r--r--   0        0        0     5350 2024-05-21 16:30:55.679637 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/get_file_by_path.py
+-rw-r--r--   0        0        0     6800 2024-05-21 16:30:55.708748 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/put_file_by_path.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:30:53.200857 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/__init__.py
+-rw-r--r--   0        0        0     4711 2024-05-21 16:30:55.716235 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_asset_administration_shell_by_id.py
+-rw-r--r--   0        0        0     5683 2024-05-21 16:30:55.708748 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_submodel_reference_by_id_aas_repository.py
+-rw-r--r--   0        0        0     4462 2024-05-21 16:30:55.676500 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_thumbnail_aas_repository.py
+-rw-r--r--   0        0        0     8256 2024-05-21 16:30:55.642266 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_all_asset_administration_shells.py
+-rw-r--r--   0        0        0     6715 2024-05-21 16:30:55.723562 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_all_submodel_references_aas_repository.py
+-rw-r--r--   0        0        0     4619 2024-05-21 16:30:55.688600 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_asset_administration_shell_by_id.py
+-rw-r--r--   0        0        0     4573 2024-05-21 16:30:55.654653 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_asset_information_aas_repository.py
+-rw-r--r--   0        0        0     4641 2024-05-21 16:30:55.621955 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_thumbnail_aas_repository.py
+-rw-r--r--   0        0        0     5369 2024-05-21 16:30:55.594896 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/post_asset_administration_shell.py
+-rw-r--r--   0        0        0     5718 2024-05-21 16:30:55.562780 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/post_submodel_reference_aas_repository.py
+-rw-r--r--   0        0        0     5590 2024-05-21 16:30:55.530974 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_asset_administration_shell_by_id.py
+-rw-r--r--   0        0        0     5451 2024-05-21 16:30:55.501471 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_asset_information_aas_repository.py
+-rw-r--r--   0        0        0     5965 2024-05-21 16:30:55.530974 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_thumbnail_aas_repository.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:30:53.276850 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/__init__.py
+-rw-r--r--   0        0        0     4674 2024-05-21 16:30:55.501471 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/delete_concept_description_by_id.py
+-rw-r--r--   0        0        0     7716 2024-05-21 16:30:55.476430 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/get_all_concept_descriptions.py
+-rw-r--r--   0        0        0     4441 2024-05-21 16:30:55.442955 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/get_concept_description_by_id.py
+-rw-r--r--   0        0        0     5076 2024-05-21 16:30:55.419463 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/post_concept_description.py
+-rw-r--r--   0        0        0     5345 2024-05-21 16:30:55.391913 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/put_concept_description_by_id.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:30:53.316443 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/environment_api/__init__.py
+-rw-r--r--   0        0        0     4549 2024-05-21 16:30:55.507038 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/environment_api/upload_environment.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:30:53.328230 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/registry_and_discovery_interface/__init__.py
+-rw-r--r--   0        0        0     4041 2024-05-21 16:30:55.421216 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/registry_and_discovery_interface/get_description.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:30:53.320597 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/serialization_api/__init__.py
+-rw-r--r--   0        0        0     7009 2024-05-21 16:30:55.372942 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/serialization_api/generate_serialization_by_ids.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:30:52.845186 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/__init__.py
+-rw-r--r--   0        0        0     4873 2024-05-21 16:30:55.445954 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/delete_submodel_by_id.py
+-rw-r--r--   0        0        0     5576 2024-05-21 16:30:55.285157 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/delete_submodel_element_by_path_submodel_repo.py
+-rw-r--r--   0        0        0     9384 2024-05-21 16:30:55.729075 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_all_submodel_elements.py
+-rw-r--r--   0        0        0     9242 2024-05-21 16:30:55.606423 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_all_submodels.py
+-rw-r--r--   0        0        0     7350 2024-05-21 16:30:55.314155 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id.py
+-rw-r--r--   0        0        0     6195 2024-05-21 16:30:55.604820 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id_metadata.py
+-rw-r--r--   0        0        0     7672 2024-05-21 16:30:55.647096 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id_value_only.py
+-rw-r--r--   0        0        0     9039 2024-05-21 16:30:55.237235 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_element_by_path_submodel_repo.py
+-rw-r--r--   0        0        0     9339 2024-05-21 16:30:55.233099 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_element_by_path_value_only_submodel_repo.py
+-rw-r--r--   0        0        0     6855 2024-05-21 16:30:55.464912 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/invoke_operation_submodel_repo.py
+-rw-r--r--   0        0        0    10207 2024-05-21 16:30:55.338292 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/patch_submodel_by_id_value_only.py
+-rw-r--r--   0        0        0     8095 2024-05-21 16:30:55.333048 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/patch_submodel_element_by_path_value_only_submodel_repo.py
+-rw-r--r--   0        0        0     4946 2024-05-21 16:30:55.287396 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel.py
+-rw-r--r--   0        0        0    12245 2024-05-21 16:30:55.553230 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel_element_by_path_submodel_repo.py
+-rw-r--r--   0        0        0     8117 2024-05-21 16:30:55.512791 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel_element_submodel_repo.py
+-rw-r--r--   0        0        0     6649 2024-05-21 16:30:55.493926 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/put_submodel_by_id.py
+-rw-r--r--   0        0        0    10186 2024-05-21 16:30:55.422842 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/put_submodel_element_by_path_submodel_repo.py
+-rw-r--r--   0        0        0    12685 2024-05-21 16:30:55.233099 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/client.py
+-rw-r--r--   0        0        0      562 2024-05-21 16:30:55.352018 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/errors.py
+-rw-r--r--   0        0        0     7350 2024-05-21 16:30:55.262473 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/__init__.py
+-rw-r--r--   0        0        0     4470 2024-05-21 16:30:55.350678 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/administrative_information.py
+-rw-r--r--   0        0        0    10044 2024-05-21 16:30:55.716235 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/asset_administration_shell.py
+-rw-r--r--   0        0        0     4784 2024-05-21 16:30:55.756286 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/asset_information.py
+-rw-r--r--   0        0        0      221 2024-05-24 14:52:21.052564 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/asset_information_asset_kind.py
+-rw-r--r--   0        0        0     2075 2024-05-21 16:30:55.649987 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/base_64_url_encoded_cursor.py
+-rw-r--r--   0        0        0     8454 2024-05-21 16:30:55.688600 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/concept_description.py
+-rw-r--r--   0        0        0     1291 2024-05-21 16:30:55.659676 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/data_specification_content.py
+-rw-r--r--   0        0        0     3450 2024-05-21 16:30:55.634611 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/embedded_data_specification.py
+-rw-r--r--   0        0        0    12350 2024-05-21 16:30:55.604820 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/entity.py
+-rw-r--r--   0        0        0      222 2024-05-21 16:30:55.080311 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/entity_entity_type.py
+-rw-r--r--   0        0        0     5254 2024-05-21 16:30:55.654653 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/extension.py
+-rw-r--r--   0        0        0      996 2024-05-21 16:30:55.049052 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/extension_value_type.py
+-rw-r--r--   0        0        0      167 2024-05-21 16:30:55.021443 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_asset_administration_shells_limit.py
+-rw-r--r--   0        0        0      161 2024-05-21 16:30:55.095953 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_concept_descriptions_limit.py
+-rw-r--r--   0        0        0      220 2024-05-21 16:30:55.028730 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_submodel_elements_extent.py
+-rw-r--r--   0        0        0      177 2024-05-21 16:30:55.017433 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_submodel_elements_level.py
+-rw-r--r--   0        0        0      158 2024-05-21 16:30:54.964213 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_submodel_elements_limit.py
+-rw-r--r--   0        0        0      173 2024-05-21 16:30:54.872331 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_submodel_references_aas_repository_limit.py
+-rw-r--r--   0        0        0      213 2024-05-21 16:30:55.042932 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_submodels_extent.py
+-rw-r--r--   0        0        0      170 2024-05-21 16:30:55.102957 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_submodels_level.py
+-rw-r--r--   0        0        0      151 2024-05-21 16:30:55.014407 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_all_submodels_limit.py
+-rw-r--r--   0        0        0     3366 2024-05-21 16:30:55.512791 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_asset_administration_shells_result.py
+-rw-r--r--   0        0        0      213 2024-05-21 16:30:54.918289 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_by_id_extent.py
+-rw-r--r--   0        0        0      170 2024-05-21 16:30:54.901163 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_by_id_level.py
+-rw-r--r--   0        0        0      178 2024-05-21 16:30:54.880888 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_by_id_metadata_level.py
+-rw-r--r--   0        0        0      222 2024-05-21 16:30:54.850590 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_by_id_value_only_extent.py
+-rw-r--r--   0        0        0      179 2024-05-21 16:30:54.777050 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_by_id_value_only_level.py
+-rw-r--r--   0        0        0      234 2024-05-21 16:30:54.736704 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_element_by_path_submodel_repo_extent.py
+-rw-r--r--   0        0        0      191 2024-05-21 16:30:54.717630 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_element_by_path_submodel_repo_level.py
+-rw-r--r--   0        0        0      243 2024-05-21 16:30:54.691478 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_element_by_path_value_only_submodel_repo_extent.py
+-rw-r--r--   0        0        0      200 2024-05-21 16:30:54.663426 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_submodel_element_by_path_value_only_submodel_repo_level.py
+-rw-r--r--   0        0        0     2059 2024-05-21 16:30:55.231286 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/key.py
+-rw-r--r--   0        0        0     1079 2024-05-24 14:59:49.626079 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/key_type.py
+-rw-r--r--   0        0        0     1880 2024-05-21 16:30:55.516808 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/lang_string_name_type.py
+-rw-r--r--   0        0        0     1880 2024-05-21 16:30:55.512791 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/lang_string_text_type.py
+-rw-r--r--   0        0        0     3139 2024-05-21 16:30:55.512791 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/message.py
+-rw-r--r--   0        0        0      224 2024-05-21 16:30:54.953636 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/message_message_type.py
+-rw-r--r--   0        0        0    12315 2024-05-21 16:30:55.386849 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation.py
+-rw-r--r--   0        0        0     4740 2024-05-21 16:30:55.350678 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation_request.py
+-rw-r--r--   0        0        0     4434 2024-05-21 16:30:55.642266 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation_request_client_timeout_duration.py
+-rw-r--r--   0        0        0     2421 2024-05-21 16:30:55.751331 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation_request_client_timeout_duration_xmlschema_type.py
+-rw-r--r--   0        0        0     2088 2024-05-21 16:30:55.362703 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation_variable.py
+-rw-r--r--   0        0        0     1717 2024-05-21 16:30:55.312407 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/paged_result_paging_metadata.py
+-rw-r--r--   0        0        0      181 2024-05-21 16:30:54.670311 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/patch_submodel_by_id_value_only_level.py
+-rw-r--r--   0        0        0      183 2024-05-21 16:30:54.642001 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/patch_submodel_element_by_path_value_only_submodel_repo_level.py
+-rw-r--r--   0        0        0      235 2024-05-21 16:30:54.620949 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/post_submodel_element_by_path_submodel_repo_extent.py
+-rw-r--r--   0        0        0      192 2024-05-21 16:30:54.609863 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/post_submodel_element_by_path_submodel_repo_level.py
+-rw-r--r--   0        0        0     2020 2024-05-21 16:30:55.232098 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/put_file_by_path_body.py
+-rw-r--r--   0        0        0      151 2024-05-21 16:30:54.563148 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/put_submodel_by_id_level.py
+-rw-r--r--   0        0        0      172 2024-05-21 16:30:54.521063 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/put_submodel_element_by_path_submodel_repo_level.py
+-rw-r--r--   0        0        0     2080 2024-05-21 16:30:55.333048 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/put_thumbnail_aas_repository_body.py
+-rw-r--r--   0        0        0     5626 2024-05-21 16:30:55.327298 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/qualifier.py
+-rw-r--r--   0        0        0      258 2024-05-21 16:30:54.922441 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/qualifier_kind.py
+-rw-r--r--   0        0        0      996 2024-05-21 16:30:54.903483 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/qualifier_value_type.py
+-rw-r--r--   0        0        0     3449 2024-05-21 16:30:55.541648 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/reference.py
+-rw-r--r--   0        0        0      211 2024-05-24 14:57:14.378767 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/reference_type.py
+-rw-r--r--   0        0        0    10356 2024-05-21 16:30:55.464098 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/relationship_element.py
+-rw-r--r--   0        0        0     1863 2024-05-21 16:30:55.422842 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/resource.py
+-rw-r--r--   0        0        0     2188 2024-05-21 16:30:55.391913 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/result.py
+-rw-r--r--   0        0        0     2576 2024-05-21 16:30:55.362703 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/service_description.py
+-rw-r--r--   0        0        0     3468 2024-05-21 16:30:55.313689 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/service_description_profiles_item.py
+-rw-r--r--   0        0        0     4591 2024-05-21 16:30:55.284407 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/specific_asset_id.py
+-rw-r--r--   0        0        0    12023 2024-05-21 16:30:55.252009 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel.py
+-rw-r--r--   0        0        0     9232 2024-05-21 16:30:55.677057 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element.py
+-rw-r--r--   0        0        0    10115 2024-05-21 16:30:55.416914 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_collection.py
+-rw-r--r--   0        0        0    13431 2024-05-21 16:30:55.415223 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_list.py
+-rw-r--r--   0        0        0      826 2024-05-21 16:30:54.981373 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_list_type_value_list_element.py
+-rw-r--r--   0        0        0     1017 2024-05-21 16:30:54.987077 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_list_value_type_list_element.py
+-rw-r--r--   0        0        0     1271 2024-05-21 16:30:55.310199 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_value.py
+-rw-r--r--   0        0        0      178 2024-05-24 14:56:31.630800 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_kind.py
+-rw-r--r--   0        0        0     2670 2024-05-21 16:30:55.252009 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_value_only.py
+-rw-r--r--   0        0        0     1889 2024-05-21 16:30:55.314155 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_value_only_values_only_map.py
+-rw-r--r--   0        0        0     1654 2024-05-21 16:30:55.284407 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/upload_environment_body.py
+-rw-r--r--   0        0        0       25 2024-05-21 16:30:51.964161 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/py.typed
+-rw-r--r--   0        0        0     1030 2024-05-21 16:30:55.231286 ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/types.py
+-rw-r--r--   0        0        0      657 2024-05-24 15:00:55.320126 ba_syx_aas_environment_component_client-2.1/pyproject.toml
+-rw-r--r--   0        0        0     5433 2024-05-21 16:30:52.065800 ba_syx_aas_environment_component_client-2.1/README.md
+-rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 ba_syx_aas_environment_component_client-2.1/PKG-INFO
```

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/delete_file_by_path.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/delete_file_by_path.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/get_file_by_path.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/get_file_by_path.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/put_file_by_path.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_api/put_file_by_path.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_asset_administration_shell_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_asset_administration_shell_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_submodel_reference_by_id_aas_repository.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_submodel_reference_by_id_aas_repository.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_thumbnail_aas_repository.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/delete_thumbnail_aas_repository.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_all_asset_administration_shells.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_all_asset_administration_shells.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_all_submodel_references_aas_repository.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_all_submodel_references_aas_repository.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_asset_administration_shell_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_asset_administration_shell_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_asset_information_aas_repository.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_asset_information_aas_repository.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_thumbnail_aas_repository.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/get_thumbnail_aas_repository.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/post_asset_administration_shell.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/post_asset_administration_shell.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/post_submodel_reference_aas_repository.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/post_submodel_reference_aas_repository.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_asset_administration_shell_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_asset_administration_shell_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_asset_information_aas_repository.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_asset_information_aas_repository.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_thumbnail_aas_repository.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/asset_administration_shell_repository_api/put_thumbnail_aas_repository.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/delete_concept_description_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/delete_concept_description_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/get_all_concept_descriptions.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/get_all_concept_descriptions.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/get_concept_description_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/get_concept_description_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/post_concept_description.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/post_concept_description.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/concept_description_repository_api/put_concept_description_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/concept_description_repository_api/put_concept_description_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/environment_api/upload_environment.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/environment_api/upload_environment.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/registry_and_discovery_interface/get_description.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/registry_and_discovery_interface/get_description.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/serialization_api/generate_serialization_by_ids.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/serialization_api/generate_serialization_by_ids.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/delete_submodel_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/delete_submodel_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/delete_submodel_element_by_path_submodel_repo.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/delete_submodel_element_by_path_submodel_repo.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_all_submodel_elements.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_all_submodel_elements.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_all_submodels.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_all_submodels.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id_metadata.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id_metadata.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id_value_only.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_by_id_value_only.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_element_by_path_submodel_repo.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_element_by_path_submodel_repo.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_element_by_path_value_only_submodel_repo.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/get_submodel_element_by_path_value_only_submodel_repo.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/invoke_operation_submodel_repo.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/invoke_operation_submodel_repo.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/patch_submodel_by_id_value_only.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/patch_submodel_by_id_value_only.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/patch_submodel_element_by_path_value_only_submodel_repo.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/patch_submodel_element_by_path_value_only_submodel_repo.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel_element_by_path_submodel_repo.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel_element_by_path_submodel_repo.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel_element_submodel_repo.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/post_submodel_element_submodel_repo.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/put_submodel_by_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/put_submodel_by_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/api/submodel_repository_api/put_submodel_element_by_path_submodel_repo.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/api/submodel_repository_api/put_submodel_element_by_path_submodel_repo.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/client.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/client.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/errors.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/errors.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/__init__.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/administrative_information.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/administrative_information.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/asset_administration_shell.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/asset_administration_shell.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/asset_information.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/asset_information.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/base_64_url_encoded_cursor.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/base_64_url_encoded_cursor.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/concept_description.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/concept_description.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/data_specification_content.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/data_specification_content.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/embedded_data_specification.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/embedded_data_specification.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/entity.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/entity.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/extension.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/extension.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/extension_value_type.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/extension_value_type.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/get_asset_administration_shells_result.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/get_asset_administration_shells_result.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/key.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/key.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/key_type.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_list_type_value_list_element.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 from enum import Enum
 
 
-class KeyType(str, Enum):
+class SubmodelElementListTypeValueListElement(str, Enum):
     ANNOTATED_RELATIONSHIP_ELEMENT = "ANNOTATED_RELATIONSHIP_ELEMENT"
-    ASSET_ADMINISTRATION_SHELL = "ASSET_ADMINISTRATION_SHELL"
     BASIC_EVENT_ELEMENT = "BASIC_EVENT_ELEMENT"
     BLOB = "BLOB"
     CAPABILITY = "CAPABILITY"
-    CONCEPT_DESCRIPTION = "CONCEPT_DESCRIPTION"
     DATA_ELEMENT = "DATA_ELEMENT"
     ENTITY = "ENTITY"
     EVENT_ELEMENT = "EVENT_ELEMENT"
     FILE = "FILE"
-    FRAGMENT_REFERENCE = "FRAGMENT_REFERENCE"
-    GLOBAL_REFERENCE = "GLOBAL_REFERENCE"
-    IDENTIFIABLE = "IDENTIFIABLE"
     MULTI_LANGUAGE_PROPERTY = "MULTI_LANGUAGE_PROPERTY"
     OPERATION = "OPERATION"
     PROPERTY = "PROPERTY"
     RANGE = "RANGE"
-    REFERABLE = "REFERABLE"
     REFERENCE_ELEMENT = "REFERENCE_ELEMENT"
     RELATIONSHIP_ELEMENT = "RELATIONSHIP_ELEMENT"
-    SUBMODEL = "SUBMODEL"
     SUBMODEL_ELEMENT = "SUBMODEL_ELEMENT"
     SUBMODEL_ELEMENT_COLLECTION = "SUBMODEL_ELEMENT_COLLECTION"
     SUBMODEL_ELEMENT_LIST = "SUBMODEL_ELEMENT_LIST"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/lang_string_name_type.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/lang_string_name_type.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/lang_string_text_type.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/lang_string_text_type.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/message.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/message.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation_request.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation_request.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation_request_client_timeout_duration.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation_request_client_timeout_duration.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation_request_client_timeout_duration_xmlschema_type.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation_request_client_timeout_duration_xmlschema_type.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/operation_variable.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/operation_variable.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/paged_result_paging_metadata.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/paged_result_paging_metadata.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/put_file_by_path_body.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/put_file_by_path_body.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/put_thumbnail_aas_repository_body.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/put_thumbnail_aas_repository_body.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/qualifier.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/qualifier.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/qualifier_value_type.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/qualifier_value_type.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/reference.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/reference.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/relationship_element.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/relationship_element.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/resource.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/result.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/result.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/service_description.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/service_description.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/service_description_profiles_item.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/service_description_profiles_item.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/specific_asset_id.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/specific_asset_id.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_collection.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_collection.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_list.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_list.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_list_type_value_list_element.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/key_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from enum import Enum
 
 
-class SubmodelElementListTypeValueListElement(str, Enum):
+class KeyType(str, Enum):
     ANNOTATED_RELATIONSHIP_ELEMENT = "ANNOTATED_RELATIONSHIP_ELEMENT"
+    ASSET_ADMINISTRATION_SHELL = "AssetAdministrationShell"
     BASIC_EVENT_ELEMENT = "BASIC_EVENT_ELEMENT"
     BLOB = "BLOB"
     CAPABILITY = "CAPABILITY"
+    CONCEPT_DESCRIPTION = "CONCEPT_DESCRIPTION"
     DATA_ELEMENT = "DATA_ELEMENT"
     ENTITY = "ENTITY"
     EVENT_ELEMENT = "EVENT_ELEMENT"
     FILE = "FILE"
+    FRAGMENT_REFERENCE = "FRAGMENT_REFERENCE"
+    GLOBAL_REFERENCE = "GlobalReference"
+    IDENTIFIABLE = "IDENTIFIABLE"
     MULTI_LANGUAGE_PROPERTY = "MULTI_LANGUAGE_PROPERTY"
-    OPERATION = "OPERATION"
-    PROPERTY = "PROPERTY"
+    OPERATION = "Operation"
+    PROPERTY = "Property"
     RANGE = "RANGE"
-    REFERENCE_ELEMENT = "REFERENCE_ELEMENT"
+    REFERABLE = "REFERABLE"
+    REFERENCE_ELEMENT = "ReferenceElement"
     RELATIONSHIP_ELEMENT = "RELATIONSHIP_ELEMENT"
+    SUBMODEL = "Submodel"
     SUBMODEL_ELEMENT = "SUBMODEL_ELEMENT"
-    SUBMODEL_ELEMENT_COLLECTION = "SUBMODEL_ELEMENT_COLLECTION"
-    SUBMODEL_ELEMENT_LIST = "SUBMODEL_ELEMENT_LIST"
+    SUBMODEL_ELEMENT_COLLECTION = "SubmodelElementCollection"
+    SUBMODEL_ELEMENT_LIST = "SubmodelElementList"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_list_value_type_list_element.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_list_value_type_list_element.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_element_value.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_element_value.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_value_only.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_value_only.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/submodel_value_only_values_only_map.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/submodel_value_only_values_only_map.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/models/upload_environment_body.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/models/upload_environment_body.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/ba_syx_aas_environment_component_client/types.py` & `ba_syx_aas_environment_component_client-2.1/ba_syx_aas_environment_component_client/types.py`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/pyproject.toml` & `ba_syx_aas_environment_component_client-2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ba-syx-aas-environment-component-client"
-version = "2.0"
+version = "2.1"
 description = "A client library for accessing BaSyx AAS Environment Component"
 authors = []
 readme = "README.md"
 packages = [
     {include = "ba_syx_aas_environment_component_client"},
 ]
 include = ["CHANGELOG.md", "ba_syx_aas_environment_component_client/py.typed"]
```

### Comparing `ba_syx_aas_environment_component_client-2.0/README.md` & `ba_syx_aas_environment_component_client-2.1/README.md`

 * *Files identical despite different names*

### Comparing `ba_syx_aas_environment_component_client-2.0/PKG-INFO` & `ba_syx_aas_environment_component_client-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ba-syx-aas-environment-component-client
-Version: 2.0
+Version: 2.1
 Summary: A client library for accessing BaSyx AAS Environment Component
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

